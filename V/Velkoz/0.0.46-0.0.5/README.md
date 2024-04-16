# Comparing `tmp/Velkoz-0.0.46.tar.gz` & `tmp/Velkoz-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Velkoz-0.0.46.tar", last modified: Thu Apr 11 20:41:46 2024, max compression
+gzip compressed data, was "Velkoz-0.0.5.tar", last modified: Tue Apr 16 10:30:06 2024, max compression
```

## Comparing `Velkoz-0.0.46.tar` & `Velkoz-0.0.5.tar`

### file list

```diff
@@ -1,34 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 20:41:46.125392 Velkoz-0.0.46/
--rw-rw-rw-   0        0        0      671 2024-04-11 20:41:46.124393 Velkoz-0.0.46/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-11 20:41:46.085808 Velkoz-0.0.46/Velkoz/
--rw-rw-rw-   0        0        0      549 2024-04-10 19:54:57.000000 Velkoz-0.0.46/Velkoz/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 20:41:46.114234 Velkoz-0.0.46/Velkoz/eye/
--rw-rw-rw-   0        0        0      150 2024-03-23 23:06:35.000000 Velkoz-0.0.46/Velkoz/eye/__init__.py
--rw-rw-rw-   0        0        0      523 2024-04-10 19:31:41.000000 Velkoz-0.0.46/Velkoz/eye/account.py
--rw-rw-rw-   0        0        0      591 2024-04-09 19:37:05.000000 Velkoz-0.0.46/Velkoz/eye/champion_mastery.py
--rw-rw-rw-   0        0        0        8 2024-03-22 13:50:02.000000 Velkoz-0.0.46/Velkoz/eye/common.py
--rw-rw-rw-   0        0        0     7581 2024-04-06 09:20:19.000000 Velkoz-0.0.46/Velkoz/eye/match.py
--rw-rw-rw-   0        0        0     1976 2024-04-10 19:31:40.000000 Velkoz-0.0.46/Velkoz/eye/summoner.py
--rw-rw-rw-   0        0        0     1160 2024-04-11 20:41:20.000000 Velkoz-0.0.46/Velkoz/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 20:41:46.117242 Velkoz-0.0.46/Velkoz/supp/
--rw-rw-rw-   0        0        0      129 2024-04-05 19:15:06.000000 Velkoz-0.0.46/Velkoz/supp/__init__.py
--rw-rw-rw-   0        0        0      601 2024-04-10 19:50:35.000000 Velkoz-0.0.46/Velkoz/supp/account.py
--rw-rw-rw-   0        0        0     1165 2024-04-11 18:26:45.000000 Velkoz-0.0.46/Velkoz/supp/champion_mastery.py
--rw-rw-rw-   0        0        0      270 2024-04-11 20:40:37.000000 Velkoz-0.0.46/Velkoz/supp/match.py
--rw-rw-rw-   0        0        0     1681 2024-04-10 19:50:14.000000 Velkoz-0.0.46/Velkoz/supp/summoner.py
-drwxrwxrwx   0        0        0        0 2024-04-11 20:41:46.122391 Velkoz-0.0.46/Velkoz/tentacles/
--rw-rw-rw-   0        0        0      213 2024-03-18 23:45:33.000000 Velkoz-0.0.46/Velkoz/tentacles/__init__.py
--rw-rw-rw-   0        0        0     1224 2024-03-22 11:07:43.000000 Velkoz-0.0.46/Velkoz/tentacles/account.py
--rw-rw-rw-   0        0        0     3340 2024-04-10 19:40:42.000000 Velkoz-0.0.46/Velkoz/tentacles/champion_mastery.py
--rw-rw-rw-   0        0        0     4505 2024-04-06 09:36:14.000000 Velkoz-0.0.46/Velkoz/tentacles/common.py
--rw-rw-rw-   0        0        0       60 2024-04-05 19:09:48.000000 Velkoz-0.0.46/Velkoz/tentacles/config.py
--rw-rw-rw-   0        0        0     1650 2024-03-22 13:51:43.000000 Velkoz-0.0.46/Velkoz/tentacles/match.py
--rw-rw-rw-   0        0        0     1416 2024-03-22 11:06:12.000000 Velkoz-0.0.46/Velkoz/tentacles/summoner.py
--rw-rw-rw-   0        0        0     5325 2024-04-11 20:40:50.000000 Velkoz-0.0.46/Velkoz/velkoz.py
-drwxrwxrwx   0        0        0        0 2024-04-11 20:41:46.123392 Velkoz-0.0.46/Velkoz.egg-info/
--rw-rw-rw-   0        0        0      671 2024-04-11 20:41:46.000000 Velkoz-0.0.46/Velkoz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      667 2024-04-11 20:41:46.000000 Velkoz-0.0.46/Velkoz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 20:41:46.000000 Velkoz-0.0.46/Velkoz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-11 20:41:46.000000 Velkoz-0.0.46/Velkoz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-11 20:41:46.000000 Velkoz-0.0.46/Velkoz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 20:41:46.125392 Velkoz-0.0.46/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-16 10:30:06.642367 Velkoz-0.0.5/
+-rw-rw-rw-   0        0        0      562 2024-04-16 10:30:06.639374 Velkoz-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-16 10:30:06.419611 Velkoz-0.0.5/Velkoz/
+-rw-rw-rw-   0        0        0      731 2024-04-16 00:05:02.000000 Velkoz-0.0.5/Velkoz/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:30:06.468625 Velkoz-0.0.5/Velkoz/data/
+-rw-rw-rw-   0        0        0       48 2024-04-13 20:58:45.000000 Velkoz-0.0.5/Velkoz/data/__init__.py
+-rw-rw-rw-   0        0        0     2553 2024-04-16 00:04:58.000000 Velkoz-0.0.5/Velkoz/data/champion.py
+-rw-rw-rw-   0        0        0     1738 2024-04-16 00:04:58.000000 Velkoz-0.0.5/Velkoz/data/common.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:30:06.541258 Velkoz-0.0.5/Velkoz/eye/
+-rw-rw-rw-   0        0        0      150 2024-03-23 23:06:35.000000 Velkoz-0.0.5/Velkoz/eye/__init__.py
+-rw-rw-rw-   0        0        0      523 2024-04-10 19:31:41.000000 Velkoz-0.0.5/Velkoz/eye/account.py
+-rw-rw-rw-   0        0        0      591 2024-04-09 19:37:05.000000 Velkoz-0.0.5/Velkoz/eye/champion_mastery.py
+-rw-rw-rw-   0        0        0        8 2024-03-22 13:50:02.000000 Velkoz-0.0.5/Velkoz/eye/common.py
+-rw-rw-rw-   0        0        0     7581 2024-04-12 12:51:42.000000 Velkoz-0.0.5/Velkoz/eye/match.py
+-rw-rw-rw-   0        0        0     1976 2024-04-10 19:31:40.000000 Velkoz-0.0.5/Velkoz/eye/summoner.py
+-rw-rw-rw-   0        0        0     1031 2024-04-16 10:29:33.000000 Velkoz-0.0.5/Velkoz/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:30:06.552260 Velkoz-0.0.5/Velkoz/supp/
+-rw-rw-rw-   0        0        0      154 2024-04-16 10:08:55.000000 Velkoz-0.0.5/Velkoz/supp/__init__.py
+-rw-rw-rw-   0        0        0      601 2024-04-10 19:50:35.000000 Velkoz-0.0.5/Velkoz/supp/account.py
+-rw-rw-rw-   0        0        0      280 2024-04-16 10:16:36.000000 Velkoz-0.0.5/Velkoz/supp/champion.py
+-rw-rw-rw-   0        0        0     1165 2024-04-11 21:19:17.000000 Velkoz-0.0.5/Velkoz/supp/champion_mastery.py
+-rw-rw-rw-   0        0        0      270 2024-04-11 21:19:18.000000 Velkoz-0.0.5/Velkoz/supp/match.py
+-rw-rw-rw-   0        0        0     1681 2024-04-10 19:50:14.000000 Velkoz-0.0.5/Velkoz/supp/summoner.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:30:06.635471 Velkoz-0.0.5/Velkoz/tentacles/
+-rw-rw-rw-   0        0        0      213 2024-04-11 21:19:17.000000 Velkoz-0.0.5/Velkoz/tentacles/__init__.py
+-rw-rw-rw-   0        0        0     1224 2024-03-22 11:07:43.000000 Velkoz-0.0.5/Velkoz/tentacles/account.py
+-rw-rw-rw-   0        0        0     3340 2024-04-11 21:19:18.000000 Velkoz-0.0.5/Velkoz/tentacles/champion_mastery.py
+-rw-rw-rw-   0        0        0     4543 2024-04-12 22:57:44.000000 Velkoz-0.0.5/Velkoz/tentacles/common.py
+-rw-rw-rw-   0        0        0       60 2024-04-05 19:09:48.000000 Velkoz-0.0.5/Velkoz/tentacles/config.py
+-rw-rw-rw-   0        0        0     1650 2024-03-22 13:51:43.000000 Velkoz-0.0.5/Velkoz/tentacles/match.py
+-rw-rw-rw-   0        0        0     1416 2024-03-22 11:06:12.000000 Velkoz-0.0.5/Velkoz/tentacles/summoner.py
+-rw-rw-rw-   0        0        0     6371 2024-04-16 10:20:41.000000 Velkoz-0.0.5/Velkoz/velkoz.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:30:06.637370 Velkoz-0.0.5/Velkoz.egg-info/
+-rw-rw-rw-   0        0        0      562 2024-04-16 10:30:06.000000 Velkoz-0.0.5/Velkoz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      761 2024-04-16 10:30:06.000000 Velkoz-0.0.5/Velkoz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 10:30:06.000000 Velkoz-0.0.5/Velkoz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-16 10:30:06.000000 Velkoz-0.0.5/Velkoz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-16 10:30:06.000000 Velkoz-0.0.5/Velkoz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 10:30:06.642367 Velkoz-0.0.5/setup.cfg
```

### Comparing `Velkoz-0.0.46/PKG-INFO` & `Velkoz-0.0.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: Velkoz
-Version: 0.0.46
+Version: 0.0.5
 Summary: Velkoz Riot Api package
 Author: Nabattis
 Author-email: <ferreirafernando6205@gmail.com>
