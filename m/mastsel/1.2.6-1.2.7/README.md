# Comparing `tmp/mastsel-1.2.6.tar.gz` & `tmp/mastsel-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mastsel-1.2.6.tar", last modified: Thu Mar  7 11:54:08 2024, max compression
+gzip compressed data, was "mastsel-1.2.7.tar", last modified: Tue Apr 16 14:29:54 2024, max compression
```

## Comparing `mastsel-1.2.6.tar` & `mastsel-1.2.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:54:08.170196 mastsel-1.2.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:54:08.162196 mastsel-1.2.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:54:08.162196 mastsel-1.2.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-03-07 11:53:52.000000 mastsel-1.2.6/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-03-07 11:53:52.000000 mastsel-1.2.6/.github/workflows/run_tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-03-07 11:53:52.000000 mastsel-1.2.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-07 11:53:52.000000 mastsel-1.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-07 11:53:52.000000 mastsel-1.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-07 11:54:08.170196 mastsel-1.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-03-07 11:53:52.000000 mastsel-1.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:54:08.166195 mastsel-1.2.6/mastsel/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-07 11:53:52.000000 mastsel-1.2.6/mastsel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-07 11:54:07.000000 mastsel-1.2.6/mastsel/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-03-07 11:53:52.000000 mastsel-1.2.6/mastsel/ini_to_yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)    26323 2024-03-07 11:53:52.000000 mastsel-1.2.6/mastsel/mavisFormulas.py
--rw-r--r--   0 runner    (1001) docker     (127)    55852 2024-03-07 11:53:52.000000 mastsel-1.2.6/mastsel/mavisLO.py
--rw-r--r--   0 runner    (1001) docker     (127)     6165 2024-03-07 11:53:52.000000 mastsel-1.2.6/mastsel/mavisParams.py
--rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-03-07 11:53:52.000000 mastsel-1.2.6/mastsel/mavisParamsOld.py
--rw-r--r--   0 runner    (1001) docker     (127)    13555 2024-03-07 11:53:52.000000 mastsel-1.2.6/mastsel/mavisPsf.py
--rw-r--r--   0 runner    (1001) docker     (127)     9155 2024-03-07 11:53:52.000000 mastsel-1.2.6/mastsel/mavisUtilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:54:08.166195 mastsel-1.2.6/mastsel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-07 11:54:07.000000 mastsel-1.2.6/mastsel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-03-07 11:54:08.000000 mastsel-1.2.6/mastsel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 11:54:07.000000 mastsel-1.2.6/mastsel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-07 11:54:07.000000 mastsel-1.2.6/mastsel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-07 11:54:07.000000 mastsel-1.2.6/mastsel.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:54:08.166195 mastsel-1.2.6/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-03-07 11:53:52.000000 mastsel-1.2.6/notebooks/MAVIS-CONVOLUTION-TEST.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-03-07 11:53:52.000000 mastsel-1.2.6/notebooks/MAVIS-CONVOLUTION.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10266 2024-03-07 11:53:52.000000 mastsel-1.2.6/notebooks/MAVIS.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10100 2024-03-07 11:53:52.000000 mastsel-1.2.6/notebooks/MAVIS2.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-03-07 11:53:52.000000 mastsel-1.2.6/notebooks/MAVIS3.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7064 2024-03-07 11:53:52.000000 mastsel-1.2.6/notebooks/MAVIS_INT_REC.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-03-07 11:53:52.000000 mastsel-1.2.6/notebooks/MAVIS_MAIN.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-07 11:53:52.000000 mastsel-1.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 11:54:08.170196 mastsel-1.2.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:54:08.166195 mastsel-1.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7575 2024-03-07 11:53:52.000000 mastsel-1.2.6/tests/allTests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-03-07 11:53:52.000000 mastsel-1.2.6/tests/testTfOpt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:29:54.659911 mastsel-1.2.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:29:54.651910 mastsel-1.2.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:29:54.655911 mastsel-1.2.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-16 14:29:45.000000 mastsel-1.2.7/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-16 14:29:45.000000 mastsel-1.2.7/.github/workflows/run_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-16 14:29:45.000000 mastsel-1.2.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-16 14:29:45.000000 mastsel-1.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-16 14:29:45.000000 mastsel-1.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-16 14:29:54.659911 mastsel-1.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-16 14:29:45.000000 mastsel-1.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:29:54.655911 mastsel-1.2.7/mastsel/
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-16 14:29:45.000000 mastsel-1.2.7/mastsel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-16 14:29:54.000000 mastsel-1.2.7/mastsel/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-16 14:29:45.000000 mastsel-1.2.7/mastsel/ini_to_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26605 2024-04-16 14:29:45.000000 mastsel-1.2.7/mastsel/mavisFormulas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64522 2024-04-16 14:29:45.000000 mastsel-1.2.7/mastsel/mavisLO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6165 2024-04-16 14:29:45.000000 mastsel-1.2.7/mastsel/mavisParams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-04-16 14:29:45.000000 mastsel-1.2.7/mastsel/mavisParamsOld.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13555 2024-04-16 14:29:45.000000 mastsel-1.2.7/mastsel/mavisPsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9155 2024-04-16 14:29:45.000000 mastsel-1.2.7/mastsel/mavisUtilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:29:54.659911 mastsel-1.2.7/mastsel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-16 14:29:54.000000 mastsel-1.2.7/mastsel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-16 14:29:54.000000 mastsel-1.2.7/mastsel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:29:54.000000 mastsel-1.2.7/mastsel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-16 14:29:54.000000 mastsel-1.2.7/mastsel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-16 14:29:54.000000 mastsel-1.2.7/mastsel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:29:54.659911 mastsel-1.2.7/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-16 14:29:45.000000 mastsel-1.2.7/notebooks/MAVIS-CONVOLUTION-TEST.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-04-16 14:29:45.000000 mastsel-1.2.7/notebooks/MAVIS-CONVOLUTION.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10266 2024-04-16 14:29:45.000000 mastsel-1.2.7/notebooks/MAVIS.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10100 2024-04-16 14:29:45.000000 mastsel-1.2.7/notebooks/MAVIS2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-04-16 14:29:45.000000 mastsel-1.2.7/notebooks/MAVIS3.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7064 2024-04-16 14:29:45.000000 mastsel-1.2.7/notebooks/MAVIS_INT_REC.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-04-16 14:29:45.000000 mastsel-1.2.7/notebooks/MAVIS_MAIN.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-16 14:29:45.000000 mastsel-1.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 14:29:54.659911 mastsel-1.2.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:29:54.659911 mastsel-1.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-04-16 14:29:45.000000 mastsel-1.2.7/tests/allTests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-04-16 14:29:45.000000 mastsel-1.2.7/tests/testTfOpt.py
```

### Comparing `mastsel-1.2.6/.github/workflows/publish.yml` & `mastsel-1.2.7/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.6/.github/workflows/run_tests.yml` & `mastsel-1.2.7/.github/workflows/run_tests.yml`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.6/.gitignore` & `mastsel-1.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.6/LICENSE` & `mastsel-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.6/PKG-INFO` & `mastsel-1.2.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mastsel
-Version: 1.2.6
+Version: 1.2.7
 Summary: Asterism Selection for MAVIS instrument
 Author-email: Fabio Rossi <fabio.rossi@inaf.it>
 License: MIT License
 Project-URL: repository, https://github.com/astro-tiptop/MASTSEL
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mastsel-1.2.6/README.md` & `mastsel-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.6/mastsel/__init__.py` & `mastsel-1.2.7/mastsel/__init__.py`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.6/mastsel/ini_to_yaml.py` & `mastsel-1.2.7/mastsel/ini_to_yaml.py`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.6/mastsel/mavisFormulas.py` & `mastsel-1.2.7/mastsel/mavisFormulas.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,27 +173,28 @@
 
     def ztfTiltNoiseMono():
         return sp.Eq(H_N_tiltz, g_0_tilt*z**-d/(1-z**-1+g_0_tilt*z**-d))
     # end
 
     # 4 tf in z with 2 gains each to tune
     def ztfTipWind():
-        return sp.Eq(H_R_tipz, (1-z**-1)**2/((1-z**-1+g_0_tip*z**-d)*(1-z**-1+g_1_tip)))
+        return sp.Eq( H_R_tipz, (1-1.9995*z**-1+0.9995*z**-2)/ \
+                     ((1-1.9995*z**-1+0.9995*z**-2)+g_0_tip*g_1_tip*(1-1.3*z**-1+0.3825*z**-2)*(z**-d)) )
 
     def ztfTiltWind():
-        return sp.Eq(H_R_tiltz, (1-z**-1)**2/ \
-                     ((1-z**-1+g_0_tilt*z**-d)*(1-z**-1+g_1_tilt)))
+        return sp.Eq( H_R_tiltz, (1-1.9995*z**-1+0.9995*z**-2)/ \
+                     ((1-1.9995*z**-1+0.9995*z**-2)+g_0_tilt*g_1_tilt*(1-1.3*z**-1+0.3825*z**-2)*(z**-d)) )
 
     def ztfTipNoise():
-        return sp.Eq(H_N_tipz, g_0_tip*g_1_tip*z**-d/ \
-                     ((1-z**-1+g_0_tip*z**-d)*(1-z**-1+g_1_tip)))
+        return sp.Eq( H_N_tipz, (g_0_tip*g_1_tip*(1-1.3*z**-1+0.3825*z**-2)*(z**-d))/ \
+                     ((1-1.9995*z**-1+0.9995*z**-2)+g_0_tip*g_1_tip*(1-1.3*z**-1+0.3825*z**-2)*(z**-d)) )
 
     def ztfTiltNoise():
-        return sp.Eq(H_N_tiltz, g_0_tilt*g_1_tilt*z**-d/ \
-                     ((1-z**-1+g_0_tilt*z**-d)*(1-z**-1+g_1_tilt))  )
+        return sp.Eq( H_N_tiltz, (g_0_tilt*g_1_tilt*(1-1.3*z**-1+0.3825*z**-2)*(z**-d))/ \
+                     ((1-1.9995*z**-1+0.9995*z**-2)+g_0_tilt*g_1_tilt*(1-1.3*z**-1+0.3825*z**-2)*(z**-d)) )
     # end
 
     # 4 tf in f obtained from corresponding tf in z
     def tfTipWind(ztf = ztfTipWind()):
         return sp.Eq(H_R_tipf, 
                      subsParamsByName(ztf.rhs, {'z':sp.exp(2*sp.pi*f*sp.I/f_loop)}))
```

