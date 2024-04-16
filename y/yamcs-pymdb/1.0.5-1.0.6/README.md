# Comparing `tmp/yamcs-pymdb-1.0.5.tar.gz` & `tmp/yamcs_pymdb-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yamcs-pymdb-1.0.5.tar", last modified: Sun Apr  7 22:18:46 2024, max compression
+gzip compressed data, was "yamcs_pymdb-1.0.6.tar", last modified: Tue Apr 16 07:57:04 2024, max compression
```

## Comparing `yamcs-pymdb-1.0.5.tar` & `yamcs_pymdb-1.0.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-07 22:18:46.922074 yamcs-pymdb-1.0.5/
--rw-r--r--   0 fdi        (503) staff       (20)     7652 2024-02-09 08:16:29.000000 yamcs-pymdb-1.0.5/LICENSE
--rw-r--r--   0 fdi        (503) staff       (20)       34 2024-02-09 08:18:18.000000 yamcs-pymdb-1.0.5/MANIFEST.in
--rw-r--r--   0 fdi        (503) staff       (20)     1915 2024-04-07 22:18:46.921820 yamcs-pymdb-1.0.5/PKG-INFO
--rw-r--r--   0 fdi        (503) staff       (20)     1007 2024-02-09 09:41:58.000000 yamcs-pymdb-1.0.5/README.md
--rw-r--r--   0 fdi        (503) staff       (20)       38 2024-04-07 22:18:46.922130 yamcs-pymdb-1.0.5/setup.cfg
--rw-r--r--   0 fdi        (503) staff       (20)     1244 2024-04-07 22:16:02.000000 yamcs-pymdb-1.0.5/setup.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-07 22:18:46.892946 yamcs-pymdb-1.0.5/src/
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-07 22:18:46.892724 yamcs-pymdb-1.0.5/src/yamcs/
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-07 22:18:46.904308 yamcs-pymdb-1.0.5/src/yamcs/pymdb/
--rw-r--r--   0 fdi        (503) staff       (20)      687 2024-03-14 22:48:46.000000 yamcs-pymdb-1.0.5/src/yamcs/pymdb/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)     4166 2024-03-22 09:18:23.000000 yamcs-pymdb-1.0.5/src/yamcs/pymdb/alarms.py
--rw-r--r--   0 fdi        (503) staff       (20)     6569 2024-04-05 11:18:43.000000 yamcs-pymdb-1.0.5/src/yamcs/pymdb/algorithms.py
--rw-r--r--   0 fdi        (503) staff       (20)     1173 2024-03-22 09:19:10.000000 yamcs-pymdb-1.0.5/src/yamcs/pymdb/ancillary.py
--rw-r--r--   0 fdi        (503) staff       (20)     1110 2024-02-23 15:50:36.000000 yamcs-pymdb-1.0.5/src/yamcs/pymdb/calibrators.py
--rw-r--r--   0 fdi        (503) staff       (20)     6124 2024-02-25 20:53:48.000000 yamcs-pymdb-1.0.5/src/yamcs/pymdb/ccsds.py
--rw-r--r--   0 fdi        (503) staff       (20)     4561 2024-03-28 20:39:32.000000 yamcs-pymdb-1.0.5/src/yamcs/pymdb/checks.py
--rw-r--r--   0 fdi        (503) staff       (20)    17143 2024-03-28 12:30:59.000000 yamcs-pymdb-1.0.5/src/yamcs/pymdb/commands.py
--rw-r--r--   0 fdi        (503) staff       (20)     6642 2024-03-28 12:28:20.000000 yamcs-pymdb-1.0.5/src/yamcs/pymdb/containers.py
--rw-r--r--   0 fdi        (503) staff       (20)     8015 2024-03-28 21:21:31.000000 yamcs-pymdb-1.0.5/src/yamcs/pymdb/csp.py
--rw-r--r--   0 fdi        (503) staff       (20)    18231 2024-03-28 12:30:59.000000 yamcs-pymdb-1.0.5/src/yamcs/pymdb/datatypes.py
--rw-r--r--   0 fdi        (503) staff       (20)     8370 2024-04-05 09:43:14.000000 yamcs-pymdb-1.0.5/src/yamcs/pymdb/encodings.py
--rw-r--r--   0 fdi        (503) staff       (20)       86 2024-01-04 13:44:01.000000 yamcs-pymdb-1.0.5/src/yamcs/pymdb/exceptions.py
--rw-r--r--   0 fdi        (503) staff       (20)     4045 2024-03-22 07:37:40.000000 yamcs-pymdb-1.0.5/src/yamcs/pymdb/expressions.py
--rw-r--r--   0 fdi        (503) staff       (20)    16520 2024-04-04 12:25:17.000000 yamcs-pymdb-1.0.5/src/yamcs/pymdb/parameters.py
--rw-r--r--   0 fdi        (503) staff       (20)     8350 2024-04-05 09:43:14.000000 yamcs-pymdb-1.0.5/src/yamcs/pymdb/systems.py
--rw-r--r--   0 fdi        (503) staff       (20)     4427 2024-04-05 09:50:48.000000 yamcs-pymdb-1.0.5/src/yamcs/pymdb/verifiers.py
--rw-r--r--   0 fdi        (503) staff       (20)    78132 2024-04-05 11:47:37.000000 yamcs-pymdb-1.0.5/src/yamcs/pymdb/xtce.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-07 22:18:46.921505 yamcs-pymdb-1.0.5/src/yamcs_pymdb.egg-info/
--rw-r--r--   0 fdi        (503) staff       (20)     1915 2024-04-07 22:18:46.000000 yamcs-pymdb-1.0.5/src/yamcs_pymdb.egg-info/PKG-INFO
--rw-r--r--   0 fdi        (503) staff       (20)      737 2024-04-07 22:18:46.000000 yamcs-pymdb-1.0.5/src/yamcs_pymdb.egg-info/SOURCES.txt
--rw-r--r--   0 fdi        (503) staff       (20)        1 2024-04-07 22:18:46.000000 yamcs-pymdb-1.0.5/src/yamcs_pymdb.egg-info/dependency_links.txt
--rw-r--r--   0 fdi        (503) staff       (20)        1 2023-12-13 14:35:06.000000 yamcs-pymdb-1.0.5/src/yamcs_pymdb.egg-info/not-zip-safe
--rw-r--r--   0 fdi        (503) staff       (20)        6 2024-04-07 22:18:46.000000 yamcs-pymdb-1.0.5/src/yamcs_pymdb.egg-info/top_level.txt
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-16 07:57:04.134244 yamcs_pymdb-1.0.6/
+-rw-r--r--   0 fdi        (503) staff       (20)     7652 2024-02-09 08:16:29.000000 yamcs_pymdb-1.0.6/LICENSE
+-rw-r--r--   0 fdi        (503) staff       (20)       34 2024-02-09 08:18:18.000000 yamcs_pymdb-1.0.6/MANIFEST.in
+-rw-r--r--   0 fdi        (503) staff       (20)     1915 2024-04-16 07:57:04.133983 yamcs_pymdb-1.0.6/PKG-INFO
+-rw-r--r--   0 fdi        (503) staff       (20)     1007 2024-02-09 09:41:58.000000 yamcs_pymdb-1.0.6/README.md
+-rw-r--r--   0 fdi        (503) staff       (20)       38 2024-04-16 07:57:04.134306 yamcs_pymdb-1.0.6/setup.cfg
+-rw-r--r--   0 fdi        (503) staff       (20)     1244 2024-04-16 07:47:15.000000 yamcs_pymdb-1.0.6/setup.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-16 07:57:04.105446 yamcs_pymdb-1.0.6/src/
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-16 07:57:04.105254 yamcs_pymdb-1.0.6/src/yamcs/
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-16 07:57:04.115456 yamcs_pymdb-1.0.6/src/yamcs/pymdb/
+-rw-r--r--   0 fdi        (503) staff       (20)      687 2024-03-14 22:48:46.000000 yamcs_pymdb-1.0.6/src/yamcs/pymdb/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)     4166 2024-03-22 09:18:23.000000 yamcs_pymdb-1.0.6/src/yamcs/pymdb/alarms.py
+-rw-r--r--   0 fdi        (503) staff       (20)     6569 2024-04-05 11:18:43.000000 yamcs_pymdb-1.0.6/src/yamcs/pymdb/algorithms.py
+-rw-r--r--   0 fdi        (503) staff       (20)     1173 2024-03-22 09:19:10.000000 yamcs_pymdb-1.0.6/src/yamcs/pymdb/ancillary.py
+-rw-r--r--   0 fdi        (503) staff       (20)     1110 2024-02-23 15:50:36.000000 yamcs_pymdb-1.0.6/src/yamcs/pymdb/calibrators.py
+-rw-r--r--   0 fdi        (503) staff       (20)     6049 2024-04-15 20:41:06.000000 yamcs_pymdb-1.0.6/src/yamcs/pymdb/ccsds.py
+-rw-r--r--   0 fdi        (503) staff       (20)     4561 2024-03-28 20:39:32.000000 yamcs_pymdb-1.0.6/src/yamcs/pymdb/checks.py
+-rw-r--r--   0 fdi        (503) staff       (20)    18698 2024-04-15 21:15:24.000000 yamcs_pymdb-1.0.6/src/yamcs/pymdb/commands.py
+-rw-r--r--   0 fdi        (503) staff       (20)     7602 2024-04-15 21:22:33.000000 yamcs_pymdb-1.0.6/src/yamcs/pymdb/containers.py
+-rw-r--r--   0 fdi        (503) staff       (20)     7999 2024-04-15 21:28:28.000000 yamcs_pymdb-1.0.6/src/yamcs/pymdb/csp.py
+-rw-r--r--   0 fdi        (503) staff       (20)    18231 2024-03-28 12:30:59.000000 yamcs_pymdb-1.0.6/src/yamcs/pymdb/datatypes.py
+-rw-r--r--   0 fdi        (503) staff       (20)     8370 2024-04-05 09:43:14.000000 yamcs_pymdb-1.0.6/src/yamcs/pymdb/encodings.py
+-rw-r--r--   0 fdi        (503) staff       (20)       86 2024-01-04 13:44:01.000000 yamcs_pymdb-1.0.6/src/yamcs/pymdb/exceptions.py
+-rw-r--r--   0 fdi        (503) staff       (20)     4045 2024-03-22 07:37:40.000000 yamcs_pymdb-1.0.6/src/yamcs/pymdb/expressions.py
+-rw-r--r--   0 fdi        (503) staff       (20)    16520 2024-04-04 12:25:17.000000 yamcs_pymdb-1.0.6/src/yamcs/pymdb/parameters.py
+-rw-r--r--   0 fdi        (503) staff       (20)     8350 2024-04-05 09:43:14.000000 yamcs_pymdb-1.0.6/src/yamcs/pymdb/systems.py
+-rw-r--r--   0 fdi        (503) staff       (20)     4427 2024-04-05 09:50:48.000000 yamcs_pymdb-1.0.6/src/yamcs/pymdb/verifiers.py
+-rw-r--r--   0 fdi        (503) staff       (20)    78883 2024-04-15 21:26:03.000000 yamcs_pymdb-1.0.6/src/yamcs/pymdb/xtce.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-16 07:57:04.133662 yamcs_pymdb-1.0.6/src/yamcs_pymdb.egg-info/
+-rw-r--r--   0 fdi        (503) staff       (20)     1915 2024-04-16 07:57:04.000000 yamcs_pymdb-1.0.6/src/yamcs_pymdb.egg-info/PKG-INFO
+-rw-r--r--   0 fdi        (503) staff       (20)      737 2024-04-16 07:57:04.000000 yamcs_pymdb-1.0.6/src/yamcs_pymdb.egg-info/SOURCES.txt
+-rw-r--r--   0 fdi        (503) staff       (20)        1 2024-04-16 07:57:04.000000 yamcs_pymdb-1.0.6/src/yamcs_pymdb.egg-info/dependency_links.txt
+-rw-r--r--   0 fdi        (503) staff       (20)        1 2023-12-13 14:35:06.000000 yamcs_pymdb-1.0.6/src/yamcs_pymdb.egg-info/not-zip-safe
+-rw-r--r--   0 fdi        (503) staff       (20)        6 2024-04-16 07:57:04.000000 yamcs_pymdb-1.0.6/src/yamcs_pymdb.egg-info/top_level.txt
```

### Comparing `yamcs-pymdb-1.0.5/LICENSE` & `yamcs_pymdb-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yamcs-pymdb-1.0.5/PKG-INFO` & `yamcs_pymdb-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamcs-pymdb
-Version: 1.0.5
+Version: 1.0.6
 Summary: Generate XTCE for use with Yamcs
 Home-page: https://github.com/yamcs/pymdb
 Author: Space Applications Services
 Author-email: yamcs@spaceapplications.com
 License: LGPL
 Keywords: packet telemetry ccsds xtce yamcs
 Platform: Posix; MacOS X; Windows
