# Comparing `tmp/libsrg-4.1.5-py3-none-any.whl.zip` & `tmp/libsrg-4.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 54662 bytes, number of entries: 45
+Zip file size: 54817 bytes, number of entries: 45
 -rw-r--r--  2.0 unx     1027 b- defN 24-Feb-08 14:38 libsrg/AppTemplate.py
--rw-r--r--  2.0 unx     9663 b- defN 24-Apr-12 18:46 libsrg/Config.py
+-rw-r--r--  2.0 unx    10039 b- defN 24-Apr-16 16:36 libsrg/Config.py
 -rw-r--r--  2.0 unx     1878 b- defN 24-Apr-02 14:40 libsrg/ElapsedTime.py
 -rw-r--r--  2.0 unx     6715 b- defN 24-Apr-13 13:50 libsrg/Info.py
 -rw-r--r--  2.0 unx     3532 b- defN 23-Jan-31 15:26 libsrg/LevelBanner.py
 -rw-r--r--  2.0 unx     1492 b- defN 23-Jan-18 20:30 libsrg/LoggerGUIProxy.py
 -rw-r--r--  2.0 unx     6113 b- defN 24-Apr-12 20:43 libsrg/LoggingAppBase.py
 -rw-r--r--  2.0 unx     7048 b- defN 24-Apr-13 10:03 libsrg/LoggingCounter.py
 -rw-r--r--  2.0 unx      413 b- defN 23-Jan-31 15:26 libsrg/LoggingUtils.py
@@ -35,13 +35,13 @@
 -rw-r--r--  2.0 unx     2607 b- defN 24-Apr-11 00:45 libsrg/Statistics/UnitTests/DiscteteStatsSlidingWindow_test.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Apr-07 19:48 libsrg/Statistics/UnitTests/__init__.py
 -rw-r--r--  2.0 unx     2222 b- defN 24-Apr-09 15:09 libsrg/TKGUI/GuiBase.py
 -rw-r--r--  2.0 unx      448 b- defN 24-Apr-09 15:09 libsrg/TKGUI/GuiRequest.py
 -rw-r--r--  2.0 unx     3424 b- defN 24-Apr-09 15:09 libsrg/TKGUI/GuiRequestQueue.py
 -rw-r--r--  2.0 unx    10694 b- defN 24-Apr-09 15:09 libsrg/TKGUI/LoggerGUI.py
 -rw-r--r--  2.0 unx        1 b- defN 23-Jan-31 17:16 libsrg/TKGUI/__init__.py
--rw-rw-rw-  2.0 unx     1069 b- defN 24-Apr-13 14:08 libsrg-4.1.5.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     3357 b- defN 24-Apr-13 14:08 libsrg-4.1.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-13 14:08 libsrg-4.1.5.dist-info/WHEEL
--rw-rw-rw-  2.0 unx        7 b- defN 24-Apr-13 14:08 libsrg-4.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     3900 b- defN 24-Apr-13 14:08 libsrg-4.1.5.dist-info/RECORD
-45 files, 160984 bytes uncompressed, 48408 bytes compressed:  69.9%
+-rw-rw-rw-  2.0 unx     1069 b- defN 24-Apr-16 16:40 libsrg-4.2.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     3357 b- defN 24-Apr-16 16:40 libsrg-4.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-16 16:40 libsrg-4.2.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx        7 b- defN 24-Apr-16 16:40 libsrg-4.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3901 b- defN 24-Apr-16 16:40 libsrg-4.2.0.dist-info/RECORD
+45 files, 161361 bytes uncompressed, 48563 bytes compressed:  69.9%
```

## zipnote {}

```diff
@@ -114,23 +114,23 @@
 
 Filename: libsrg/TKGUI/LoggerGUI.py
 Comment: 
 
 Filename: libsrg/TKGUI/__init__.py
 Comment: 
 
-Filename: libsrg-4.1.5.dist-info/LICENSE.txt
+Filename: libsrg-4.2.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: libsrg-4.1.5.dist-info/METADATA
+Filename: libsrg-4.2.0.dist-info/METADATA
 Comment: 
 
-Filename: libsrg-4.1.5.dist-info/WHEEL
+Filename: libsrg-4.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: libsrg-4.1.5.dist-info/top_level.txt
+Filename: libsrg-4.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: libsrg-4.1.5.dist-info/RECORD
+Filename: libsrg-4.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## libsrg/Config.py

```diff
@@ -1,16 +1,19 @@
 import configparser
 import json
+import os
 import re
 from collections import ChainMap
 from pathlib import Path
-from typing import Any, Self, Optional, Tuple
+from typing import Any, Self, Optional, Tuple, TypeAlias
 
 from jinja2 import Template
 
+FileName: TypeAlias = str | bytes | os.PathLike
+ConfigSource: TypeAlias = ChainMap[str,Any]|dict[str,Any]|FileName
 
 class Config(ChainMap):
     """
     The Config class extends the ChainMap class to provide access to config files.
 
     From outside, a Config looks like a series of python dictionaries which get searched in
     order for a given configuation item,
@@ -24,32 +27,32 @@
     configuration files. One file of secrets can be read from a secure location and referenced by items
     in the normal config files.
 
     """
     _secret_config: Self | None = None
 
     @classmethod
-    def set_secrets(cls, *args: Self | ChainMap | dict[str, Any] | Path) -> None:
+    def set_secrets(cls, *args: ConfigSource) -> None:
         """
         Sets the secret config held by this class.
         :param args: zero or more Config, ChainMap, dict[str, Any], Path
         :return: None
         """
         cls._secret_config = cls(*args)
 
-    def __init__(self, *args: Self | ChainMap | dict[str, Any] | Path):
+    def __init__(self, *args: ConfigSource):
         """
         Constructs a new Config object.
         :param args: zero or more Config, ChainMap, dict[str, Any], Path
         """
         args2 = self.process_args(*args)
         super().__init__(*args2)
 
     @classmethod
-    def process_args(cls, *args: Self | ChainMap | dict[str, Any] | Path) -> list[dict[str, Any]]:
+    def process_args(cls, *args: ConfigSource) -> list[dict[str, Any]]:
         """
         Processes a mixed list of Config like inputs to a list of dictionaries.
         * Paths or str filenames are opened and loaded from disk.
         * Config or ChainMap inputs are split into their internal maps (preserving order)
         :param args: zero or more Config, ChainMap, dict[str, Any], Path
         :return: an ordered list of dict objects
         """
@@ -232,7 +235,18 @@
         names = list(config.keys())
         names.sort()
         lst = []
         for name in names:
             depth, val = config.find_item_depth(name)
             lst.append((name, val, depth))
         return lst
+
+    def to_json_str(self,**kwargs)->str:
+        return json.dumps(self.to_flat_dict(), **kwargs)
+
+    def to_json_file(self,file:FileName,**kwargs):
+        txt = self.to_json_str(**kwargs)
+        with open(file,'w') as f:
+            f.write(txt)
+
+    def to_flat_dict(self,)->dict[str,Any]:
+        return dict(self)
```

