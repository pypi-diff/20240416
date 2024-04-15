# Comparing `tmp/zcached.py-1.0.1.tar.gz` & `tmp/zcached.py-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zcached.py-1.0.1.tar", last modified: Fri Mar 22 21:04:53 2024, max compression
+gzip compressed data, was "zcached.py-1.1.1.tar", last modified: Mon Apr 15 22:47:28 2024, max compression
```

## Comparing `zcached.py-1.0.1.tar` & `zcached.py-1.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 szymon    (1000) szymon    (1000)        0 2024-03-22 21:04:53.862249 zcached.py-1.0.1/
--rw-r--r--   0 szymon    (1000) szymon    (1000)     1063 2024-03-12 17:47:09.000000 zcached.py-1.0.1/LICENSE
--rw-r--r--   0 szymon    (1000) szymon    (1000)     3702 2024-03-22 21:04:53.862249 zcached.py-1.0.1/PKG-INFO
--rw-r--r--   0 szymon    (1000) szymon    (1000)      119 2024-03-19 00:15:51.000000 zcached.py-1.0.1/pyproject.toml
--rw-r--r--   0 szymon    (1000) szymon    (1000)       38 2024-03-22 21:04:53.862249 zcached.py-1.0.1/setup.cfg
--rw-r--r--   0 szymon    (1000) szymon    (1000)     1811 2024-03-22 21:04:53.000000 zcached.py-1.0.1/setup.py
-drwxr-xr-x   0 szymon    (1000) szymon    (1000)        0 2024-03-22 21:04:53.862249 zcached.py-1.0.1/tests/
--rw-r--r--   0 szymon    (1000) szymon    (1000)        0 2024-03-10 15:35:07.000000 zcached.py-1.0.1/tests/__init__.py
--rw-r--r--   0 szymon    (1000) szymon    (1000)      567 2024-03-10 20:30:36.000000 zcached.py-1.0.1/tests/test_backoff.py
--rw-r--r--   0 szymon    (1000) szymon    (1000)     1685 2024-03-19 20:31:25.000000 zcached.py-1.0.1/tests/test_connection.py
--rw-r--r--   0 szymon    (1000) szymon    (1000)     1289 2024-03-18 22:59:57.000000 zcached.py-1.0.1/tests/test_deserializer.py
--rw-r--r--   0 szymon    (1000) szymon    (1000)      564 2024-03-18 22:59:57.000000 zcached.py-1.0.1/tests/test_reader.py
--rw-r--r--   0 szymon    (1000) szymon    (1000)      716 2024-03-18 22:59:57.000000 zcached.py-1.0.1/tests/test_result.py
--rw-r--r--   0 szymon    (1000) szymon    (1000)     2190 2024-03-19 16:03:05.000000 zcached.py-1.0.1/tests/test_serializer.py
-drwxr-xr-x   0 szymon    (1000) szymon    (1000)        0 2024-03-22 21:04:53.862249 zcached.py-1.0.1/zcached/
--rw-r--r--   0 szymon    (1000) szymon    (1000)      501 2024-03-22 21:03:23.000000 zcached.py-1.0.1/zcached/__init__.py
--rw-r--r--   0 szymon    (1000) szymon    (1000)     1692 2024-03-10 20:48:50.000000 zcached.py-1.0.1/zcached/backoff.py
--rw-r--r--   0 szymon    (1000) szymon    (1000)     5911 2024-03-22 21:03:08.000000 zcached.py-1.0.1/zcached/client.py
--rw-r--r--   0 szymon    (1000) szymon    (1000)     7507 2024-03-19 20:31:25.000000 zcached.py-1.0.1/zcached/connection.py
--rw-r--r--   0 szymon    (1000) szymon    (1000)     2831 2024-03-19 16:03:13.000000 zcached.py-1.0.1/zcached/deserializer.py
--rw-r--r--   0 szymon    (1000) szymon    (1000)     1998 2024-03-18 22:59:57.000000 zcached.py-1.0.1/zcached/reader.py
--rw-r--r--   0 szymon    (1000) szymon    (1000)     1987 2024-03-18 22:59:57.000000 zcached.py-1.0.1/zcached/result.py
--rw-r--r--   0 szymon    (1000) szymon    (1000)     3227 2024-03-19 16:03:05.000000 zcached.py-1.0.1/zcached/serializer.py
-drwxr-xr-x   0 szymon    (1000) szymon    (1000)        0 2024-03-22 21:04:53.862249 zcached.py-1.0.1/zcached.py.egg-info/
--rw-r--r--   0 szymon    (1000) szymon    (1000)     3702 2024-03-22 21:04:53.000000 zcached.py-1.0.1/zcached.py.egg-info/PKG-INFO
--rw-r--r--   0 szymon    (1000) szymon    (1000)      520 2024-03-22 21:04:53.000000 zcached.py-1.0.1/zcached.py.egg-info/SOURCES.txt
--rw-r--r--   0 szymon    (1000) szymon    (1000)        1 2024-03-22 21:04:53.000000 zcached.py-1.0.1/zcached.py.egg-info/dependency_links.txt
--rw-r--r--   0 szymon    (1000) szymon    (1000)       26 2024-03-22 21:04:53.000000 zcached.py-1.0.1/zcached.py.egg-info/requires.txt
--rw-r--r--   0 szymon    (1000) szymon    (1000)       14 2024-03-22 21:04:53.000000 zcached.py-1.0.1/zcached.py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 22:47:28.131732 zcached.py-1.1.1/
+-rw-rw-rw-   0        0        0     1084 2024-04-08 18:44:53.000000 zcached.py-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     3702 2024-04-15 22:47:28.130226 zcached.py-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      126 2024-04-08 18:44:53.000000 zcached.py-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-15 22:47:28.131732 zcached.py-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1385 2024-04-15 22:47:05.000000 zcached.py-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:47:28.110210 zcached.py-1.1.1/tests/
+-rw-rw-rw-   0        0        0      589 2024-04-08 18:44:53.000000 zcached.py-1.1.1/tests/test_backoff.py
+-rw-rw-rw-   0        0        0     1742 2024-04-15 22:08:29.000000 zcached.py-1.1.1/tests/test_connection.py
+-rw-rw-rw-   0        0        0     1338 2024-04-08 18:44:53.000000 zcached.py-1.1.1/tests/test_deserializer.py
+-rw-rw-rw-   0        0        0      587 2024-04-08 18:44:53.000000 zcached.py-1.1.1/tests/test_reader.py
+-rw-rw-rw-   0        0        0      820 2024-04-15 22:09:01.000000 zcached.py-1.1.1/tests/test_result.py
+-rw-rw-rw-   0        0        0     2271 2024-04-08 18:44:53.000000 zcached.py-1.1.1/tests/test_serializer.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:47:28.120711 zcached.py-1.1.1/zcached/
+-rw-rw-rw-   0        0        0      584 2024-04-15 22:37:38.000000 zcached.py-1.1.1/zcached/__init__.py
+-rw-rw-rw-   0        0        0     1757 2024-04-08 18:44:53.000000 zcached.py-1.1.1/zcached/backoff.py
+-rw-rw-rw-   0        0        0     6175 2024-04-15 22:22:20.000000 zcached.py-1.1.1/zcached/client.py
+-rw-rw-rw-   0        0        0     7530 2024-04-15 22:09:11.000000 zcached.py-1.1.1/zcached/connection.py
+-rw-rw-rw-   0        0        0     2739 2024-04-15 22:09:01.000000 zcached.py-1.1.1/zcached/deserializer.py
+-rw-rw-rw-   0        0        0     1058 2024-04-15 22:09:11.000000 zcached.py-1.1.1/zcached/enums.py
+-rw-rw-rw-   0        0        0     2073 2024-04-08 21:02:12.000000 zcached.py-1.1.1/zcached/reader.py
+-rw-rw-rw-   0        0        0     2274 2024-04-15 22:09:01.000000 zcached.py-1.1.1/zcached/result.py
+-rw-rw-rw-   0        0        0     3324 2024-04-15 22:09:01.000000 zcached.py-1.1.1/zcached/serializer.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:47:28.129229 zcached.py-1.1.1/zcached.py.egg-info/
+-rw-rw-rw-   0        0        0     3702 2024-04-15 22:47:27.000000 zcached.py-1.1.1/zcached.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      519 2024-04-15 22:47:27.000000 zcached.py-1.1.1/zcached.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 22:47:27.000000 zcached.py-1.1.1/zcached.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-15 22:47:27.000000 zcached.py-1.1.1/zcached.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-15 22:47:27.000000 zcached.py-1.1.1/zcached.py.egg-info/top_level.txt
```

### Comparing `zcached.py-1.0.1/PKG-INFO` & `zcached.py-1.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,89 +1,84 @@
-Metadata-Version: 2.1
-Name: zcached.py
-Version: 1.0.1
-Summary: A lightweight client-side library for zcached, written in Python.
-Home-page: https://github.com/xxenvy/zcached.py
-Author: xXenvy
-Author-email: <xpimpek01@gmail.com>
-License: MIT
-Project-URL: Issue tracker, https://github.com/xxenvy/zcached.py/issues
-Keywords: python,redis,redisclient
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Typing :: Typed
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: typing_extensions==4.10.0
-
-
-# Zcached.py - A client-side library for zcached.
-
-![commits](https://img.shields.io/github/commit-activity/w/xXenvy/zcached.py?style=for-the-badge&color=%2315b328)
-![license](https://img.shields.io/github/license/xXenvy/zcached.py?style=for-the-badge&color=%2315b328)
-
-## `📜` Introduction
-Zcached.py is a Python client-side library designed to interact with zcached, a high-performance caching system.
-This library provides developers with an easy-to-use interface for integrating zcached into their Python applications, enabling efficient data caching.
-
-For more information, please see [zcached repository](https://github.com/sectasy0/zcached).
-
-## `🌟` Features
-- **Simplified Caching:** Zcached.py simplifies the process of caching data by providing intuitive functions for storing and retrieving values.
-- **Efficient Communication:** The library optimizes communication with the zcached server, ensuring minimal overhead and efficient data transfer.
-- **Properly Typehinted:** The codebase of zcached.py is properly typehinted, enhancing code readability.
-
-## `🔧` Installation
-> [!IMPORTANT]  
-> **Library requires python version 3.8 or newer.** (Older should also work, but untested).
-
-Before installing zcached.py, ensure that you have the zcached server. Instructions for installing the server can be found [here](https://github.com/sectasy0/zcached).
-
-Once the zcached server is installed, you can proceed to install zcached.py using pip:
-```shell
-pip install -U zcached.py
-```
-
-## `🖊️` Usage
-Here's a basic example demonstrating how to use zcached.py in your Python code:
-```py
-from typing import List
-from zcached import ZCached, Result
-
-client = ZCached(host="localhost", port=5555)
-
-if client.is_alive() is False:
-  raise RuntimeError("Something went wrong.")
-
-client.set(key="dogs", value=["Pimpek", "Laika"])
-
-dogs_result: Result[List[str]] = client.get(key="dogs")
-dbsize_result: Result[int] = client.dbsize()
-keys_result: Result[List[str]] = client.keys()
-print(keys_result.value)
-
-client.save()
-client.delete("dogs")
-client.flush()
-```
-**See more examples [here](https://github.com/xXenvy/zcached.py/tree/master/examples)**
-
-## `👥` Contributing
-Contributions to zcached.py are welcome!
-If you encounter any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request.
-
-## `📕` License
-Zcached.py is licensed under the MIT License.
+Metadata-Version: 2.1
+Name: zcached.py
+Version: 1.1.1
+Summary: A lightweight client-side library for zcached, written in Python.
+Home-page: https://github.com/xXenvy/zcached.py
+Author: xXenvy
+Project-URL: Bug Reports, https://github.com/xXenvy/zcached.py/issues
+Project-URL: Source, https://github.com/xXenvy/zcached.py
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: typing-extensions
+
+# Zcached.py - A client-side library for zcached.
+
+![commits](https://img.shields.io/github/commit-activity/w/xXenvy/zcached.py?style=for-the-badge&color=%2315b328)
+![license](https://img.shields.io/github/license/xXenvy/zcached.py?style=for-the-badge&color=%2315b328)
+![release](https://img.shields.io/github/v/release/xXenvy/zcached.py?include_prereleases&style=for-the-badge&color=%2315b328)
+
+## `📜` Introduction
+Zcached.py is a Python client-side library designed to interact with zcached, a high-performance caching system.
+This library provides developers an easy-to-use interface for integrating zcached into their Python applications, enabling efficient data caching.
+
+For more information, please see [zcached repository](https://github.com/sectasy0/zcached).
+
+## `🌟` Features
+- **Simplified Caching:** Zcached.py simplifies the process of caching data by providing intuitive functions for storing and retrieving values.
+- **Efficient Communication:** The library optimizes communication with the zcached server, ensuring minimal overhead and efficient data transfer.
+- **Properly Typehinted:** The codebase of zcached.py is properly typehinted, enhancing code readability.
+
+## `🔧` Installation
+> [!IMPORTANT]  
+> **Library requires python version 3.8 or newer.** (Older also should work, but untested).
+
+Before installing zcached.py, ensure that you have the zcached server. Instructions for installing the server can be found [here](https://github.com/sectasy0/zcached).
+
+Once the zcached server is installed, you can proceed to install zcached.py using pip:
+```shell
+pip install -U zcached.py
+```
+
+## `🖊️` Usage
+Here's a basic example demonstrating how to use zcached.py in your Python code:
+```py
+from typing import List
+from zcached import ZCached, Result
+
+client = ZCached(host="localhost", port=5555)
+client.run()
+
+if client.is_alive() is False:
+  raise RuntimeError("Something went wrong.")
+
+client.set(key="dogs", value=["Pimpek", "Laika"])
+
+dogs_result: Result[List[str]] = client.get(key="dogs")
+dbsize_result: Result[int] = client.dbsize()
+keys_result: Result[List[str]] = client.keys()
+print(keys_result.value)
+
+client.save()
+client.delete("dogs")
+client.flush()
+```
+**See more examples [here](https://github.com/xXenvy/zcached.py/tree/master/examples)**
+
+## `👥` Contributing
+Contributions to zcached.py are welcome!
+If you encounter any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request.
+
+## `📕` License
+Zcached.py is licensed under the MIT License.
```

### Comparing `zcached.py-1.0.1/tests/test_connection.py` & `zcached.py-1.1.1/tests/test_connection.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-import pytest
-from zcached import Connection, Result, ZCached
-
-IS_SERVER_RUNNING = False
-
-
-def test_connection():
-    connection = Connection(
-        host="localhost", port=5555, connection_attempts=2, buff_size=2, reconnect=False
-    )
-
-    assert connection.host == "localhost"
-    assert connection.port == 5555
-    assert connection.buff_size == 2
-    assert connection.connection_attempts == 2
-    assert connection.is_connected is False
-    assert connection.socket.getblocking() is True
-
-    if not IS_SERVER_RUNNING:
-        connection.connect()
-        assert not connection.is_connected
-
-        with pytest.raises(OSError):
-            connection.receive()
-        with pytest.raises(OSError):
-            connection.wait_for_response()
-    else:
-        connection.connect()
-        assert connection.is_connected is True
-
-        client = ZCached.from_connection(connection)
-
-        for _ in range(5):
-            result: Result[str] = client.ping()
-            assert result.success and result.value == "PONG"
-            assert not result.is_empty()
-
-        assert client.connection.receive() is None
-
-        result = client.set(
-            "randomkey",
-            {
-                "key": "value1",
-                "key2": 1233,
-                "key3": -32,
-                "key4": 5.4,
-                "key5": True,
-                "key6": False,
-                "key7": None,
-                "key8": ["abc", 123, False, None, True, {"a": "b", "c": "d"}],
-                "key9": "4343434343",
-                "key10": (-50, -60, -70, None),
-            },
-        )
-        assert result.error is None
-        assert result.value == "OK"
-        client.flush()
+import pytest
+from zcached import Connection, Result, ZCached
+
+IS_SERVER_RUNNING = False
+
+
+def test_connection():
+    connection = Connection(
+        host="localhost", port=5555, connection_attempts=2, buff_size=2, reconnect=False
+    )
+
+    assert connection.host == "localhost"
+    assert connection.port == 5555
+    assert connection.buff_size == 2
+    assert connection.connection_attempts == 2
+    assert connection.is_connected is False
+    assert connection.socket.getblocking() is True
+
+    if not IS_SERVER_RUNNING:
+        connection.connect()
+        assert not connection.is_connected
+
+        with pytest.raises(OSError):
+            connection.receive()
+        with pytest.raises(OSError):
+            connection.wait_for_response()
+    else:
+        connection.connect()
+        assert connection.is_connected is True
+
+        client = ZCached.from_connection(connection)
+
+        for _ in range(5):
+            result: Result[str] = client.ping()
+            assert result.success and result.value == "PONG"
+            assert not result.is_empty()
+
+        assert client.connection.receive() is None
+
+        result = client.set(
+            "randomkey",
+            {
+                "key": "value1",
+                "key2": 1233,
+                "key3": -32,
+                "key4": 5.4,
+                "key5": True,
+                "key6": False,
+                "key7": None,
+                "key8": ["abc", 123, False, None, True, {"a": "b", "c": "d"}],
+                "key9": "4343434343",
+                "key10": (-50, -60, -70, None),
+            },
+        )
+        assert result.error is None
+        assert result.value == "OK"
+        client.flush()
```

### Comparing `zcached.py-1.0.1/tests/test_deserializer.py` & `zcached.py-1.1.1/tests/test_deserializer.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-from __future__ import annotations
-
-import pytest
-from zcached import Deserializer, Reader
-
-test_values = {
-    b"%3\r\n$1\r\n2\r\n$5\r\nhello\r\n$1\r\n1\r\n:50\r\n$1\r\n5\r\n,-5\r\n": {
-        "2": "hello",
-        "1": 50,
-        "5": -5.0,
-    },
-    b"$7\r\ntest123\r\n": "test123",
-    b"*6\r\n,5\r\n,1\r\n#f\r\n:10\r\n_\r\n$5\r\narray\r\n": [
-        5.0,
-        1.0,
-        False,
-        10,
-        None,
-        "array",
-    ],
-    b"%1\r\n$3\r\npik\r\n*3\r\n_\r\n#f\r\n*2\r\n:1\r\n:2\r\n": {
-        "pik": [None, False, [1, 2]]
-    },
-    b"#f\r\n": False,
-    b"#t\r\n": True,
-    b"_\r\n": None,
-    b":420\r\n": 420,
-    b"$11\r\nhello world\r\n": "hello world",
-}
-
-
-def test_basic() -> None:
-    deserializer: Deserializer = Deserializer()
-
-    assert deserializer.process(Reader(b"#t\r\n")) is True
-    assert deserializer.process(Reader(b"#f\r\n")) is False
-    assert deserializer.process(Reader(b"$3\r\nlol\r\n")) == "lol"
-
-
-@pytest.mark.parametrize("buffer", tuple(test_values.keys()))
-def test_advanced(buffer: bytes) -> None:
-    deserializer: Deserializer = Deserializer()
-
-    expected = test_values[buffer]
-    reader = Reader(buffer)
-    assert deserializer.process(reader) == expected
-
-    with pytest.raises(KeyError):
-        deserializer.process(reader)
+from __future__ import annotations
+
+import pytest
+from zcached import Deserializer, Reader
+
+test_values = {
+    b"%3\r\n$1\r\n2\r\n$5\r\nhello\r\n$1\r\n1\r\n:50\r\n$1\r\n5\r\n,-5\r\n": {
+        "2": "hello",
+        "1": 50,
+        "5": -5.0,
+    },
+    b"$7\r\ntest123\r\n": "test123",
+    b"*6\r\n,5\r\n,1\r\n#f\r\n:10\r\n_\r\n$5\r\narray\r\n": [
+        5.0,
+        1.0,
+        False,
+        10,
+        None,
+        "array",
+    ],
+    b"%1\r\n$3\r\npik\r\n*3\r\n_\r\n#f\r\n*2\r\n:1\r\n:2\r\n": {
+        "pik": [None, False, [1, 2]]
+    },
+    b"#f\r\n": False,
+    b"#t\r\n": True,
+    b"_\r\n": None,
+    b":420\r\n": 420,
+    b"$11\r\nhello world\r\n": "hello world",
+}
+
+
+def test_basic() -> None:
+    deserializer: Deserializer = Deserializer()
+
+    assert deserializer.process(Reader(b"#t\r\n")) is True
+    assert deserializer.process(Reader(b"#f\r\n")) is False
+    assert deserializer.process(Reader(b"$3\r\nlol\r\n")) == "lol"
+
+
+@pytest.mark.parametrize("buffer", tuple(test_values.keys()))
+def test_advanced(buffer: bytes) -> None:
+    deserializer: Deserializer = Deserializer()
+
+    expected = test_values[buffer]
+    reader = Reader(buffer)
+    assert deserializer.process(reader) == expected
+
+    with pytest.raises(KeyError):
+        deserializer.process(reader)
```

### Comparing `zcached.py-1.0.1/tests/test_reader.py` & `zcached.py-1.1.1/tests/test_reader.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import pytest
-from zcached import Reader
-
-
-def test_reader():
-    reader = Reader(b"*3\r\n+test\r\n$3\r\nlol\r\n:590")
-
-    assert reader.position == 0
-    assert reader.buffer == b"*3\n+test\n$3\nlol\n:590"
-
-    assert reader.read(1) == b"*"
-    assert int(reader.read(1)) == 3
-    assert reader.position == 2
-
-    with pytest.raises(RuntimeError):
-        assert reader.read_until(b"4343")
-
-    assert reader.read_until(b"lol") == b"\n+test\n$3\n"
-
-    with pytest.raises(RuntimeError):
-        assert reader.read_until(b"lol")
-
-    assert reader.position == 15
+import pytest
+from zcached import Reader
+
+
+def test_reader():
+    reader = Reader(b"*3\r\n+test\r\n$3\r\nlol\r\n:590")
+
+    assert reader.position == 0
+    assert reader.buffer == b"*3\n+test\n$3\nlol\n:590"
+
+    assert reader.read(1) == b"*"
+    assert int(reader.read(1)) == 3
+    assert reader.position == 2
+
+    with pytest.raises(RuntimeError):
+        assert reader.read_until(b"4343")
+
+    assert reader.read_until(b"lol") == b"\n+test\n$3\n"
+
+    with pytest.raises(RuntimeError):
+        assert reader.read_until(b"lol")
+
+    assert reader.position == 15
```

### Comparing `zcached.py-1.0.1/tests/test_serializer.py` & `zcached.py-1.1.1/tests/test_serializer.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-from typing import Any, List
-
-import pytest
-from zcached import Serializer
-
-test_values = {
-    "test_string_new_abc_test": "$24\r\ntest_string_new_abc_test\r\n",
-    52: ":52\r\n",
-    0.01: ",0.01\r\n",
-    0.5: ",0.5\r\n",
-    None: "_\r\n",
-    False: "#f\r\n",
-    True: "#t\r\n",
-    "5454": "$4\r\n5454\r\n",
-    -1: ":-1\r\n",
-    -0.001: ",-0.001\r\n",
-}
-
-
-def test_basic_serializer():
-    serializer = Serializer()
-
-    with pytest.raises(TypeError):
-        serializer.process(object())  # type: ignore
-
-    assert serializer.process("string_test") == "$11\r\nstring_test\r\n"
-
-    with pytest.raises(AssertionError):
-        serializer.serialize_bool("string_test")
-
-
-def test_dict_serializer():
-    value = {"a": 10, "b": 1.0, "c": "text", "d": True, "e": False, "f": None}
-    serializer = Serializer()
-
-    assert serializer.process(value) == (
-        "%6\r\n$1\r\na\r\n:10\r\n$1\r\nb\r\n,1.0\r\n$1\r\nc\r\n"
-        "$4\r\ntext\r\n$1\r\nd\r\n#t\r\n$1\r\ne\r\n#f\r\n$1\r\nf\r\n_\r\n"
-    )
-
-
-@pytest.mark.parametrize("value", tuple(test_values.keys()))
-def test_serializer(value: Any):
-    serializer = Serializer()
-
-    assert serializer.process(value) == test_values[value]
-
-    with pytest.raises(AssertionError):
-        _ = serializer.serialize_list(value)
-
-
-def test_list_serializer():
-    arrays: List[List[Any]] = []
-
-    for index, value in enumerate(test_values.keys()):
-        arrays.append(list(test_values.keys())[: index + 1])
-
-    for array in arrays:
-        expected_expression: str = f"*{len(array)}\r\n"
-
-        for element in array:
-            expected_expression += test_values[element]
-
-        serializer = Serializer()
-
-        with pytest.raises(AssertionError):
-            _ = serializer.serialize_int(array)
-
-        assert serializer.process(array) == expected_expression
-
-
-@pytest.mark.parametrize("value", ("bul^)^+kstr#!ing$!%@#" * 25 * x for x in range(5)))
-def test_bulk_serializer(value: str):
-    expected_expression: str = f"${len(value)}\r\n{value}\r\n"
-
-    serializer = Serializer()
-
-    with pytest.raises(AssertionError):
-        _ = serializer.serialize_float(value)
-
-    assert serializer.process(value) == expected_expression
+from typing import Any, List
+
+import pytest
+from zcached import Serializer
+
+test_values = {
+    "test_string_new_abc_test": "$24\r\ntest_string_new_abc_test\r\n",
+    52: ":52\r\n",
+    0.01: ",0.01\r\n",
+    0.5: ",0.5\r\n",
+    None: "_\r\n",
+    False: "#f\r\n",
+    True: "#t\r\n",
+    "5454": "$4\r\n5454\r\n",
+    -1: ":-1\r\n",
+    -0.001: ",-0.001\r\n",
+}
+
+
+def test_basic_serializer():
+    serializer = Serializer()
+
+    with pytest.raises(TypeError):
+        serializer.process(object())  # type: ignore
+
+    assert serializer.process("string_test") == "$11\r\nstring_test\r\n"
+
+    with pytest.raises(AssertionError):
+        serializer.serialize_bool("string_test")
+
+
+def test_dict_serializer():
+    value = {"a": 10, "b": 1.0, "c": "text", "d": True, "e": False, "f": None}
+    serializer = Serializer()
+
+    assert serializer.process(value) == (
+        "%6\r\n$1\r\na\r\n:10\r\n$1\r\nb\r\n,1.0\r\n$1\r\nc\r\n"
+        "$4\r\ntext\r\n$1\r\nd\r\n#t\r\n$1\r\ne\r\n#f\r\n$1\r\nf\r\n_\r\n"
+    )
+
+
+@pytest.mark.parametrize("value", tuple(test_values.keys()))
+def test_serializer(value: Any):
+    serializer = Serializer()
+
+    assert serializer.process(value) == test_values[value]
+
+    with pytest.raises(AssertionError):
+        _ = serializer.serialize_list(value)
+
+
+def test_list_serializer():
+    arrays: List[List[Any]] = []
+
+    for index, value in enumerate(test_values.keys()):
+        arrays.append(list(test_values.keys())[: index + 1])
+
+    for array in arrays:
+        expected_expression: str = f"*{len(array)}\r\n"
+
+        for element in array:
+            expected_expression += test_values[element]
+
+        serializer = Serializer()
+
+        with pytest.raises(AssertionError):
+            _ = serializer.serialize_int(array)
+
+        assert serializer.process(array) == expected_expression
+
+
+@pytest.mark.parametrize("value", ("bul^)^+kstr#!ing$!%@#" * 25 * x for x in range(5)))
+def test_bulk_serializer(value: str):
+    expected_expression: str = f"${len(value)}\r\n{value}\r\n"
+
+    serializer = Serializer()
+
+    with pytest.raises(AssertionError):
+        _ = serializer.serialize_float(value)
+
+    assert serializer.process(value) == expected_expression
```

### Comparing `zcached.py-1.0.1/zcached/backoff.py` & `zcached.py-1.1.1/zcached/backoff.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-from __future__ import annotations
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from typing_extensions import Self
-
-
-class ExponentialBackoff:
-    """
-    Implementation of the exponential backoff algorithm.
-
-    Parameters
-    ----------
-    initial:
-        The initial value for the exponential.
-    multiplier:
-        Value to multiply initial value.
-    max_value:
-        The maximum value of the exponential.
-
-    Attributes
-    ----------
-    current: :class:`float`
-        The current value of the exponential.
-    """
-
-    __slots__ = ("current", "_multiplier", "_max", "_initial", "_total")
-
-    def __init__(self, initial: float, multiplier: float, max_value: float) -> None:
-        self.current: float = 0
-
-        self._multiplier: float = multiplier
-        self._max: float = max_value
-        self._total: float = 0.0
-
-        self._initial: float = initial
-
-    def __repr__(self) -> str:
-        return f"<ExponentialBackoff(current={self.current}, next={self.next}, total={self.total})>"
-
-    def __iter__(self) -> Self:
-        return self
-
-    def __next__(self) -> float:
-        if self.current:
-            self.current = self.next
-            self._total += self.current
-        else:
-            self.current = self._initial
-        return self.current
-
-    @property
-    def next(self) -> float:
-        """Next value of exponential."""
-        return min(self._max, self.current * self._multiplier)
-
-    @property
-    def total(self) -> float:
-        """Total value of exponential."""
-        return self._total
-
-    def reset(self) -> None:
-        """Method to reset the exponential backoff."""
-        self.current = 0
-        self._total = 0.0
+from __future__ import annotations
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from typing_extensions import Self
+
+
+class ExponentialBackoff:
+    """
+    Implementation of the exponential backoff algorithm.
+
+    Parameters
+    ----------
+    initial:
+        The initial value for the exponential.
+    multiplier:
+        Value to multiply initial value.
+    max_value:
+        The maximum value of the exponential.
+
+    Attributes
+    ----------
+    current: :class:`float`
+        The current value of the exponential.
+    """
+
+    __slots__ = ("current", "_multiplier", "_max", "_initial", "_total")
+
+    def __init__(self, initial: float, multiplier: float, max_value: float) -> None:
+        self.current: float = 0
+
+        self._multiplier: float = multiplier
+        self._max: float = max_value
+        self._total: float = 0.0
+
+        self._initial: float = initial
+
+    def __repr__(self) -> str:
+        return f"<ExponentialBackoff(current={self.current}, next={self.next}, total={self.total})>"
+
+    def __iter__(self) -> Self:
+        return self
+
+    def __next__(self) -> float:
+        if self.current:
+            self.current = self.next
+            self._total += self.current
+        else:
+            self.current = self._initial
+        return self.current
+
+    @property
+    def next(self) -> float:
+        """Next value of exponential."""
+        return min(self._max, self.current * self._multiplier)
+
+    @property
+    def total(self) -> float:
+        """Total value of exponential."""
+        return self._total
+
+    def reset(self) -> None:
+        """Method to reset the exponential backoff."""
+        self.current = 0
+        self._total = 0.0
```

### Comparing `zcached.py-1.0.1/zcached/connection.py` & `zcached.py-1.1.1/zcached/connection.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,227 +1,224 @@
-from __future__ import annotations
-
-import logging
-from socket import socket, SOCK_STREAM, AF_INET
-
-from time import sleep
-
-from .backoff import ExponentialBackoff
-from .result import Result
-
-
-class Connection:
-    """
-    An object to establish and manage a connection with the database server.
-
-    Parameters
-    ----------
-    host:
-        The host address of the server to connect to.
-    port:
-        The port number of the server to connect to.
-    buff_size:
-        The size of the buffer for receiving data from the server, in bytes.
-        Larger values for buff_size may allow for more data to be received in a single operation,
-        while smaller values can be more memory-efficient but slower.
-    connection_attempts:
-        The maximum number of attempts to establish a connection with the server.
-        If the maximum number of attempts is exceeded, an error will be raised.
-    reconnect:
-        Flag indicating whether automatic reconnection attempt should be made
-        in case of a broken connection.
-
-    Attributes
-    ----------
-    socket: :class:`socket`
-        The socket object for communicating with the server.
-    buff_size: :class:`int`
-        The size of the buffer for receiving data from the server.
-    connection_attempts:
-        The maximum number of attempts to establish a connection with the server.
-    reconnect:
-        Flag indicating whether automatic reconnection attempt should be made
-        in case of a broken connection.
-    """
-
-    __slots__ = (
-        "socket",
-        "buff_size",
-        "connection_attempts",
-        "reconnect",
-        "_backoff",
-        "_port",
-        "_host",
-        "_connected",
-    )
-
-    def __init__(
-        self,
-        host: str,
-        port: int,
-        connection_attempts: int,
-        reconnect: bool,
-        buff_size: int = 1024,
-    ):
-        self.socket: socket = socket(AF_INET, SOCK_STREAM)
-        self.buff_size: int = buff_size
-        self.connection_attempts: int = connection_attempts
-        self.reconnect: bool = reconnect
-
-        self._host: str = host
-        self._port: int = port
-
-        self._connected: bool = False
-        self._backoff = ExponentialBackoff(0.5, 2, 3)
-
-    def __repr__(self) -> str:
-        return f"<Connection(host={self.host}, port={self.port}, buff_size={self.buff_size})>"
-
-    @property
-    def host(self) -> str:
-        """Connection host."""
-        return self._host
-
-    @property
-    def port(self) -> int:
-        """Connection port."""
-        return self._port
-
-    @property
-    def is_connected(self) -> bool:
-        """
-        A boolean indicating whether the `connect` method was successfully invoked.
-
-        .. note::
-            This does not mean that the socket has a connection to the server.
-            The socket connection may be broken, and we do not update it constantly.
-        """
-        return self._connected
-
-    def connect(self) -> None:
-        """
-        Method to connect a socket to a database server.
-        """
-        logging.debug(f"Connecting to {self.host}:{self.port}...")
-
-        for attempt, timeout in enumerate(self._backoff):
-            try:
-                self.socket.connect((self.host, self.port))
-                self.socket.setblocking(False)
-
-                logging.info("Connected to the server.")
-                self._connected = True
-                break
-            except Exception as exception:
-                if attempt + 1 >= self.connection_attempts:
-                    break
-
-                logging.exception(exception)
-                logging.warning("Connecting to the server failed. Retrying...")
-                sleep(timeout)
-
-    def receive(self) -> bytes | None:
-        """
-        Method to receive the response from the server.
-        None if the server didn't receive any data yet.
-        """
-        try:
-            data: bytes = self.socket.recv(self.buff_size)
-            logging.debug("Received a response -> %s", data)
-        except BlockingIOError:
-            return None
-
-        return data
-
-    def send(self, data: bytes) -> Result:
-        """
-        Method to send data to the server.
-
-        Parameters
-        ----------
-        data: :class:`bytes`
-            Data to send.
-        """
-        try:
-            logging.debug("Sending data to the server -> %s", data)
-            self.socket.send(data)
-        except BrokenPipeError:
-            # This exception occurs when the socket has no connection to the database server.
-            if not self.reconnect:
-                return Result.fail("The connection has been terminated.")
-
-            return self.try_reconnect()
-
-        result: Result = self.wait_for_response()
-        if not self.reconnect or result.error is None:
-            return result
-
-        if result.error != "The connection has been terminated.":
-            return result
-
-        return self.try_reconnect()
-
-    def try_reconnect(self) -> Result[bytes]:
-        """
-        A method to attempt to reconnect to the server if the connection is broken.
-
-        .. note::
-            If the connection is successfully reestablished, the method return a Result object
-            with a failure status and an informational message indicating that the connection
-            was terminated but managed to reestablish it.
-        """
-        logging.debug("Attempting to reconnect to the server...")
-
-        self.socket: socket = socket(AF_INET, SOCK_STREAM)
-        self._connected = False
-        self.connect()
-
-        if self.is_connected is True:
-            return Result.fail(
-                "The connection was terminated, but managed to reestablish it."
-            )
-
-        return Result.fail("The connection has been terminated.")
-
-    def wait_for_response(self) -> Result:
-        """A loop to wait for the response from the server."""
-        backoff: ExponentialBackoff = ExponentialBackoff(0.1, 1.5, 0.5)
-
-        total_bytes: bytes = bytes()
-        transfer_complete: bool = False
-
-        for timeout in backoff:
-            data: bytes | None = self.receive()
-
-            if not isinstance(data, bytes):
-                if len(total_bytes) > 0:
-                    # If we already have some data, and this iteration gave us None,
-                    # it means that the data transfer has been completed.
-                    transfer_complete = True
-                else:
-                    # We haven't received any data yet.
-                    logging.debug(
-                        f"There is no data in the socket. Timeout: {timeout}s."
-                    )
-                    sleep(timeout)
-                    continue
-
-            if transfer_complete:
-                # If the first byte is "-", it means that the response is an error.
-                if total_bytes.startswith(b"-"):
-                    return Result.fail(total_bytes.decode())
-
-                return Result.ok(total_bytes)
-
-            if len(data) == 0:  # type: ignore
-                # When socket lose connection to the server it receives empty bytes.
-                return Result.fail("The connection has been terminated.")
-
-            total_bytes += data  # type: ignore
-
-            # ExponentialBackoff should be increased only when we receive None.
-            backoff.reset()
-
-        # This should never happen, but the type checker yells.
-        return Result.fail(
-            "This is probably a bug. Please report it here: https://github.com/xXenvy/zcached.py"
-        )
+from __future__ import annotations
+
+import logging
+from socket import socket, SOCK_STREAM, AF_INET
+
+from time import sleep
+
+from .backoff import ExponentialBackoff
+from .result import Result
+from .enums import Errors
+
+
+class Connection:
+    """
+    An object to establish and manage a connection with the database server.
+
+    Parameters
+    ----------
+    host:
+        The host address of the server to connect to.
+    port:
+        The port number of the server to connect to.
+    buff_size:
+        The size of the buffer for receiving data from the server, in bytes.
+        Larger values for buff_size may allow for more data to be received in a single operation,
+        while smaller values can be more memory-efficient but slower.
+    connection_attempts:
+        The maximum number of attempts to establish a connection with the server.
+        If the maximum number of attempts is exceeded, an error will be raised.
+    reconnect:
+        Flag indicating whether automatic reconnection attempt should be made
+        in case of a broken connection.
+
+    Attributes
+    ----------
+    socket:
+        The socket object for communicating with the server.
+    buff_size:
+        The size of the buffer for receiving data from the server.
+    connection_attempts:
+        The maximum number of attempts to establish a connection with the server.
+    reconnect:
+        Flag indicating whether automatic reconnection attempt should be made
+        in case of a broken connection.
+    """
+
+    __slots__ = (
+        "socket",
+        "buff_size",
+        "connection_attempts",
+        "reconnect",
+        "_backoff",
+        "_port",
+        "_host",
+        "_connected",
+    )
+
+    def __init__(
+        self,
+        host: str,
+        port: int,
+        connection_attempts: int,
+        reconnect: bool,
+        buff_size: int = 1024,
+    ):
+        self.socket: socket = socket(AF_INET, SOCK_STREAM)
+        self.buff_size: int = buff_size
+        self.connection_attempts: int = connection_attempts
+        self.reconnect: bool = reconnect
+
+        self._host: str = host
+        self._port: int = port
+
+        self._connected: bool = False
+        self._backoff = ExponentialBackoff(0.5, 2, 3)
+
+    def __repr__(self) -> str:
+        return f"<Connection(host={self.host}, port={self.port}, buff_size={self.buff_size})>"
+
+    @property
+    def host(self) -> str:
+        """Connection host."""
+        return self._host
+
+    @property
+    def port(self) -> int:
+        """Connection port."""
+        return self._port
+
+    @property
+    def is_connected(self) -> bool:
+        """
+        A boolean indicating whether the `connect` method was successfully invoked.
+
+        .. note::
+            This does not mean that the socket has a connection to the server.
+            The socket connection may be broken, and we do not update it constantly.
+        """
+        return self._connected
+
+    def connect(self) -> None:
+        """
+        Method to connect a socket to the database server.
+        """
+        logging.debug(f"Connecting to {self.host}:{self.port}...")
+
+        for attempt, timeout in enumerate(self._backoff):
+            try:
+                self.socket.connect((self.host, self.port))
+                self.socket.setblocking(False)
+
+                logging.info("Connected to the server.")
+                self._connected = True
+                break
+            except Exception as exception:
+                if attempt + 1 >= self.connection_attempts:
+                    break
+
+                logging.exception(exception)
+                logging.warning("Connecting to the server failed. Retrying...")
+                sleep(timeout)
+
+    def receive(self) -> bytes | None:
+        """
+        Method to receive the response from the server.
+        None if there is no data in the socket yet.
+        """
+        try:
+            data: bytes = self.socket.recv(self.buff_size)
+            logging.debug("Received a response -> %s", data)
+        except BlockingIOError:
+            return None
+
+        return data
+
+    def send(self, data: bytes) -> Result:
+        """
+        Method to send data to the server.
+
+        Parameters
+        ----------
+        data:
+            Bytes to send.
+        """
+        try:
+            logging.debug("Sending data to the server -> %s", data)
+            self.socket.send(data)
+        except (BrokenPipeError, OSError):
+            if not self.reconnect:
+                return Result.fail(Errors.ConnectionClosed.value)
+
+            return self.try_reconnect()
+
+        result: Result = self.wait_for_response()
+        if not self.reconnect or result.error is None:
+            return result
+
+        if result.error == Errors.ConnectionClosed:
+            return self.try_reconnect()
+
+        return result
+
+    def try_reconnect(self) -> Result[bytes]:
+        """
+        A method to attempt to reconnect to the server if the connection is broken.
+
+        .. note::
+            If the connection is successfully reestablished, the method return a Result object
+            with a failure status and an informational message indicating that the connection
+            was terminated but managed to reestablish it.
+        """
+        logging.debug("Attempting to reconnect to the server...")
+
+        self.socket: socket = socket(AF_INET, SOCK_STREAM)
+        self._connected = False
+        self.connect()
+
+        if self.is_connected is True:
+            return Result.fail(Errors.ConnectionReestablished.value)
+
+        return Result.fail(Errors.ConnectionClosed.value)
+
+    def wait_for_response(self) -> Result:
+        """A loop to wait for the response from the server."""
+        backoff: ExponentialBackoff = ExponentialBackoff(0.1, 1.5, 0.5)
+
+        total_bytes: bytes = bytes()
+        transfer_complete: bool = False
+
+        for timeout in backoff:
+            data: bytes | None = self.receive()
+
+            if not isinstance(data, bytes):
+                if len(total_bytes) > 0:
+                    # If we already have some data, and this iteration gave us None,
+                    # it means that the data transfer has been completed.
+                    transfer_complete = True
+                else:
+                    # We haven't received any data yet.
+                    logging.debug(
+                        f"There is no data in the socket. Timeout: {timeout}s."
+                    )
+                    sleep(timeout)
+                    continue
+
+            if transfer_complete:
+                # If the first byte is "-", it means that the response is an error.
+                if total_bytes.startswith(b"-"):
+                    error_message: str = total_bytes.decode()[1::]
+                    return Result.fail(error_message.replace("\r\n", ""))
+
+                return Result.ok(total_bytes)
+
+            if len(data) == 0:  # type: ignore
+                # When socket lose connection to the server it receives empty bytes.
+                return Result.fail(Errors.ConnectionClosed.value)
+
+            total_bytes += data  # type: ignore
+
+            # ExponentialBackoff should be increased only when we receive None.
+            backoff.reset()
+
+        # This should never happen, but the type checker yells.
+        return Result.fail(Errors.LibraryBug.value)
```

### Comparing `zcached.py-1.0.1/zcached/reader.py` & `zcached.py-1.1.1/zcached/reader.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-from __future__ import annotations
-
-
-class Reader:
-    """
-    Implementation of the reader interface which helps reading data from raw bytes.
-
-    Parameters
-    ----------
-    payload:
-        Payload to read.
-
-    Attributes
-    ----------
-    buffer:
-        Provided payload.
-    position:
-        Current reader position.
-    """
-
-    __slots__ = ("buffer", "position")
-
-    def __init__(self, payload: bytes) -> None:
-        self.buffer: bytes = payload.replace(b"\r", b"")
-        self.position: int = 0
-
-    def __repr__(self) -> str:
-        return f"<Reader(position={self.position})>"
-
-    def read_until(self, element: bytes) -> bytes:
-        """
-        Method to read bytes from the buffer until the specified element is encountered.
-
-        Parameters
-        ----------
-        element:
-            The byte sequence indicating the end of reading.
-
-        Raises
-        ------
-        RuntimeError
-            There is no specific item in the buffer starting from the current position.
-
-        Notes
-        -----
-        This method reads bytes from the buffer until the specified `element` is encountered.
-        It starts reading from the current position in the buffer.
-        """
-        if element not in self.buffer[self.position : :]:
-            raise RuntimeError(
-                "There is no specific element in the buffer starting from the current position."
-            )
-
-        total: bytes = self.read(1)
-
-        while not total.endswith(element):
-            total += self.read(1)
-
-        return total[: -len(element)]
-
-    def read(self, size: int | None = None) -> bytes:
-        """
-        Method to read bytes starting at current position.
-
-        Parameters
-        ----------
-        size:
-            Number of bytes to read.
-        """
-        if size is None:
-            size = len(self.buffer) - self.position
-
-        data: bytes = self.buffer[self.position : self.position + size]
-        self.position += len(data)
-        return data
+from __future__ import annotations
+
+
+class Reader:
+    """
+    Implementation of the reader interface which helps reading data from raw bytes.
+
+    Parameters
+    ----------
+    payload:
+        Payload to read.
+
+    Attributes
+    ----------
+    buffer:
+        Provided payload.
+    position:
+        Current reader position.
+    """
+
+    __slots__ = ("buffer", "position")
+
+    def __init__(self, payload: bytes) -> None:
+        self.buffer: bytes = payload.replace(b"\r", b"")
+        self.position: int = 0
+
+    def __repr__(self) -> str:
+        return f"<Reader(position={self.position})>"
+
+    def read_until(self, element: bytes) -> bytes:
+        """
+        Method to read bytes from the buffer until the specified element is encountered.
+
+        Parameters
+        ----------
+        element:
+            The byte sequence indicating the end of reading.
+
+        Raises
+        ------
+        RuntimeError
+            There is no specific item in the buffer starting from the current position.
+
+        Notes
+        -----
+        This method reads bytes from the buffer until the specified `element` is encountered.
+        It starts reading from the current position in the buffer.
+        """
+        if element not in self.buffer[self.position : :]:
+            raise RuntimeError(
+                "There is no specific element in the buffer starting from the current position."
+            )
+
+        total: bytes = self.read(1)
+
+        while not total.endswith(element):
+            total += self.read(1)
+
+        return total[: -len(element)]
+
+    def read(self, size: int | None = None) -> bytes:
+        """
+        Method to read bytes starting at current position.
+
+        Parameters
+        ----------
+        size:
+            Number of bytes to read.
+        """
+        if size is None:
+            size = len(self.buffer) - self.position
+
+        data: bytes = self.buffer[self.position : self.position + size]
+        self.position += len(data)
+        return data
```

### Comparing `zcached.py-1.0.1/zcached/result.py` & `zcached.py-1.1.1/zcached/result.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,79 @@
-from __future__ import annotations
-from typing import Any, Generic, TypeVar, ClassVar
-
-from .deserializer import Deserializer
-from .reader import Reader
-
-T = TypeVar("T")
-
-
-class Result(Generic[T]):
-    """
-    Represents the result of the server response.
-
-    Attributes
-    ----------
-    value:
-        Operation result. Stores empty bytes if the operation fails.
-    error:
-        Error message detailing why the operation failed, value is None if
-        operation was successful.
-    """
-
-    __slots__ = ("value", "error")
-    _deserializer: ClassVar[Deserializer] = Deserializer()
-
-    def __init__(self, value: bytes, error: str | None = None):
-        if error is not None:
-            # If we have an error, the value will be empty, so there is no point in deserializing it.
-            self.value: T = value  # type: ignore
-        else:
-            self.value: T = self._deserializer.process(Reader(value))
-
-        self.error: str | None = error
-
-    def __hash__(self) -> int:
-        return hash((self.value, self.error))
-
-    def __eq__(self, other: Any) -> bool:
-        return hash(other) == hash(self)
-
-    def __ne__(self, other: Any) -> bool:
-        return not self.__eq__(other)
-
-    def __repr__(self):
-        return f"<Result(success={self.success})>"
-
-    @property
-    def success(self) -> bool:
-        """True if the operation was successful."""
-        return self.error is None
-
-    @property
-    def failure(self) -> bool:
-        """True if operation failed."""
-        return self.error is not None
-
-    @classmethod
-    def fail(cls, error: str):
-        """Create a Result object for a failed operation."""
-        return cls(value=bytes(), error=error)
-
-    @classmethod
-    def ok(cls, value: bytes):
-        """Create a Result object for a successful operation."""
-        return cls(value=value)
-
-    def is_empty(self) -> bool:
-        """Checks if the value is empty."""
-        return isinstance(self.value, bytes) and not bool(self.value)
+from __future__ import annotations
+from typing import Any, Generic, TypeVar, ClassVar
+
+from .deserializer import Deserializer
+from .reader import Reader
+
+T = TypeVar("T")
+
+
+class Result(Generic[T]):
+    """
+    Represents the result of the server response.
+
+    Parameters
+    ----------
+    value:
+        A raw value to deserialize.
+    error:
+        Error message detailing why the operation failed.
+
+    Attributes
+    ----------
+    value:
+        Operation result. Stores empty bytes if the operation fails.
+    error:
+        Error message detailing why the operation failed, value is None if
+        operation was successful.
+    """
+
+    __slots__ = ("value", "error")
+    _deserializer: ClassVar[Deserializer] = Deserializer()
+
+    def __init__(self, value: bytes, error: str | None = None):
+        if error is not None:
+            # If we have an error, the value will be empty, so there is no point in deserializing it.
+            self.value: T = value  # type: ignore
+        else:
+            self.value: T = self._deserializer.process(Reader(value))
+
+        self.error: str | None = error
+
+    def __hash__(self) -> int:
+        return hash((self.value, self.error))
+
+    def __eq__(self, other: Any) -> bool:
+        return hash(other) == hash(self)
+
+    def __ne__(self, other: Any) -> bool:
+        return not self.__eq__(other)
+
+    def __bool__(self) -> bool:
+        return self.success
+
+    def __repr__(self):
+        return f"<Result(success={self.success})>"
+
+    @property
+    def success(self) -> bool:
+        """True if the operation was successful."""
+        return self.error is None
+
+    @property
+    def failure(self) -> bool:
+        """True if operation failed."""
+        return self.error is not None
+
+    @classmethod
+    def fail(cls, error: str):
+        """Create a Result object for a failed operation."""
+        return cls(value=bytes(), error=error)
+
+    @classmethod
+    def ok(cls, value: bytes):
+        """Create a Result object for a successful operation."""
+        return cls(value=value)
+
+    def is_empty(self) -> bool:
+        """Checks if the value is empty."""
+        return isinstance(self.value, bytes) and not bool(self.value)
```

### Comparing `zcached.py-1.0.1/zcached/serializer.py` & `zcached.py-1.1.1/zcached/serializer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-from typing import Union, Callable
-
-SupportedTypes = Union[str, int, float, bool, list, tuple, dict, set, None]
-
-
-class Serializer:
-    """
-    A class for serializing Python objects into string payload.
-    """
-
-    def process(self, value: SupportedTypes) -> str:
-        """
-        Serialize the given value into its string representation.
-
-        Parameters
-        ----------
-        value:
-            Object to serialize.
-
-        Raises
-        ------
-        TypeError
-            If the type of value is not supported for serialization.
-        """
-        if not isinstance(value, SupportedTypes):
-            raise TypeError(
-                "Specified value for serialization has an unsupported type."
-                f"Currently the serializer supports: {SupportedTypes}"
-            )
-
-        if value is None:
-            return self.none()
-
-        # Python versions 3.9, 3.8 do not support match statements ahh moment.
-        handlers: dict[type, Callable[[SupportedTypes], str]] = {
-            str: self.serialize_str,
-            int: self.serialize_int,
-            float: self.serialize_float,
-            bool: self.serialize_bool,
-            list: self.serialize_list,
-            tuple: self.serialize_tuple,
-            set: self.serialize_set,
-            dict: self.serialize_dict,
-        }
-        return handlers[type(value)](value)
-
-    @staticmethod
-    def serialize_str(value: SupportedTypes) -> str:
-        """Returns the serialized value of type str."""
-        assert isinstance(value, str)
-        return f"${len(value)}\r\n{value}\r\n"
-
-    @staticmethod
-    def serialize_int(value: SupportedTypes) -> str:
-        """Returns the serialized value of type int."""
-        assert isinstance(value, int)
-        return f":{value}\r\n"
-
-    @staticmethod
-    def serialize_float(value: SupportedTypes) -> str:
-        """Returns the serialized value of type float."""
-        assert isinstance(value, float)
-        return f",{value}\r\n"
-
-    @staticmethod
-    def serialize_bool(value: SupportedTypes) -> str:
-        """Returns the serialized value of type bool."""
-        assert isinstance(value, bool)
-        return "#{}\r\n".format("t" if value else "f")
-
-    def serialize_list(self, value: SupportedTypes) -> str:
-        """Returns the serialized value of type list."""
-        assert isinstance(value, (list, tuple, set))
-        return f"*{len(value)}\r\n" + "".join((self.process(item) for item in value))
-
-    def serialize_tuple(self, value: SupportedTypes) -> str:
-        """Returns the serialized value of type tuple."""
-        return self.serialize_list(value)
-
-    def serialize_set(self, value: SupportedTypes) -> str:
-        """Returns the serialized value of type set."""
-        return self.serialize_list(value)
-
-    def serialize_dict(self, value: SupportedTypes) -> str:
-        """Returns the serialized value of type dict."""
-        assert isinstance(value, dict)
-        text: str = f"%{len(value)}\r\n"
-
-        for k, v in value.items():
-            text += f"${len(str(k))}\r\n{k}\r\n{self.process(v)}"
-
-        return text
-
-    @staticmethod
-    def none() -> str:
-        """Returns the serialized value of type None."""
-        return "_\r\n"
+from typing import Union, Callable
+
+SupportedTypes = Union[str, int, float, bool, list, tuple, dict, set, None]
+
+
+class Serializer:
+    """
+    A class for serializing Python objects into string payload.
+    """
+
+    def process(self, value: SupportedTypes) -> str:
+        """
+        Serialize the given value into its string representation.
+
+        Parameters
+        ----------
+        value:
+            The Object to serialize.
+
+        Raises
+        ------
+        TypeError
+            If the type of value is not supported by serializer.
+        """
+        if not isinstance(value, SupportedTypes):
+            raise TypeError(
+                "Specified value for serialization has an unsupported type."
+                f"Currently the serializer supports: {SupportedTypes}"
+            )
+
+        if value is None:
+            return self.none()
+
+        # Python versions 3.9, 3.8 do not support match statements ahh moment.
+        handlers: dict[type, Callable[[SupportedTypes], str]] = {
+            str: self.serialize_str,
+            int: self.serialize_int,
+            float: self.serialize_float,
+            bool: self.serialize_bool,
+            list: self.serialize_list,
+            tuple: self.serialize_tuple,
+            set: self.serialize_set,
+            dict: self.serialize_dict,
+        }
+        return handlers[type(value)](value)
+
+    @staticmethod
+    def serialize_str(value: SupportedTypes) -> str:
+        """Returns the serialized value of type str."""
+        assert isinstance(value, str)
+        return f"${len(value)}\r\n{value}\r\n"
+
+    @staticmethod
+    def serialize_int(value: SupportedTypes) -> str:
+        """Returns the serialized value of type int."""
+        assert isinstance(value, int)
+        return f":{value}\r\n"
+
+    @staticmethod
+    def serialize_float(value: SupportedTypes) -> str:
+        """Returns the serialized value of type float."""
+        assert isinstance(value, float)
+        return f",{value}\r\n"
+
+    @staticmethod
+    def serialize_bool(value: SupportedTypes) -> str:
+        """Returns the serialized value of type bool."""
+        assert isinstance(value, bool)
+        return "#{}\r\n".format("t" if value else "f")
+
+    def serialize_list(self, value: SupportedTypes) -> str:
+        """Returns the serialized value of type list."""
+        assert isinstance(value, (list, tuple, set))
+        return f"*{len(value)}\r\n" + "".join((self.process(item) for item in value))
+
+    def serialize_tuple(self, value: SupportedTypes) -> str:
+        """Returns the serialized value of type tuple."""
+        return self.serialize_list(value)
+
+    def serialize_set(self, value: SupportedTypes) -> str:
+        """Returns the serialized value of type set."""
+        return self.serialize_list(value)
+
+    def serialize_dict(self, value: SupportedTypes) -> str:
+        """Returns the serialized value of type dict."""
+        assert isinstance(value, dict)
+        text: str = f"%{len(value)}\r\n"
+
+        for k, v in value.items():
+            text += f"${len(str(k))}\r\n{k}\r\n{self.process(v)}"
+
+        return text
+
+    @staticmethod
+    def none() -> str:
+        """Returns the serialized value of type None."""
+        return "_\r\n"
```

### Comparing `zcached.py-1.0.1/zcached.py.egg-info/PKG-INFO` & `zcached.py-1.1.1/zcached.py.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,89 +1,84 @@
-Metadata-Version: 2.1
-Name: zcached.py
-Version: 1.0.1
-Summary: A lightweight client-side library for zcached, written in Python.
-Home-page: https://github.com/xxenvy/zcached.py
-Author: xXenvy
-Author-email: <xpimpek01@gmail.com>
-License: MIT
-Project-URL: Issue tracker, https://github.com/xxenvy/zcached.py/issues
-Keywords: python,redis,redisclient
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Typing :: Typed
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: typing_extensions==4.10.0
-
-
-# Zcached.py - A client-side library for zcached.
-
-![commits](https://img.shields.io/github/commit-activity/w/xXenvy/zcached.py?style=for-the-badge&color=%2315b328)
-![license](https://img.shields.io/github/license/xXenvy/zcached.py?style=for-the-badge&color=%2315b328)
-
-## `📜` Introduction
-Zcached.py is a Python client-side library designed to interact with zcached, a high-performance caching system.
-This library provides developers with an easy-to-use interface for integrating zcached into their Python applications, enabling efficient data caching.
-
-For more information, please see [zcached repository](https://github.com/sectasy0/zcached).
-
-## `🌟` Features
-- **Simplified Caching:** Zcached.py simplifies the process of caching data by providing intuitive functions for storing and retrieving values.
-- **Efficient Communication:** The library optimizes communication with the zcached server, ensuring minimal overhead and efficient data transfer.
-- **Properly Typehinted:** The codebase of zcached.py is properly typehinted, enhancing code readability.
-
-## `🔧` Installation
-> [!IMPORTANT]  
-> **Library requires python version 3.8 or newer.** (Older should also work, but untested).
-
-Before installing zcached.py, ensure that you have the zcached server. Instructions for installing the server can be found [here](https://github.com/sectasy0/zcached).
-
-Once the zcached server is installed, you can proceed to install zcached.py using pip:
-```shell
-pip install -U zcached.py
-```
-
-## `🖊️` Usage
-Here's a basic example demonstrating how to use zcached.py in your Python code:
-```py
-from typing import List
-from zcached import ZCached, Result
-
-client = ZCached(host="localhost", port=5555)
-
-if client.is_alive() is False:
-  raise RuntimeError("Something went wrong.")
-
-client.set(key="dogs", value=["Pimpek", "Laika"])
-
-dogs_result: Result[List[str]] = client.get(key="dogs")
-dbsize_result: Result[int] = client.dbsize()
-keys_result: Result[List[str]] = client.keys()
-print(keys_result.value)
-
-client.save()
-client.delete("dogs")
-client.flush()
-```
-**See more examples [here](https://github.com/xXenvy/zcached.py/tree/master/examples)**
-
-## `👥` Contributing
-Contributions to zcached.py are welcome!
-If you encounter any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request.
-
-## `📕` License
-Zcached.py is licensed under the MIT License.
+Metadata-Version: 2.1
+Name: zcached.py
+Version: 1.1.1
+Summary: A lightweight client-side library for zcached, written in Python.
+Home-page: https://github.com/xXenvy/zcached.py
+Author: xXenvy
+Project-URL: Bug Reports, https://github.com/xXenvy/zcached.py/issues
+Project-URL: Source, https://github.com/xXenvy/zcached.py
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: typing-extensions
+
+# Zcached.py - A client-side library for zcached.
+
+![commits](https://img.shields.io/github/commit-activity/w/xXenvy/zcached.py?style=for-the-badge&color=%2315b328)
+![license](https://img.shields.io/github/license/xXenvy/zcached.py?style=for-the-badge&color=%2315b328)
+![release](https://img.shields.io/github/v/release/xXenvy/zcached.py?include_prereleases&style=for-the-badge&color=%2315b328)
+
+## `📜` Introduction
+Zcached.py is a Python client-side library designed to interact with zcached, a high-performance caching system.
+This library provides developers an easy-to-use interface for integrating zcached into their Python applications, enabling efficient data caching.
+
+For more information, please see [zcached repository](https://github.com/sectasy0/zcached).
+
+## `🌟` Features
+- **Simplified Caching:** Zcached.py simplifies the process of caching data by providing intuitive functions for storing and retrieving values.
+- **Efficient Communication:** The library optimizes communication with the zcached server, ensuring minimal overhead and efficient data transfer.
+- **Properly Typehinted:** The codebase of zcached.py is properly typehinted, enhancing code readability.
+
+## `🔧` Installation
+> [!IMPORTANT]  
+> **Library requires python version 3.8 or newer.** (Older also should work, but untested).
+
+Before installing zcached.py, ensure that you have the zcached server. Instructions for installing the server can be found [here](https://github.com/sectasy0/zcached).
+
+Once the zcached server is installed, you can proceed to install zcached.py using pip:
+```shell
+pip install -U zcached.py
+```
+
+## `🖊️` Usage
+Here's a basic example demonstrating how to use zcached.py in your Python code:
+```py
+from typing import List
+from zcached import ZCached, Result
+
+client = ZCached(host="localhost", port=5555)
+client.run()
+
+if client.is_alive() is False:
+  raise RuntimeError("Something went wrong.")
+
+client.set(key="dogs", value=["Pimpek", "Laika"])
+
+dogs_result: Result[List[str]] = client.get(key="dogs")
+dbsize_result: Result[int] = client.dbsize()
+keys_result: Result[List[str]] = client.keys()
+print(keys_result.value)
+
+client.save()
+client.delete("dogs")
+client.flush()
+```
+**See more examples [here](https://github.com/xXenvy/zcached.py/tree/master/examples)**
+
+## `👥` Contributing
+Contributions to zcached.py are welcome!
+If you encounter any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request.
+
+## `📕` License
+Zcached.py is licensed under the MIT License.
```

### Comparing `zcached.py-1.0.1/zcached.py.egg-info/SOURCES.txt` & `zcached.py-1.1.1/zcached.py.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 LICENSE
 pyproject.toml
 setup.py
-tests/__init__.py
 tests/test_backoff.py
 tests/test_connection.py
 tests/test_deserializer.py
 tests/test_reader.py
 tests/test_result.py
 tests/test_serializer.py
 zcached/__init__.py
 zcached/backoff.py
 zcached/client.py
 zcached/connection.py
 zcached/deserializer.py
+zcached/enums.py
 zcached/reader.py
 zcached/result.py
 zcached/serializer.py
 zcached.py.egg-info/PKG-INFO
 zcached.py.egg-info/SOURCES.txt
 zcached.py.egg-info/dependency_links.txt
 zcached.py.egg-info/requires.txt
```