```

### Comparing `yamcs-pymdb-1.0.5/README.md` & `yamcs_pymdb-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `yamcs-pymdb-1.0.5/setup.py` & `yamcs_pymdb-1.0.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with io.open("README.md", encoding="utf-8") as f:
     readme = f.read()
 
 setuptools.setup(
     name="yamcs-pymdb",
-    version="1.0.5",
+    version="1.0.6",
     description="Generate XTCE for use with Yamcs",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/yamcs/pymdb",
     author="Space Applications Services",
     author_email="yamcs@spaceapplications.com",
     license="LGPL",
```

### Comparing `yamcs-pymdb-1.0.5/src/yamcs/pymdb/__init__.py` & `yamcs_pymdb-1.0.6/src/yamcs/pymdb/__init__.py`

 * *Files identical despite different names*

### Comparing `yamcs-pymdb-1.0.5/src/yamcs/pymdb/alarms.py` & `yamcs_pymdb-1.0.6/src/yamcs/pymdb/alarms.py`

 * *Files identical despite different names*

### Comparing `yamcs-pymdb-1.0.5/src/yamcs/pymdb/algorithms.py` & `yamcs_pymdb-1.0.6/src/yamcs/pymdb/algorithms.py`

 * *Files identical despite different names*

### Comparing `yamcs-pymdb-1.0.5/src/yamcs/pymdb/ancillary.py` & `yamcs_pymdb-1.0.6/src/yamcs/pymdb/ancillary.py`

 * *Files identical despite different names*

