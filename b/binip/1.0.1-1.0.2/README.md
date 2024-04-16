# Comparing `tmp/binip-1.0.1.tar.gz` & `tmp/binip-1.0.2.tar.gz`

## Comparing `binip-1.0.1.tar` & `binip-1.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 binip-1.0.1/.vscode/settings.json
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 binip-1.0.1/src/binip/__init__.py
--rw-r--r--   0        0        0    43766 2020-02-02 00:00:00.000000 binip-1.0.1/src/binip/classes.py
--rw-r--r--   0        0        0    28261 2020-02-02 00:00:00.000000 binip-1.0.1/src/binip/functions.py
--rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 binip-1.0.1/tests/class_test.py
--rw-r--r--   0        0        0     5100 2020-02-02 00:00:00.000000 binip-1.0.1/tests/function_test.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 binip-1.0.1/LICENSE
--rw-r--r--   0        0        0     6388 2020-02-02 00:00:00.000000 binip-1.0.1/README.md
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 binip-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 binip-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 binip-1.0.2/.vscode/settings.json
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 binip-1.0.2/src/binip/__init__.py
+-rw-r--r--   0        0        0    43912 2020-02-02 00:00:00.000000 binip-1.0.2/src/binip/classes.py
+-rw-r--r--   0        0        0    28388 2020-02-02 00:00:00.000000 binip-1.0.2/src/binip/functions.py
+-rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 binip-1.0.2/tests/class_test.py
+-rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 binip-1.0.2/tests/function_test.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 binip-1.0.2/LICENSE
+-rw-r--r--   0        0        0     6350 2020-02-02 00:00:00.000000 binip-1.0.2/README.md
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 binip-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     8158 2020-02-02 00:00:00.000000 binip-1.0.2/PKG-INFO
```

### Comparing `binip-1.0.1/src/binip/classes.py` & `binip-1.0.2/src/binip/classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,14 +142,16 @@
             -----
             Returns
             ---
             expanded: str
                 Expanded IPv6 address.  Adds leading zeros and expands contraced zeros.
         '''
         split = address.split(':')
+        if address[-2:] == '::':
+            split.pop()
         zeros = ['0000' for i in range(0,9-len(split))]
         new_split = []
         for hexadecatet in split:
             if hexadecatet == '':
                 new_split += zeros
             elif hexadecatet == '0':
                 new_split.append('0000')
@@ -190,28 +192,30 @@
         i=0
         replacing_zeros = []
         while i < 8:
             zeros = []
             if ipv6_contracted[i] == '0':
                 zeros.append(i)
                 j=1
-                while ipv6_contracted[i+j] == '0':
+                while i+j < 8 and ipv6_contracted[i+j] == '0':
                     zeros.append(i+j)
                     j+=1
                 i+=j
                 if len(zeros) >= len(replacing_zeros):
                     replacing_zeros = zeros
             else:
                 i+=1
         #Replace first zeros with empty string and remove the rest
         ipv6_contracted[replacing_zeros[0]] = ''
         i = 0
         for item in replacing_zeros[1:]:
             ipv6_contracted.pop(item-i)
             i += 1
+        if ipv6_contracted[-1] == '':
+            ipv6_contracted.append('')
         contracted = ':'.join(ipv6_contracted)
         return contracted
     
     def binip(self) -> str:
         '''
             Given an IP will return the IP in binary format.  Works for both IPv4 and IPv6.
             -----
```

### Comparing `binip-1.0.1/src/binip/functions.py` & `binip-1.0.2/src/binip/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         Returns a RegEx pattern to match the given IPv6 subnet.
         -----
         Parameters
         ---
         subnet: Subnet class object
             Subnet to get RegEx pattern of.
         or_logic: str
