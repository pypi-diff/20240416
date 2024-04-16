# Comparing `tmp/Velkoz-0.0.5.tar.gz` & `tmp/Velkoz-0.0.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Velkoz-0.0.5.tar", last modified: Tue Apr 16 10:30:06 2024, max compression
+gzip compressed data, was "Velkoz-0.0.52.tar", last modified: Tue Apr 16 15:12:36 2024, max compression
```

## Comparing `Velkoz-0.0.5.tar` & `Velkoz-0.0.52.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 10:30:06.642367 Velkoz-0.0.5/
--rw-rw-rw-   0        0        0      562 2024-04-16 10:30:06.639374 Velkoz-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-16 10:30:06.419611 Velkoz-0.0.5/Velkoz/
--rw-rw-rw-   0        0        0      731 2024-04-16 00:05:02.000000 Velkoz-0.0.5/Velkoz/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 10:30:06.468625 Velkoz-0.0.5/Velkoz/data/
--rw-rw-rw-   0        0        0       48 2024-04-13 20:58:45.000000 Velkoz-0.0.5/Velkoz/data/__init__.py
--rw-rw-rw-   0        0        0     2553 2024-04-16 00:04:58.000000 Velkoz-0.0.5/Velkoz/data/champion.py
--rw-rw-rw-   0        0        0     1738 2024-04-16 00:04:58.000000 Velkoz-0.0.5/Velkoz/data/common.py
-drwxrwxrwx   0        0        0        0 2024-04-16 10:30:06.541258 Velkoz-0.0.5/Velkoz/eye/
--rw-rw-rw-   0        0        0      150 2024-03-23 23:06:35.000000 Velkoz-0.0.5/Velkoz/eye/__init__.py
--rw-rw-rw-   0        0        0      523 2024-04-10 19:31:41.000000 Velkoz-0.0.5/Velkoz/eye/account.py
--rw-rw-rw-   0        0        0      591 2024-04-09 19:37:05.000000 Velkoz-0.0.5/Velkoz/eye/champion_mastery.py
--rw-rw-rw-   0        0        0        8 2024-03-22 13:50:02.000000 Velkoz-0.0.5/Velkoz/eye/common.py
--rw-rw-rw-   0        0        0     7581 2024-04-12 12:51:42.000000 Velkoz-0.0.5/Velkoz/eye/match.py
--rw-rw-rw-   0        0        0     1976 2024-04-10 19:31:40.000000 Velkoz-0.0.5/Velkoz/eye/summoner.py
--rw-rw-rw-   0        0        0     1031 2024-04-16 10:29:33.000000 Velkoz-0.0.5/Velkoz/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-16 10:30:06.552260 Velkoz-0.0.5/Velkoz/supp/
--rw-rw-rw-   0        0        0      154 2024-04-16 10:08:55.000000 Velkoz-0.0.5/Velkoz/supp/__init__.py
--rw-rw-rw-   0        0        0      601 2024-04-10 19:50:35.000000 Velkoz-0.0.5/Velkoz/supp/account.py
--rw-rw-rw-   0        0        0      280 2024-04-16 10:16:36.000000 Velkoz-0.0.5/Velkoz/supp/champion.py
--rw-rw-rw-   0        0        0     1165 2024-04-11 21:19:17.000000 Velkoz-0.0.5/Velkoz/supp/champion_mastery.py
--rw-rw-rw-   0        0        0      270 2024-04-11 21:19:18.000000 Velkoz-0.0.5/Velkoz/supp/match.py
--rw-rw-rw-   0        0        0     1681 2024-04-10 19:50:14.000000 Velkoz-0.0.5/Velkoz/supp/summoner.py
-drwxrwxrwx   0        0        0        0 2024-04-16 10:30:06.635471 Velkoz-0.0.5/Velkoz/tentacles/
--rw-rw-rw-   0        0        0      213 2024-04-11 21:19:17.000000 Velkoz-0.0.5/Velkoz/tentacles/__init__.py
--rw-rw-rw-   0        0        0     1224 2024-03-22 11:07:43.000000 Velkoz-0.0.5/Velkoz/tentacles/account.py
--rw-rw-rw-   0        0        0     3340 2024-04-11 21:19:18.000000 Velkoz-0.0.5/Velkoz/tentacles/champion_mastery.py
--rw-rw-rw-   0        0        0     4543 2024-04-12 22:57:44.000000 Velkoz-0.0.5/Velkoz/tentacles/common.py
--rw-rw-rw-   0        0        0       60 2024-04-05 19:09:48.000000 Velkoz-0.0.5/Velkoz/tentacles/config.py
--rw-rw-rw-   0        0        0     1650 2024-03-22 13:51:43.000000 Velkoz-0.0.5/Velkoz/tentacles/match.py
--rw-rw-rw-   0        0        0     1416 2024-03-22 11:06:12.000000 Velkoz-0.0.5/Velkoz/tentacles/summoner.py
--rw-rw-rw-   0        0        0     6371 2024-04-16 10:20:41.000000 Velkoz-0.0.5/Velkoz/velkoz.py
-drwxrwxrwx   0        0        0        0 2024-04-16 10:30:06.637370 Velkoz-0.0.5/Velkoz.egg-info/
--rw-rw-rw-   0        0        0      562 2024-04-16 10:30:06.000000 Velkoz-0.0.5/Velkoz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      761 2024-04-16 10:30:06.000000 Velkoz-0.0.5/Velkoz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 10:30:06.000000 Velkoz-0.0.5/Velkoz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-16 10:30:06.000000 Velkoz-0.0.5/Velkoz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-16 10:30:06.000000 Velkoz-0.0.5/Velkoz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 10:30:06.642367 Velkoz-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-16 15:12:36.162689 Velkoz-0.0.52/
+-rw-rw-rw-   0        0        0      563 2024-04-16 15:12:36.161402 Velkoz-0.0.52/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-16 15:12:35.846274 Velkoz-0.0.52/Velkoz/
+-rw-rw-rw-   0        0        0      785 2024-04-16 11:13:15.000000 Velkoz-0.0.52/Velkoz/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 15:12:35.901290 Velkoz-0.0.52/Velkoz/data/
+-rw-rw-rw-   0        0        0       48 2024-04-13 20:58:45.000000 Velkoz-0.0.52/Velkoz/data/__init__.py
+-rw-rw-rw-   0        0        0     2638 2024-04-16 15:11:09.000000 Velkoz-0.0.52/Velkoz/data/champion.py
+-rw-rw-rw-   0        0        0     1738 2024-04-16 00:04:58.000000 Velkoz-0.0.52/Velkoz/data/common.py
+drwxrwxrwx   0        0        0        0 2024-04-16 15:12:35.976179 Velkoz-0.0.52/Velkoz/eye/
+-rw-rw-rw-   0        0        0      150 2024-03-23 23:06:35.000000 Velkoz-0.0.52/Velkoz/eye/__init__.py
+-rw-rw-rw-   0        0        0      523 2024-04-10 19:31:41.000000 Velkoz-0.0.52/Velkoz/eye/account.py
+-rw-rw-rw-   0        0        0      591 2024-04-09 19:37:05.000000 Velkoz-0.0.52/Velkoz/eye/champion_mastery.py
+-rw-rw-rw-   0        0        0        8 2024-03-22 13:50:02.000000 Velkoz-0.0.52/Velkoz/eye/common.py
+-rw-rw-rw-   0        0        0     7581 2024-04-12 12:51:42.000000 Velkoz-0.0.52/Velkoz/eye/match.py
+-rw-rw-rw-   0        0        0     1976 2024-04-10 19:31:40.000000 Velkoz-0.0.52/Velkoz/eye/summoner.py
+-rw-rw-rw-   0        0        0     3276 2024-04-16 15:09:23.000000 Velkoz-0.0.52/Velkoz/settings.py
+-rw-rw-rw-   0        0        0     1032 2024-04-16 15:12:10.000000 Velkoz-0.0.52/Velkoz/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 15:12:36.067685 Velkoz-0.0.52/Velkoz/supp/
+-rw-rw-rw-   0        0        0      154 2024-04-16 10:08:55.000000 Velkoz-0.0.52/Velkoz/supp/__init__.py
+-rw-rw-rw-   0        0        0      601 2024-04-10 19:50:35.000000 Velkoz-0.0.52/Velkoz/supp/account.py
+-rw-rw-rw-   0        0        0      280 2024-04-16 11:05:52.000000 Velkoz-0.0.52/Velkoz/supp/champion.py
+-rw-rw-rw-   0        0        0     1165 2024-04-11 21:19:17.000000 Velkoz-0.0.52/Velkoz/supp/champion_mastery.py
+-rw-rw-rw-   0        0        0      270 2024-04-11 21:19:18.000000 Velkoz-0.0.52/Velkoz/supp/match.py
+-rw-rw-rw-   0        0        0     1681 2024-04-10 19:50:14.000000 Velkoz-0.0.52/Velkoz/supp/summoner.py
+drwxrwxrwx   0        0        0        0 2024-04-16 15:12:36.159220 Velkoz-0.0.52/Velkoz/tentacles/
+-rw-rw-rw-   0        0        0      213 2024-04-11 21:19:17.000000 Velkoz-0.0.52/Velkoz/tentacles/__init__.py
+-rw-rw-rw-   0        0        0     1224 2024-03-22 11:07:43.000000 Velkoz-0.0.52/Velkoz/tentacles/account.py
+-rw-rw-rw-   0        0        0     3340 2024-04-11 21:19:18.000000 Velkoz-0.0.52/Velkoz/tentacles/champion_mastery.py
+-rw-rw-rw-   0        0        0     4543 2024-04-12 22:57:44.000000 Velkoz-0.0.52/Velkoz/tentacles/common.py
+-rw-rw-rw-   0        0        0       60 2024-04-05 19:09:48.000000 Velkoz-0.0.52/Velkoz/tentacles/config.py
+-rw-rw-rw-   0        0        0     1650 2024-03-22 13:51:43.000000 Velkoz-0.0.52/Velkoz/tentacles/match.py
+-rw-rw-rw-   0        0        0     1416 2024-03-22 11:06:12.000000 Velkoz-0.0.52/Velkoz/tentacles/summoner.py
+-rw-rw-rw-   0        0        0     6575 2024-04-16 15:11:30.000000 Velkoz-0.0.52/Velkoz/velkoz.py
+drwxrwxrwx   0        0        0        0 2024-04-16 15:12:36.160752 Velkoz-0.0.52/Velkoz.egg-info/
+-rw-rw-rw-   0        0        0      563 2024-04-16 15:12:35.000000 Velkoz-0.0.52/Velkoz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      780 2024-04-16 15:12:35.000000 Velkoz-0.0.52/Velkoz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 15:12:35.000000 Velkoz-0.0.52/Velkoz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-16 15:12:35.000000 Velkoz-0.0.52/Velkoz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-16 15:12:35.000000 Velkoz-0.0.52/Velkoz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 15:12:36.162689 Velkoz-0.0.52/setup.cfg
```

### Comparing `Velkoz-0.0.5/PKG-INFO` & `Velkoz-0.0.52/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Velkoz
-Version: 0.0.5
+Version: 0.0.52
 Summary: Velkoz Riot Api package
 Author: Nabattis
 Author-email: <ferreirafernando6205@gmail.com>
 Keywords: python,riotapi,api,velkoz
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `Velkoz-0.0.5/Velkoz/data/champion.py` & `Velkoz-0.0.52/Velkoz/data/champion.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,18 @@
 
     def __init__(self, **kwargs):
         self.request = kwargs.get('ddragon', None)
         dto = kwargs.get('dto', None)
         RiotJson.__init__(self, dto)
         self.champ = kwargs.get('champion', None)
         self.championDto = self.data.get(self.champ, None)
-        self._general(self.championDto)
+        try:
+            self._general(self.championDto)
+        except Exception as error:
+            print(self.champ)
    
     def _general(self, Dto:dict):
         self.id = Dto.get('id', self.champ)
         self.key = Dto.get('key', None)
         self.name = Dto.get('name', None)
         self.title = Dto.get('title', None)
```

