# Comparing `tmp/dukes-1.3.0.tar.gz` & `tmp/dukes-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dukes-1.3.0.tar", last modified: Sun Apr 14 10:12:22 2024, max compression
+gzip compressed data, was "dukes-1.3.1.tar", last modified: Mon Apr 15 23:06:04 2024, max compression
```

## Comparing `dukes-1.3.0.tar` & `dukes-1.3.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-04-14 10:12:22.902336 dukes-1.3.0/
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)    35129 2024-03-28 13:38:04.000000 dukes-1.3.0/LICENSE
--rw-r--r--   0 yenhsun   (1000) yenhsun   (1000)    45438 2024-04-14 10:12:22.902336 dukes-1.3.0/PKG-INFO
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     4449 2024-04-02 05:16:34.000000 dukes-1.3.0/README.md
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     1058 2024-04-14 10:11:57.000000 dukes-1.3.0/pyproject.toml
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)       38 2024-04-14 10:12:22.902336 dukes-1.3.0/setup.cfg
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)       49 2024-03-28 13:38:04.000000 dukes-1.3.0/setup.py
-drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-04-14 10:12:22.894336 dukes-1.3.0/src/
-drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-04-14 10:12:22.898336 dukes-1.3.0/src/dukes/
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     1077 2024-04-14 10:11:57.000000 dukes-1.3.0/src/dukes/__init__.py
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     3177 2024-04-05 11:34:53.000000 dukes-1.3.0/src/dukes/constant.py
-drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-04-14 10:12:22.898336 dukes-1.3.0/src/dukes/dat/
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)       13 2024-03-28 13:38:04.000000 dukes-1.3.0/src/dukes/dat/__init__.py
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)      911 2024-04-04 16:32:02.000000 dukes-1.3.0/src/dukes/dat/cosmicAgeFit.py
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)      619 2024-03-28 13:38:04.000000 dukes-1.3.0/src/dukes/dat/densityParamFit.py
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)  1936503 2024-03-28 13:38:04.000000 dukes-1.3.0/src/dukes/dat/galacticAreaDensityFit.py
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)    20192 2024-04-14 10:09:04.000000 dukes-1.3.0/src/dukes/dukesMain.py
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     7209 2024-04-03 08:17:21.000000 dukes-1.3.0/src/dukes/galDensity.py
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     2827 2024-04-04 16:29:42.000000 dukes-1.3.0/src/dukes/galMassFunction.py
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)      973 2024-04-01 23:57:07.000000 dukes-1.3.0/src/dukes/sysmsg.py
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)    13672 2024-04-14 09:58:02.000000 dukes-1.3.0/src/dukes/utils.py
-drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-04-14 10:12:22.902336 dukes-1.3.0/src/dukes.egg-info/
--rw-r--r--   0 yenhsun   (1000) yenhsun   (1000)    45438 2024-04-14 10:12:22.000000 dukes-1.3.0/src/dukes.egg-info/PKG-INFO
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)      493 2024-04-14 10:12:22.000000 dukes-1.3.0/src/dukes.egg-info/SOURCES.txt
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)        1 2024-04-14 10:12:22.000000 dukes-1.3.0/src/dukes.egg-info/dependency_links.txt
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)       41 2024-04-14 10:12:22.000000 dukes-1.3.0/src/dukes.egg-info/requires.txt
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)        6 2024-04-14 10:12:22.000000 dukes-1.3.0/src/dukes.egg-info/top_level.txt
+drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-04-15 23:06:04.918317 dukes-1.3.1/
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)    35129 2024-03-28 13:38:04.000000 dukes-1.3.1/LICENSE
+-rw-r--r--   0 yenhsun   (1000) yenhsun   (1000)    45756 2024-04-15 23:06:04.918317 dukes-1.3.1/PKG-INFO
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     4767 2024-04-15 01:45:28.000000 dukes-1.3.1/README.md
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     1058 2024-04-15 23:04:35.000000 dukes-1.3.1/pyproject.toml
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)       38 2024-04-15 23:06:04.918317 dukes-1.3.1/setup.cfg
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)       49 2024-03-28 13:38:04.000000 dukes-1.3.1/setup.py
+drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-04-15 23:06:04.914317 dukes-1.3.1/src/
+drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-04-15 23:06:04.914317 dukes-1.3.1/src/dukes/
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     1077 2024-04-14 10:11:57.000000 dukes-1.3.1/src/dukes/__init__.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     3177 2024-04-05 11:34:53.000000 dukes-1.3.1/src/dukes/constant.py
+drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-04-15 23:06:04.914317 dukes-1.3.1/src/dukes/dat/
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)       13 2024-03-28 13:38:04.000000 dukes-1.3.1/src/dukes/dat/__init__.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)      911 2024-04-04 16:32:02.000000 dukes-1.3.1/src/dukes/dat/cosmicAgeFit.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)      619 2024-03-28 13:38:04.000000 dukes-1.3.1/src/dukes/dat/densityParamFit.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)  1936503 2024-03-28 13:38:04.000000 dukes-1.3.1/src/dukes/dat/galacticAreaDensityFit.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)    20184 2024-04-15 22:53:31.000000 dukes-1.3.1/src/dukes/dukesMain.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     7209 2024-04-03 08:17:21.000000 dukes-1.3.1/src/dukes/galDensity.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     2827 2024-04-04 16:29:42.000000 dukes-1.3.1/src/dukes/galMassFunction.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)      973 2024-04-01 23:57:07.000000 dukes-1.3.1/src/dukes/sysmsg.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)    13664 2024-04-15 22:53:47.000000 dukes-1.3.1/src/dukes/utils.py
+drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-04-15 23:06:04.918317 dukes-1.3.1/src/dukes.egg-info/
+-rw-r--r--   0 yenhsun   (1000) yenhsun   (1000)    45756 2024-04-15 23:06:04.000000 dukes-1.3.1/src/dukes.egg-info/PKG-INFO
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)      493 2024-04-15 23:06:04.000000 dukes-1.3.1/src/dukes.egg-info/SOURCES.txt
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)        1 2024-04-15 23:06:04.000000 dukes-1.3.1/src/dukes.egg-info/dependency_links.txt
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)       41 2024-04-15 23:06:04.000000 dukes-1.3.1/src/dukes.egg-info/requires.txt
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)        6 2024-04-15 23:06:04.000000 dukes-1.3.1/src/dukes.egg-info/top_level.txt
```

### Comparing `dukes-1.3.0/LICENSE` & `dukes-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dukes-1.3.0/PKG-INFO` & `dukes-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dukes
-Version: 1.3.0
+Version: 1.3.1
 Summary: This package evaluates the signatures of diffuse boosted dark matter by supernova neutrinos in the early Universe
 Author-email: Yen-Hsun Lin <yenhsun@phys.ncku.edu.tw>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -685,17 +685,24 @@
 Requires-Dist: numpy>=1.20.0
 Requires-Dist: scipy>=1.10.0
 Requires-Dist: vegas>=6.0.1
 
 # dukes: *D*iff*U*se-boosted dar*K* matt*E*r by *S*upernova neutrinos
 
 
