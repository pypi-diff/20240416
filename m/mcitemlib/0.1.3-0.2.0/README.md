# Comparing `tmp/mcitemlib-0.1.3.tar.gz` & `tmp/mcitemlib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcitemlib-0.1.3.tar", max compression
+gzip compressed data, was "mcitemlib-0.2.0.tar", max compression
```

## Comparing `mcitemlib-0.1.3.tar` & `mcitemlib-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1060 2024-03-20 01:07:11.643195 mcitemlib-0.1.3/LICENSE
--rw-r--r--   0        0        0      599 2024-03-22 02:04:24.820036 mcitemlib-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-03-20 01:07:11.643195 mcitemlib-0.1.3/mcitemlib/__init__.py
--rw-r--r--   0        0        0    16010 2024-03-23 04:55:50.608644 mcitemlib-0.1.3/mcitemlib/itemlib.py
--rw-r--r--   0        0        0     5866 2024-03-22 03:03:21.285709 mcitemlib-0.1.3/mcitemlib/style.py
--rw-r--r--   0        0        0      407 2024-03-23 04:56:55.481490 mcitemlib-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 mcitemlib-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-03-20 01:07:11.643195 mcitemlib-0.2.0/LICENSE
+-rw-r--r--   0        0        0      599 2024-03-22 02:04:24.820036 mcitemlib-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-03-20 01:07:11.643195 mcitemlib-0.2.0/mcitemlib/__init__.py
+-rw-r--r--   0        0        0    17725 2024-04-16 14:00:32.162781 mcitemlib-0.2.0/mcitemlib/itemlib.py
+-rw-r--r--   0        0        0     8053 2024-04-15 15:23:13.976056 mcitemlib-0.2.0/mcitemlib/style.py
+-rw-r--r--   0        0        0      432 2024-04-16 14:06:02.895928 mcitemlib-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1353 1970-01-01 00:00:00.000000 mcitemlib-0.2.0/PKG-INFO
```

### Comparing `mcitemlib-0.1.3/LICENSE` & `mcitemlib-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mcitemlib-0.1.3/README.md` & `mcitemlib-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mcitemlib-0.1.3/mcitemlib/itemlib.py` & `mcitemlib-0.2.0/mcitemlib/itemlib.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 A library for creating and editing Minecraft items using python.
 """
 
 import json
 import time
 import socket
 import websocket
+import nbtlib
 from typing import List, Literal
-from mcitemlib.style import StyledString, ampersand_to_section_format, snake_to_capitalized
+from mcitemlib.style import StyledString, ampersand_to_section_format, snake_to_capitalized, PyNbtStyleException
 
 
 BOOK_ITEMS = {
     'minecraft:writable_book',
     'minecraft:written_book'
 }
 
@@ -27,15 +28,25 @@
 class AutoDict:
     """
     Dictionary that automatically adds nested dictionaries if a key does not exist already.
     """
 
     def __init__(self, d: dict):
         self.data = d
+    
 
+    @staticmethod
+    def from_dict(d: dict):
+        auto_dict = AutoDict({})
+        for k, v in d.items():
+            if isinstance(v, dict):
+                auto_dict[k] = AutoDict.from_dict(v)
+            else:
+                auto_dict[k] = v
+        return auto_dict
 
     def __repr__(self):
         return str(self.data)
     
 
     def __getitem__(self, key):
         if key not in self.key_set():
@@ -52,14 +63,16 @@
     
 
     def as_dict(self) -> dict:
         new_dict = {}
         for key, value in self.data.items():
             if isinstance(value, AutoDict):
                 new_dict[key] = value.as_dict()
+            elif isinstance(value, list):
+                new_dict[key] = [v.as_dict() if isinstance(v, AutoDict) else v for v in value]
             else:
                 new_dict[key] = value
         return new_dict
 
 
     def set_list(self, key) -> list:
         """
@@ -71,15 +84,15 @@
         return self.data[key]
 
 
 class MCItemlibException(Exception):
     pass
 
 
-class TypedInt:
+class _TypedInt:
     def __init__(self, value: int, type: str):
         self.value = value
         self.type = type
     
     def __repr__(self) -> str:
         return f'{self.value}{self.type}'
 
@@ -122,14 +135,23 @@
             'Count': count,
         })
         if item_id == 'written_book':
             self.nbt['tag']['author'] = 'pynbt'
             self.nbt['tag']['title'] = 'Written Book'
     
 
+    @staticmethod
+    def from_nbt(nbt: str):
+        i = Item('stone')
+        print(nbtlib.parse_nbt(nbt))
+        nbt = convert_nbt_tag(nbtlib.parse_nbt(nbt))
+        i.nbt = nbt
+        return i
+    
+
     def __repr__(self):
         return f'Item({self.nbt.__repr__()})'
     
 
     def __str__(self):
         return self.__repr__()
     
