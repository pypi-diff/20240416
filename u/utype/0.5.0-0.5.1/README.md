# Comparing `tmp/utype-0.5.0.tar.gz` & `tmp/utype-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utype-0.5.0.tar", last modified: Sat Mar 30 15:31:34 2024, max compression
+gzip compressed data, was "utype-0.5.1.tar", last modified: Tue Apr 16 02:45:21 2024, max compression
```

## Comparing `utype-0.5.0.tar` & `utype-0.5.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-03-30 15:31:34.197128 utype-0.5.0/
--rw-rw-rw-   0        0        0      588 2022-11-30 10:26:26.000000 utype-0.5.0/LICENSE
--rw-rw-rw-   0        0        0    10191 2024-03-30 15:31:34.197128 utype-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     8759 2024-01-09 06:17:39.000000 utype-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-30 15:31:34.123948 utype-0.5.0/examples/
--rw-rw-rw-   0        0        0        0 2024-01-27 10:18:42.000000 utype-0.5.0/examples/__init__.py
--rw-rw-rw-   0        0        0       42 2024-03-30 15:31:34.197128 utype-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1824 2022-12-16 10:42:48.000000 utype-0.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-30 15:31:34.131926 utype-0.5.0/utype/
--rw-rw-rw-   0        0        0     1231 2024-03-30 15:30:29.000000 utype-0.5.0/utype/__init__.py
--rw-rw-rw-   0        0        0     6219 2023-02-18 08:54:07.000000 utype-0.5.0/utype/decorator.py
-drwxrwxrwx   0        0        0        0 2024-03-30 15:31:34.158854 utype-0.5.0/utype/parser/
--rw-rw-rw-   0        0        0        0 2022-12-02 05:43:17.000000 utype-0.5.0/utype/parser/__init__.py
--rw-rw-rw-   0        0        0    23012 2024-02-22 10:40:50.000000 utype-0.5.0/utype/parser/base.py
--rw-rw-rw-   0        0        0    22768 2024-03-28 04:21:05.000000 utype-0.5.0/utype/parser/cls.py
--rw-rw-rw-   0        0        0    48651 2024-03-29 04:45:00.000000 utype-0.5.0/utype/parser/field.py
--rw-rw-rw-   0        0        0    36928 2023-12-19 13:21:17.000000 utype-0.5.0/utype/parser/func.py
--rw-rw-rw-   0        0        0    16412 2023-04-08 06:18:37.000000 utype-0.5.0/utype/parser/options.py
--rw-rw-rw-   0        0        0    67642 2024-02-24 04:49:43.000000 utype-0.5.0/utype/parser/rule.py
--rw-rw-rw-   0        0        0    18029 2024-02-22 10:45:55.000000 utype-0.5.0/utype/schema.py
-drwxrwxrwx   0        0        0        0 2024-03-30 15:31:34.160849 utype-0.5.0/utype/specs/
--rw-rw-rw-   0        0        0        0 2022-11-30 10:26:26.000000 utype-0.5.0/utype/specs/__init__.py
--rw-rw-rw-   0        0        0    14846 2024-03-29 03:44:08.000000 utype-0.5.0/utype/specs/json_schema.py
--rw-rw-rw-   0        0        0     5515 2023-03-19 14:44:00.000000 utype-0.5.0/utype/types.py
-drwxrwxrwx   0        0        0        0 2024-03-30 15:31:34.196135 utype-0.5.0/utype/utils/
--rw-rw-rw-   0        0        0        0 2022-11-30 10:26:26.000000 utype-0.5.0/utype/utils/__init__.py
--rw-rw-rw-   0        0        0     3676 2023-03-04 11:33:54.000000 utype-0.5.0/utype/utils/base.py
--rw-rw-rw-   0        0        0     3278 2024-03-01 09:02:51.000000 utype-0.5.0/utype/utils/compat.py
--rw-rw-rw-   0        0        0     2017 2022-12-16 09:30:29.000000 utype-0.5.0/utype/utils/datastructures.py
--rw-rw-rw-   0        0        0     3786 2024-03-01 07:29:41.000000 utype-0.5.0/utype/utils/encode.py
--rw-rw-rw-   0        0        0     7863 2024-02-22 10:54:09.000000 utype-0.5.0/utype/utils/example.py
--rw-rw-rw-   0        0        0     8483 2024-01-03 07:03:53.000000 utype-0.5.0/utype/utils/exceptions.py
--rw-rw-rw-   0        0        0     1621 2023-06-30 09:41:30.000000 utype-0.5.0/utype/utils/functional.py
--rw-rw-rw-   0        0        0     6219 2022-12-16 09:43:52.000000 utype-0.5.0/utype/utils/style.py
--rw-rw-rw-   0        0        0    24094 2024-01-03 08:18:27.000000 utype-0.5.0/utype/utils/transform.py
-drwxrwxrwx   0        0        0        0 2024-03-30 15:31:34.149878 utype-0.5.0/utype.egg-info/
--rw-rw-rw-   0        0        0    10191 2024-03-30 15:31:34.000000 utype-0.5.0/utype.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      703 2024-03-30 15:31:34.000000 utype-0.5.0/utype.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-30 15:31:34.000000 utype-0.5.0/utype.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-03-30 15:31:34.000000 utype-0.5.0/utype.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-03-30 15:31:34.000000 utype-0.5.0/utype.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 02:45:21.745885 utype-0.5.1/
+-rw-rw-rw-   0        0        0      588 2022-11-30 10:26:26.000000 utype-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0    10191 2024-04-16 02:45:21.745885 utype-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8759 2024-01-09 06:17:39.000000 utype-0.5.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 02:45:21.706990 utype-0.5.1/examples/
+-rw-rw-rw-   0        0        0        0 2024-01-27 10:18:42.000000 utype-0.5.1/examples/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-16 02:45:21.745885 utype-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1824 2022-12-16 10:42:48.000000 utype-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 02:45:21.708985 utype-0.5.1/utype/
+-rw-rw-rw-   0        0        0     1231 2024-04-16 02:36:41.000000 utype-0.5.1/utype/__init__.py
+-rw-rw-rw-   0        0        0     6219 2023-02-18 08:54:07.000000 utype-0.5.1/utype/decorator.py
+drwxrwxrwx   0        0        0        0 2024-04-16 02:45:21.728931 utype-0.5.1/utype/parser/
+-rw-rw-rw-   0        0        0        0 2022-12-02 05:43:17.000000 utype-0.5.1/utype/parser/__init__.py
+-rw-rw-rw-   0        0        0    23012 2024-02-22 10:40:50.000000 utype-0.5.1/utype/parser/base.py
+-rw-rw-rw-   0        0        0    22768 2024-03-28 04:21:05.000000 utype-0.5.1/utype/parser/cls.py
+-rw-rw-rw-   0        0        0    48651 2024-03-29 04:45:00.000000 utype-0.5.1/utype/parser/field.py
+-rw-rw-rw-   0        0        0    36928 2023-12-19 13:21:17.000000 utype-0.5.1/utype/parser/func.py
+-rw-rw-rw-   0        0        0    16412 2023-04-08 06:18:37.000000 utype-0.5.1/utype/parser/options.py
+-rw-rw-rw-   0        0        0    67750 2024-04-16 02:41:01.000000 utype-0.5.1/utype/parser/rule.py
+-rw-rw-rw-   0        0        0    18029 2024-02-22 10:45:55.000000 utype-0.5.1/utype/schema.py
+drwxrwxrwx   0        0        0        0 2024-04-16 02:45:21.729928 utype-0.5.1/utype/specs/
+-rw-rw-rw-   0        0        0        0 2022-11-30 10:26:26.000000 utype-0.5.1/utype/specs/__init__.py
+-rw-rw-rw-   0        0        0    14933 2024-03-31 08:20:40.000000 utype-0.5.1/utype/specs/json_schema.py
+-rw-rw-rw-   0        0        0     5515 2024-04-03 15:29:32.000000 utype-0.5.1/utype/types.py
+drwxrwxrwx   0        0        0        0 2024-04-16 02:45:21.744894 utype-0.5.1/utype/utils/
+-rw-rw-rw-   0        0        0        0 2022-11-30 10:26:26.000000 utype-0.5.1/utype/utils/__init__.py
+-rw-rw-rw-   0        0        0     3676 2023-03-04 11:33:54.000000 utype-0.5.1/utype/utils/base.py
+-rw-rw-rw-   0        0        0     3381 2024-04-16 02:41:01.000000 utype-0.5.1/utype/utils/compat.py
+-rw-rw-rw-   0        0        0     2017 2022-12-16 09:30:29.000000 utype-0.5.1/utype/utils/datastructures.py
+-rw-rw-rw-   0        0        0     3928 2024-04-04 11:29:24.000000 utype-0.5.1/utype/utils/encode.py
+-rw-rw-rw-   0        0        0     7863 2024-02-22 10:54:09.000000 utype-0.5.1/utype/utils/example.py
+-rw-rw-rw-   0        0        0     8483 2024-01-03 07:03:53.000000 utype-0.5.1/utype/utils/exceptions.py
+-rw-rw-rw-   0        0        0     1621 2023-06-30 09:41:30.000000 utype-0.5.1/utype/utils/functional.py
+-rw-rw-rw-   0        0        0     6219 2022-12-16 09:43:52.000000 utype-0.5.1/utype/utils/style.py
+-rw-rw-rw-   0        0        0    24094 2024-01-03 08:18:27.000000 utype-0.5.1/utype/utils/transform.py
+drwxrwxrwx   0        0        0        0 2024-04-16 02:45:21.724945 utype-0.5.1/utype.egg-info/
+-rw-rw-rw-   0        0        0    10191 2024-04-16 02:45:21.000000 utype-0.5.1/utype.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      703 2024-04-16 02:45:21.000000 utype-0.5.1/utype.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 02:45:21.000000 utype-0.5.1/utype.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-16 02:45:21.000000 utype-0.5.1/utype.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-16 02:45:21.000000 utype-0.5.1/utype.egg-info/top_level.txt
```

### Comparing `utype-0.5.0/LICENSE` & `utype-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `utype-0.5.0/PKG-INFO` & `utype-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utype
-Version: 0.5.0
+Version: 0.5.1
 Summary: Declare & parse types / dataclasses / functions based on Python type annotations
 Home-page: https://utype.io
 Author: XuLin Zhou
 Author-email: zxl@utilmeta.com
 License: Apache 2.0
 Project-URL: Project Home, https://utype.io
 Project-URL: Documentation, https://utype.io
```