-Keywords: python,riotapi,api
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Education
-Classifier: Programming Language :: Python :: 2
+Keywords: python,riotapi,api,velkoz
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Dist: requests
+Requires-Dist: pillow
 
 Package that uses RiotApi to get information.
  Made to gain experience so it is not something as advanced as the other packages that do the same. Would not recommend.
```

### Comparing `Velkoz-0.0.46/Velkoz/eye/account.py` & `Velkoz-0.0.5/Velkoz/eye/account.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.46/Velkoz/eye/champion_mastery.py` & `Velkoz-0.0.5/Velkoz/eye/champion_mastery.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.46/Velkoz/eye/match.py` & `Velkoz-0.0.5/Velkoz/eye/match.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.46/Velkoz/eye/summoner.py` & `Velkoz-0.0.5/Velkoz/eye/summoner.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.46/Velkoz/setup.py` & `Velkoz-0.0.5/Velkoz/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 from setuptools import setup, find_packages
 
  #python setup.py sdist bdist_wheel
-VERSION = '0.0.46' 
+VERSION = '0.0.5' 
 DESCRIPTION = 'Velkoz Riot Api package'
 LONG_DESCRIPTION = 'Package that uses RiotApi to get information.\n Made to gain experience so it is not something as advanced as the other packages that do the same. Would not recommend.'
 
 # Setting up
 setup(
         name="Velkoz", 
         version=VERSION,
         author="Nabattis",
         author_email="<ferreirafernando6205@gmail.com>",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
-        install_requires=['requests'], # add any additional packages that 
+        install_requires=['requests','pillow'], # add any additional packages that 
         # needs to be installed along with your package. Eg: 'caer'
         
-        keywords=['python', 'riotapi', 'api'],
+        keywords=['python', 'riotapi', 'api', 'velkoz'],
         classifiers= [
-            "Development Status :: 3 - Alpha",
-            "Intended Audience :: Education",
-            "Programming Language :: Python :: 2",
             "Programming Language :: Python :: 3",
             "Operating System :: MacOS :: MacOS X",
             "Operating System :: Microsoft :: Windows",
         ]
 )