## Comparing `libsrg-4.1.5.dist-info/LICENSE.txt` & `libsrg-4.2.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `libsrg-4.1.5.dist-info/METADATA` & `libsrg-4.2.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libsrg
-Version: 4.1.5
+Version: 4.2.0
 Summary: Base class for logging apps, Nagios, utilities
 Home-page: https://gitlab.com/SRG_gitlab/libsrg
 Author: Steven Goncalo
 Author-email: srg_pypi@ice9mail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `libsrg-4.1.5.dist-info/RECORD` & `libsrg-4.2.0.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 libsrg/AppTemplate.py,sha256=539vznudLggwi-PtQIljiMlsQWIXMZ5ruSMQ3SGqNNM,1027
-libsrg/Config.py,sha256=ubMe7UnrxYTbWYVAEgfV5lmFqccJGybUfznMolwhLWQ,9663
+libsrg/Config.py,sha256=V8FJLYkB8-XCFQlJurZ8IkSmYaBVqBb7VGOOZxIlgNM,10039
 libsrg/ElapsedTime.py,sha256=m-DxzdpfbElWAPpC0aZXWfrAOODUDb0I-x4w8FWlrZw,1878
 libsrg/Info.py,sha256=XVHrTjZGKfR7uiy39oEEFeH80fYeW9KZ-RIjVcA-BXw,6715
 libsrg/LevelBanner.py,sha256=k2JC41LkQz9_bPCiGhejqkd7SO7_fiuBmo4Y_ETW9H4,3532
 libsrg/LoggerGUIProxy.py,sha256=qrgLnB0Gtmu5IXP9EzBpIpKWYphcVVQOmIpqWOH9Y6k,1492
 libsrg/LoggingAppBase.py,sha256=7jA69DrLkZ5IRuODLNwdNwx0IedCV73CduywcjH5HJc,6113
 libsrg/LoggingCounter.py,sha256=UVGsQnmQCTKVJJfAOpXEQXOswTeTJ4k6KpwcfRWXfzA,7048
 libsrg/LoggingUtils.py,sha256=brhP-2YaCd69vI0CKWTFUZtiTRhj1ud4i-tApP4FWg0,413
@@ -34,12 +34,12 @@
 libsrg/Statistics/UnitTests/DiscteteStatsSlidingWindow_test.py,sha256=2idi1NA9X2wnLBD_Qle7NOJIB2Vlv5XEKf1oSArSNEw,2607
 libsrg/Statistics/UnitTests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 libsrg/TKGUI/GuiBase.py,sha256=D6Jnzh5BZigjJ9XV9n9q4JcfcmX0qYwVfL2jf5TWQ6I,2222
 libsrg/TKGUI/GuiRequest.py,sha256=376qIPvpgg8l4crgPnjqwRnzdTND-mjicNC5VtkY5Hg,448
 libsrg/TKGUI/GuiRequestQueue.py,sha256=WVvdNXLtIaxkdRNbtsUCM7O4BOP-qLdYWVUVju3-xmc,3424
 libsrg/TKGUI/LoggerGUI.py,sha256=jXK77Zw2ettkItf9t5-FEKmQv65honqD27L_X8zOS0I,10694
 libsrg/TKGUI/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-libsrg-4.1.5.dist-info/LICENSE.txt,sha256=ACwmltkrXIz5VsEQcrqljq-fat6ZXAMepjXGoe40KtE,1069
-libsrg-4.1.5.dist-info/METADATA,sha256=neydLmAywt7CkzLWGS8V4mxThPThyGOE-vvNgqNqLY8,3357
-libsrg-4.1.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-libsrg-4.1.5.dist-info/top_level.txt,sha256=NYEOHhvqWFavgb_q4ADmjraMpsan8oFEQPXmMMHGvZ0,7
-libsrg-4.1.5.dist-info/RECORD,,
+libsrg-4.2.0.dist-info/LICENSE.txt,sha256=ACwmltkrXIz5VsEQcrqljq-fat6ZXAMepjXGoe40KtE,1069
+libsrg-4.2.0.dist-info/METADATA,sha256=E_FrQoSCCO2yAPjfyHaNOcaGUGCzIvt0G0m42Ue7iTo,3357
+libsrg-4.2.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+libsrg-4.2.0.dist-info/top_level.txt,sha256=NYEOHhvqWFavgb_q4ADmjraMpsan8oFEQPXmMMHGvZ0,7
+libsrg-4.2.0.dist-info/RECORD,,
```