### Comparing `mastsel-1.2.6/mastsel/mavisLO.py` & `mastsel-1.2.7/mastsel/mavisLO.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,16 @@
 
     def __init__(self, path, parametersFile, verbose=False):
 
         self.verbose = verbose
         self.plot4debug = False
         self.displayEquation = False
 
+        if self.verbose: np.set_printoptions(precision=3)
+        
         filename_ini = os.path.join(path, parametersFile + '.ini')
         filename_yml = os.path.join(path, parametersFile + '.yml')
 
         self.error = False
         if os.path.exists(filename_yml):
             self.configType = 'yml'
             with open(filename_yml) as f:
@@ -478,27 +480,16 @@
             return R_1, R_1.transpose()
         else:        
             P, P_func = self.specializedIM()
             p_mat_list = []
             for ii in range(nstars):
                 p_mat_list.append(P_func(aCartNGSCoords[ii,0]*arcsecsToRadians, aCartNGSCoords[ii,1]*arcsecsToRadians))
             P_mat = np.vstack(p_mat_list) # aka Interaction Matrix, im
-
-    #        rec_tomo = scipy.linalg.pinv(P_mat) # aka W, 5x6    
-            u, s, vh = np.linalg.svd(P_mat)
-            sv_threshold = 0.05 * s[0]
-            s_inv = np.reciprocal(s)
-            sRes = np.where(s < sv_threshold, 0, s_inv)
-
-            sRes = np.diag(sRes)
-            sRes = np.append(sRes, np.zeros((1,sRes.shape[1])), axis=0 )
-            if nstars==3:
-                sRes = sRes.transpose()
-
-            rec_tomo = vh.transpose() @  ( sRes  @ u.transpose() )
+            
+            rec_tomo = scipy.linalg.pinv(P_mat,rcond=0.05) # aka W, 5x(2*nstars)    
 
             vx = np.asarray(aCartPointingCoordsV[:,0])
             vy = np.asarray(aCartPointingCoordsV[:,1])
             R_1 = np.zeros((2*npointings, 2*nstars))
             for k in range(npointings):
                 P_alpha1 = P_func(vx[k]*arcsecsToRadians, vy[k]*arcsecsToRadians)
                 R_1[2*k:2*(k+1), :] = cp.dot(P_alpha1, rec_tomo)
@@ -651,15 +642,15 @@
                 zplot1.append(rr[1])
 
         #print('x,z:', len(xplot1), len(zplot1))
         psd_freq = xplot1[0]
         psd_focus_turb = zplot1*scaleFactor
         
         psd_focus_sodium_lambda1 = lambdifyByName( self.sSodiumPSDFocus.rhs, ['f'], alib)