### Comparing `yamcs-pymdb-1.0.5/src/yamcs/pymdb/calibrators.py` & `yamcs_pymdb-1.0.6/src/yamcs/pymdb/calibrators.py`

 * *Files identical despite different names*

### Comparing `yamcs-pymdb-1.0.5/src/yamcs/pymdb/ccsds.py` & `yamcs_pymdb-1.0.6/src/yamcs/pymdb/ccsds.py`

 * *Files 4% similar despite different names*

```diff
@@ -161,38 +161,38 @@
         arguments=[
             tc_secondary_header,
             tc_apid,
         ],
         entries=[
             FixedValueEntry(
                 name="ccsds_version",
-                binary=bytes.fromhex("00"),
+                binary="00",
                 bits=3,
             ),
             FixedValueEntry(
                 name="ccsds_type",
-                binary=bytes.fromhex("01"),
+                binary="01",
                 bits=1,
             ),
             ArgumentEntry(tc_secondary_header),
             ArgumentEntry(tc_apid),
             FixedValueEntry(
                 name="ccsds_group_flags",
-                binary=bytes.fromhex("03"),  # Always standalone
+                binary="03",  # Always standalone
                 bits=2,
             ),
             FixedValueEntry(
                 name="ccsds_source_sequence_count",
-                binary=bytes.fromhex("0000"),
+                binary="0000",
                 bits=14,
                 short_description="Value set by Yamcs during link post-processing",
             ),
             FixedValueEntry(
                 name="ccsds_packet_length",
-                binary=bytes.fromhex("0000"),
+                binary="0000",
                 bits=16,
                 short_description="Value set by Yamcs during link post-processing",
             ),
         ],
     )
 
     tm_version = ParameterMember(
```