@@ -149,21 +171,21 @@
         Get the ID of this item.
 
         :return: The ID of this item.
         """
         return self.nbt['id']
     
 
-    def get_count(self) -> str:
+    def get_count(self) -> int:
         """
         Get the count of this item.
 
         :return: The count of this item.
         """
-        return self.nbt['Count']
+        return self.nbt['Count'].value
     
 
     def get_durability(self) -> int:
         """
         Get the durability of this item as the amount of damage done to it.
 
         :return: The damage done to this item
@@ -255,15 +277,15 @@
     
     def set_count(self, count: int):
         """
         Set the count of this item.
 
         :param int count: The count to set.
         """
-        self.nbt['Count'] = count
+        self.nbt['Count'] = _TypedInt(count, 'b')
     
 
     def set_durability(self, damage: int):
         """
         Set the durability damage of this item
 
         :param int damage: The amount of damage to set.
@@ -315,15 +337,15 @@
         """
         Set an enchantment on this item.
 
         :param str enchant_id: The ID of the enchantment to set.
         :param int enchant_level: The level of the enchantment to set.
         """
         self.nbt['tag'].set_list('Enchantments')
-        self.nbt['tag']['Enchantments'].append({'id': f'minecraft:{enchant_id}', 'lvl': TypedInt(enchant_level, 's')})
+        self.nbt['tag']['Enchantments'].append({'id': f'minecraft:{enchant_id}', 'lvl': _TypedInt(enchant_level, 's')})
     
 
     def set_shulker_box_item(self, item, slot: int=-1):
         """
         Set an item in this shulker box.
 
         :param Item item: The item to set.
@@ -412,15 +434,15 @@
         self.nbt['tag'][tag_name] = tag_value
 
     
     def _format_as_nbt(self, value) -> str:
         if isinstance(value, int):
             return f'{value}b'
         
-        if isinstance(value, TypedInt):
+        if isinstance(value, _TypedInt):
             return f'{value.value}{value.type}'
 
         if isinstance(value, float):
             return f'{value}d'
         
         if isinstance(value, _RawTagValue):
             return str(value)
@@ -464,15 +486,15 @@
         """
         if method == 'recode':
             return send_recode(self)
         if method == 'codeclient':
             return send_codeclient(self)
         return -1
 
-
+# TODO: change "template sent successfully" message into a more generic item sent message
 def send_recode(item: Item) -> int:
     """
     Sends a template to DiamondFire via recode item api.
 
     :param str templateCode: The code for the template as a base64 string.
     :param str name: The name of the template.
     :param str author: The author of the template.
@@ -529,7 +551,33 @@
             print(f'    - Minecraft is not open')
             print(f'    - CodeClient is not installed (get it here: https://modrinth.com/mod/codeclient)')
             print(f'    - CodeClient API is not enabled (enable it in CodeClient general settings)')
             return 1
         
         print(f'Connection failed: {e}')
         return 2