-        psd_focus_sodium = psd_focus_sodium_lambda1( psd_freq) 
+        psd_focus_sodium = psd_focus_sodium_lambda1( cp.array(psd_freq)) 
         return psd_focus_turb, psd_focus_sodium
 
     def checkStability(self,keys,values,TFeq):
         # substitute values in sympy expression
         dictTf = {'d':self.loopDelaySteps_LO}
         for key, value in zip(keys,values):
             dictTf[key] = value
@@ -716,15 +707,15 @@
             psd_tilt_turb = cp.asarray(psd_tilt_turb)        
         else:
             xp = np
         if self.LoopGain_LO == 'optimize':
             # add small values of gain to have a good optimization
             # when the noise level is high.
             g0 = (0.00000001,0.0000001,0.000001,0.00001,0.0001,0.001)
-            g0g = xp.concatenate((xp.asarray( g0),xp.linspace(0.01, 0.99, npoints)))
+            g0g = xp.concatenate((xp.asarray( g0),xp.linspace(0.01, 0.8, npoints)))
         elif self.LoopGain_LO == 'test':
             g0g = xp.asarray( xp.linspace(0.01, 0.99, npoints) )
         else:
             # if gain is set no optimization is done and bias is not compensated
             g0 = (bias*self.LoopGain_LO,bias*self.LoopGain_LO)
             g0g = xp.asarray(g0)
         
@@ -736,30 +727,100 @@
                
         if self.plot4debug:
             fig, ax2 = plt.subplots(1,1)
             for x in range(g0g.shape[0]):
                 im = ax2.plot(cpuArray(psd_freq),(self.fTipS_lambda1( g0g_ext, psd_freq_ext, psd_tip_turb_ext).get())[x,:]) 
             ax2.set_xscale('log')
             ax2.set_yscale('log')
-            ax2.set_title('residual PSD', color='black')
+            ax2.set_title('residual turb. PSD', color='black')
             ax2.set_xlabel('frequency [Hz]')
             ax2.set_ylabel('Power')
         
         resultTip = xp.absolute((xp.sum(self.fTipS_lambda1( g0g_ext, psd_freq_ext, psd_tip_turb_ext), axis=(1)) ) )
         resultTilt = xp.absolute((xp.sum(self.fTiltS_lambda1( g0g_ext, psd_freq_ext, psd_tilt_turb_ext), axis=(1)) ) )
         minTipIdx = xp.where(resultTip == xp.nanmin(resultTip))
         minTiltIdx = xp.where(resultTilt == xp.nanmin(resultTilt))
         if self.verbose:
-            print('         best tip gain (noise)',g0g[minTipIdx[0][0]])
-            print('         best tilt gain (noise)',g0g[minTiltIdx[0][0]])
+            print('         best tip & tilt gain (noise):',g0g[minTipIdx[0][0]],g0g[minTiltIdx[0][0]])
         if alib==gpulib and gpuEnabled:
             return cp.asnumpy(resultTip[minTipIdx[0][0]]), cp.asnumpy(resultTilt[minTiltIdx[0][0]])
         else:
             return (resultTip[minTipIdx[0][0]], resultTilt[minTiltIdx[0][0]])
 
+    def computeFocusNoiseResidual(self, fmin, fmax, freq_samples, varX, bias, alib):
+        npoints = 99
+        Cfloat = self.fCValue.evalf()
+        psd_focus_turb, psd_focus_sodium = self.computeFocusPSDs(fmin, fmax, freq_samples, alib)
+        psd_freq = np.asarray(np.linspace(fmin, fmax, freq_samples))
+
+        if self.plot4debug:
+            fig, ax1 = plt.subplots(1,1)
+            im = ax1.plot(psd_freq,psd_focus_turb)
+            im = ax1.plot(psd_freq,psd_focus_sodium)
+            ax1.set_xscale('log')
+            ax1.set_yscale('log')
+            ax1.set_title('Turbulence and Sodium PSD', color='black')
+            ax1.set_xlabel('frequency [Hz]')
+            ax1.set_ylabel('Power')
+
+        df = psd_freq[1]-psd_freq[0]
+        Df = psd_freq[-1]-psd_freq[0]
+        sigma2Noise =  cpuArray(varX) / bias**2 * Cfloat / (Df / df)
+        # must wait till this moment to substitute the noise level
+        self.fFocusS1 = subsParamsByName(self.fTipS_LO, {'phi^noise_Tip': sigma2Noise})
+        self.fFocusS_lambda1 = lambdifyByName( self.fFocusS1, ['g^Tip_0', 'f', 'phi^wind_Tip'], alib)
+        if self.displayEquation:
+            print('computeNoiseResidual')
+            try:
+                display(self.fFocusS1)
+            except:
+                print('    no self.fFocusS1')
+
+        if alib==gpulib and gpuEnabled:
+            xp = cp
+            psd_freq = cp.asarray(psd_freq)
+            psd_focus_turb = cp.asarray(psd_focus_turb)
+        else:
+            xp = np
+        if self.LoopGain_LO == 'optimize':
+            # add small values of gain to have a good optimization
+            # when the noise level is high.
+            g0 = (0.00000001,0.0000001,0.000001,0.00001,0.0001,0.001)
+            g0g = xp.concatenate((xp.asarray( g0),xp.linspace(0.01, 0.99, npoints)))
+        elif self.LoopGain_LO == 'test':
+            g0g = xp.asarray( xp.linspace(0.01, 0.99, npoints) )
+        else:
+            # if gain is set no optimization is done and bias is not compensated
+            g0 = (bias*self.LoopGain_LO)
+            g0g = xp.asarray(g0)
+
+        e1 = psd_freq.reshape((1,psd_freq.shape[0]))
+        e2 = psd_focus_turb.reshape((1,psd_focus_turb.shape[0]))
+        e3 = g0g.reshape((g0g.shape[0], 1))
+        psd_freq_ext, psd_focus_turb_ext, g0g_ext = xp.broadcast_arrays(e1, e2, e3)
+
+        if self.plot4debug:
+            fig, ax2 = plt.subplots(1,1)
+            for x in range(g0g.shape[0]):
+                im = ax2.plot(cpuArray(psd_freq),(self.fFocusS_lambda1( g0g_ext, psd_freq_ext, psd_focus_turb_ext).get())[x,:])
+            ax2.set_xscale('log')
+            ax2.set_yscale('log')
+            ax2.set_title('residual PSD', color='black')
+            ax2.set_xlabel('frequency [Hz]')
+            ax2.set_ylabel('Power')
+
+        resultFocus = xp.absolute((xp.sum(self.fFocusS_lambda1( g0g_ext, psd_freq_ext, psd_focus_turb_ext), axis=(1)) ) )
+
+        minFocusIdx = xp.where(resultFocus == xp.nanmin(resultFocus))
+        if self.verbose:
+            print('         best focus gain (noise):',g0g[minFocusIdx[0][0]])
+        if alib==gpulib and gpuEnabled:
+            return cp.asnumpy(resultFocus[minFocusIdx[0][0]])
+        else:
+            return (resultFocus[minFocusIdx[0][0]])
         
     def computeWindResidual(self, psd_freq, psd_tip_wind0, psd_tilt_wind0, var1x, bias, alib):
         npoints = 99
         Cfloat = self.fCValue.evalf()
         df = psd_freq[1]-psd_freq[0]
         Df = psd_freq[-1]-psd_freq[0]
         psd_tip_wind = psd_tip_wind0 * df
