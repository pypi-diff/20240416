# Comparing `tmp/tidbytes-0.1.0.tar.gz` & `tmp/tidbytes-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidbytes-0.1.0.tar", max compression
+gzip compressed data, was "tidbytes-0.1.1.tar", max compression
```

## Comparing `tidbytes-0.1.0.tar` & `tidbytes-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2024-03-15 05:50:05.694525 tidbytes-0.1.0/LICENSE
--rw-r--r--   0        0        0    19964 2024-03-15 05:50:05.694525 tidbytes-0.1.0/README.md
--rw-r--r--   0        0        0      485 2024-03-15 05:50:05.694525 tidbytes-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      165 2024-03-15 05:50:05.694525 tidbytes-0.1.0/tidbytes/__init__.py
--rw-r--r--   0        0        0    26053 2024-03-15 05:50:05.694525 tidbytes-0.1.0/tidbytes/codec.py
--rw-r--r--   0        0        0    30605 2024-03-15 05:50:05.694525 tidbytes-0.1.0/tidbytes/idiomatic.py
--rw-r--r--   0        0        0     2890 2024-03-15 05:50:05.694525 tidbytes-0.1.0/tidbytes/mem_types.py
--rw-r--r--   0        0        0    15671 2024-03-15 05:50:05.694525 tidbytes-0.1.0/tidbytes/natural.py
--rw-r--r--   0        0        0    20497 1970-01-01 00:00:00.000000 tidbytes-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-16 06:04:39.832461 tidbytes-0.1.1/LICENSE
+-rw-r--r--   0        0        0    20369 2024-04-16 06:04:39.832461 tidbytes-0.1.1/README.md
+-rw-r--r--   0        0        0      581 2024-04-16 06:04:39.832461 tidbytes-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      165 2024-04-16 06:04:39.832461 tidbytes-0.1.1/tidbytes/__init__.py
+-rw-r--r--   0        0        0    26029 2024-04-16 06:04:39.832461 tidbytes-0.1.1/tidbytes/codec.py
+-rw-r--r--   0        0        0    32108 2024-04-16 06:04:39.832461 tidbytes-0.1.1/tidbytes/idiomatic.py
+-rw-r--r--   0        0        0     2890 2024-04-16 06:04:39.832461 tidbytes-0.1.1/tidbytes/mem_types.py
+-rw-r--r--   0        0        0    15671 2024-04-16 06:04:39.832461 tidbytes-0.1.1/tidbytes/natural.py
+-rw-r--r--   0        0        0    20902 1970-01-01 00:00:00.000000 tidbytes-0.1.1/PKG-INFO
```

### Comparing `tidbytes-0.1.0/LICENSE` & `tidbytes-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tidbytes-0.1.0/README.md` & `tidbytes-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -513,23 +513,36 @@
 # So What Truly Is The “Ninth Bit”
 
 By taking a foreign memory region and applying it’s own bit and byte order as a
 transformation upon itself it yields a region with identity memory order,
 wherein the “ninth bit” is always the leftmost bit of the second byte from the
 left.
 
-### Desirable Future Additions
+# Desirable Future Additions
 
+- Rewrite the natural memory type to use bytes instead lists of lists of bits
+- Make the indexed_meta type work with Mypy type checking
 - Describe exact bit layout for a data type (struct)
     ```python
+    class Struct(Mem):
+        def __init__(self, *args, **kwargs):
+            self.buffer = Mem(sum(args))
+
+    class Union(Mem):
+        "Works similarly"
+
     class Ieee754Single(Struct):
-        sign: Mem[1] = '0'
-        exponent: Num[12] = 0
-        mantissa: Num[19]
+        Sign: Unsigned[1] = 0
+        Exponent: Unsigned[23] = '0101010'
+        Mantissa: Unsigned[12]
+
+        def __float__(self):
+            return float(self.buffer)
     ```