### Comparing `utype-0.5.0/README.md` & `utype-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `utype-0.5.0/setup.py` & `utype-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `utype-0.5.0/utype/__init__.py` & `utype-0.5.1/utype/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from .utils.transform import (TypeTransformer, type_transform)
 from .utils.datastructures import unprovided
 from .specs.json_schema import JsonSchemaGenerator
 
 register_transformer = TypeTransformer.registry.register
 
 
-VERSION = (0, 5, 0, None)
+VERSION = (0, 5, 1, None)
 
 
 def _get_version():
     pre_release = VERSION[3] if len(VERSION) > 3 else ""
     version = ".".join([str(v) for v in VERSION[:3]])
     if pre_release:
         version += f"-{pre_release}"
```

### Comparing `utype-0.5.0/utype/decorator.py` & `utype-0.5.1/utype/decorator.py`

 * *Files identical despite different names*

### Comparing `utype-0.5.0/utype/parser/base.py` & `utype-0.5.1/utype/parser/base.py`

 * *Files identical despite different names*

### Comparing `utype-0.5.0/utype/parser/cls.py` & `utype-0.5.1/utype/parser/cls.py`

 * *Files identical despite different names*

### Comparing `utype-0.5.0/utype/parser/field.py` & `utype-0.5.1/utype/parser/field.py`

 * *Files identical despite different names*

### Comparing `utype-0.5.0/utype/parser/func.py` & `utype-0.5.1/utype/parser/func.py`

 * *Files identical despite different names*

### Comparing `utype-0.5.0/utype/parser/options.py` & `utype-0.5.1/utype/parser/options.py`

 * *Files identical despite different names*

### Comparing `utype-0.5.0/utype/parser/rule.py` & `utype-0.5.1/utype/parser/rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-import inspect
 import re
 import typing
 import warnings
 from collections import deque
 from decimal import Decimal
 from enum import Enum, EnumMeta
 from functools import partial
 from typing import (Any, AsyncGenerator, Callable, Dict, Generator, List,
                     Mapping, Optional, Tuple, Type, TypeVar, Union, Iterator)
 
 from ..utils import exceptions as exc
 from ..utils.compat import (ForwardRef, Literal, evaluate_forward_ref,
-                            get_args, get_origin)
+                            get_args, get_origin, UnionType)
 from ..utils.datastructures import unprovided
 from ..utils.functional import multi, pop
 from ..utils.transform import TypeTransformer
 from .options import RuntimeContext
 
 T = typing.TypeVar("T")
 OTHER = TypeVar("OTHER")