@@ -772,59 +833,121 @@
             ax1.set_xscale('log')
             ax1.set_yscale('log')
             ax1.set_title('wind shake PSD', color='black')
             ax1.set_xlabel('frequency [Hz]')
             ax1.set_ylabel('Power')
                
         sigma2Noise = cpuArray(var1x) / bias**2 * Cfloat / (Df / df)
-        self.fTipS1 = subsParamsByName(self.fTipS, {'phi^noise_Tip': sigma2Noise})
-        self.fTiltS1 = subsParamsByName( self.fTiltS, {'phi^noise_Tilt': sigma2Noise})
-        self.fTipS_lambda1 = lambdifyByName( self.fTipS1, ['g^Tip_0', 'g^Tip_1', 'f', 'phi^wind_Tip'], alib)
-        self.fTiltS_lambda1 = lambdifyByName( self.fTiltS1, ['g^Tilt_0', 'g^Tilt_1', 'f', 'phi^wind_Tilt'], alib)
+        
+        if self.plot4debug:
+            dict1 = {'d':self.loopDelaySteps_LO, 'f_loop':self.SensorFrameRate_LO}
+            RTFwind = subsParamsByName( self.fTipS1tfW, dict1)
+            NTFwind = subsParamsByName( self.fTipS1tfN, dict1)
+            RTFwind_lambda1 = lambdifyByName( RTFwind, ['g^Tip_0', 'g^Tip_1', 'f'], cpulib)
+            NTFwind_lambda1 = lambdifyByName( NTFwind, ['g^Tip_0', 'g^Tip_1', 'f'], cpulib)
+            RTFwindL1 = RTFwind_lambda1( 0.25, 1.0, psd_freq)
+            NTFwindL1 = NTFwind_lambda1( 0.25, 1.0, psd_freq)
+
+            fig, ax2 = plt.subplots(1,1)
+            im = ax2.plot(cpuArray(psd_freq),np.abs(RTFwindL1))
+            im = ax2.plot(cpuArray(psd_freq),np.abs(NTFwindL1))
+            ax2.set_xscale('log')
+            ax2.set_yscale('log')
+            ax2.set_xlabel('frequency [Hz]')
+            ax2.set_ylabel('Amplitude')
+            
+        if self.LoopGain_LO == 'optimize' or self.LoopGain_LO == 'test':
+            self.fTipS1 = subsParamsByName(self.fTipS, {'phi^noise_Tip': sigma2Noise})
+            self.fTiltS1 = subsParamsByName( self.fTiltS, {'phi^noise_Tilt': sigma2Noise})
+            self.fTipS_lambda1 = lambdifyByName( self.fTipS1, ['g^Tip_0', 'g^Tip_1', 'f', 'phi^wind_Tip'], alib)
+            self.fTiltS_lambda1 = lambdifyByName( self.fTiltS1, ['g^Tilt_0', 'g^Tilt_1', 'f', 'phi^wind_Tilt'], alib)
+        else:
+            self.fTipS1 = subsParamsByName(self.fTipS_LO, {'phi^noise_Tip': sigma2Noise})
+            self.fTiltS1 = subsParamsByName( self.fTiltS_LO, {'phi^noise_Tilt': sigma2Noise})
+            self.fTipS_lambda1 = lambdifyByName( self.fTipS1, ['g^Tip_0', 'f', 'phi^wind_Tip'], alib)
+            self.fTiltS_lambda1 = lambdifyByName( self.fTiltS1, ['g^Tilt_0', 'f', 'phi^wind_Tilt'], alib)
         if alib==gpulib and gpuEnabled:
             xp = cp
             psd_freq = cp.asarray(psd_freq)
             psd_tip_wind = cp.asarray(psd_tip_wind)
             psd_tilt_wind = cp.asarray(psd_tilt_wind)        
         else:
             xp = np
         
         if self.LoopGain_LO == 'optimize':
             # add small values of gain to have a good optimization
             # when the noise level is high.
             g0 = (0.00000001,0.0000001,0.000001,0.00001,0.0001,0.001)
-            g0g = xp.concatenate((xp.asarray( g0),xp.linspace(0.01, 0.99, npoints)))
+            g0g = xp.concatenate((xp.asarray( g0),xp.linspace(0.01, 0.8, npoints)))
             g0g, g1g = xp.meshgrid( g0g,g0g )
         elif self.LoopGain_LO == 'test':
             g0g = xp.asarray( xp.linspace(0.01, 0.99, npoints) )
             g0g, g1g = xp.meshgrid( g0g,g0g )
         else:
             # if gain is set no optimization is done and bias is not compensated
             g0 = (bias*self.LoopGain_LO,bias*self.LoopGain_LO)
             g0g = xp.asarray(g0)
-            g0g, g1g = xp.meshgrid( g0g,g0g )
-            g1g *= 1e-6
         
