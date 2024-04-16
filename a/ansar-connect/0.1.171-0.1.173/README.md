# Comparing `tmp/ansar_connect-0.1.171.tar.gz` & `tmp/ansar_connect-0.1.173.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.171.tar", last modified: Mon Apr 15 14:16:46 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.173.tar", last modified: Tue Apr 16 08:59:01 2024, max compression
```

## Comparing `ansar_connect-0.1.171.tar` & `ansar_connect-0.1.173.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-15 14:16:46.207885 ansar_connect-0.1.171/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.171/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-15 14:16:46.207885 ansar_connect-0.1.171/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.171/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      723 2024-03-28 18:04:29.000000 ansar_connect-0.1.171/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-15 14:16:46.207885 ansar_connect-0.1.171/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2210 2024-03-28 18:04:17.000000 ansar_connect-0.1.171/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-15 14:16:46.203885 ansar_connect-0.1.171/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-15 14:16:46.203885 ansar_connect-0.1.171/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-15 14:16:46.203885 ansar_connect-0.1.171/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14522 2024-04-12 09:29:14.000000 ansar_connect-0.1.171/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3441 2024-04-12 14:58:30.000000 ansar_connect-0.1.171/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.171/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9054 2024-04-12 15:15:53.000000 ansar_connect-0.1.171/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-15 14:16:46.207885 ansar_connect-0.1.171/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3055 2024-04-15 14:16:42.000000 ansar_connect-0.1.171/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14167 2024-04-15 03:23:57.000000 ansar_connect-0.1.171/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    78025 2024-04-13 03:14:49.000000 ansar_connect-0.1.171/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar_connect-0.1.171/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.171/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar_connect-0.1.171/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.171/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.171/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar_connect-0.1.171/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.171/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.171/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.171/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    33015 2024-04-13 00:35:04.000000 ansar_connect-0.1.171/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2372 2024-04-12 15:15:53.000000 ansar_connect-0.1.171/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    37650 2024-04-15 14:15:08.000000 ansar_connect-0.1.171/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.171/src/ansar/connect/standard.py
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2205 2024-04-14 02:42:33.000000 ansar_connect-0.1.171/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6532 2024-04-13 00:17:21.000000 ansar_connect-0.1.171/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-15 14:16:46.207885 ansar_connect-0.1.171/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-15 14:16:46.000000 ansar_connect-0.1.171/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      984 2024-04-15 14:16:46.000000 ansar_connect-0.1.171/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-15 14:16:46.000000 ansar_connect-0.1.171/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-15 14:16:46.000000 ansar_connect-0.1.171/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       21 2024-04-15 14:16:46.000000 ansar_connect-0.1.171/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-15 14:16:46.000000 ansar_connect-0.1.171/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-16 08:59:01.687646 ansar_connect-0.1.173/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.173/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-16 08:59:01.687646 ansar_connect-0.1.173/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.173/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      723 2024-04-16 08:58:45.000000 ansar_connect-0.1.173/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-16 08:59:01.687646 ansar_connect-0.1.173/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2210 2024-04-16 08:58:37.000000 ansar_connect-0.1.173/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-16 08:59:01.683646 ansar_connect-0.1.173/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-16 08:59:01.683646 ansar_connect-0.1.173/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-16 08:59:01.683646 ansar_connect-0.1.173/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14522 2024-04-12 09:29:14.000000 ansar_connect-0.1.173/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3441 2024-04-12 14:58:30.000000 ansar_connect-0.1.173/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.173/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9054 2024-04-12 15:15:53.000000 ansar_connect-0.1.173/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-16 08:59:01.683646 ansar_connect-0.1.173/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3055 2024-04-16 08:58:58.000000 ansar_connect-0.1.173/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14167 2024-04-15 03:23:57.000000 ansar_connect-0.1.173/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    78025 2024-04-13 03:14:49.000000 ansar_connect-0.1.173/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar_connect-0.1.173/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.173/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar_connect-0.1.173/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.173/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.173/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar_connect-0.1.173/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.173/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.173/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.173/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    33015 2024-04-13 00:35:04.000000 ansar_connect-0.1.173/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2372 2024-04-12 15:15:53.000000 ansar_connect-0.1.173/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    43240 2024-04-16 08:43:56.000000 ansar_connect-0.1.173/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.173/src/ansar/connect/standard.py
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2205 2024-04-14 02:42:33.000000 ansar_connect-0.1.173/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6532 2024-04-13 00:17:21.000000 ansar_connect-0.1.173/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-16 08:59:01.687646 ansar_connect-0.1.173/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-16 08:59:01.000000 ansar_connect-0.1.173/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      984 2024-04-16 08:59:01.000000 ansar_connect-0.1.173/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-16 08:59:01.000000 ansar_connect-0.1.173/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-16 08:59:01.000000 ansar_connect-0.1.173/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       21 2024-04-16 08:59:01.000000 ansar_connect-0.1.173/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-16 08:59:01.000000 ansar_connect-0.1.173/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.171/LICENSE` & `ansar_connect-0.1.173/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.171/PKG-INFO` & `ansar_connect-0.1.173/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.171
+Version: 0.1.173
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.171/README.md` & `ansar_connect-0.1.173/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.171/pyproject.toml` & `ansar_connect-0.1.173/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.171/setup.py` & `ansar_connect-0.1.173/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.171/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.173/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.171/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.173/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.171/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.173/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.171/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.173/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.171/src/ansar/connect/__init__.py` & `ansar_connect-0.1.173/src/ansar/connect/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: 2bfb4bbdeef25c69f910abd39cae282ce89b2e7d
-Version: 0.1.170 (2024-04-16@02:16:42+NZST)
+Commit: 3c147a10303c290c24fa9375a64bfb36296332a4
+Version: 0.1.172 (2024-04-16@20:58:58+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.171/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.173/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.171/src/ansar/connect/directory.py` & `ansar_connect-0.1.173/src/ansar/connect/directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.171/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.173/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.171/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.173/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.171/src/ansar/connect/group_if.py` & `ansar_connect-0.1.173/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.171/src/ansar/connect/grouping.py` & `ansar_connect-0.1.173/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.171/src/ansar/connect/moving.py` & `ansar_connect-0.1.173/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.171/src/ansar/connect/networking.py` & `ansar_connect-0.1.173/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.171/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.173/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.171/src/ansar/connect/node.py` & `ansar_connect-0.1.173/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.171/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.173/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.171/src/ansar/connect/procedure.py` & `ansar_connect-0.1.173/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.171/src/ansar/connect/product.py` & `ansar_connect-0.1.173/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.171/src/ansar/connect/socketry.py` & `ansar_connect-0.1.173/src/ansar/connect/socketry.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 
 import queue as sq
 import threading as thr
 import errno
 import socket
 import select
 import re
+import uuid
+import nacl.utils
+from nacl.public import PrivateKey, PublicKey, Box
 import ansar.create as ar
 
 from copy import copy
 
 __all__ = [
 	'HostPort',
 	'LocalPort',
@@ -324,20 +327,21 @@
 		self.s = s
 		self.request = request
 		self.listening = listening
 		self.controller_address = controller_address
 		self.upgrade = upgrade
 
 class TcpClient(object):
-	def __init__(self, s, request, connected, controller_address, upgrade):
+	def __init__(self, s, request, connected, controller_address, upgrade, encrypted):
 		self.s = s
 		self.request = request
 		self.connected = connected
 		self.controller_address = controller_address
 		self.upgrade = upgrade
+		self.encrypted = encrypted
 
 # Underlying network constraints.
 #
 TCP_RECV = 1024
 TCP_SEND = 1024
 UDP_RECV = 4096
 UDP_SEND = 4096
@@ -351,21 +355,21 @@
 #
 class Header(object):
 	def __init__(self, to_address=None, return_address=None, tunnel=False):
 		self.to_address = to_address
 		self.return_address = return_address
 		self.tunnel = tunnel
 
-HEADING_SCHEMA = {
+HEADER_SCHEMA = {
 	"to_address": ar.TargetAddress(),
 	"return_address": ar.Address(),
 	"tunnel": ar.Boolean(),
 }
 
-ar.bind(Header, object_schema=HEADING_SCHEMA)
+ar.bind(Header, object_schema=HEADER_SCHEMA)
 
 HEADING = ar.UserDefined(Header)
 SPACE = ar.VectorOf(ar.Address())
 
 #
 #
 class Relay(object):
@@ -443,15 +447,21 @@
 				continue
 			if self.byte_part is self.byte_body:
 				self.analysis_state = 1
 				self.size_digits.clear()
 				self.jump_size = 0
 				self.byte_part = self.byte_space
 				continue
-			yield self.byte_header, self.byte_body, self.byte_space
+			if self.encrypting:
+				h = self.encrypting.decrypt(self.byte_header)
+				b_ = self.encrypting.decrypt(self.byte_body)
+				s = self.encrypting.decrypt(self.byte_space)
+				yield h, b_, s
+			else:
+				yield self.byte_header, self.byte_body, self.byte_space
 			self.analysis_state = 1
 			self.size_digits.clear()
 			self.jump_size = 0
 			# Ownership passed with yield. Make new
 			# ones.
 			self.byte_header = bytearray()
 			self.byte_body = bytearray()
@@ -481,62 +491,76 @@
 			a.extend(self.pending)
 			self.pending = []
 		finally:
 			self.lock.release()
 		return count
 
 	def best_block(self, encoded_bytes, codec):
+		encrypted = self.encrypted
 		while len(encoded_bytes) < TCP_SEND:
 			if len(self.messages_to_encode) == 0:
 				added = self.drain(self.messages_to_encode)
 				if added == 0:
 					break
 			m, t, r = self.messages_to_encode.popleft()
 			f = isinstance(m, Blob)
 			h = Header(t, r, f)
 			e = codec.encode(h, HEADING)
 			e = e.encode('utf-8')
+			if encrypted:
+				e = encrypted.encrypt(e)
 			n = len(e)
+			# Stream the header
 			encoded_bytes += str(n).encode('ascii')
 			encoded_bytes += b'\n'
 			encoded_bytes += e
 			encoded_bytes += b'\n'
+			# Then a tunnelled bock, relay or normal message.
 			if f:
 				e = m.block
+				if encrypted:
+					e = encrypted.encrypt(e)
 				n = len(e)
 				encoded_bytes += str(n).encode('ascii')
 				encoded_bytes += b'\n'
 				encoded_bytes += e
 				encoded_bytes += b'\n'
 				# Tunnel block contains no addresses
 				# Could just assign '[]' (an empty JSON list)
 				s = codec.encode([], SPACE)
 			elif isinstance(m, Relay):
 				e = m.block
+				if encrypted:
+					e = encrypted.encrypt(e)
 				n = len(e)
 				encoded_bytes += str(n).encode('ascii')
 				encoded_bytes += b'\n'
 				encoded_bytes += e
 				encoded_bytes += b'\n'
 				s = codec.encode(m.space, SPACE)
 			else:
 				space = []
 				e = codec.encode(m, ar.Any(), space=space)
 				e = e.encode('utf-8')
+				if encrypted:
+					e = encrypted.encrypt(e)
 				n = len(e)
 				encoded_bytes += str(n).encode('ascii')
 				encoded_bytes += b'\n'
 				encoded_bytes += e
 				encoded_bytes += b'\n'
 				s = codec.encode(space, SPACE)
-			s = s.encode('utf-8')
-			n = len(s)
+			# And lastly, the mutated section.
+			e = s.encode('utf-8')
+			if encrypted:
+				e = encrypted.encrypt(e)
+			n = len(e)
 			encoded_bytes += str(n).encode('ascii')
 			encoded_bytes += b'\n'
-			encoded_bytes += s
+			encoded_bytes += e
 			encoded_bytes += b'\n'
 		return len(encoded_bytes)
 
 class TcpStream(StreamingIn, StreamingOut):
 	def __init__(self, parent, controller_address, upgrade, opened, tag):
 		StreamingIn.__init__(self)
 		StreamingOut.__init__(self)
@@ -546,14 +570,16 @@
 		self.upgrade = upgrade
 		self.opened = opened
 		self.tag = tag
 		self.closing = False
 		self.value = None
 		self.codec = None
 		self.encoded_bytes = bytearray()
+		self.encrypted = None
+		self.handshaking = None
 
 	def routing(self, return_proxy, local_termination, remote_address):
 		# Define addresses for message forwarding.
 		# return_proxy ........ address that response should go back to.
 		# local_termination ... address of default target, actor or session.
 		# remote_address ...... source address of connection updates, session or proxy.
 		self.codec = ar.CodecJson(return_proxy=return_proxy, local_termination=local_termination)
@@ -577,15 +603,18 @@
 
 			s = b_.decode('utf-8')
 			body, v = self.codec.decode(s, ar.Any(), space=space)
 			if v is not None:
 				if not self.upgrade:
 					raise ValueError(f'body version "{v}" and no upgrade')
 				body = self.upgrade(body, v)
-			sockets.forward(body, header.to_address, header.return_address)
+			
+			to_address = self.handshaking or header.to_address
+
+			sockets.forward(body, to_address, header.return_address)
 
 	def send_a_block(self, s):
 		t = self.best_block(self.encoded_bytes, self.codec)
 		if t == 0:
 			return False
 		n = t if t <= TCP_SEND else TCP_SEND
 		chunk = self.encoded_bytes[:n]
@@ -594,14 +623,15 @@
 			self.encoded_bytes = self.encoded_bytes[n:]
 			return True
 		return False
 
 #
 #
 class INITIAL: pass
+class PENDING: pass
 class NORMAL: pass
 
 class SocketProxy(ar.Point, ar.StateMachine):
 	def __init__(self, s, channel, stream):
 		ar.Point.__init__(self)
 		ar.StateMachine.__init__(self, INITIAL)
 		self.s = s
@@ -775,15 +805,15 @@
 				self.send(NotConnected(requested_ipp, e, 'Connect incomplete and no pending indication.', m.tag), r)
 				return
 
 			# Build a transient "session" that just exists to catch
 			# an initial, either send or fault (a receive is treated
 			# as an error). True session is constructed on receiving
 			# a "normal" send event.
-			pending = TcpClient(client, m, None, r, m.upgrade)
+			pending = TcpClient(client, m, None, r, m.upgrade, m.encrypted)
 
 			self.networking[client] = pending
 			self.receiving.append(client)
 			self.sending.append(client)
 			self.faulting.append(client)
 			return
 
@@ -802,29 +832,38 @@
 		return
 
 	hap = client.getsockname()
 
 	self.trace('Connected to "%s"(%d), at local address "%s"(%d)' %
 					(requested_ipp.host, requested_ipp.port,
 					hap[0], hap[1]))
+	connected_ipp = HostPort(hap[0], hap[1])
 
 	connected = Connected(requested_ipp=m.requested_ipp,
-		connected_ipp=HostPort(hap[0], hap[1]),
+		connected_ipp=connected_ipp,
 		opened_at=ar.world_now(),
 		tag=m.tag)
 
-	parent = TcpClient(client, m, connected, r, m.upgrade)
+	parent = TcpClient(client, m, connected, r, m.upgrade, m.encrypted)
 	stream, proxy_address = open_stream(self, parent, client, connected)
 	connected.remote_address = proxy_address
 
 	self.networking[client] = stream
 	self.receiving.append(client)
 	self.sending.append(client)
 	self.faulting.append(client)
 
+	if m.encrypted:
+		self.trace(f'Connected (encrypted) "{connected_ipp}", requested "{m.requested_ipp}"')
+		connected_id = uuid.uuid4()
+		self.client_handshake[connected_id] = (connected, r, stream.remote_address)
+		h = self.create(ClientHandshake, connected_id, proxy_address, object_ending=no_ending)
+		stream.handshaking = h
+		return
+
 	self.forward(connected, r, stream.remote_address)
 
 def ControlChannel_StopListening(self, control, mr):
 	m, r = mr
 	listening_ipp = m.listening_ipp
 	def server(t):
 		if not isinstance(t, TcpServer):
@@ -902,34 +941,37 @@
 	try:
 		accepted, hap = s.accept()
 		accepted.setblocking(False)
 	except socket.error as e:
 		self.send(NotAccepted(listening.requested_ipp, e.errno, str(e), listening.tag), server.controller_address)
 		return
 
-	if listening.context:
-		self.trace(f'Encrypting accept as TLS server')
-
-	self.trace( 'Accepted "%s"(%d), server at "%s"(%d)' %
-				   (hap[0], hap[1],
-				   listening.listening_ipp.host, listening.listening_ipp.port))
-
 	opened_at = ar.world_now()
 	stream, proxy_address = open_stream(self, server, accepted, None)
 	self.receiving.append(accepted)
 	self.sending.append(accepted)
 	self.faulting.append(accepted)
 
+	accepted_ipp = HostPort(hap[0], hap[1])
+
 	accepted = Accepted(listening_ipp=listening.listening_ipp,
-		accepted_ipp=HostPort(hap[0], hap[1]),
-		remote_address=stream.remote_address,
-		opened_at=opened_at,
-		tag=listening.tag)
+		accepted_ipp=accepted_ipp, remote_address=stream.remote_address,
+		opened_at=opened_at, tag=listening.tag)
 	stream.opened = accepted
 
+	if listening.context:
+		self.trace(f'Accepted (encrypted) "{accepted_ipp}", listening at "{listening.listening_ipp}"')
+		accepted_id = uuid.uuid4()
+		self.server_handshake[accepted_id] = (accepted, server.controller_address, stream.remote_address)
+		h = self.create(ServerHandshake, accepted_id, object_ending=no_ending)
+		stream.handshaking = h
+		return
+
+	self.trace(f'Accepted "{accepted_ipp}", listening at "{listening.listening_ipp}"')
+
 	self.forward(accepted, server.controller_address, stream.remote_address)
 
 def TcpServer_BrokenTransport(self, server, s):
 	listening = server.listening
 	self.send(NotListening(listening.listening_ipp, 0, "signaled by networking subsystem"), server.controller_address)
 	self.clear(s, TcpServer)
 
@@ -954,28 +996,36 @@
 	#stream, proxy_address = open_stream(self, selector, client, connected.opened_at)
 	#connected.remote_address = proxy_address
 
 	try:
 		scrap = s.recv(TCP_RECV)
 
 		# No exception. New stream.
+		connected_ipp = HostPort(hap[0], hap[1])
 		connected = Connected(requested_ipp=request.requested_ipp,
-			connected_ipp=HostPort(hap[0], hap[1]),
+			connected_ipp=connected_ipp,
 			opened_at=ar.world_now(),
 			tag=request.tag)
 
 		selector.connected = connected
 		stream, proxy_address = open_stream(self, selector, client, connected)
 		connected.remote_address = proxy_address
 
 		self.trace( 'Connected to "%s"(%d), at local address "%s"(%d)' %
 					   (request.requested_ipp.host, request.requested_ipp.port,
 					   hap[0], hap[1]))
 
-		self.forward(connected, stream.controller_address, stream.remote_address)
+		if selector.encrypted:
+			self.trace(f'Connected (encrypted) "{connected_ipp}", requested "{request.requested_ipp}"')
+			connected_id = uuid.uuid4()
+			self.client_handshake[connected_id] = (connected, stream.controller_address, stream.remote_address)
+			h = self.create(ClientHandshake, connected_id, object_ending=no_ending)
+			stream.handshaking = h
+		else:
+			self.forward(connected, stream.controller_address, stream.remote_address)
 
 		if not scrap:
 			# Immediate shutdown. Need to
 			# generate the full set of messages.
 			#self.clear(s, TcpStream)
 			return
 
@@ -996,29 +1046,38 @@
 
 def TcpClient_ReadyToSend(self, selector, s):
 	client = s
 	#self.sending.remove(client)
 
 	request = selector.request
 	hap = client.getsockname()
+	connected_ipp=HostPort(hap[0], hap[1])
 	connected = Connected(requested_ipp=request.requested_ipp,
-		connected_ipp=HostPort(hap[0], hap[1]),
+		connected_ipp=connected_ipp,
 		opened_at=ar.world_now(),
 		tag=request.tag)
 	selector.connected = connected
 
 	self.trace( 'Connected to "%s"(%d), at local address "%s"(%d)' %
 				   (request.requested_ipp.host, request.requested_ipp.port,
 				   hap[0], hap[1]))
 
 	stream, proxy_address = open_stream(self, selector, client, connected)
 	connected.remote_address = proxy_address
 	#receiving.append( client)
 	#self.faulting.append( client)
 
+	if selector.encrypted:
+		self.trace(f'Connected (encrypted) "{connected_ipp}", requested "{request.requested_ipp}"')
+		connected_id = uuid.uuid4()
+		self.client_handshake[connected_id] = (connected, stream.controller_address, stream.remote_address)
+		h = self.create(ClientHandshake, connected_id, object_ending=no_ending)
+		stream.handshaking = h
+		return
+
 	self.forward(connected, stream.controller_address, stream.remote_address)
 
 def TcpClient_BrokenTransport(self, selector, s):
 	text = 'fault on pending connect, unreachable, no service at that address or blocked'
 	self.send(NotConnected(selector.requested_ipp, 0, text, selector.tag), selector.controller_address)
 	self.clear(s, TcpClient)
 
@@ -1207,15 +1266,16 @@
 		self.sending = []
 		self.faulting = self.receiving + self.sending
 
 		# Live.
 		self.running = True
 
 		# Encryption.
-		self.handshaking = set()
+		self.server_handshake = {}
+		self.client_handshake = {}
 
 	def clear(self, s, expected=None):
 		# Remove the specified socket from operations.
 		try:
 			t = self.networking[s]
 		except KeyError:
 			self.warning('Attempt to remove unknown socket')
@@ -1312,7 +1372,124 @@
 				continue
 			j(self, a, f)
 
 	control_close(self.lac)
 	self.complete()
 
 ar.bind(SocketSelect, (ar.Start,))
+
+#
+#
+class ServerEncrypting(object):
+	def __init__(self, accepted_id=None, private_key=None, public_key=None):
+		self.accepted_id = accepted_id
+		self.private_key = private_key
+		self.public_key = public_key
+
+class ClientEncrypting(object):
+	def __init__(self, connected_id=None, private_key=None, public_key=None):
+		self.connected_id = connected_id
+		self.private_key = private_key
+		self.public_key = public_key
+
+class NotEncrypting(object):
+	def __init__(self):
+		pass
+
+ENCRYPTING_SCHEMA = {
+	'accepted_id': ar.UUID(),
+	'connected_id': ar.UUID(),
+	'private_key': ar.Any(),
+	'public_key': ar.Any(),
+}
+
+ar.bind(ServerEncrypting, object_schema=ENCRYPTING_SCHEMA, copy_before_sending=False)
+ar.bind(ClientEncrypting, object_schema=ENCRYPTING_SCHEMA, copy_before_sending=False)
+ar.bind(NotEncrypting, object_schema=ENCRYPTING_SCHEMA, copy_before_sending=False)
+
+class ServerHandshake(ar.Point, ar.StateMachine):
+	def __init__(self, accepted_id):
+		ar.Point.__init__(self)
+		ar.StateMachine.__init__(self, INITIAL)
+		self.accepted_id = accepted_id
+		self.private_key = None
+
+def ServerHandshake_INITIAL_Start(self, message):
+	self.private_key = PrivateKey.generate()
+	self.start(ar.T1, seconds=4.0)
+	return PENDING
+
+def ServerHandshake_PENDING_Blob(self, message):
+	# Got the clients public key.
+	# Respond with our own.
+	public_key = self.private_key.public_key
+	public_blob = Blob(public_key.encode())
+	self.reply(public_blob)
+	self.send(ServerEncrypting(self.accepted_id, self.private_key, PublicKey(message.block)), socket_thread)
+	self.complete()
+
+def ServerHandshake_PENDING_Unknown(self, message):
+	self.send(NotEncrypting(self.accepted_id), socket_thread)
+	self.complete()
+
+def ServerHandshake_PENDING_T1(self, message):
+	self.send(NotEncrypting(self.accepted_id), socket_thread)
+	self.complete()
+
+def ServerHandshake_PENDING_Stop(self, message):
+	self.complete()
+
+SERVER_HANDSHAKE_DISPATCH = {
+	INITIAL: (
+		(ar.Start,), ()
+	),
+	PENDING: (
+		(Blob, ar.Unknown, ar.T1, ar.Stop), ()
+	),
+}
+
+ar.bind(ServerHandshake, SERVER_HANDSHAKE_DISPATCH)
+
+
+class ClientHandshake(ar.Point, ar.StateMachine):
+	def __init__(self, connected_id, remote_address):
+		ar.Point.__init__(self)
+		ar.StateMachine.__init__(self, INITIAL)
+		self.connected_id = connected_id
+		self.remote_address = remote_address
+		self.private_key = None
+
+def ClientHandshake_INITIAL_Start(self, message):
+	self.private_key = PrivateKey.generate()
+	public_key = self.private_key.public_key
+	public_blob = Blob(public_key.encode())
+	self.send(public_blob, self.remote_address)
+	self.start(ar.T1, seconds=4.0)
+	return PENDING
+
+def ClientHandshake_PENDING_Blob(self, message):
+	# Sent our public key.
+	# Expecting one from remote.
+	self.send(ClientEncrypting(self.connected_id, self.private_key, PublicKey(message.block)), socket_thread)
+	self.complete()
+
+def ClientHandshake_PENDING_Unknown(self, message):
+	self.send(NotEncrypting(self.connected_id), socket_thread)
+	self.complete()
+
+def ClientHandshake_PENDING_T1(self, message):
+	self.send(NotEncrypting(self.connected_id), socket_thread)
+	self.complete()
+
+def ClientHandshake_PENDING_Stop(self, message):
+	self.complete()
+
+CLIENT_HANDSHAKE_DISPATCH = {
+	INITIAL: (
+		(ar.Start,), ()
+	),
+	PENDING: (
+		(Blob, ar.Unknown, ar.T1, ar.Stop), ()
+	),
+}
+
+ar.bind(ClientHandshake, CLIENT_HANDSHAKE_DISPATCH)
```

### Comparing `ansar_connect-0.1.171/src/ansar/connect/standard.py` & `ansar_connect-0.1.173/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.171/src/ansar/connect/transporting.py` & `ansar_connect-0.1.173/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.171/src/ansar/connect/wan.py` & `ansar_connect-0.1.173/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.171/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.173/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.171
+Version: 0.1.173
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.171/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.173/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

