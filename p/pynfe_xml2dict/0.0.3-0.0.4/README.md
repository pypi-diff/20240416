# Comparing `tmp/pynfe_xml2dict-0.0.3.tar.gz` & `tmp/pynfe_xml2dict-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynfe_xml2dict-0.0.3.tar", max compression
+gzip compressed data, was "pynfe_xml2dict-0.0.4.tar", max compression
```

## Comparing `pynfe_xml2dict-0.0.3.tar` & `pynfe_xml2dict-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       92 2024-04-15 14:30:20.395539 pynfe_xml2dict-0.0.3/README.md
--rw-r--r--   0        0        0        0 2024-04-15 21:28:14.047643 pynfe_xml2dict-0.0.3/pynfe_xml2dict/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 14:00:19.622087 pynfe_xml2dict-0.0.3/pynfe_xml2dict/cte/__init__.py
--rw-r--r--   0        0        0       25 2024-04-15 14:00:19.622087 pynfe_xml2dict-0.0.3/pynfe_xml2dict/cte/index.py
--rw-r--r--   0        0        0        0 2024-04-15 14:00:19.622087 pynfe_xml2dict-0.0.3/pynfe_xml2dict/nfce/__init__.py
--rw-r--r--   0        0        0       28 2024-04-15 21:31:42.855707 pynfe_xml2dict-0.0.3/pynfe_xml2dict/nfe/__init__.py
--rw-r--r--   0        0        0     1844 2024-04-15 18:32:14.713733 pynfe_xml2dict-0.0.3/pynfe_xml2dict/nfe/__tag_dest__.py
--rw-r--r--   0        0        0     2704 2024-04-15 14:48:41.674789 pynfe_xml2dict-0.0.3/pynfe_xml2dict/nfe/__tag_det__.py
--rw-r--r--   0        0        0     1569 2024-04-15 14:48:16.866926 pynfe_xml2dict-0.0.3/pynfe_xml2dict/nfe/__tag_emit__.py
--rw-r--r--   0        0        0     1468 2024-04-15 21:30:43.580809 pynfe_xml2dict-0.0.3/pynfe_xml2dict/nfe/__tag_ide__.py
--rw-r--r--   0        0        0     2126 2024-04-15 21:31:25.180035 pynfe_xml2dict-0.0.3/pynfe_xml2dict/nfe/ler_nfe.py
--rw-r--r--   0        0        0        0 2024-04-15 14:00:19.622087 pynfe_xml2dict-0.0.3/pynfe_xml2dict/nfse/__init__.py
--rw-r--r--   0        0        0       26 2024-04-15 14:00:19.622087 pynfe_xml2dict-0.0.3/pynfe_xml2dict/nfse/index.py
--rw-r--r--   0        0        0      178 2024-04-15 14:42:39.400938 pynfe_xml2dict-0.0.3/pynfe_xml2dict/utils/__init__.py
--rw-r--r--   0        0        0     4087 2024-04-15 14:41:41.869318 pynfe_xml2dict-0.0.3/pynfe_xml2dict/utils/functions.py
--rw-r--r--   0        0        0      491 2024-04-15 14:00:19.622087 pynfe_xml2dict-0.0.3/pynfe_xml2dict/utils/read_xml.py
--rw-r--r--   0        0        0      461 2024-04-15 21:32:18.827617 pynfe_xml2dict-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 pynfe_xml2dict-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       92 2024-04-15 14:30:20.395539 pynfe_xml2dict-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 21:28:14.047643 pynfe_xml2dict-0.0.4/pynfe_xml2dict/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 14:00:19.622087 pynfe_xml2dict-0.0.4/pynfe_xml2dict/cte/__init__.py
+-rw-r--r--   0        0        0       25 2024-04-15 14:00:19.622087 pynfe_xml2dict-0.0.4/pynfe_xml2dict/cte/index.py
+-rw-r--r--   0        0        0        0 2024-04-15 14:00:19.622087 pynfe_xml2dict-0.0.4/pynfe_xml2dict/nfce/__init__.py
+-rw-r--r--   0        0        0       28 2024-04-15 21:31:42.855707 pynfe_xml2dict-0.0.4/pynfe_xml2dict/nfe/__init__.py
+-rw-r--r--   0        0        0     1844 2024-04-15 18:32:14.713733 pynfe_xml2dict-0.0.4/pynfe_xml2dict/nfe/__tag_dest__.py
+-rw-r--r--   0        0        0     2704 2024-04-15 14:48:41.674789 pynfe_xml2dict-0.0.4/pynfe_xml2dict/nfe/__tag_det__.py
+-rw-r--r--   0        0        0     1569 2024-04-15 14:48:16.866926 pynfe_xml2dict-0.0.4/pynfe_xml2dict/nfe/__tag_emit__.py
+-rw-r--r--   0        0        0     1468 2024-04-15 21:30:43.580809 pynfe_xml2dict-0.0.4/pynfe_xml2dict/nfe/__tag_ide__.py
+-rw-r--r--   0        0        0     2409 2024-04-15 21:52:13.006635 pynfe_xml2dict-0.0.4/pynfe_xml2dict/nfe/ler_nfe.py
+-rw-r--r--   0        0        0        0 2024-04-15 14:00:19.622087 pynfe_xml2dict-0.0.4/pynfe_xml2dict/nfse/__init__.py
+-rw-r--r--   0        0        0       26 2024-04-15 14:00:19.622087 pynfe_xml2dict-0.0.4/pynfe_xml2dict/nfse/index.py
+-rw-r--r--   0        0        0      178 2024-04-15 14:42:39.400938 pynfe_xml2dict-0.0.4/pynfe_xml2dict/utils/__init__.py
+-rw-r--r--   0        0        0     4087 2024-04-15 14:41:41.869318 pynfe_xml2dict-0.0.4/pynfe_xml2dict/utils/functions.py
+-rw-r--r--   0        0        0      679 2024-04-15 21:49:25.505316 pynfe_xml2dict-0.0.4/pynfe_xml2dict/utils/read_xml.py
+-rw-r--r--   0        0        0      461 2024-04-15 21:52:59.206894 pynfe_xml2dict-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 pynfe_xml2dict-0.0.4/PKG-INFO
```

### Comparing `pynfe_xml2dict-0.0.3/pynfe_xml2dict/nfe/__tag_dest__.py` & `pynfe_xml2dict-0.0.4/pynfe_xml2dict/nfe/__tag_dest__.py`

 * *Files identical despite different names*

### Comparing `pynfe_xml2dict-0.0.3/pynfe_xml2dict/nfe/__tag_det__.py` & `pynfe_xml2dict-0.0.4/pynfe_xml2dict/nfe/__tag_det__.py`

 * *Files identical despite different names*

### Comparing `pynfe_xml2dict-0.0.3/pynfe_xml2dict/nfe/__tag_emit__.py` & `pynfe_xml2dict-0.0.4/pynfe_xml2dict/nfe/__tag_emit__.py`

 * *Files identical despite different names*

### Comparing `pynfe_xml2dict-0.0.3/pynfe_xml2dict/nfe/__tag_ide__.py` & `pynfe_xml2dict-0.0.4/pynfe_xml2dict/nfe/__tag_ide__.py`

 * *Files identical despite different names*

### Comparing `pynfe_xml2dict-0.0.3/pynfe_xml2dict/nfe/ler_nfe.py` & `pynfe_xml2dict-0.0.4/pynfe_xml2dict/nfe/ler_nfe.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 from typing import Union, Dict
 
 from pynfe_xml2dict.utils.functions import returnDataInDictOrArray