-        e1 = psd_freq.reshape((1,1,psd_freq.shape[0]))
-        e2 = psd_tip_wind.reshape((1,1,psd_tip_wind.shape[0]))
-        e3 = psd_tilt_wind.reshape((1,1,psd_tilt_wind.shape[0]))
-        e4 = g0g.reshape((g0g.shape[0],g0g.shape[1],1))
-        e5 = g1g.reshape((g1g.shape[0],g1g.shape[1],1))
-        psd_freq_ext, psd_tip_wind_ext, psd_tilt_wind_ext, g0g_ext, g1g_ext  = xp.broadcast_arrays(e1, e2, e3, e4, e5)
-        resultTip = xp.absolute((xp.sum(self.fTipS_lambda1( g0g_ext, g1g_ext, psd_freq_ext, psd_tip_wind_ext), axis=(2)) ) )
-        resultTilt = xp.absolute((xp.sum(self.fTiltS_lambda1( g0g_ext, g1g_ext, psd_freq_ext, psd_tilt_wind_ext), axis=(2)) ) )
+        if self.LoopGain_LO == 'optimize' or self.LoopGain_LO == 'test':
+            e1 = psd_freq.reshape((1,1,psd_freq.shape[0]))
+            e2 = psd_tip_wind.reshape((1,1,psd_tip_wind.shape[0]))
+            e3 = psd_tilt_wind.reshape((1,1,psd_tilt_wind.shape[0]))
+            e4 = g0g.reshape((g0g.shape[0],g0g.shape[1],1))
+            e5 = g1g.reshape((g1g.shape[0],g1g.shape[1],1))
+            psd_freq_ext, psd_tip_wind_ext, psd_tilt_wind_ext, g0g_ext, g1g_ext  = xp.broadcast_arrays(e1, e2, e3, e4, e5)
+            resultTip = xp.absolute((xp.sum(self.fTipS_lambda1( g0g_ext, g1g_ext, psd_freq_ext, psd_tip_wind_ext), axis=(2)) ) )
+            resultTilt = xp.absolute((xp.sum(self.fTiltS_lambda1( g0g_ext, g1g_ext, psd_freq_ext, psd_tilt_wind_ext), axis=(2)) ) )
+            if self.plot4debug:
+                fig, ax2 = plt.subplots(1,1)
+                for x in range(g0g.shape[0]):
+                    im = ax2.plot(cpuArray(psd_freq),\
+                        (self.fTipS_lambda1( g0g_ext, g1g_ext, psd_freq_ext, psd_tip_wind_ext).get())[x,int(npoints/2),:]) 
+                ax2.set_xscale('log')
+                ax2.set_yscale('log')
+                ax2.set_title('residual wind PSD', color='black')
+                ax2.set_xlabel('frequency [Hz]')
+                ax2.set_ylabel('Power')
+        else:
+            e1 = psd_freq.reshape((1,psd_freq.shape[0]))
+            e2 = psd_tip_wind.reshape((1,psd_tip_wind.shape[0]))
+            e3 = psd_tilt_wind.reshape((1,psd_tilt_wind.shape[0]))
+            e4 = g0g.reshape((g0g.shape[0], 1))
+            psd_freq_ext, psd_tip_wind_ext, psd_tilt_wind_ext, g0g_ext  = xp.broadcast_arrays(e1, e2, e3, e4)
+            resultTip = xp.absolute((xp.sum(self.fTipS_lambda1( g0g_ext, psd_freq_ext, psd_tip_wind_ext), axis=(1)) ) )
+            resultTilt = xp.absolute((xp.sum(self.fTiltS_lambda1( g0g_ext, psd_freq_ext, psd_tilt_wind_ext), axis=(1)) ) )
+            if self.plot4debug:
+                fig, ax2 = plt.subplots(1,1)
+                for x in range(g0g.shape[0]):
+                    im = ax2.plot(cpuArray(psd_freq),(self.fTipS_lambda1( g0g_ext, psd_freq_ext, psd_tip_wind_ext).get())[x,:]) 
+                ax2.set_xscale('log')
+                ax2.set_yscale('log')
+                ax2.set_title('residual wind PSD', color='black')
+                ax2.set_xlabel('frequency [Hz]')
+                ax2.set_ylabel('Power')
+                
         minTipIdx = xp.where(resultTip == xp.nanmin(resultTip))
         minTiltIdx = xp.where(resultTilt == xp.nanmin(resultTilt))
+        
         if self.verbose:
-            print('         best tip gain (wind)',g0g[minTipIdx[0][0],minTipIdx[1][0]])
-            print('         best tilt gain (wind)',g0g[minTiltIdx[0][0],minTiltIdx[1][0]])
-        if alib==gpulib and gpuEnabled:
-            return cp.asnumpy(resultTip[minTipIdx[0][0], minTipIdx[1][0]]), cp.asnumpy(resultTilt[minTiltIdx[0][0], minTiltIdx[1][0]])
+            if self.LoopGain_LO == 'optimize' or self.LoopGain_LO == 'test':
+                print('         best tip & tilt gain (wind)',g0g[minTipIdx[0][0],minTipIdx[1][0]]*g1g[minTipIdx[0][0],minTipIdx[1][0]],\
+                                                             g0g[minTiltIdx[0][0],minTiltIdx[1][0]]*g1g[minTipIdx[0][0],minTipIdx[1][0]])
+            else:
+                print('         best tip & tilt gain (wind)',g0g[minTipIdx[0][0]],g0g[minTiltIdx[0][0]])
+                    
+        if self.LoopGain_LO == 'optimize' or self.LoopGain_LO == 'test':
+            if alib==gpulib and gpuEnabled:
+                return cp.asnumpy(resultTip[minTipIdx[0][0], minTipIdx[1][0]]), cp.asnumpy(resultTilt[minTiltIdx[0][0], minTiltIdx[1][0]])
+            else:
+                return (resultTip[minTipIdx[0][0], minTipIdx[1][0]], resultTilt[minTiltIdx[0][0], minTiltIdx[1][0]])
         else:
-            return (resultTip[minTipIdx[0][0], minTipIdx[1][0]], resultTilt[minTiltIdx[0][0], minTiltIdx[1][0]])
+            if alib==gpulib and gpuEnabled:
+                return cp.asnumpy(resultTip[minTipIdx[0][0]]), cp.asnumpy(resultTilt[minTiltIdx[0][0]])
+            else:
+                return (resultTip[minTipIdx[0][0]], resultTilt[minTiltIdx[0][0]])
 
         
     def covValue(self, ii,jj, pp, hh):
         p =sp.symbols('p', real=False)
         h =sp.symbols('h', positive=True)
 #    with self.mutex:
         xplot1, zplot1 = self.mItcomplex.IntegralEval(sp.Function('C_v')(p, h),
@@ -865,32 +988,31 @@
                 polarPointingCoordsD[1] *= degToRad
                 polarPointingCoordsD[0] *= arcsecsToRadians
                 polarPointingCoordsD[0] = max( polarPointingCoordsD[0], 1e-9)
                 pp = polarPointingCoordsD[0]*xp.exp(1j*polarPointingCoordsD[1])
                 inputsArray[nstars*points+iidd] = pp
                 iidd = iidd+1
         
-        _idx0 = {2:[0], 3:[1]}
-        if nstars==3:
-            _idx0 = {2:[0,2,4], 3:[1,3,5]}
-        elif nstars==2:
-            _idx0 = {2:[0,2], 3:[1,3]}
+        _idx0 = {2:np.arange(0, 2*nstars, 2), 3:np.arange(1, 2*nstars, 2)}
 
         for ii in [2,3]:
             for jj in [2,3]:
                 outputArray1 = self.covValue(ii, jj, inputsArray, hh)
                 for pind in range(points):
                     for hidx, h_weight in enumerate(self.Cn2Weights):
                         matCasValue[ii-2+pind*2][_idx0[jj]] +=  h_weight*outputArray1[pind:nstars*points:points, hidx]
                         if pind==0:
                             matCssValue[ xp.ix_(_idx0[ii], _idx0[jj]) ] +=  xp.reshape( h_weight*outputArray1[nstars*points:,hidx], (nstars,nstars))
         return scaleF*matCaaValue, scaleF*matCasValue, scaleF*matCssValue
 
     def computeFocusCovMatrices(self, aCartPointingCoords, aCartNGSCoords, xp=np):
-        points = aCartPointingCoords.shape[0]
+        if len(aCartPointingCoords.shape) > 1:
+            points = aCartPointingCoords.shape[0]
+        else:
+            points = 1
         nstars = aCartNGSCoords.shape[0]        
         scaleF = (500.0/(2*np.pi))**2
         matCasValue = xp.zeros((points,nstars), dtype=xp.float32)
         matCssValue = xp.zeros((nstars,nstars), dtype=xp.float32)
         matCaaValue = self.covValue(4, 4, xp.asarray([1e-10, 1e-10]), xp.asarray([1]))[0,0]
         hh = xp.asarray(self.Cn2Heights)
         inputsArray = np.zeros( nstars*points + nstars*nstars, dtype=complex)
@@ -913,21 +1035,15 @@
                 polarPointingCoordsD[1] *= degToRad
                 polarPointingCoordsD[0] *= arcsecsToRadians
                 polarPointingCoordsD[0] = max( polarPointingCoordsD[0], 1e-9)
                 pp = polarPointingCoordsD[0]*xp.exp(1j*polarPointingCoordsD[1])
                 inputsArray[nstars*points+iidd] = pp
                 iidd = iidd+1
         
-        _idx0 = {4:[0]}
-        if nstars==6:
-            _idx0 = {4:[0,1,2,3,4,5]}
-        if nstars==3:
-            _idx0 = {4:[0,1,2]}
-        elif nstars==2:
-            _idx0 = {4:[0,1]}
+        _idx0 = {4:np.arange(0, nstars, 1)}
 
         for ii in [4]:
             for jj in [4]:
                 outputArray1 = self.covValue(4, 4, inputsArray, hh)
                 for pind in range(points):
                     for hidx, h_weight in enumerate(self.Cn2Weights):
                         matCasValue[ii-4+pind][_idx0[jj]] +=  h_weight*outputArray1[pind:nstars*points:points, hidx]
@@ -977,39 +1093,32 @@
         maxFluxIndex = np.where(aNGS_flux==np.amax(aNGS_flux))
         nNaturalGS = len(indices)
         C1 = np.zeros((2,2))
         Cnn = np.zeros((2*nNaturalGS,2*nNaturalGS))
         if self.verbose:
             print('mavisLO.computeTotalResidualMatrix')
             print('         aNGS_flux',aNGS_flux)
-            print('         self.N_sa_tot_LO',self.N_sa_tot_LO)
         for starIndex in range(nNaturalGS):
             bias, amu, avar = self.bias[indices[starIndex]], self.amu[indices[starIndex]], self.avar[indices[starIndex]]            
-            if self.verbose:
-                print('         bias',bias)
-                print('         amu', amu)
-                print('         avar', avar)
-                print('         ratio', cpuArray(cp.asarray(avar))/bias**2)
             nr = self.nr[indices[starIndex]] 
-            # TODO: this second computation must be embedded in the previous one.
             wr = self.wr[indices[starIndex]] 
             if self.verbose:
-                print('         noise residual:     ',nr)
-                print('         wind-shake residual:',wr)
+                print('         turb. + noise residual [nm\u00b2]:',np.array(nr))
             Cnn[2*starIndex,2*starIndex] = nr[0]
             Cnn[2*starIndex+1,2*starIndex+1] = nr[1]
             if starIndex == maxFluxIndex[0][0]:
                 C1[0,0] = wr[0]
                 C1[1,1] = wr[1]
+                if self.verbose:
+                    print('         wind-shake residual    [nm\u00b2]:',np.array(wr))
 
         # C1 and Cnn do not depend on aCartPointingCoords[i]
         Ctot = self.multiCMatAssemble(aCartPointingCoords, aCartNGSCoords, Cnn, C1)
         if self.verbose:
-            print('         Ctot:')
-            print(Ctot)
+            print('         Ctot [nm\u00b2]:',Ctot)
         return Ctot.reshape((nPointings,2,2))
 
 
     def computeTotalResidualMatrix(self, aCartPointingCoords, aCartNGSCoords, aNGS_flux, aNGS_freq, aNGS_SR_LO, aNGS_EE_LO, aNGS_FWHM_mas, doAll=True):
         self.bias = []
         self.amu = []
         self.avar = []
@@ -1019,28 +1128,22 @@
         maxFluxIndex = np.where(aNGS_flux==np.amax(aNGS_flux))
         nNaturalGS = aCartNGSCoords.shape[0]
         C1 = np.zeros((2,2))
         Cnn = np.zeros((2*nNaturalGS,2*nNaturalGS))
 
         if self.verbose:
             print('mavisLO.computeTotalResidualMatrix')
-            print('         aNGS_flux',aNGS_flux)
-            print('         self.N_sa_tot_LO',self.N_sa_tot_LO)
+            print('         aNGS_flux:',aNGS_flux)
             
         for starIndex in range(nNaturalGS):
             self.configLOFreq( aNGS_freq[starIndex] )
             if self.simpleVarianceComputation:
                 bias, amu, avar = self.simplifiedComputeBiasAndVariance(aNGS_flux[starIndex], aNGS_freq[starIndex], aNGS_EE_LO[starIndex], aNGS_FWHM_mas[starIndex]) # one scalar, two
             else:
                 bias, amu, avar = self.computeBiasAndVariance(aNGS_flux[starIndex], aNGS_freq[starIndex], aNGS_EE_LO[starIndex], aNGS_FWHM_mas[starIndex]) # one scalar, two tuples of 2
-            if self.verbose:
-                print('         bias',bias)
-                print('         amu',amu)
-                print('         avar',avar)
-                print('         ratio',cpuArray(cp.asarray(avar))/bias**2)
             
             # normalized by the number of subapertures
             avar = tuple((1.0/self.N_sa_tot_LO) * elem for elem in avar)
 
             self.bias.append(bias)
             self.amu.append(amu)
             self.avar.append(avar)
@@ -1053,32 +1156,77 @@
             else:
                 wr = (0,0)
 
             self.nr.append(nr)
             self.wr.append(wr)
 
             if self.verbose:
-                print('         noise residual:     ',nr)
-                print('         wind-shake residual:',wr)
+                print('         turb. + noise residual [nm\u00b2]:',np.array(nr))
+                print('         wind-shake residual    [nm\u00b2]:',np.array(wr))
             Cnn[2*starIndex,2*starIndex] = nr[0]
             Cnn[2*starIndex+1,2*starIndex+1] = nr[1]
             if starIndex == maxFluxIndex[0][0]:
                 C1[0,0] = wr[0]
                 C1[1,1] = wr[1]
 
         if doAll:
             # C1 and Cnn do not depend on aCartPointingCoords[i]
             Ctot = self.multiCMatAssemble(aCartPointingCoords, aCartNGSCoords, Cnn, C1)
             if self.verbose:
-                print('         Ctot:')
-                print(Ctot)
+                print('         Ctot [nm\u00b2]:',Ctot)
             return Ctot.reshape((nPointings,2,2))
         else:
             return None
 
+    def computeFocusTotalResidualMatrix(self, aCartNGSCoords, aNGS_flux, aNGS_freq, aNGS_SR_LO, aNGS_EE_LO, aNGS_FWHM_mas):
+        maxFluxIndex = np.where(aNGS_flux==np.amax(aNGS_flux))
+        nNaturalGS = aCartNGSCoords.shape[0]
+        Cnn = np.zeros((nNaturalGS,nNaturalGS))
+        
+        if self.verbose:
+            print('mavisLO.computeFocusTotalResidualMatrix')
+            
+        for starIndex in range(nNaturalGS):
+            self.configLOFreq( aNGS_freq[starIndex] )
+            if self.simpleVarianceComputation:
+                bias, amu, avar = self.simplifiedComputeBiasAndVariance(aNGS_flux[starIndex], aNGS_freq[starIndex], aNGS_EE_LO[starIndex], aNGS_FWHM_mas[starIndex]) # one scalar, two
+            else:
+                bias, amu, avar = self.computeBiasAndVariance(aNGS_flux[starIndex], aNGS_freq[starIndex], aNGS_EE_LO[starIndex], aNGS_FWHM_mas[starIndex]) # one scalar, two tuples of 2
+            
+            # normalized by the number of subapertures
+            avar = tuple((1.0/self.N_sa_tot_LO) * elem for elem in avar) # TODO update with noise propagation for focus
+            var1x = avar[0] * self.PixelScale_LO**2
+            Cnn[starIndex,starIndex] = self.computeFocusNoiseResidual(0.25, self.maxLOtFreq, int(4*self.maxLOtFreq), var1x, bias, self.platformlib )
+            
+        # NGS Rec. Mat.
+        R = np.array(np.repeat(1, aCartNGSCoords.shape[0]))*1/np.float32(aCartNGSCoords.shape[0])
+        RT = R.transpose()
+        Caa, Cas, Css = self.computeFocusCovMatrices(np.asarray((0,0)), np.asarray(aCartNGSCoords), xp=np)
+        # sum tomography and noise (Css) errors for a on-axis star
+        Ctot = Caa + np.dot(R, np.dot(Css, RT)) - np.dot(Cas, RT) - np.dot(R, Cas.transpose()) + np.dot(R, np.dot(Cnn, RT))
+        
+        # reference error for LGS case
+        HO_zen_field    = self.get_config_value('sources_HO','Zenith')
+        HO_az_field     = self.get_config_value('sources_HO','Azimuth')
+        HO_pointings = polarToCartesian(np.array( [HO_zen_field, HO_az_field]))
+        aCartLGSCoords = np.dstack( (HO_pointings[0,:], HO_pointings[1,:]) ).reshape(-1, 2)
+        # LGS Rec. Mat.
+        RL = np.array(np.repeat(1, aCartLGSCoords.shape[0]))*1/np.float32(aCartLGSCoords.shape[0])
+        RLT = RL.transpose()
+        CaaL, CasL, CssL = self.computeFocusCovMatrices(np.asarray((0,0)), np.asarray(aCartLGSCoords), xp=np)
+        # tomography error for a on-axis star for LGS WFSs
+        CtotL = CaaL + np.dot(RL, np.dot(CssL, RLT)) - np.dot(CasL, RLT) - np.dot(RL, CasL.transpose())
+        # difference
+        CtotDiff = Ctot - CtotL
+        
+        if self.verbose:
+            print('         focus residual [nm]:',np.sqrt(CtotDiff))
+        
+        return CtotDiff    
+        
     def ellipsesFromCovMats(self, Ctot):
         theta = sp.symbols('theta')
         sigma_1 = sp.symbols('sigma^2_1')
         sigma_2 = sp.symbols('sigma^2_2')
         sigma_X = sp.symbols('sigma^2_X')
         sigma_Y = sp.symbols('sigma^2_Y')
         sigma_XY = sp.symbols('sigma_XY')
```

### Comparing `mastsel-1.2.6/mastsel/mavisParams.py` & `mastsel-1.2.7/mastsel/mavisParams.py`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.6/mastsel/mavisParamsOld.py` & `mastsel-1.2.7/mastsel/mavisParamsOld.py`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.6/mastsel/mavisPsf.py` & `mastsel-1.2.7/mastsel/mavisPsf.py`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.6/mastsel/mavisUtilities.py` & `mastsel-1.2.7/mastsel/mavisUtilities.py`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.6/mastsel.egg-info/PKG-INFO` & `mastsel-1.2.7/mastsel.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mastsel
-Version: 1.2.6
+Version: 1.2.7
 Summary: Asterism Selection for MAVIS instrument
 Author-email: Fabio Rossi <fabio.rossi@inaf.it>
 License: MIT License
 Project-URL: repository, https://github.com/astro-tiptop/MASTSEL
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mastsel-1.2.6/mastsel.egg-info/SOURCES.txt` & `mastsel-1.2.7/mastsel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.6/notebooks/MAVIS-CONVOLUTION-TEST.ipynb` & `mastsel-1.2.7/notebooks/MAVIS-CONVOLUTION-TEST.ipynb`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.6/notebooks/MAVIS-CONVOLUTION.ipynb` & `mastsel-1.2.7/notebooks/MAVIS-CONVOLUTION.ipynb`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.6/notebooks/MAVIS.ipynb` & `mastsel-1.2.7/notebooks/MAVIS.ipynb`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.6/notebooks/MAVIS2.ipynb` & `mastsel-1.2.7/notebooks/MAVIS2.ipynb`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.6/notebooks/MAVIS3.ipynb` & `mastsel-1.2.7/notebooks/MAVIS3.ipynb`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.6/notebooks/MAVIS_INT_REC.ipynb` & `mastsel-1.2.7/notebooks/MAVIS_INT_REC.ipynb`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.6/notebooks/MAVIS_MAIN.ipynb` & `mastsel-1.2.7/notebooks/MAVIS_MAIN.ipynb`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.6/pyproject.toml` & `mastsel-1.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mastsel-1.2.6/tests/allTests.py` & `mastsel-1.2.7/tests/allTests.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,23 +86,23 @@
         NGS_FWHM_mas = [51.677, 81.673, 42.373]
         
         mItGPU = Integrator(cp, cp.float64, '')
         r1 = TestMavisLO.mLO.computeBiasAndVariance(NGS_flux[0], NGS_freq[0], NGS_SR_1650[0], NGS_FWHM_mas[0])
         r2 = TestMavisLO.mLO.computeBiasAndVariance(NGS_flux[1], NGS_freq[1], NGS_SR_1650[1], NGS_FWHM_mas[1])
         r3 = TestMavisLO.mLO.computeBiasAndVariance(NGS_flux[2], NGS_freq[2], NGS_SR_1650[2], NGS_FWHM_mas[2])
 
-        self.assertTrue( np.testing.assert_allclose(np.array(r1[0]), np.array((0.4648798155634258)), rtol=1e-03, atol=1e-5)==None)
-        self.assertTrue( np.testing.assert_allclose(np.array(r1[1]), np.array((0.11621995389085645, 0.0)), rtol=1e-03, atol=1e-5)==None)
-        self.assertTrue( np.testing.assert_allclose(np.array(r1[2]), np.array((0.09879586049734693, 0.09879586135784874)), rtol=1e-03, atol=1e-5)==None)
-        self.assertTrue( np.testing.assert_allclose(np.array(r2[0]), np.array((0.414152240493474)), rtol=1e-03, atol=1e-5)==None)
-        self.assertTrue( np.testing.assert_allclose(np.array(r2[1]), np.array((0.1035380601233685, -3.649587997405677e-09)), rtol=1e-03, atol=1e-5)==None)
-        self.assertTrue( np.testing.assert_allclose(np.array(r2[2]), np.array((0.10850660436150454, 0.10850660702593513)), rtol=1e-03, atol=1e-5)==None)
-        self.assertTrue( np.testing.assert_allclose(np.array(r3[0]), np.array((0.41736352182872927)), rtol=1e-03, atol=1e-5)==None)
-        self.assertTrue( np.testing.assert_allclose(np.array(r3[1]), np.array((0.10434088045718232, 0.0)), rtol=1e-03, atol=1e-5)==None)
-        self.assertTrue( np.testing.assert_allclose(np.array(r3[2]), np.array((0.10727464025272455, 0.10727464025272455)), rtol=1e-03, atol=1e-5)==None)
+        self.assertTrue( np.testing.assert_allclose(np.array(r1[0]), np.array((0.3305086490286356)), rtol=1e-03, atol=1e-5)==None)
+        self.assertTrue( np.testing.assert_allclose(np.array(r1[1]), np.array((0.0826271622571589, 0.0)), rtol=1e-03, atol=1e-5)==None)
+        self.assertTrue( np.testing.assert_allclose(np.array(r1[2]), np.array((0.12942792320851965, 0.12942792320851965)), rtol=1e-03, atol=1e-5)==None)
+        self.assertTrue( np.testing.assert_allclose(np.array(r2[0]), np.array((0.3067767436965856)), rtol=1e-03, atol=1e-5)==None)
+        self.assertTrue( np.testing.assert_allclose(np.array(r2[1]), np.array((0.0766941859241464, 0.0)), rtol=1e-03, atol=1e-5)==None)
+        self.assertTrue( np.testing.assert_allclose(np.array(r2[2]), np.array((0.1381058202766471, 0.1381058202766471)), rtol=1e-03, atol=1e-5)==None)
+        self.assertTrue( np.testing.assert_allclose(np.array(r3[0]), np.array((0.28524614382590824)), rtol=1e-03, atol=1e-5)==None)
+        self.assertTrue( np.testing.assert_allclose(np.array(r3[1]), np.array((0.07131153595647706, 0.0)), rtol=1e-03, atol=1e-5)==None)
+        self.assertTrue( np.testing.assert_allclose(np.array(r3[2]), np.array((0.13778324257626204, 0.13778324257626204)), rtol=1e-03, atol=1e-5)==None)
 
 
 class TestNoiseResiduals(TestMavisLO):
     def test_noise_residuals(self):
         """
         Test 
         """
@@ -113,17 +113,17 @@
         nr = TestMavisLO.mLO.computeNoiseResidual(0.25, 250.0, 1000, var1x, bias, gpulib )
         wr = TestMavisLO.mLO.computeWindResidual(psd_freq, psd_tip_wind, psd_tilt_wind, var1x, bias, gpulib )
         result = nr[0]
         self.assertTrue( np.testing.assert_allclose(result, 3827.13, rtol=1e-03, atol=1e-5)==None)
         result = nr[1]
         self.assertTrue( np.testing.assert_allclose(result, 2387.49, rtol=1e-03, atol=1e-5)==None)
         result = wr[0]
-        self.assertTrue( np.testing.assert_allclose(result, 71.85, rtol=1e-03, atol=1e-5)==None)
+        self.assertTrue( np.testing.assert_allclose(result, 243.63, rtol=1e-03, atol=1e-5)==None)
         result = wr[1]
-        self.assertTrue( np.testing.assert_allclose(result, 60.95, rtol=1e-03, atol=1e-5)==None)
+        self.assertTrue( np.testing.assert_allclose(result, 173.69, rtol=1e-03, atol=1e-5)==None)
 
 
 
 def suite():
     suite = unittest.TestSuite()
     suite.addTest(TestReconstructor('test_reconstructor'))
     suite.addTest(TestCovMatrices('test_cov_matrices'))
```

### Comparing `mastsel-1.2.6/tests/testTfOpt.py` & `mastsel-1.2.7/tests/testTfOpt.py`

 * *Files identical despite different names*

