# Comparing `tmp/netsome-0.3.1.tar.gz` & `tmp/netsome-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netsome-0.3.1.tar", max compression
+gzip compressed data, was "netsome-0.3.2.tar", max compression
```

## Comparing `netsome-0.3.1.tar` & `netsome-0.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1286 2024-04-10 20:10:43.205830 netsome-0.3.1/LICENSE
--rw-r--r--   0        0        0      355 2024-04-10 20:11:01.192038 netsome-0.3.1/README.md
--rw-r--r--   0        0        0        0 2024-03-27 19:13:03.131810 netsome-0.3.1/netsome/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 20:10:43.207381 netsome-0.3.1/netsome/_converters/__init__.py
--rw-r--r--   0        0        0      940 2024-04-10 20:10:43.208074 netsome-0.3.1/netsome/_converters/bgp.py
--rw-r--r--   0        0        0      321 2024-04-10 20:10:43.208868 netsome-0.3.1/netsome/_converters/ipv4.py
--rw-r--r--   0        0        0      284 2024-04-10 20:10:43.209946 netsome-0.3.1/netsome/constants.py
--rw-r--r--   0        0        0        0 2024-04-10 20:10:43.210124 netsome-0.3.1/netsome/pools/__init__.py
--rw-r--r--   0        0        0      125 2024-04-10 20:10:43.210773 netsome-0.3.1/netsome/pools/bgp.py
--rw-r--r--   0        0        0     1027 2024-04-10 20:10:43.211302 netsome-0.3.1/netsome/pools/ipv4.py
--rw-r--r--   0        0        0     1409 2024-04-10 20:10:43.211781 netsome-0.3.1/netsome/pools/number.py
--rw-r--r--   0        0        0      130 2024-04-10 20:10:43.212210 netsome-0.3.1/netsome/pools/vlans.py
--rw-r--r--   0        0        0        0 2024-04-08 18:56:12.740789 netsome-0.3.1/netsome/types/__init__.py
--rw-r--r--   0        0        0     2191 2024-04-10 20:10:43.213168 netsome-0.3.1/netsome/types/bgp.py
--rw-r--r--   0        0        0     4014 2024-04-10 20:10:43.214313 netsome-0.3.1/netsome/types/ipv4.py
--rw-r--r--   0        0        0      848 2024-04-10 20:10:43.216655 netsome-0.3.1/netsome/types/vlans.py
--rw-r--r--   0        0        0        0 2024-04-06 10:10:11.723380 netsome-0.3.1/netsome/validators/__init__.py
--rw-r--r--   0        0        0     1654 2024-04-10 20:10:43.218579 netsome-0.3.1/netsome/validators/bgp.py
--rw-r--r--   0        0        0     2024 2024-04-10 20:10:43.219606 netsome-0.3.1/netsome/validators/ipv4.py
--rw-r--r--   0        0        0      289 2024-04-10 20:10:43.220448 netsome-0.3.1/netsome/validators/vlans.py
--rw-r--r--   0        0        0     1262 2024-04-10 20:11:11.836463 netsome-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1182 1970-01-01 00:00:00.000000 netsome-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1286 2024-04-11 18:59:46.819718 netsome-0.3.2/LICENSE
+-rw-r--r--   0        0        0      355 2024-04-15 07:10:06.582777 netsome-0.3.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-11 18:59:46.820411 netsome-0.3.2/netsome/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 18:59:46.820647 netsome-0.3.2/netsome/_converters/__init__.py
+-rw-r--r--   0        0        0      967 2024-04-15 07:10:54.993891 netsome-0.3.2/netsome/_converters/bgp.py
+-rw-r--r--   0        0        0      343 2024-04-15 07:10:54.994197 netsome-0.3.2/netsome/_converters/ipv4.py
+-rw-r--r--   0        0        0      662 2024-04-15 18:22:42.950755 netsome-0.3.2/netsome/constants.py
+-rw-r--r--   0        0        0        0 2024-04-11 18:59:46.821874 netsome-0.3.2/netsome/pools/__init__.py
+-rw-r--r--   0        0        0      125 2024-04-11 18:59:46.822131 netsome-0.3.2/netsome/pools/bgp.py
+-rw-r--r--   0        0        0     1027 2024-04-16 07:37:52.154983 netsome-0.3.2/netsome/pools/ipv4.py
+-rw-r--r--   0        0        0     1409 2024-04-11 18:59:46.822516 netsome-0.3.2/netsome/pools/number.py
+-rw-r--r--   0        0        0      130 2024-04-11 18:59:46.822953 netsome-0.3.2/netsome/pools/vlans.py
+-rw-r--r--   0        0        0        0 2024-04-11 18:59:46.823365 netsome-0.3.2/netsome/types/__init__.py
+-rw-r--r--   0        0        0     2219 2024-04-15 07:10:54.995099 netsome-0.3.2/netsome/types/bgp.py
+-rw-r--r--   0        0        0     4510 2024-04-15 07:10:55.013884 netsome-0.3.2/netsome/types/ipv4.py
+-rw-r--r--   0        0        0      906 2024-04-15 07:10:55.014565 netsome-0.3.2/netsome/types/vlans.py
+-rw-r--r--   0        0        0        0 2024-04-11 18:59:46.824730 netsome-0.3.2/netsome/validators/__init__.py
+-rw-r--r--   0        0        0     2022 2024-04-15 18:35:57.465187 netsome-0.3.2/netsome/validators/bgp.py
+-rw-r--r--   0        0        0     2112 2024-04-15 19:18:19.904520 netsome-0.3.2/netsome/validators/ipv4.py
+-rw-r--r--   0        0        0      381 2024-04-15 07:10:55.016488 netsome-0.3.2/netsome/validators/vlans.py
+-rw-r--r--   0        0        0     1262 2024-04-16 07:37:58.242228 netsome-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1284 1970-01-01 00:00:00.000000 netsome-0.3.2/PKG-INFO
```

### Comparing `netsome-0.3.1/LICENSE` & `netsome-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `netsome-0.3.1/netsome/_converters/bgp.py` & `netsome-0.3.2/netsome/_converters/bgp.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 from netsome import constants as c
 
 
 def asdotplus_to_asplain(string: str) -> int:
-    high_order, low_order = map(int, string.split(c.DOT, maxsplit=1))
-    return high_order * c.TWO_BYTES + low_order
+    high_order, low_order = map(int, string.split(c.DELIMITERS.DOT, maxsplit=1))
+    return high_order * c.BYTES.TWO + low_order
 
 
 def asdot_to_asplain(string: str) -> int:
-    if c.DOT in string:
+    if c.DELIMITERS.DOT in string:
         return asdotplus_to_asplain(string)
 
     return int(string)
 
 
 def asplain_to_asdot(number: int) -> str:
-    high_order, low_order = divmod(number, c.TWO_BYTES)
-    return f"{high_order}{c.DOT}{low_order}" if high_order else str(low_order)
+    high_order, low_order = divmod(number, c.BYTES.TWO)
+    if high_order:
+        return c.DELIMITERS.DOT.join_as_str((high_order, low_order))
+
+    return str(low_order)
 
 
 def asplain_to_asdotplus(number: int) -> str:
-    high_order, low_order = divmod(number, c.TWO_BYTES)
-    return f"{high_order}{c.DOT}{low_order}"
+    return c.DELIMITERS.DOT.join_as_str(divmod(number, c.BYTES.TWO))
 
 
 def asplain_to_community(number: int) -> str:
-    asn, value = divmod(number, c.TWO_BYTES)
-    return f"{asn}{c.COLON}{value}"
+    return c.DELIMITERS.COLON.join_as_str(divmod(number, c.BYTES.TWO))
 
 
 def community_to_asplain(string: str) -> int:
-    asn, value = map(int, string.split(c.COLON, maxsplit=1))
-    return asn * c.TWO_BYTES + value
+    asn, value = map(int, string.split(c.DELIMITERS.COLON, maxsplit=1))
+    return asn * c.BYTES.TWO + value
```