-            Symbol to be used as OR, default it |.
+            Symbol to be used as OR, default is |.
         -----
         Returns
         ---
         regex: str
             RegEx pattern to match every IP address in the given IPv6subnet.
     '''
     subnet_split = subnet.split('/')
@@ -456,14 +456,16 @@
     if iptype == 'v4':
         raise ValueError('Invalid IP type: IP must be v6.')
     if '/' in ipv6:
         ipv6, mask = ipv6.split('/')[0], ipv6.split('/')[1]
     else:
         mask = ''
     split = ipv6.split(':')
+    if ipv6[-2:] == '::':
+        split.pop()
     zeros = ['0000' for i in range(0,9-len(split))]
     new_split = []
     for hexadecatet in split:
         if hexadecatet == '':
             new_split += zeros
         elif hexadecatet == '0':
             new_split.append('0000')
@@ -513,28 +515,30 @@
     i=0
     replacing_zeros = []
     while i < 8:
         zeros = []
         if ipv6_contracted[i] == '0':
             zeros.append(i)
             j=1
-            while ipv6_contracted[i+j] == '0':
+            while i+j < 8 and ipv6_contracted[i+j] == '0':
                 zeros.append(i+j)
                 j+=1
             i+=j
             if len(zeros) >= len(replacing_zeros):
                 replacing_zeros = zeros
         else:
             i+=1
     #Replace first zeros with empty string and remove the rest
     ipv6_contracted[replacing_zeros[0]] = ''
     i = 0
     for item in replacing_zeros[1:]:
         ipv6_contracted.pop(item-i)
         i += 1
+    if ipv6_contracted[-1] == '':
+        ipv6_contracted.append('')
     if mask == '':
         ipv6_contracted = ':'.join(ipv6_contracted)
     else:
         ipv6_contracted = ':'.join(ipv6_contracted) + '/' + mask
     return ipv6_contracted
 
 def ip2bin(ip: str):
```

### Comparing `binip-1.0.1/tests/class_test.py` & `binip-1.0.2/tests/class_test.py`

 * *Files identical despite different names*

### Comparing `binip-1.0.1/tests/function_test.py` & `binip-1.0.2/tests/function_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,17 +73,17 @@
     subnetv6 = 'ac43:34f:45bc:2c::12/64'
     expected = ['ac43:034f:45bc:002c:0000:0000:0000:0012', 'ac43:034f:45bc:002c:0000:0000:0000:0012/64']
     actual = [ipv6_expand(ipv6), ipv6_expand(subnetv6)]
     assert expected == actual, "ipv6_expand function fails IPv6 expansion."
 
 def test_ipv6_contract():
     '''Test the ipv6_contract function.'''
-    ipv6 = 'ac43:034f:45bc:002c:0000:0000:0000:0012'
-    subnetv6 = 'ac43:034f:45bc:002c:0000:0000:0000:0012/64'
-    expected = ['ac43:34f:45bc:2c::12', 'ac43:34f:45bc:2c::12/64']
+    ipv6 = 'ac43:034f:0000:002c:0000:0000:0000:0000'
+    subnetv6 = 'ac43:034f:0000:002c:0000:0000:0000:0000/64'
+    expected = ['ac43:34f:0:2c::12', 'ac43:34f:0:2c::12/64']
     actual = [ipv6_contract(ipv6), ipv6_contract(subnetv6)]
     assert expected == actual, "ipv6_contract function fails IPv6 contraction."
 
 def test_ipv6_expand_contract_error():
     '''Test that the ipv6_expand and ipv6_contract functions raise the correct error when given an IPv4 address.'''
     with pytest.raises(ValueError):
         ipv6_expand('192.168.1.24')
```

### Comparing `binip-1.0.1/LICENSE` & `binip-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `binip-1.0.1/README.md` & `binip-1.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 
         subnetv4.iptype
         'v4'
 
 - info: dict, info on subnet.
 
         subnetv4.info
-        {'Network address:': '192.168.1.0', 'Broadcast address': '192.168.1.255', 'Number of client IPs:': 254, 'Client IP range:': '192.168.1.1 - 192.168.1.254'}
+        {'Network': '192.168.1.0', 'Broadcast': '192.168.1.255', 'Clients:': 254, 'Range:': ('192.168.1.1','192.168.1.254')}
 
 
 Methods:
 
 - validate_address:
   
   Validates a given IP address, works for both IPv4 and IPv6.
```

### Comparing `binip-1.0.1/pyproject.toml` & `binip-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "binip"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
     { name="Loïc James McKeever", email="loicjamesmckeever@gmail.com"},
 ]
 description = "A package for facilitating various IP and subnet operations."
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `binip-1.0.1/PKG-INFO` & `binip-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: binip
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package for facilitating various IP and subnet operations.
 Project-URL: Homepage, https://github.com/loicjamesmckeever/binip
 Project-URL: Issues, https://github.com/loicjamesmckeever/binip/issues
 Author-email: Loïc James McKeever <loicjamesmckeever@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -153,15 +153,15 @@
 
         subnetv4.iptype
         'v4'
 
 - info: dict, info on subnet.
 
         subnetv4.info
-        {'Network address:': '192.168.1.0', 'Broadcast address': '192.168.1.255', 'Number of client IPs:': 254, 'Client IP range:': '192.168.1.1 - 192.168.1.254'}
+        {'Network': '192.168.1.0', 'Broadcast': '192.168.1.255', 'Clients:': 254, 'Range:': ('192.168.1.1','192.168.1.254')}
 
 
 Methods:
 
 - validate_address:
   
   Validates a given IP address, works for both IPv4 and IPv6.
```