+- Implement Union type
 - Type layout with default values (`foo: Signed = 3`)
 - Types with templates that can be filled in later (like inst constant in ASM)
 - Effective sizeof & effective alignof (not the same as bit len)
 - Bit-level Cursor API for parsing data structures
 - Cursor API bit-level read ahead and skip for reading small integers like u3
 - File-like bit-level write API for assembling (write(bits=4, value=3))
 - Store and query endianness of region
```

### Comparing `tidbytes-0.1.0/tidbytes/codec.py` & `tidbytes-0.1.1/tidbytes/codec.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,17 +36,15 @@
     to validate the returned memory because all operations validate memory
     before returning.
 - The "op" nomenclature always refers to algebraic operations with Natural
     inputs and Natural outputs (the Mem type). Think arithmetic: all ops take
     numbers and return numbers.
 """
 
-import ctypes
-import sys
-import struct
+import ctypes, sys, struct
 from typing import TypeVar
 from .mem_types import u8, u16, u32, u64, i8, i16, i32, i64, f32, f64, ensure
 from .natural import (
     MemRgn, op_identity, op_reverse, contract_validate_memory,
     op_ensure_bit_length, group_bits_into_bytes, meta_op_bit_length,
     iterate_logical_bits
 )
@@ -735,10 +733,9 @@
         return int(bits, base=2)
 
 
 def into_natural_big_integer(mem: MemRgn) -> int:
     "Always assumes destination is signed since Python's big integer type is."
     out = 0
     for i, bit in enumerate(reversed(list(iterate_logical_bits(mem.bytes)))):
-        if bit:
-            out |= 1 << i
+        out |= (1 << i) * bit
     return out
```

### Comparing `tidbytes-0.1.0/tidbytes/idiomatic.py` & `tidbytes-0.1.1/tidbytes/idiomatic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """
 Design decisions:
     - Operator overloads for idiomatic types return new copies of themselves
         since there should be no side-effects.
 """
 
-import copy
-import indexed_meta
-from typing import Any, TypeVar, Union
+import sys, copy, indexed_meta
+from typing import Any, TypeVar, Union, Optional
 from .mem_types import (
-    ensure, MemException, Order, u8, u16, u32, u64, i8, i16, i32, i64, f32, f64,
-    UnderOverflowException, MathOpUnderOverflowException, InvalidSemanticsException,
-    ContractViolationException, InvalidInitializerException,
-    InvalidComparisonException,
+    ensure, Order, L2R, R2L, u8, u16, u32, u64, i8, i16, i32, i64, f32, f64,
+    UnderOverflowException, MathOpUnderOverflowException, MemException,
+    InvalidSemanticsException, ContractViolationException,
+    InvalidInitializerException, InvalidComparisonException,
 )
 from .natural import (
     MemRgn, meta_op_bit_length, contract_validate_memory, group_bits_into_bytes,
     iterate_logical_bits, op_transform, op_identity, op_reverse,
     op_reverse_bytes, op_reverse_bits, op_get_bit, op_get_byte, op_get_bits,
     op_get_bytes, op_set_bit, op_set_bits, op_set_byte, op_set_bytes,
     op_truncate, op_extend, op_ensure_bit_length, op_ensure_byte_length,
@@ -214,16 +213,18 @@
             case [None, None, -1]:
                 return self.reverse()
 
             # mem[::-8] Reverse bytes
             case [None, None, -8]:
                 return self.reverse_bytes()
 
+            # mem[i:] Start
+            # mem[i::] Start
             # mem[i::1] Start, step bit
-            case [int(), None, 1]:
+            case [int(), None, None] | [int(), None, 1]:
                 out.rgn = op_get_bits(self.rgn, start, len(self))
 
             # mem[i::8] Start, step byte
             case [int(), None, 8]:
                 out.rgn = op_get_bytes(
                     self.rgn,
                     start,
@@ -305,14 +306,20 @@
                 raise InvalidSemanticsException(
                     'Cannot interpret negative big integer as slice of raw '
                     'memory since raw bytes are unsigned. Use `Signed` instead'
                 )
             return from_natural_big_integer_unsigned(init, bit_length)
 
         elif isinstance(init, float):
+            from tidbytes.codec import PYTHON_X64_FLOATS  # Unit tests modify
+            if bit_length and 32 <= bit_length < 64 and PYTHON_X64_FLOATS:
+                raise InvalidInitializerException(
+                    'Cannot interpret Python float as fewer than 64 bits: use '
+                    '`codec.f32` if value can be downcasted'
+                )
             return from_natural_float(init, bit_length)
 
         elif isinstance(init, u8):
             return from_natural_u8(init, bit_length)
 
         elif isinstance(init, u16):
             return from_natural_u16(init, bit_length)
@@ -486,14 +493,38 @@
         "See docs for `tidbytes.natural.op_concatenate`"
         self.rgn = op_concatenate(
             self.rgn,
             indexed_meta.root_type(type(self))(mem_right).rgn
         )
         return self
 
+    def as_bytes(self, byte_order: Optional[Order] = None) -> bytes:
+        """
+        Convert the memory region to the built-in `bytes` type. Specify a byte
+        order of left to right for little endian and right to left for big
+        endian. If no byte order is provided, system endianness is assumed.
+        """
+        byte_order = byte_order or (L2R, R2L)[sys.byteorder == 'big']
+        it = (reversed(self.rgn.bytes), self.rgn.bytes)[byte_order == L2R]
+        buffer = b''
+        for byte in map(lambda b: [*filter(lambda i: i is not None, b)], it):
+            acc = 0
+            for index, bit in enumerate(reversed(byte)):
+                acc |= (1 << index) * bit
+            buffer += bytes([acc])
+        return buffer
+
+    def as_be_bytes(self) -> bytes:
+        "Convert the memory region into bytes using right to left byte order"
+        return self.as_bytes(R2L)
+
+    def as_le_bytes(self) -> bytes:
+        "Convert the memory region into bytes using left to right byte order"
+        return self.as_bytes(L2R)
+
     clone = identity
 
 NullMem = Mem()
 
 
 class Unsigned(Mem):
     """