### Comparing `netsome-0.3.1/netsome/pools/ipv4.py` & `netsome-0.3.2/netsome/pools/ipv4.py`

 * *Files identical despite different names*

### Comparing `netsome-0.3.1/netsome/pools/number.py` & `netsome-0.3.2/netsome/pools/number.py`

 * *Files identical despite different names*

### Comparing `netsome-0.3.1/netsome/types/bgp.py` & `netsome-0.3.2/netsome/types/bgp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 import typing as t
 
 from netsome import constants as c
-from netsome._converters import bgp as converters
-from netsome.validators import bgp as validators
+from netsome._converters import bgp as convs
+from netsome.validators import bgp as valids
 
 # TODO(kuderr): can move some common stuff to Base class
 
 
 class ASN:
+
+    MIN = c.BGP.ASN_MIN
+    MAX = c.BGP.ASN_MAX
+    ORDER_MAX = c.BGP.ASN_ORDER_MAX
+
     def __init__(self, number: int) -> None:
-        validators.validate_asplain(number)
+        valids.validate_asplain(number)
         self._number = number
 
     @classmethod
     def from_asdot(cls, string: str) -> "ASN":
-        validators.validate_asdot(string)
-        return cls(converters.asdot_to_asplain(string))
+        valids.validate_asdot(string)
+        return cls(convs.asdot_to_asplain(string))
 
     @classmethod
     def from_asdotplus(cls, string: str) -> "ASN":