### Comparing `yamcs-pymdb-1.0.5/src/yamcs/pymdb/checks.py` & `yamcs_pymdb-1.0.6/src/yamcs/pymdb/checks.py`

 * *Files identical despite different names*

### Comparing `yamcs-pymdb-1.0.5/src/yamcs/pymdb/commands.py` & `yamcs_pymdb-1.0.6/src/yamcs/pymdb/commands.py`

 * *Files 16% similar despite different names*

```diff
@@ -391,51 +391,108 @@
 
 class ArgumentEntry:
     def __init__(
         self,
         argument: Argument,
         *,
         short_description: str | None = None,
-        absolute: bool = False,
-        location_in_bits: int = 0,
+        bitpos: int | None = None,
+        offset: int = 0,
         condition: Expression | None = None,
     ) -> None:
         self.argument: Argument = argument
 
         self.short_description: str | None = short_description
         """Oneline description"""
 
-        self.absolute: bool = absolute
-        self.location_in_bits: int = location_in_bits
+        self.bitpos: int | None = bitpos
+        """
+        Absolute position within the container, in bits.
+
+        If unspecified, this entry is positioned relative to the preceding
+        entry.
+        """
+
+        self.offset: int = offset
+        """
+        Distance in bits to the preceding entry.
+
+        While not expected, if both :attr:`bitpos` and :attr:`offset` are
+        specified, the two are added together for establishing the real
+        absolute bit position.
+        """
+
         self.condition: Expression | None = condition
+        """If set, this entry is only present when the condition is met"""
 
 
 class FixedValueEntry:
     def __init__(
         self,
-        binary: bytes,
+        binary: bytes | str,
         name: str | None = None,
         *,
         short_description: str | None = None,
-        absolute: bool = False,
-        location_in_bits: int = 0,
+        bitpos: int | None = None,
+        offset: int = 0,
         condition: Expression | None = None,
         bits: int | None = None,
     ) -> None:
-        self.binary: bytes = binary
+
+        self.binary: bytes
+        """
+        The fixed value to be encoded.
+
+        The value may be provided in any of these ways:
+
+        * Bytes: :python:`b\xDE\xAD\xBE\xEF`
+        * Hex string: :python:`"DEADBEEF"`
+        """
+        if isinstance(binary, str):
+            self.binary = bytes.fromhex(binary)
+        else:
+            self.binary = binary
 
         self.name: str | None = name
+        """Optional name"""
 
         self.short_description: str | None = short_description
-        """Onleine description"""
+        """Oneline description"""
+
+        self.bitpos: int | None = bitpos
+        """
+        Absolute position within the container, in bits.
+
+        If unspecified, this entry is positioned relative to the preceding
+        entry.
+        """
+
+        self.offset: int = offset
+        """
+        Distance in bits to the preceding entry.
+
+        While not expected, if both :attr:`bitpos` and :attr:`offset` are
+        specified, the two are added together for establishing the real
+        absolute bit position.
+        """
 
-        self.absolute: bool = absolute
-        self.location_in_bits: int = location_in_bits
         self.condition: Expression | None = condition
+        """If set, encode this entry only when the condition is met"""
+
         self.bits: int | None = bits
+        """
+        If unspecified, its value is derived from the provided
+        :attr:`binary` value.
+
+        If less than the bit size of the :attr:`binary` attribute,
+        the value is left-padded with zeros.
+
+        If larger than the bit size of the :attr:`binary` attribute,
+        the most-significant bits are dropped.
+        """
 
 
 CommandEntry = ArgumentEntry | ParameterEntry | FixedValueEntry
 
 
 class Command:
     def __init__(
@@ -444,16 +501,15 @@
         name: str,
         *,
         aliases: Mapping[str, str] | None = None,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
         abstract: bool = False,
-        parent: Command | None = None,
-        condition: Expression | None = None,
+        base: Command | str | None = None,
         assignments: Mapping[str, Any] | None = None,
         arguments: Sequence[Argument] | None = None,
         entries: Sequence[CommandEntry] | None = None,
         level: CommandLevel = CommandLevel.NORMAL,
         warning_message: str | None = None,
     ):
         self.name: str = name
@@ -471,16 +527,15 @@
         self.long_description: str | None = long_description
         """Multiline description"""
 
         self.extra: dict[str, str] = dict(extra or {})
         """Arbitrary information, keyed by name"""
 
         self.abstract: bool = abstract
-        self.parent: Command | str | None = parent
-        self.condition: Expression | None = condition
+        self.base: Command | str | None = base
         self.assignments: dict[str, Any] = dict(assignments or {})
         self.arguments: list[Argument] = list(arguments or [])
         self._entries: list[CommandEntry] | None = (
             list(entries) if entries is not None else None
         )
 
         self.transferred_to_range_verifier: TransferredToRangeVerifier | None = None
@@ -547,16 +602,16 @@
         :param visit_parents:
             Search upwards in parent commands
         """
         for argument in self.arguments:
             if argument.name == name:
                 return argument
 
-        if visit_parents and self.parent and isinstance(self.parent, Command):
-            return self.parent.get_argument(name)
+        if visit_parents and self.base and isinstance(self.base, Command):
+            return self.base.get_argument(name)
         else:
             return None
 
     @property
     def entries(self) -> list[CommandEntry]:
         """
         The order and placement of entries in the encoded command.
```