### Comparing `Velkoz-0.0.5/Velkoz/data/common.py` & `Velkoz-0.0.52/Velkoz/data/common.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.5/Velkoz/eye/account.py` & `Velkoz-0.0.52/Velkoz/eye/account.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.5/Velkoz/eye/champion_mastery.py` & `Velkoz-0.0.52/Velkoz/eye/champion_mastery.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.5/Velkoz/eye/match.py` & `Velkoz-0.0.52/Velkoz/eye/match.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.5/Velkoz/eye/summoner.py` & `Velkoz-0.0.52/Velkoz/eye/summoner.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.5/Velkoz/setup.py` & `Velkoz-0.0.52/Velkoz/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
  #python setup.py sdist bdist_wheel
-VERSION = '0.0.5' 
+VERSION = '0.0.52' 
 DESCRIPTION = 'Velkoz Riot Api package'
 LONG_DESCRIPTION = 'Package that uses RiotApi to get information.\n Made to gain experience so it is not something as advanced as the other packages that do the same. Would not recommend.'
 
 # Setting up
 setup(
         name="Velkoz", 
         version=VERSION,
```

### Comparing `Velkoz-0.0.5/Velkoz/supp/account.py` & `Velkoz-0.0.52/Velkoz/supp/account.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.5/Velkoz/supp/champion_mastery.py` & `Velkoz-0.0.52/Velkoz/supp/champion_mastery.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.5/Velkoz/supp/summoner.py` & `Velkoz-0.0.52/Velkoz/supp/summoner.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.5/Velkoz/tentacles/account.py` & `Velkoz-0.0.52/Velkoz/tentacles/account.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.5/Velkoz/tentacles/champion_mastery.py` & `Velkoz-0.0.52/Velkoz/tentacles/champion_mastery.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.5/Velkoz/tentacles/common.py` & `Velkoz-0.0.52/Velkoz/tentacles/common.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.5/Velkoz/tentacles/match.py` & `Velkoz-0.0.52/Velkoz/tentacles/match.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.5/Velkoz/tentacles/summoner.py` & `Velkoz-0.0.52/Velkoz/tentacles/summoner.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.5/Velkoz/velkoz.py` & `Velkoz-0.0.52/Velkoz/velkoz.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from .supp import ( #dont forget the dots
     summoner as summ,
     account as acc,
     match as mat,
     champion_mastery as mastery
 
         ) 
-
+from .settings import (all_champion_id)
 
 #CHANGE THIS
 #ERROR HANDLING FOR INVALID API_KEY
 
 def set_api_key(api_key:str):
     global service
     service = RiotApiService(api_key)
@@ -89,19 +89,21 @@
     account = acc._get_account_by_parameters(service, parameters)
     return account
 
 '''
 Function to get summoner
 Usage: Must be provided with a riotId, summonerName or summonerId. Having priority in the order they were mentioned here. Region parameter defualts to 'euw1', but should be changed if the summoner you are looking for is not from the euw server.
 '''
-def get_summoner(riotId:str = '\0', summonerName:str = '\0', summonerId:str = 0, region:str = 'euw1'):
+def get_summoner(puuid:str = '\0', riotId:str = '\0', summonerName:str = '\0', summonerId:str = 0, region:str = 'euw1'):
     
     if riotId != '\0':
         account = acc._get_account_by_riotId(service, riotId)
         parameters = {'puuid' : account.puuid}
+    elif puuid != '\0':
+        parameters = {'puuid': puuid}
 
     elif summonerName != '\0':
         parameters = {'summonerName': summonerName}
 
     elif summonerId != 0:
         parameters = {'summonerId' : summonerId}
 
@@ -188,15 +190,15 @@
 ############
 # Champion #
 ############
 
 
 def get_champion(champion:str):
     champDto = ddragon._get_data(get_type='champion', champion=champion)
-    champ = Champion(ddragon=ddragon, dto=champDto, champion='Aatrox')
+    champ = Champion(ddragon=ddragon, dto=champDto, champion=champion)
     return champ
 
 def get_champ_image(champion:str, **kwargs):
     champ = get_champion(champion)
 
     img_type = kwargs.get('image', 'splash')
     number = kwargs.get('skin', 0)
@@ -214,15 +216,17 @@
             image = champ.skins.get_tile(number)
 
         case _:
             raise Exception ('That type of image doesnt exist')
 
     return image
 
-    
+
+def get_champName_by_key(champId:int):
+    return all_champion_id.get(champId, None)
 
 
 
 #############
 # DEBUGGING #
 #############
```

### Comparing `Velkoz-0.0.5/Velkoz.egg-info/PKG-INFO` & `Velkoz-0.0.52/Velkoz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Velkoz
-Version: 0.0.5
+Version: 0.0.52
 Summary: Velkoz Riot Api package
 Author: Nabattis
 Author-email: <ferreirafernando6205@gmail.com>
 Keywords: python,riotapi,api,velkoz
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `Velkoz-0.0.5/Velkoz.egg-info/SOURCES.txt` & `Velkoz-0.0.52/Velkoz.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 Velkoz/__init__.py
+Velkoz/settings.py
 Velkoz/setup.py
 Velkoz/velkoz.py
 Velkoz.egg-info/PKG-INFO
 Velkoz.egg-info/SOURCES.txt
 Velkoz.egg-info/dependency_links.txt
 Velkoz.egg-info/requires.txt
 Velkoz.egg-info/top_level.txt
```