```

### Comparing `Velkoz-0.0.46/Velkoz/supp/account.py` & `Velkoz-0.0.5/Velkoz/supp/account.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.46/Velkoz/supp/champion_mastery.py` & `Velkoz-0.0.5/Velkoz/supp/champion_mastery.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.46/Velkoz/supp/summoner.py` & `Velkoz-0.0.5/Velkoz/supp/summoner.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.46/Velkoz/tentacles/account.py` & `Velkoz-0.0.5/Velkoz/tentacles/account.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.46/Velkoz/tentacles/champion_mastery.py` & `Velkoz-0.0.5/Velkoz/tentacles/champion_mastery.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.46/Velkoz/tentacles/common.py` & `Velkoz-0.0.5/Velkoz/tentacles/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,23 +135,23 @@
             print(f'Invalid Header')
             return(self.service._headers)
         except requests.exceptions.HTTPError as errh:
             print(f'HTTPError - {errh.args[0]}')
             return self._retry_request_on_error(errh)
     
     def _retry_request_on_error(self, errh):
-        print(errh)
+        raise Exception (errh)
         #since I do not know how it reports the error it will stay unhandled for now
         
     def _handle_errorcode(self, code):
         if code == 400:
-            return (f'Request failed with status code {code}: Bad request')
+            raise Exception (f'Request failed with status code {code}: Bad request')
         elif code == 403:
-            return (f'Request failed with status code {code}: Forbidden')
+            raise Exception (f'Request failed with status code {code}: Forbidden')
         elif code == 429:
-            return (f'Request failed with status code {code}: Rate Limit Exceeded')
+            raise Exception (f'Request failed with status code {code}: Rate Limit Exceeded')
 
         
 
 
 if __name__ == '__main__':
     pass