@@ -1303,15 +1302,16 @@
                     continue
                 args.append(annotation)
 
         # if not args and not constraints:
         #     return type_
 
         name = cls.__name__
-        if type_ == Union:
+        if type_ == Union or type_ == UnionType:
+            # in Python >= 3.10, native logic operator like int | str will be a UnionType
             type_ = LogicalType.any_of(*args)
             # clear the args for union
             args = []
 
         if isinstance(type_, LogicalType):
             # if type_.combinator:
             #     # we cannot directly inherit combined rules
```

### Comparing `utype-0.5.0/utype/schema.py` & `utype-0.5.1/utype/schema.py`

 * *Files identical despite different names*

### Comparing `utype-0.5.0/utype/specs/json_schema.py` & `utype-0.5.1/utype/specs/json_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,15 +261,17 @@
 
         extra = getattr(t, 'extra', None)
         if extra and isinstance(extra, dict):
             data.update(extra)
         if t.__args__:
             data.update(self._get_args(t))
         if isinstance(self.defs, dict) and name != 'Rule':
-            return {"$ref": f"{self.ref_prefix}{self.set_def(name, t, data)}"}
+            if '<locals>' not in name:
+                # not a auto created rule
+                return {"$ref": f"{self.ref_prefix}{self.set_def(name, t, data)}"}
         return data
 
     def get_def_name(self, t: type):
         if t in self.defs:
             for k, v in self.names.items():
                 if v == t:
                     return k