-`dukes` is a pyhon package for evaluating the signatures of diffuse boosted dark matter by supernova neutrinos in the early Universe based on arXiv:24xx.xxxxx.
+`dukes` is a pyhon package for evaluating the signatures of diffuse boosted dark matter by supernova neutrinos in the early Universe based on [arXiv:2404.08528](https://arxiv.org/abs/2404.08528).
 It also supports an *experimental* feature that implements particle-model-dependent differential cross sections for DM-neutrino and DM-electron.
 
+### Citation
+
+If you use this package or part of the code in your research, please cite the following:
+
+1. Yen-Hsun Lin and Meng-Ru Wu, *Echoes of darkness: Supernova-neutrino-boosted dark matter from all galaxies*, arXiv:2404.08528
+2. `dukes`: https://github.com/yenhsunlin/dukes
+
 ## Installation
 
 To install, excute the following command on the prompt
 
     $ pip install dukes
 
 and everything should be processed on-the-fly.
```

### Comparing `dukes-1.3.0/README.md` & `dukes-1.3.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 # dukes: *D*iff*U*se-boosted dar*K* matt*E*r by *S*upernova neutrinos
 
 
-`dukes` is a pyhon package for evaluating the signatures of diffuse boosted dark matter by supernova neutrinos in the early Universe based on arXiv:24xx.xxxxx.
+`dukes` is a pyhon package for evaluating the signatures of diffuse boosted dark matter by supernova neutrinos in the early Universe based on [arXiv:2404.08528](https://arxiv.org/abs/2404.08528).
 It also supports an *experimental* feature that implements particle-model-dependent differential cross sections for DM-neutrino and DM-electron.
 
+### Citation
+
+If you use this package or part of the code in your research, please cite the following:
+
+1. Yen-Hsun Lin and Meng-Ru Wu, *Echoes of darkness: Supernova-neutrino-boosted dark matter from all galaxies*, arXiv:2404.08528
+2. `dukes`: https://github.com/yenhsunlin/dukes
+
 ## Installation
 
 To install, excute the following command on the prompt
 
     $ pip install dukes
 
 and everything should be processed on-the-fly.
```

### Comparing `dukes-1.3.0/pyproject.toml` & `dukes-1.3.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dukes"
-version = "1.3.0"
+version = "1.3.1"
 description = "This package evaluates the signatures of diffuse boosted dark matter by supernova neutrinos in the early Universe"
 readme = "README.md"
 authors = [{ name = "Yen-Hsun Lin", email = "yenhsun@phys.ncku.edu.tw" }]
 license = { file = "LICENSE" }
 dependencies = [
     "numpy >= 1.20.0",
     "scipy >= 1.10.0",
```

### Comparing `dukes-1.3.0/src/dukes/__init__.py` & `dukes-1.3.1/src/dukes/__init__.py`

 * *Files identical despite different names*

### Comparing `dukes-1.3.0/src/dukes/constant.py` & `dukes-1.3.1/src/dukes/constant.py`

 * *Files identical despite different names*

### Comparing `dukes-1.3.0/src/dukes/dat/cosmicAgeFit.py` & `dukes-1.3.1/src/dukes/dat/cosmicAgeFit.py`

 * *Files identical despite different names*

### Comparing `dukes-1.3.0/src/dukes/dat/densityParamFit.py` & `dukes-1.3.1/src/dukes/dat/densityParamFit.py`

 * *Files identical despite different names*

### Comparing `dukes-1.3.0/src/dukes/dat/galacticAreaDensityFit.py` & `dukes-1.3.1/src/dukes/dat/galacticAreaDensityFit.py`

 * *Files identical despite different names*

### Comparing `dukes-1.3.0/src/dukes/dukesMain.py` & `dukes-1.3.1/src/dukes/dukesMain.py`

 * *Files 0% similar despite different names*

```diff
@@ -504,18 +504,18 @@
             if usefit is True:
                 galArealDensity = galacticAreaDensityFit((R,m))
             elif usefit is False:
                 galArealDensity = galacticAreaDensity(R,zRange=[-10,10],MG=MG)
             else:
                 raise FlagError('Flag \'usefit\' must be a boolean.')
             
-            return (2*_np.pi*R)*rhoDotSFR(z)*R*galArealDensity*dnG(m,z)*self._diffSpectrum(Txp,mx,
-                                                                                           MG,R,l,theta,
-                                                                                           thetaCM,
-                                                                                           is_spike,sigv,tBH,rhosMW,rsMW,eta)/_E(z)    
+            return (2*_np.pi*R)*rhoDotSFR(z)*galArealDensity*dnG(m,z)*self._diffSpectrum(Txp,mx,
+                                                                                         MG,R,l,theta,
+                                                                                         thetaCM,
+                                                                                         is_spike,sigv,tBH,rhosMW,rsMW,eta)/_E(z)    
         else:
             return 0
     
     def __call__(self,z,m,Tx,mx,R,l,theta,thetaCM,is_spike,is_weighted,sigv,rhosMW,rsMW,eta,usefit):
         if is_weighted is True:
             return self._dbdmSpectrumWeighted(z,m,Tx,mx,R,l,theta,thetaCM,is_spike,sigv,rhosMW,rsMW,eta,usefit)
         elif is_weighted is False:
```

### Comparing `dukes-1.3.0/src/dukes/galDensity.py` & `dukes-1.3.1/src/dukes/galDensity.py`

 * *Files identical despite different names*

### Comparing `dukes-1.3.0/src/dukes/galMassFunction.py` & `dukes-1.3.1/src/dukes/galMassFunction.py`

 * *Files identical despite different names*

### Comparing `dukes-1.3.0/src/dukes/sysmsg.py` & `dukes-1.3.1/src/dukes/sysmsg.py`

 * *Files identical despite different names*

### Comparing `dukes-1.3.0/src/dukes/utils.py` & `dukes-1.3.1/src/dukes/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,18 +174,18 @@
             if usefit is True:
                 galArealDensity = galacticAreaDensityFit((R,m))
             elif usefit is False:
                 galArealDensity = galacticAreaDensity(R,zRange=[-10,10],MG=MG)
             else:
                 raise FlagError('Flag \'usefit\' must be a boolean.')
             
-            return (2*_np.pi*R)*rhoDotSFR(z)*R*galArealDensity*dnG(m,z)*self._diffSpectrum(Txp,mx,
-                                                                                           MG,R,l,theta,
-                                                                                           thetaCM_vx, 
-                                                                                           is_spike,sigv,tBH,rhosMW,rsMW,eta)/_E(z)
+            return (2*_np.pi*R)*rhoDotSFR(z)*galArealDensity*dnG(m,z)*self._diffSpectrum(Txp,mx,
+                                                                                         MG,R,l,theta,
+                                                                                         thetaCM_vx, 
+                                                                                         is_spike,sigv,tBH,rhosMW,rsMW,eta)/_E(z)
         else:
             return 0
 
     def flux(self,Tx,mx,                                                          
              R=0,Rmax=30,rmax=30,tau=10,is_spike=True,is_average=True,      
              sigv=None,rhosMW=184,rsMW=24.42,eta=24.3856,usefit=True, 
              nitn=10,neval=50000) -> float:
```

### Comparing `dukes-1.3.0/src/dukes.egg-info/PKG-INFO` & `dukes-1.3.1/src/dukes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dukes
-Version: 1.3.0
+Version: 1.3.1
 Summary: This package evaluates the signatures of diffuse boosted dark matter by supernova neutrinos in the early Universe
 Author-email: Yen-Hsun Lin <yenhsun@phys.ncku.edu.tw>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -685,17 +685,24 @@
 Requires-Dist: numpy>=1.20.0
 Requires-Dist: scipy>=1.10.0
 Requires-Dist: vegas>=6.0.1
 
 # dukes: *D*iff*U*se-boosted dar*K* matt*E*r by *S*upernova neutrinos
 
 
-`dukes` is a pyhon package for evaluating the signatures of diffuse boosted dark matter by supernova neutrinos in the early Universe based on arXiv:24xx.xxxxx.
+`dukes` is a pyhon package for evaluating the signatures of diffuse boosted dark matter by supernova neutrinos in the early Universe based on [arXiv:2404.08528](https://arxiv.org/abs/2404.08528).
 It also supports an *experimental* feature that implements particle-model-dependent differential cross sections for DM-neutrino and DM-electron.
 
+### Citation
+
+If you use this package or part of the code in your research, please cite the following:
+
+1. Yen-Hsun Lin and Meng-Ru Wu, *Echoes of darkness: Supernova-neutrino-boosted dark matter from all galaxies*, arXiv:2404.08528
+2. `dukes`: https://github.com/yenhsunlin/dukes
+
 ## Installation
 
 To install, excute the following command on the prompt
 
     $ pip install dukes
 
 and everything should be processed on-the-fly.
```