### Comparing `yamcs-pymdb-1.0.5/src/yamcs/pymdb/containers.py` & `yamcs_pymdb-1.0.6/src/yamcs/pymdb/containers.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,50 +11,82 @@
     from yamcs.pymdb.systems import System
 
 
 class ParameterEntry:
     def __init__(
         self,
         parameter: Parameter,
-        location_in_bits: int = 0,
+        bitpos: int | None = None,
         *,
-        absolute: bool = False,
+        offset: int = 0,
         short_description: str | None = None,
         condition: Expression | None = None,
     ) -> None:
         self.parameter: Parameter = parameter
 
         self.short_description: str | None = short_description
         """Oneline description"""
 
-        self.absolute: bool = absolute
-        self.location_in_bits: int = location_in_bits
+        self.bitpos: int | None = bitpos
+        """
+        Absolute position within the container, in bits.
+
+        If unspecified, this entry is positioned relative to the preceding
+        entry.
+        """
+
+        self.offset: int = offset
+        """
+        Distance in bits to the preceding entry.
+
+        While not expected, if both :attr:`bitpos` and :attr:`offset` are
+        specified, the two are added together for establishing the real
+        absolute bit position.
+        """
+
         self.condition: Expression | None = condition
+        """If set, this entry is only present when the condition is met"""
 
     def __str__(self) -> str:
         return self.parameter.__str__()
 
 
 class ContainerEntry:
     def __init__(
         self,
         container: Container,
         short_description: str | None = None,
-        absolute: bool = False,
-        location_in_bits: int = 0,
+        bitpos: int | None = None,
+        offset: int = 0,
         condition: Expression | None = None,
     ) -> None:
         self.container: Container = container
 
         self.short_description: str | None = short_description
         """Oneline description"""
 