```

### Comparing `utype-0.5.0/utype/types.py` & `utype-0.5.1/utype/types.py`

 * *Files identical despite different names*

### Comparing `utype-0.5.0/utype/utils/base.py` & `utype-0.5.1/utype/utils/base.py`

 * *Files identical despite different names*

### Comparing `utype-0.5.0/utype/utils/compat.py` & `utype-0.5.1/utype/utils/compat.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,19 @@
 
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 
 try:
+    from types import UnionType
+except ImportError:
+    UnionType = Union
+
+try:
     from typing import Final
 except ImportError:
     from typing_extensions import Final
 
 try:
     from typing import Annotated
 except ImportError:
@@ -23,14 +28,15 @@
 
 
 __all__ = [
     "get_origin",
     "get_args",
     'Literal',
     'Final',
+    'UnionType',
     "ForwardRef",
     "Annotated",
     "is_final",
     "is_union",
     "is_classvar",
     "is_annotated",
     "evaluate_forward_ref",
```

### Comparing `utype-0.5.0/utype/utils/datastructures.py` & `utype-0.5.1/utype/utils/datastructures.py`

 * *Files identical despite different names*

### Comparing `utype-0.5.0/utype/utils/encode.py` & `utype-0.5.1/utype/utils/encode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import decimal
+import io
 import uuid
 from collections.abc import Mapping
 from datetime import date, datetime, time, timedelta
 from enum import Enum
 from typing import Union
 from .base import TypeRegistry
 import json
@@ -90,14 +91,19 @@
 
 
 @register_encoder(bytes)
 def from_bytes(data: bytes):
     return data.decode("utf-8", errors="replace")
 
 
+@register_encoder(io.BytesIO)
+def from_bytes_io(data: io.BytesIO):
+    return data.read().decode("utf-8", errors="replace")
+
+
 @register_encoder(date)
 def from_datetime(data: Union[datetime, date]):
     return data.isoformat()
 
 
 @register_encoder(IPv4Network, IPv4Address, IPv6Network, IPv6Address)
 def from_ip(data):
```

### Comparing `utype-0.5.0/utype/utils/example.py` & `utype-0.5.1/utype/utils/example.py`

 * *Files identical despite different names*

### Comparing `utype-0.5.0/utype/utils/exceptions.py` & `utype-0.5.1/utype/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `utype-0.5.0/utype/utils/functional.py` & `utype-0.5.1/utype/utils/functional.py`

 * *Files identical despite different names*

### Comparing `utype-0.5.0/utype/utils/style.py` & `utype-0.5.1/utype/utils/style.py`

 * *Files identical despite different names*

### Comparing `utype-0.5.0/utype/utils/transform.py` & `utype-0.5.1/utype/utils/transform.py`

 * *Files identical despite different names*

### Comparing `utype-0.5.0/utype.egg-info/PKG-INFO` & `utype-0.5.1/utype.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utype
-Version: 0.5.0
+Version: 0.5.1
 Summary: Declare & parse types / dataclasses / functions based on Python type annotations
 Home-page: https://utype.io
 Author: XuLin Zhou
 Author-email: zxl@utilmeta.com
 License: Apache 2.0
 Project-URL: Project Home, https://utype.io
 Project-URL: Documentation, https://utype.io
```

### Comparing `utype-0.5.0/utype.egg-info/SOURCES.txt` & `utype-0.5.1/utype.egg-info/SOURCES.txt`

 * *Files identical despite different names*