```

### Comparing `tidbytes-0.1.0/tidbytes/mem_types.py` & `tidbytes-0.1.1/tidbytes/mem_types.py`

 * *Files identical despite different names*

### Comparing `tidbytes-0.1.0/tidbytes/natural.py` & `tidbytes-0.1.1/tidbytes/natural.py`

 * *Files identical despite different names*

### Comparing `tidbytes-0.1.0/PKG-INFO` & `tidbytes-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidbytes
-Version: 0.1.0
+Version: 0.1.1
 Summary: Memory manipulation reimagined with bit addressing
 License: MIT
 Author: pebaz
 Author-email: pebazium@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -529,23 +529,36 @@
 # So What Truly Is The “Ninth Bit”
 
 By taking a foreign memory region and applying it’s own bit and byte order as a
 transformation upon itself it yields a region with identity memory order,
 wherein the “ninth bit” is always the leftmost bit of the second byte from the
 left.
 
-### Desirable Future Additions
+# Desirable Future Additions
 
+- Rewrite the natural memory type to use bytes instead lists of lists of bits
+- Make the indexed_meta type work with Mypy type checking
 - Describe exact bit layout for a data type (struct)
     ```python
+    class Struct(Mem):
+        def __init__(self, *args, **kwargs):
+            self.buffer = Mem(sum(args))
+
+    class Union(Mem):
+        "Works similarly"
+
     class Ieee754Single(Struct):
-        sign: Mem[1] = '0'
-        exponent: Num[12] = 0
-        mantissa: Num[19]
+        Sign: Unsigned[1] = 0
+        Exponent: Unsigned[23] = '0101010'
+        Mantissa: Unsigned[12]
+
+        def __float__(self):
+            return float(self.buffer)
     ```
+- Implement Union type
 - Type layout with default values (`foo: Signed = 3`)
 - Types with templates that can be filled in later (like inst constant in ASM)
 - Effective sizeof & effective alignof (not the same as bit len)
 - Bit-level Cursor API for parsing data structures
 - Cursor API bit-level read ahead and skip for reading small integers like u3
 - File-like bit-level write API for assembling (write(bits=4, value=3))
 - Store and query endianness of region
```