```

### Comparing `Velkoz-0.0.46/Velkoz/tentacles/match.py` & `Velkoz-0.0.5/Velkoz/tentacles/match.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.46/Velkoz/tentacles/summoner.py` & `Velkoz-0.0.5/Velkoz/tentacles/summoner.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.46/Velkoz/velkoz.py` & `Velkoz-0.0.5/Velkoz/velkoz.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,29 +9,39 @@
 from .eye import ( #dont forget the dots
     Summoner,
     Match,
     Participant,
     Account
         )
 
+from .data import(
+    DdragonRequest,
+    Champion,
+    RiotJson
+        )
+
 from .supp import ( #dont forget the dots
     summoner as summ,
     account as acc,
     match as mat,
     champion_mastery as mastery
 
         ) 
 
+
 #CHANGE THIS
 #ERROR HANDLING FOR INVALID API_KEY
 
 def set_api_key(api_key:str):
     global service
     service = RiotApiService(api_key)
 
+def set_ddragon(path:str):
+    global ddragon
+    ddragon = DdragonRequest(ddragon_path=path)
 
 def _initialize_service(api_key=api_key):
     return RiotApiService(api_key) # Service should be initiated in the needed file
 
 
 
 
@@ -133,14 +143,17 @@
 
     parameters = {'matchId' : matchId, 'routing': routing}
     matchDto = mat._get_matchDto_by_parameters(service, parameters)
     match = Match(matchDto)
     return match
 
 
+
+
+
 ####################
 # Champion Mastery 
 ####################
 
 def get_all_masteries(puuid:str = '\0', riotId:str = '\0', region = 'euw1', routing = 'europe'):
     
     new_puuid = _get_puuid(puuid, riotId, routing)
@@ -168,15 +181,48 @@
 
 def get_masteryscore(puuid:str='\0', riotId:str='\0',region:str='euw1', routing:str='europe'):
 
     new_puuid = _get_puuid(puuid, riotId, routing)
 
     return mastery._get_masteryscore(service, puuid=new_puuid, region=region)
 
+############
+# Champion #
+############
+
 
+def get_champion(champion:str):
+    champDto = ddragon._get_data(get_type='champion', champion=champion)
+    champ = Champion(ddragon=ddragon, dto=champDto, champion='Aatrox')
+    return champ
+
+def get_champ_image(champion:str, **kwargs):
+    champ = get_champion(champion)
+
+    img_type = kwargs.get('image', 'splash')
+    number = kwargs.get('skin', 0)
+    match img_type:
+        case 'splash':
+            image = champ.skins.get_splash(number)
+
+        case 'loading':
+            image = champ.skins.get_loading(number)
+
+        case 'centered':
+            image = champ.skins.get_centered(number)
+
+        case 'get_tile':
+            image = champ.skins.get_tile(number)
+
+        case _:
+            raise Exception ('That type of image doesnt exist')
+
+    return image
+
+    
 
 
 
 #############
 # DEBUGGING #
 #############
```

### Comparing `Velkoz-0.0.46/Velkoz.egg-info/PKG-INFO` & `Velkoz-0.0.5/Velkoz.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: Velkoz
-Version: 0.0.46
+Version: 0.0.5
 Summary: Velkoz Riot Api package
 Author: Nabattis
 Author-email: <ferreirafernando6205@gmail.com>
-Keywords: python,riotapi,api
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Education
-Classifier: Programming Language :: Python :: 2
+Keywords: python,riotapi,api,velkoz
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Dist: requests
+Requires-Dist: pillow
 
 Package that uses RiotApi to get information.
  Made to gain experience so it is not something as advanced as the other packages that do the same. Would not recommend.
```

### Comparing `Velkoz-0.0.46/Velkoz.egg-info/SOURCES.txt` & `Velkoz-0.0.5/Velkoz.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -2,22 +2,26 @@
 Velkoz/setup.py
 Velkoz/velkoz.py
 Velkoz.egg-info/PKG-INFO
 Velkoz.egg-info/SOURCES.txt
 Velkoz.egg-info/dependency_links.txt
 Velkoz.egg-info/requires.txt
 Velkoz.egg-info/top_level.txt
+Velkoz/data/__init__.py
+Velkoz/data/champion.py
+Velkoz/data/common.py
 Velkoz/eye/__init__.py
 Velkoz/eye/account.py
 Velkoz/eye/champion_mastery.py
 Velkoz/eye/common.py
 Velkoz/eye/match.py
 Velkoz/eye/summoner.py
 Velkoz/supp/__init__.py
 Velkoz/supp/account.py
+Velkoz/supp/champion.py
 Velkoz/supp/champion_mastery.py
 Velkoz/supp/match.py
 Velkoz/supp/summoner.py
 Velkoz/tentacles/__init__.py
 Velkoz/tentacles/account.py
 Velkoz/tentacles/champion_mastery.py
 Velkoz/tentacles/common.py
```