-        validators.validate_asdotplus(string)
-        return cls(converters.asdotplus_to_asplain(string))
+        valids.validate_asdotplus(string)
+        return cls(convs.asdotplus_to_asplain(string))
 
     @classmethod
     def from_asplain(cls, number: int) -> "ASN":
-        validators.validate_asplain(number)
+        valids.validate_asplain(number)
         return cls(number)
 
     def to_asdot(self):
-        return converters.asplain_to_asdot(self._number)
+        return convs.asplain_to_asdot(self._number)
 
     def to_asdotplus(self):
-        return converters.asplain_to_asdotplus(self._number)
+        return convs.asplain_to_asdotplus(self._number)
 
     def to_asplain(self):
         return self._number
 
     def __eq__(self, other: t.Any) -> bool:
         return isinstance(other, self.__class__) and (self._number == other._number)
 
@@ -47,21 +52,21 @@
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self._number})"
 
 
 class Community:
     def __init__(self, number: int) -> None:
-        validators.validate_asplain(number)
+        valids.validate_asplain(number)
         self._number = number
 
     @classmethod
     def from_str(cls, value: str) -> "Community":
-        validators.validate_community(value)
-        return cls(converters.community_to_asplain(value))
+        valids.validate_community(value)
+        return cls(convs.community_to_asplain(value))
 
     def __eq__(self, other: t.Any) -> bool:
         return isinstance(other, self.__class__) and (self._number == other._number)
 
     def __lt__(self, other: t.Any) -> bool:
         return isinstance(other, self.__class__) and (self._number < other._number)
```

### Comparing `netsome-0.3.1/netsome/types/vlans.py` & `netsome-0.3.2/netsome/types/vlans.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import typing as t
 
 from netsome import constants as c
-from netsome.validators import vlans as validators
+from netsome.validators import vlans as valids
 
 
 class VID:
     """VLAN ID"""
 
-    _RESERVED = {c.ZERO, c.DEFAULT_VID, c.VID_MAX}
+    MIN = c.VLAN.VID_MIN
+    MAX = c.VLAN.VID_MAX
+    DEFAULT = c.VLAN.VID_DEFAULT
+
+    RESERVED = {MIN, DEFAULT, MAX}
 
     def __init__(self, vid: int) -> None:
-        validators.validate_vid(vid)
+        valids.validate_vid(vid)
         self._vid = vid
 
     def __eq__(self, other: t.Any) -> bool:
         return isinstance(other, self.__class__) and (self._vid == other._vid)
 
     def __lt__(self, other: t.Any) -> bool:
         return isinstance(other, self.__class__) and (self._vid < other._vid)
@@ -22,11 +26,11 @@
     def __hash__(self) -> int:
         return hash(self._vid)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self._vid})"
 
     def is_reserved(self) -> bool:
-        return self._vid in self._RESERVED
+        return self._vid in self.RESERVED
 
     def is_default(self) -> bool:
-        return self._vid == c.DEFAULT_VID
+        return self._vid == self.DEFAULT
```

### Comparing `netsome-0.3.1/netsome/validators/ipv4.py` & `netsome-0.3.2/netsome/validators/ipv4.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from netsome import constants as c
 
 
 def validate_address_str(string: str):
     if not isinstance(string, str):
         raise TypeError("Invalid type")
 
-    octets = string.split(c.DOT)
+    octets = tuple(map(int, string.split(c.DELIMITERS.DOT)))
     if len(octets) != 4:
         raise ValueError()
 
     for octet in octets:
-        validate_octet_str(octet)
+        validate_octet_int(octet)
 
 
 def validate_address_int(number: int) -> None:
     if not isinstance(number, int):
         raise TypeError("Invalid type")
 
-    if not (c.ZERO <= number <= c.IPV4_MAX):
+    if not (c.IPV4.ADDRESS_MIN <= number <= c.IPV4.ADDRESS_MAX):
         raise ValueError("Invalid value")
 
 
 def validate_octet_str(string: str) -> None:
     if not isinstance(string, str):
         raise TypeError("Invalid type")
 
@@ -34,15 +34,15 @@
     validate_octet_int(int(string))
 
 
 def validate_octet_int(number: int) -> None:
     if not isinstance(number, int):
         raise TypeError("Invalid type")
 
-    if not (c.ZERO <= number <= c.IPV4_OCTET_MAX):
+    if not (c.IPV4.OCTET_MIN <= number <= c.IPV4.OCTET_MAX):
         raise ValueError("Invalid value")
 
 
 def validate_prefixlen_str(string: str) -> None:
     if not isinstance(string, str):
         raise TypeError()
 
@@ -52,21 +52,21 @@
 
     validate_prefixlen_int(int(string))
 
 
 # TODO(dm.a.kudryavtsev): можно сделать общим валидатором на значение
 def validate_prefixlen_int(
     number: int,
-    min_len: int = c.ZERO,
-    max_len: int = c.IPV4_PREFIXLEN_MAX,
+    min_len: int = c.IPV4.PREFIXLEN_MIN,
+    max_len: int = c.IPV4.PREFIXLEN_MAX,
 ) -> None:
     if not isinstance(number, int):
         raise TypeError()
 
     if not (min_len <= number <= max_len):
         raise ValueError()
 
 
 def validate_network_int(address: int, prefixlen: int):
-    netmask = c.IPV4_MAX ^ (c.IPV4_MAX >> prefixlen)
+    netmask = c.IPV4.ADDRESS_MAX ^ (c.IPV4.ADDRESS_MAX >> prefixlen)
     if address & netmask != address:
         raise ValueError("host bits set")
```

### Comparing `netsome-0.3.1/pyproject.toml` & `netsome-0.3.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -26,23 +26,23 @@
 ]
 description = "The one and only library to make your network code handsome"
 keywords = ["library", "network"]
 license = "X11 License Distribution Modification Variant"
 name = "netsome"
 readme = "README.md"
 repository = "https://github.com/kuderr/netsome"
-version = "0.3.1"
+version = "0.3.2"
 
 [tool.poetry.dependencies]
-python = "^3.12"
+python = "^3.10"
 sortedcontainers = "^2.4.0"
 
 [tool.poetry.group.dev.dependencies]
 poethepoet = "^0.25.0"
 pytest = "^8.1.1"
 pytest-cov = "^5.0.0"
-toml-sort = "^0.23.1"
 ruff = "^0.3.5"
+toml-sort = "^0.23.1"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/kuderr/netsome/issues"
 "Homepage" = "https://github.com/kuderr/netsome"
```

### Comparing `netsome-0.3.1/PKG-INFO` & `netsome-0.3.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: netsome
-Version: 0.3.1
+Version: 0.3.2
 Summary: The one and only library to make your network code handsome
 Home-page: https://github.com/kuderr/netsome
 License: X11-distribute-modifications-variant
 Keywords: library,network
 Author: kuderr
 Author-email: dakudryavcev@gmail.com
-Requires-Python: >=3.12,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Networking
 Requires-Dist: sortedcontainers (>=2.4.0,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/kuderr/netsome/issues
 Project-URL: Repository, https://github.com/kuderr/netsome
 Description-Content-Type: text/markdown
```