+
+
+def convert_nbt_tag(nbt_tag: nbtlib.Base):
+    """
+    Converts nbtlib tags into mcitemlib objects
+    """
+    if isinstance(nbt_tag, nbtlib.Compound):
+        unpacked = nbt_tag.unpack()
+        if 'text' in unpacked:
+            return StyledString.from_nbt_dict(unpacked)
+        new_tag = {}
+        for k, v in nbt_tag.items():
+            if ':' in k:    # bad fix for Diamondfire custom item tags
+                k = _RawTagValue(f'"{k}"')
+            new_tag[k] = convert_nbt_tag(v)
+        return AutoDict(new_tag)
+    elif isinstance(nbt_tag, nbtlib.List):
+        return [convert_nbt_tag(t) for t in nbt_tag]
+    elif isinstance(nbt_tag, nbtlib.Numeric):
+        return _TypedInt(nbt_tag.unpack(), nbt_tag.suffix)
+    elif isinstance(nbt_tag, nbtlib.String):
+        try:
+            return StyledString.from_nbt(nbt_tag.unpack())
+        except PyNbtStyleException:
+            return nbt_tag.unpack()
+    return nbt_tag.unpack()
```

### Comparing `mcitemlib-0.1.3/mcitemlib/style.py` & `mcitemlib-0.2.0/mcitemlib/style.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Functions related to styling text.
 """
 
 import re
-from typing import List
+import json
+from typing import List, Any
 
 
 class PyNbtStyleException(Exception):
     pass
 
 STYLE_CODE_REGEX = r'(&([0-9A-Fa-fklmnorKLMNOR]|x&[0-9A-Fa-f]&[0-9A-Fa-f]&[0-9A-Fa-f]&[0-9A-Fa-f]&[0-9A-Fa-f]&[0-9A-Fa-f]))+'
 
@@ -40,14 +41,32 @@
 
 KEPT_FORMATTING = {
     'text',
     'italic',
 }
 
 
+def _some_or(value: Any, none_value: Any):
+    """
+    Returns `none_value` if `value` is None, otherwise returns `value`.
+    """
+    if value is None:
+        return none_value
+    return value
+
+
+def _add_new_keys(d1: dict, d2: dict):
+    """
+    Sets keys from `d2` into `d1` but only if the key doesn't already exist in `d1`.
+    """
+    for k, v in d2.items():
+        if k not in d1:
+            d1[k] = v
+
+
 def _add_quote_escapes(string: str):
     new_string_list = []
     for c in string:
         if c == '"':
             new_string_list.append(r'\\"')
         elif c == "'":
             new_string_list.append(r'\'')
@@ -133,14 +152,28 @@
             elif c == 'x':
                 sub.data['color'] = f'#{raw_code[i+1:i+7].upper()}'
                 i += 6
             else:
                 raise PyNbtStyleException(f'Unexpected format character "{c}" found in substring.')
             i += 1
         return sub
+    
+
+    @staticmethod
+    def from_nbt(nbt: str|dict):
+        style_data = nbt
+        if isinstance(nbt, str):
+            style_data = json.loads(nbt)
+        bold = _some_or(style_data.get('bold'), False)
+        italic = _some_or(style_data.get('italic'), False)
+        underlined = _some_or(style_data.get('underlined'), False)
+        strikethrough = _some_or(style_data.get('strikethrough'), False)
+        obfuscated = _some_or(style_data.get('obfuscated'), False)
+
+        return StyledSubstring(style_data['text'], style_data.get('color'), bold, italic, underlined, strikethrough, obfuscated)
 
     
     def format(self) -> str:
         format_data = {}
         for key, value in self.data.items():
             if value or key in KEPT_FORMATTING:
                 format_data[key] = value
@@ -150,15 +183,15 @@
 
 class StyledString:
     def __init__(self, substrings: List[StyledSubstring]):
         self.substrings = substrings
     
 
     def __repr__(self):
-        return f'StyledString([{self.substrings}])'
+        return f'StyledString({self.substrings})'
 
 
     @staticmethod
     def from_codes(codes: str):
         pattern = re.compile(STYLE_CODE_REGEX)
         matches = list(pattern.finditer(codes))
         if len(matches) == 0:
@@ -183,14 +216,43 @@
 
 
     @staticmethod
     def from_string(string: str):
         return StyledString([StyledSubstring(string)])
     
 
+    @staticmethod
+    def from_nbt_dict(nbt_dict: dict):
+        if 'extra' in nbt_dict:
+            substrings = []
+            extra = nbt_dict['extra']
+            outside_extra = {k: v for k, v in nbt_dict.items() if k != 'extra'}
+            if nbt_dict['text'] != '':
+                substrings = [StyledSubstring.from_nbt(outside_extra)]
+            for substring_dict in extra:
+                if isinstance(substring_dict, str):
+                    substring_dict = {'text': substring_dict}
+                _add_new_keys(substring_dict, outside_extra)
+                substrings.extend(StyledString.from_nbt_dict(substring_dict).substrings)
+            return StyledString(substrings)
+
+        return StyledString([StyledSubstring.from_nbt(nbt_dict)])
+    
+
+    @staticmethod
+    def from_nbt(nbt: str):
+        try:
+            nbt_dict = json.loads(nbt)
+            if 'text' in nbt_dict:
+                return StyledString.from_nbt_dict(nbt_dict)
+            raise PyNbtStyleException('String is not a formatted styled string.')
+        except json.JSONDecodeError:
+            raise PyNbtStyleException('Invalid JSON string.')
+        
+
     def to_string(self) -> str:
         """
         Returns an unformatted representation of this string.
         """
         return ''.join([sub.data['text'] for sub in self.substrings])
```

### Comparing `mcitemlib-0.1.3/PKG-INFO` & `mcitemlib-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: mcitemlib
-Version: 0.1.3
+Version: 0.2.0
 Summary: A library for creating and editing Minecraft items using python.
 Home-page: https://github.com/Amp63/mcitemlib
 License: MIT
-Keywords: minecraft,item,block
+Keywords: minecraft,item,block,nbt
 Author: Amp
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: nbtlib (>=2.0.4,<3.0.0)
 Project-URL: Repository, https://github.com/Amp63/mcitemlib
 Description-Content-Type: text/markdown
 
 # mcitemlib
 
 A library for creating and editing Minecraft items using python.
```