-from pynfe_xml2dict.utils.read_xml import readXml
+from pynfe_xml2dict.utils.read_xml import readXml, readXmlFromStr
 from .__tag_ide__ import TagIde
 from .__tag_emit__ import TagEmit
 from .__tag_dest__ import TagDest
 from .__tag_det__ import TagDet
 
 
 class LerNfe():
-    def __init__(self, pathXml: str):
-        self.__dataXml = readXml(pathXml)
+    def __init__(self, pathXml: str = None, xmlData: str = None):
+        if pathXml is None and xmlData is not None:
+            self.__dataXml = readXmlFromStr(xmlData)
+        elif pathXml is not None:
+            self.__dataXml = readXml(pathXml)
+        else:
+            raise Exception('Its necessary pass as argument pathXml or xmlData')
+
         self.__objNf: Dict['str', dict] = {}
 
     def __isNfe(self):
         keyNf = returnDataInDictOrArray(self.__dataXml, ['nfeProc', 'NFe', 'infNFe', '@Id'])
         return True if keyNf != '' else False
 
     def __tagIde(self):
```

### Comparing `pynfe_xml2dict-0.0.3/pynfe_xml2dict/utils/functions.py` & `pynfe_xml2dict-0.0.4/pynfe_xml2dict/utils/functions.py`

 * *Files identical despite different names*

### Comparing `pynfe_xml2dict-0.0.3/PKG-INFO` & `pynfe_xml2dict-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynfe_xml2dict
-Version: 0.0.3
+Version: 0.0.4
 Summary: Leitura de XML referente a notas fiscais NF-e, NFC-e e CT-e para dicionário
 License: MIT
 Keywords: python,nfe,xml
 Author: ElderVivot
 Author-email: eldervivot@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