-        self.absolute: bool = absolute
-        self.location_in_bits: int = location_in_bits
+        self.bitpos: int | None = bitpos
+        """
+        Absolute position within the container, in bits.
+
+        If unspecified, this entry is positioned relative to the preceding
+        entry.
+        """
+
+        self.offset: int = offset
+        """
+        Distance in bits to the preceding entry.
+
+        While not expected, if both :attr:`bitpos` and :attr:`offset` are
+        specified, the two are added together for establishing the real
+        absolute bit position.
+        """
+
         self.condition: Expression | None = condition
+        """If set, this entry is only present when the condition is met"""
 
     def __str__(self) -> str:
         return self.container.__str__()
 
 
 class Container:
     """
@@ -64,15 +96,15 @@
 
     def __init__(
         self,
         system: System,
         name: str,
         entries: Sequence[ParameterEntry | ContainerEntry] | None = None,
         *,
-        parent: Container | str | None = None,
+        base: Container | str | None = None,
         abstract: bool = False,
         condition: Expression | None = None,
         aliases: Mapping[str, str] | None = None,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
         bits: int | None = None,
@@ -124,15 +156,15 @@
         self.hint_partition: bool = hint_partition
         """
         Hint that this container's name should be used for partitioning when
         stored to Yamcs.
         """
 
         self.entries: list[ParameterEntry | ContainerEntry] = list(entries or [])
-        self.parent: Container | str | None = parent
+        self.base: Container | str | None = base
         self.abstract: bool = abstract
         self.condition: Expression | None = condition
         """Restriction criteria for this container."""
 
         if name in system._containers_by_name:
             raise Exception(
                 "System {} already contains a container {}".format(
@@ -158,15 +190,15 @@
 
         return path
 
     def fit_entries(self):
         """
         Automatically set a fixed size to this container based on the known entries.
         """
-        if self.parent:
+        if self.base:
             raise NotImplementedError()
 
         max_pos = 0
 
         prev_pos = 0
         for entry in self.entries:
             if isinstance(entry, ParameterEntry):
@@ -183,18 +215,19 @@
                     raise NotImplementedError()
                 elif parameter.encoding and parameter.encoding.bits:
                     bits = parameter.encoding.bits
 
                 if not bits:
                     raise Exception(f"Cannot determine size of {entry.parameter}")
 
-                pos = entry.location_in_bits
-                if not entry.absolute:
-                    pos += prev_pos
+                pos = entry.bitpos
+                if pos is None:
+                    pos = prev_pos
 
+                pos += entry.offset
                 pos += bits
 
                 prev_pos = pos
                 if pos > max_pos:
                     max_pos = pos
             else:
                 raise NotImplementedError()
```

### Comparing `yamcs-pymdb-1.0.5/src/yamcs/pymdb/csp.py` & `yamcs_pymdb-1.0.6/src/yamcs/pymdb/csp.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
         bits=32,
         entries=[
             ParameterEntry(tm_pri),
             ParameterEntry(tm_src),
             ParameterEntry(tm_dst),
             ParameterEntry(tm_dport),
             ParameterEntry(tm_sport),
-            ParameterEntry(tm_hmac, location_in_bits=4),
+            ParameterEntry(tm_hmac, offset=4),
             ParameterEntry(tm_xtea),
             ParameterEntry(tm_rdp),
             ParameterEntry(tm_crc),
         ],
     )
 
     tc_pri = EnumeratedArgument(
@@ -256,19 +256,19 @@
         entries=[
             ArgumentEntry(tc_pri),
             ArgumentEntry(tc_src),
             ArgumentEntry(tc_dst),
             ArgumentEntry(tc_dport),
             FixedValueEntry(
                 name=f"{prefix}sport",
-                binary=b"\x20",  # 48
+                binary="20",  # 48
                 bits=6,
                 short_description="Ephemeral port for outgoing connection",
             ),
-            FixedValueEntry(name=f"{prefix}reserved", binary=b"\x00", bits=4),
+            FixedValueEntry(name=f"{prefix}reserved", binary="00", bits=4),
             ArgumentEntry(tc_hmac),
             ArgumentEntry(tc_xtea),
             ArgumentEntry(tc_rdp),
             ArgumentEntry(tc_crc),
         ],
     )
```

### Comparing `yamcs-pymdb-1.0.5/src/yamcs/pymdb/datatypes.py` & `yamcs_pymdb-1.0.6/src/yamcs/pymdb/datatypes.py`

 * *Files identical despite different names*

### Comparing `yamcs-pymdb-1.0.5/src/yamcs/pymdb/encodings.py` & `yamcs_pymdb-1.0.6/src/yamcs/pymdb/encodings.py`

 * *Files identical despite different names*

### Comparing `yamcs-pymdb-1.0.5/src/yamcs/pymdb/expressions.py` & `yamcs_pymdb-1.0.6/src/yamcs/pymdb/expressions.py`

 * *Files identical despite different names*

### Comparing `yamcs-pymdb-1.0.5/src/yamcs/pymdb/parameters.py` & `yamcs_pymdb-1.0.6/src/yamcs/pymdb/parameters.py`

 * *Files identical despite different names*

### Comparing `yamcs-pymdb-1.0.5/src/yamcs/pymdb/systems.py` & `yamcs_pymdb-1.0.6/src/yamcs/pymdb/systems.py`

 * *Files identical despite different names*

### Comparing `yamcs-pymdb-1.0.5/src/yamcs/pymdb/verifiers.py` & `yamcs_pymdb-1.0.6/src/yamcs/pymdb/verifiers.py`

 * *Files identical despite different names*

### Comparing `yamcs-pymdb-1.0.5/src/yamcs/pymdb/xtce.py` & `yamcs_pymdb-1.0.6/src/yamcs/pymdb/xtce.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,18 +204,18 @@
 
         if command.aliases:
             self.add_aliases(el, command.aliases)
 
         if command.extra:
             self.add_ancillary_data(el, command.extra)
 
-        if command.parent:
+        if command.base:
             base_el = ET.SubElement(el, "BaseMetaCommand")
             base_el.attrib["metaCommandRef"] = self.make_command_ref(
-                target=command.parent,
+                target=command.base,
                 start=command.system,
             )
 
             if command.assignments:
                 assignments_el = ET.SubElement(base_el, "ArgumentAssignmentList")
                 for k, v in command.assignments.items():
                     arg = command.get_argument(k)
@@ -237,18 +237,18 @@
                 self.add_argument(args_el, command, argument)
 
         container_el = ET.SubElement(el, "CommandContainer")
         container_el.attrib["name"] = command.name
 
         self.add_command_entry_list(container_el, command)
 
-        if command.parent:
+        if command.base:
             base_el = ET.SubElement(container_el, "BaseContainer")
             base_el.attrib["containerRef"] = self.make_command_ref(
-                target=command.parent,
+                target=command.base,
                 start=command.system,
             )
 
         sign_el = ET.SubElement(el, "DefaultSignificance")
 
         if command.level == CommandLevel.NORMAL:
             sign_el.attrib["consequenceLevel"] = "normal"
@@ -433,35 +433,49 @@
     def add_fixed_value_entry(
         self,
         parent: ET.Element,
         command: Command,
         entry: FixedValueEntry,
     ):
         el = ET.SubElement(parent, "FixedValueEntry")
-        el.attrib["binaryValue"] = hexlify(entry.binary).decode("ascii")
 
+        bitlen: int
         if entry.bits is None:
-            el.attrib["sizeInBits"] = str(8 * len(entry.binary))
+            bitlen = 8 * len(entry.binary)
         else:
-            el.attrib["sizeInBits"] = str(entry.bits)
+            bitlen = entry.bits
+
+        hex = hexlify(entry.binary).decode("ascii")
+
+        # XTCE requires hex to be at least as large as the bit size
+        bytelen: int
+        if bitlen % 8:
+            bytelen = (bitlen + (8 - bitlen % 8)) // 8
+        else:
+            bytelen = bitlen // 8
+        hex = hex.zfill(bytelen * 2)
+
+        el.attrib["binaryValue"] = hex
+        el.attrib["sizeInBits"] = str(bitlen)
 
         if entry.name:
             el.attrib["name"] = entry.name
         if entry.short_description:
             el.attrib["shortDescription"] = entry.short_description
 
         loc_el = ET.SubElement(el, "LocationInContainerInBits")
 
-        if entry.absolute:
-            loc_el.attrib["referenceLocation"] = "containerStart"
-        else:
+        if entry.bitpos is None:
             loc_el.attrib["referenceLocation"] = "previousEntry"
-
-        fv_el = ET.SubElement(loc_el, "FixedValue")
-        fv_el.text = str(entry.location_in_bits)
+            fv_el = ET.SubElement(loc_el, "FixedValue")
+            fv_el.text = str(entry.offset)
+        else:
+            loc_el.attrib["referenceLocation"] = "containerStart"
+            fv_el = ET.SubElement(loc_el, "FixedValue")
+            fv_el.text = str(entry.bitpos + entry.offset)
 
         if entry.condition:
             cond_el = ET.SubElement(el, "IncludeCondition")
             expr_el = ET.SubElement(cond_el, "BooleanExpression")
             self.add_expression_condition(
                 expr_el,
                 system=command.system,
@@ -478,21 +492,22 @@
         el.attrib["argumentRef"] = entry.argument.name
 
         if entry.short_description:
             el.attrib["shortDescription"] = entry.short_description
 
         loc_el = ET.SubElement(el, "LocationInContainerInBits")
 
-        if entry.absolute:
-            loc_el.attrib["referenceLocation"] = "containerStart"
-        else:
+        if entry.bitpos is None:
             loc_el.attrib["referenceLocation"] = "previousEntry"
-
-        fv_el = ET.SubElement(loc_el, "FixedValue")
-        fv_el.text = str(entry.location_in_bits)
+            fv_el = ET.SubElement(loc_el, "FixedValue")
+            fv_el.text = str(entry.offset)
+        else:
+            loc_el.attrib["referenceLocation"] = "containerStart"
+            fv_el = ET.SubElement(loc_el, "FixedValue")
+            fv_el.text = str(entry.bitpos + entry.offset)
 
         if entry.condition:
             cond_el = ET.SubElement(el, "IncludeCondition")
             expr_el = ET.SubElement(cond_el, "BooleanExpression")
             self.add_expression_condition(
                 expr_el,
                 system=command.system,
@@ -1878,16 +1893,16 @@
             if isinstance(entry, ParameterEntry):
                 self.add_parameter_ref_entry(el, container, entry)
             elif isinstance(entry, ContainerEntry):
                 self.add_container_ref_entry(el, container, entry)
             else:
                 raise ExportError(f"Unexpected entry {entry.__class__}")
 
-        if container.parent:
-            self.add_base_container(parent, container.parent, container)
+        if container.base:
+            self.add_base_container(parent, container.base, container)
 
     def add_parameter_ref_entry(
         self,
         parent: ET.Element,
         container: Container,
         entry: ParameterEntry,
     ):
@@ -1897,21 +1912,22 @@
             start=container.system,
         )
         if entry.short_description:
             el.attrib["shortDescription"] = entry.short_description
 
         loc_el = ET.SubElement(el, "LocationInContainerInBits")
 
-        if entry.absolute:
-            loc_el.attrib["referenceLocation"] = "containerStart"
-        else:
+        if entry.bitpos is None:
             loc_el.attrib["referenceLocation"] = "previousEntry"
-
-        fv_el = ET.SubElement(loc_el, "FixedValue")
-        fv_el.text = str(entry.location_in_bits)
+            fv_el = ET.SubElement(loc_el, "FixedValue")
+            fv_el.text = str(entry.offset)
+        else:
+            loc_el.attrib["referenceLocation"] = "containerStart"
+            fv_el = ET.SubElement(loc_el, "FixedValue")
+            fv_el.text = str(entry.bitpos + entry.offset)
 
         if entry.condition:
             cond_el = ET.SubElement(el, "IncludeCondition")
             expr_el = ET.SubElement(cond_el, "BooleanExpression")
             self.add_expression_condition(
                 expr_el,
                 system=container.system,
@@ -1930,21 +1946,22 @@
             start=container.system,
         )
         if entry.short_description:
             el.attrib["shortDescription"] = entry.short_description
 
         loc_el = ET.SubElement(el, "LocationInContainerInBits")
 
-        if entry.absolute:
-            loc_el.attrib["referenceLocation"] = "containerStart"
-        else:
+        if entry.bitpos is None:
             loc_el.attrib["referenceLocation"] = "previousEntry"
-
-        fv_el = ET.SubElement(loc_el, "FixedValue")
-        fv_el.text = str(entry.location_in_bits)
+            fv_el = ET.SubElement(loc_el, "FixedValue")
+            fv_el.text = str(entry.offset)
+        else:
+            loc_el.attrib["referenceLocation"] = "containerStart"
+            fv_el = ET.SubElement(loc_el, "FixedValue")
+            fv_el.text = str(entry.bitpos + entry.offset)
 
         if entry.condition:
             cond_el = ET.SubElement(el, "IncludeCondition")
             expr_el = ET.SubElement(cond_el, "BooleanExpression")
             self.add_expression_condition(
                 expr_el,
                 system=container.system,
```

### Comparing `yamcs-pymdb-1.0.5/src/yamcs_pymdb.egg-info/PKG-INFO` & `yamcs_pymdb-1.0.6/src/yamcs_pymdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamcs-pymdb
-Version: 1.0.5
+Version: 1.0.6
 Summary: Generate XTCE for use with Yamcs
 Home-page: https://github.com/yamcs/pymdb
 Author: Space Applications Services
 Author-email: yamcs@spaceapplications.com
 License: LGPL
 Keywords: packet telemetry ccsds xtce yamcs
 Platform: Posix; MacOS X; Windows
```

### Comparing `yamcs-pymdb-1.0.5/src/yamcs_pymdb.egg-info/SOURCES.txt` & `yamcs_pymdb-1.0.6/src/yamcs_pymdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

