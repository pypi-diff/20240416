# Comparing `tmp/async-irc-0.1.8.tar.gz` & `tmp/async_irc-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async-irc-0.1.8.tar", last modified: Fri Mar 29 00:37:48 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `async-irc-0.1.8.tar` & `async_irc-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 00:37:48.943104 async-irc-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-29 00:37:40.000000 async-irc-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-03-29 00:37:48.943104 async-irc-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-29 00:37:40.000000 async-irc-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 00:37:48.943104 async-irc-0.1.8/async_irc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-03-29 00:37:48.000000 async-irc-0.1.8/async_irc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-29 00:37:48.000000 async-irc-0.1.8/async_irc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 00:37:48.000000 async-irc-0.1.8/async_irc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-29 00:37:48.000000 async-irc-0.1.8/async_irc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-29 00:37:48.000000 async-irc-0.1.8/async_irc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 00:37:48.943104 async-irc-0.1.8/asyncirc/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-29 00:37:40.000000 async-irc-0.1.8/asyncirc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13339 2024-03-29 00:37:40.000000 async-irc-0.1.8/asyncirc/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-03-29 00:37:40.000000 async-irc-0.1.8/asyncirc/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 00:37:48.943104 async-irc-0.1.8/asyncirc/util/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-29 00:37:40.000000 async-irc-0.1.8/asyncirc/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-03-29 00:37:40.000000 async-irc-0.1.8/asyncirc/util/backoff.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-29 00:37:48.943104 async-irc-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-29 00:37:40.000000 async-irc-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 00:37:48.943104 async-irc-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-29 00:37:40.000000 async-irc-0.1.8/tests/test_imports.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 async_irc-0.2.0/.editorconfig
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 async_irc-0.2.0/.gitattributes
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 async_irc-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 async_irc-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 async_irc-0.2.0/codecov.yml
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 async_irc-0.2.0/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 async_irc-0.2.0/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 async_irc-0.2.0/.vscode/extensions.json
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 async_irc-0.2.0/.vscode/settings.json
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 async_irc-0.2.0/asyncirc/__init__.py
+-rw-r--r--   0        0        0    16102 2020-02-02 00:00:00.000000 async_irc-0.2.0/asyncirc/protocol.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 async_irc-0.2.0/asyncirc/py.typed
+-rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 async_irc-0.2.0/asyncirc/server.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 async_irc-0.2.0/asyncirc/util/__init__.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 async_irc-0.2.0/asyncirc/util/backoff.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 async_irc-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 async_irc-0.2.0/tests/test_imports.py
+-rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 async_irc-0.2.0/tests/test_protocol.py
+-rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 async_irc-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 async_irc-0.2.0/LICENSE
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 async_irc-0.2.0/README.md
+-rw-r--r--   0        0        0     4841 2020-02-02 00:00:00.000000 async_irc-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 async_irc-0.2.0/PKG-INFO
```

### Comparing `async-irc-0.1.8/LICENSE` & `async_irc-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `async-irc-0.1.8/PKG-INFO` & `async_irc-0.2.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,28 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: async-irc
-Version: 0.1.8
+Version: 0.2.0
 Summary: A simple asyncio.Protocol implementation designed for IRC
-Home-page: https://github.com/TotallyNotRobots/async-irc
-Author: linuxdaemon
-Author-email: linuxdaemon@snoonet.org
-License: MIT
-Keywords: asyncio irc asyncirc async-irc irc-framework
+Project-URL: Homepage, https://github.com/TotallyNotRobots/async-irc
+Author-email: linuxdaemon <linuxdaemon@snoonet.org>
+License-Expression: MIT
+License-File: LICENSE
+Keywords: async-irc,asyncio,asyncirc,irc,irc-framework
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+Requires-Dist: py-irclib>=0.4.0
+Requires-Dist: typing-extensions
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: py-irclib
 
 # async-irc [![Build Status](https://travis-ci.org/snoonetIRC/async-irc.svg?branch=master)](https://travis-ci.org/snoonetIRC/async-irc)
 An implementation of asyncio.Protocol for IRC
 
 ## Using the library
 - You can install the library using pip: `pip install async-irc`
```

### Comparing `async-irc-0.1.8/README.md` & `async_irc-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `async-irc-0.1.8/asyncirc/protocol.py` & `async_irc-0.2.0/asyncirc/protocol.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,345 +1,492 @@
-# coding=utf-8
 """
 Basic asyncio.Protocol interface for IRC connections
 """
+
 import asyncio
 import base64
 import random
 import socket
 import time
-from asyncio import Protocol
+from asyncio import Protocol, Task
 from collections import defaultdict
 from enum import IntEnum, auto, unique
 from itertools import cycle
-from typing import Sequence, Optional, Tuple, Callable, Dict, Coroutine, AnyStr, TYPE_CHECKING, Any
+from typing import (
+    TYPE_CHECKING,
+    Callable,
+    Coroutine,
+    Dict,
+    List,
+    Optional,
+    Sequence,
+    Tuple,
+    Union,
+    cast,
+)
 
-from irclib.parser import Message, CapList, Cap
+from irclib.parser import Cap, CapList, Message
 
 from asyncirc.server import ConnectedServer
 from asyncirc.util.backoff import AsyncDelayer
 
 if TYPE_CHECKING:
-    from logging import Logger
-    from asyncirc.server import Server, BaseServer
     from asyncio import AbstractEventLoop, Transport
+    from logging import Logger
 
+    from asyncirc.server import BaseServer, Server
 
-__all__ = ('SASLMechanism', 'IrcProtocol')
+
+__all__ = ("SASLMechanism", "IrcProtocol")
 
 
 @unique
 class SASLMechanism(IntEnum):
     """Represents different SASL auth mechanisms"""
+
     NONE = auto()
     PLAIN = auto()
     EXTERNAL = auto()
 
 
-async def _internal_ping(conn: 'IrcProtocol', message: 'Message'):
-    conn.send("PONG {}".format(message.parameters))
+async def _internal_ping(conn: "IrcProtocol", message: "Message") -> None:
+    conn.send(f"PONG {message.parameters}")
+
 
+async def _internal_cap_handler(
+    conn: "IrcProtocol", message: "Message"
+) -> None:
+    if conn.server is None:
+        msg = "Server not set in handler"
+        raise ValueError(msg)
 
-async def _internal_cap_handler(conn: 'IrcProtocol', message: 'Message'):
-    caplist = []
+    caplist: List[Cap] = []
     if len(message.parameters) > 2:
         caplist = CapList.parse(message.parameters[-1])
 
-    if message.parameters[1] == 'LS':
+    if message.parameters[1] == "LS":
         for cap in caplist:
             if cap.name in conn.cap_handlers:
                 conn.server.caps[cap.name] = (cap, None)
 
-        if message.parameters[2] != '*':
-            for cap in conn.server.caps:
-                conn.send("CAP REQ :{}".format(cap))
+        if message.parameters[2] != "*":
+            for cap_name in conn.server.caps:
+                conn.send(f"CAP REQ :{cap_name}")
+
             if not conn.server.caps:
-                conn.send("CAP END")  # We haven't request any CAPs, send a CAP END to end negotiation
+                # We haven't request any CAPs, send a CAP END to end negotiation
+                conn.send("CAP END")
 
-    elif message.parameters[1] in ('ACK', 'NAK'):
-        enabled = message.parameters[1] == 'ACK'
+    elif message.parameters[1] in ("ACK", "NAK"):
+        enabled = message.parameters[1] == "ACK"
         for cap in caplist:
             current = conn.server.caps[cap.name][0]
-            conn.server.caps[cap.name] = (current, enabled)
             if enabled:
                 handlers = filter(None, conn.cap_handlers[cap.name])
                 await asyncio.gather(*[func(conn, cap) for func in handlers])
+
+            conn.server.caps[cap.name] = (current, enabled)
+
         if all(val[1] is not None for val in conn.server.caps.values()):
             conn.send("CAP END")
-    elif message.parameters[1] == 'LIST':
+    elif message.parameters[1] == "LIST":
         if conn.logger:
             conn.logger.info("Current Capabilities: %s", caplist)
-    elif message.parameters[1] == 'NEW':
+    elif message.parameters[1] == "NEW":
         if conn.logger:
             conn.logger.info("New capabilities advertised: %s", caplist)
+
         for cap in caplist:
             if cap.name in conn.cap_handlers:
                 conn.server.caps[cap.name] = (cap, None)
 
-        if message.parameters[2] != '*':
-            for cap in conn.server.caps:
-                conn.send("CAP REQ :{}".format(cap))
-    elif message.parameters[1] == 'DEL':
+        if message.parameters[2] != "*":
+            for cap_name in conn.server.caps:
+                conn.send(f"CAP REQ :{cap_name}")
+    elif message.parameters[1] == "DEL":
         if conn.logger:
             conn.logger.info("Capabilities removed: %s", caplist)
+
         for cap in caplist:
             current = conn.server.caps[cap.name][0]
             conn.server.caps[cap.name] = (current, False)
 
 
-async def _internal_pong(conn: 'IrcProtocol', msg: 'Message'):
-    if msg.parameters[-1].startswith('LAG'):
+async def _internal_pong(conn: "IrcProtocol", msg: "Message") -> None:
+    if conn.server is None:
+        err_msg = "Server not set in handler"
+        raise ValueError(err_msg)
+
+    if msg.parameters[-1].startswith("LAG"):
         now = time.time()
         t = float(msg.parameters[-1][3:])
         if conn.server.last_ping_sent == t:
             conn.server.last_ping_recv = now
             conn.server.lag = now - t
 
 
-async def _do_sasl(conn: 'IrcProtocol', cap):
+async def _do_sasl(conn: "IrcProtocol", cap: Cap) -> None:
+    if conn.server is None:
+        msg = "Server not set in handler"
+        raise ValueError(msg)
+
     if not conn.sasl_mech or conn.sasl_mech is SASLMechanism.NONE:
         return
-    supported_mechs = cap.value
-    if supported_mechs is not None:
-        supported_mechs = supported_mechs.split(',')
+
+    if cap.value is not None:
+        supported_mechs: Optional[List[str]] = cap.value.split(",")
+    else:
+        supported_mechs = None
+
     if supported_mechs and conn.sasl_mech.name not in supported_mechs:
         if conn.logger:
-            conn.logger.warning("Server doesn't support configured SASL mechanism '%s'", conn.sasl_mech)
+            conn.logger.warning(
+                "Server doesn't support configured SASL mechanism '%s'",
+                conn.sasl_mech,
+            )
+
         return
-    conn.send("AUTHENTICATE {}".format(conn.sasl_mech.name))
+
+    conn.send(f"AUTHENTICATE {conn.sasl_mech.name}")
     auth_msg = await conn.wait_for("AUTHENTICATE", timeout=5)
-    if auth_msg and auth_msg.parameters[0] == '+':
-        auth_line = '+'
-        if conn.sasl_mech is SASLMechanism.PLAIN:
+    if auth_msg and auth_msg.parameters[0] == "+":
+        auth_line = "+"
+        if conn.sasl_mech == SASLMechanism.PLAIN:
+            if conn.sasl_auth is None:
+                msg = "You must specify sasl_auth when using SASL PLAIN"
+                raise ValueError(msg)
+
             user, password = conn.sasl_auth
-            auth_line = '\0'.join((user, user, password))
+            auth_line = f"{user}\x00{user}\x00{password}"
             auth_line = base64.b64encode(auth_line.encode()).decode()
-        conn.send("AUTHENTICATE {}".format(auth_line))
+
+        conn.send(f"AUTHENTICATE {auth_line}")
         # Wait for SASL to complete
         # TODO log SASL response
-        await conn.wait_for('902', '903', '904', '905', '906', '907', '908', timeout=30)
+        await conn.wait_for(
+            "902", "903", "904", "905", "906", "907", "908", timeout=30
+        )
 
 
-async def _isupport_handler(conn: 'IrcProtocol', message: 'Message'):
-    tokens = message.parameters[1:-1]  # Remove the nick and trailing ':are supported by this server' message
+async def _isupport_handler(conn: "IrcProtocol", message: "Message") -> None:
+    if conn.server is None:
+        msg = "Server not set in handler"
+        raise ValueError(msg)
+
+    # Remove the nick and trailing ':are supported by this server' message
+    tokens = message.parameters[1:-1]
     for token in tokens:
-        if token[0] == '-' and token.upper() in conn.server.isupport_tokens:
+        if token[0] == "-" and token.upper() in conn.server.isupport_tokens:
             del conn.server.isupport_tokens[token.upper()]
         else:
-            name, _, value = token.partition('=')
+            name, _, value = token.partition("=")
             conn.server.isupport_tokens[name.upper()] = value or None
 
 
-async def _on_001(conn: 'IrcProtocol', message: 'Message'):
+async def _on_001(conn: "IrcProtocol", message: "Message") -> None:
+    if conn.server is None:
+        msg = "Server not set in handler"
+        raise ValueError(msg)
+
+    if not message.prefix:
+        msg = f"Missing prefix in 001: {message}"
+        raise ValueError(msg)
+
     conn.server.server_name = message.prefix.mask
 
 
 class IrcProtocol(Protocol):
     """Async IRC Interface"""
 
-    _transport: Optional['Transport'] = None
+    _transport: Optional["Transport"] = None
     _buff = b""
-    _server: Optional['ConnectedServer'] = None
+    _server: Optional["ConnectedServer"] = None
     _connected = False
     _quitting = False
 
-    def __init__(self, servers: Sequence['Server'], nick: str, user: str = None, realname: str = None,
-                 certpath: str = None, sasl_auth: Tuple[str, str] = None, sasl_mech: SASLMechanism = None,
-                 logger: 'Logger' = None, loop: 'AbstractEventLoop' = None) -> None:
+    def __init__(
+        self,
+        servers: Sequence["Server"],
+        nick: str,
+        user: Optional[str] = None,
+        realname: Optional[str] = None,
+        certpath: Optional[str] = None,
+        sasl_auth: Optional[Tuple[str, str]] = None,
+        sasl_mech: Optional[SASLMechanism] = None,
+        logger: Optional["Logger"] = None,
+        loop: Optional["AbstractEventLoop"] = None,
+    ) -> None:
         self.servers = servers
         self.nick = nick
         self._user = user
         self._realname = realname
         self.certpath = certpath
         self.sasl_auth = sasl_auth
         self.sasl_mech = SASLMechanism(sasl_mech or SASLMechanism.NONE)
         self.logger = logger
         self.loop = loop or asyncio.get_event_loop()
 
-        if self.sasl_mech == SASLMechanism.PLAIN:
-            assert self.sasl_auth, "You must specify sasl_auth when using SASL PLAIN"
-
-        self.handlers: Dict[int, Tuple[str, Callable]] = {}
-        self.cap_handlers = defaultdict(list)
+        if self.sasl_mech == SASLMechanism.PLAIN and self.sasl_auth is None:
+            msg = "You must specify sasl_auth when using SASL PLAIN"
+            raise ValueError(msg)
+
+        self.handlers: Dict[
+            int,
+            Tuple[
+                str,
+                Callable[
+                    ["IrcProtocol", "Message"], Coroutine[None, None, None]
+                ],
+            ],
+        ] = {}
+        self.cap_handlers: Dict[
+            str,
+            List[
+                Optional[
+                    Callable[
+                        ["IrcProtocol", "Cap"], Coroutine[None, None, None]
+                    ]
+                ]
+            ],
+        ] = defaultdict(list)
 
         self._connected_future = self.loop.create_future()
         self.quit_future = self.loop.create_future()
 
         self.register("PING", _internal_ping)
         self.register("PONG", _internal_pong)
         self.register("CAP", _internal_cap_handler)
-        self.register('001', _on_001)
-        self.register_cap('sasl', _do_sasl)
-
-        self._pinger = self.loop.create_task(self.pinger())
+        self.register("001", _on_001)
+        self.register("005", _isupport_handler)
+        self.register_cap("sasl", _do_sasl)
+
+        self._pinger: Optional[Task[None]] = self.loop.create_task(
+            self.pinger()
+        )
 
     def __del__(self) -> None:
-        if not self._pinger.done():
-            self._pinger.cancel()
+        self.close()
 
     async def pinger(self) -> None:
         while True:
             if self.connected:
+                if self.server is None:
+                    msg = "Server not set in ping handler"
+                    raise ValueError(msg)
+
                 if self.server.lag > 60:
                     self.loop.create_task(self.connect())
                 else:
-                    self.send("PING :LAG{}".format(time.time()))
+                    self.send(f"PING :LAG{time.time()}")
+
             await asyncio.sleep(30)
 
-    def __call__(self, *args, **kwargs) -> 'IrcProtocol':
+    def __call__(self) -> "IrcProtocol":
         """
         This is here to allow an instance of IrcProtocol to be passed
         directly to AbstractEventLoop.create_connection()
         """
         return self
 
-    async def __aenter__(self) -> 'IrcProtocol':
+    async def __aenter__(self) -> "IrcProtocol":
         return self.__enter__()
 
-    async def __aexit__(self, *exc: Any) -> None:
-        self.quit()
-        await self.quit_future
+    async def __aexit__(self, *exc: object) -> None:
+        if self.connected:
+            self.quit()
+            await self.quit_future
+
+        self.close()
 
-    def __enter__(self) -> 'IrcProtocol':
+    def __enter__(self) -> "IrcProtocol":
         return self
 
-    def __exit__(self, *exc: Any) -> None:
-        self.quit()
+    def __exit__(self, *exc: object) -> None:
+        if self.connected:
+            self.quit()
+
+        self.close()
+
+    def close(self) -> None:
+        if (
+            self._pinger
+            and self._pinger.get_loop().is_running()
+            and not self._pinger.done()
+        ):
+            self._pinger.cancel()
+            self._pinger = None
 
     async def connect(self) -> None:
         """Attempt to connect to the server, cycling through the server list until successful"""
         delayer = AsyncDelayer(2)
         for server in cycle(self.servers):
             async with delayer:
                 if await self._connect(server):
                     break
 
-    async def _connect(self, server: 'BaseServer') -> bool:
+    async def _connect(self, server: "BaseServer") -> bool:
         self._connected_future = self.loop.create_future()
         self.quit_future = self.loop.create_future()
         self._server = ConnectedServer(server)
         if self.logger:
             if self.connected:
                 self.logger.info("Reconnecting to %s", self.server)
             else:
                 self.logger.info("Connecting to %s", self.server)
 
-        fut = self.server.connection.do_connect(self)
+        fut = self._server.connection.do_connect(self)
         try:
             await asyncio.wait_for(fut, 30)
         except asyncio.TimeoutError:
             if self.logger:
-                self.logger.error("Connection timeout occurred while connecting to %s", self.server)
+                self.logger.exception(
+                    "Connection timeout occurred while connecting to %s",
+                    self.server,
+                )
+
             return False
         except (ConnectionError, socket.gaierror) as e:
             if self.logger:
-                self.logger.error("Error occurred while connecting to %s (%s)", self.server, e)
+                self.logger.exception(
+                    "Error occurred while connecting to %s (%s)", self.server, e
+                )
+
             return False
+
         return True
 
-    def register(self, cmd: str, handler: Callable[['IrcProtocol', 'Message'], Coroutine]) -> int:
+    def register(
+        self,
+        cmd: str,
+        handler: Callable[
+            ["IrcProtocol", "Message"], Coroutine[None, None, None]
+        ],
+    ) -> int:
         """Register a command handler"""
         hook_id = 0
         while not hook_id or hook_id in self.handlers:
-            hook_id = random.randint(1, (2 ** 32) - 1)
+            hook_id = random.randint(1, (2**32) - 1)
+
         self.handlers[hook_id] = (cmd, handler)
         return hook_id
 
     def unregister(self, hook_id: int) -> None:
         """Unregister a hook"""
         del self.handlers[hook_id]
 
-    def register_cap(self, cap: str, handler: Optional[Callable[['IrcProtocol', 'Cap'], Coroutine]] = None) -> None:
+    def register_cap(
+        self,
+        cap: str,
+        handler: Optional[
+            Callable[["IrcProtocol", "Cap"], Coroutine[None, None, None]]
+        ] = None,
+    ) -> None:
         """Register a CAP handler
 
         If the handler is None, the CAP will be requested from the server, but no handler will be called,
         allowing registration of CAPs that only require basic requests
         """
         self.cap_handlers[cap].append(handler)
 
-    async def wait_for(self, *cmds: str, timeout: int = None) -> None:
-        """Wait for a specific command from the server, optionally returning after [timeout] seconds"""
+    async def wait_for(
+        self, *cmds: str, timeout: Optional[int] = None
+    ) -> Optional[Message]:
+        """Wait for a specific command from the server, optionally returning after [timeout] seconds."""
         if not cmds:
-            return
-        fut = self.loop.create_future()
+            return None
+
+        fut: "asyncio.Future[Message]" = self.loop.create_future()
 
         # noinspection PyUnusedLocal
-        async def _wait(conn: 'IrcProtocol', message: 'Message') -> None:
+        async def _wait(conn: "IrcProtocol", message: "Message") -> None:
             if not fut.done():
                 fut.set_result(message)
 
-        hooks = [
-            self.register(cmd, _wait) for cmd in cmds
-        ]
+        hooks = [self.register(cmd, _wait) for cmd in cmds]
 
         try:
             result = await asyncio.wait_for(fut, timeout)
         except asyncio.TimeoutError:
             result = None
         finally:
             for hook_id in hooks:
                 self.unregister(hook_id)
+
         return result
 
-    def send(self, text: AnyStr) -> None:
+    def send(self, text: Union[str, bytes]) -> None:
         """Send a raw line to the server"""
         asyncio.run_coroutine_threadsafe(self._send(text), self.loop)
 
     def send_command(self, msg: Message) -> None:
         """Send an irclib Message object to the server"""
         return self.send(str(msg))
 
-    async def _send(self, text: AnyStr) -> None:
+    async def _send(self, text: Union[str, bytes]) -> None:
         if not self.connected:
             await self._connected_future
+
         if isinstance(text, str):
             text = text.encode()
+        elif isinstance(text, memoryview):
+            text = text.tobytes()
+
         if self.logger:
             self.logger.info(">> %s", text.decode())
-        self._transport.write(text + b'\r\n')
 
-    def quit(self, reason: str = None) -> None:
+        if self._transport is None:
+            msg = "Can't send to missing transport"
+            raise ValueError(msg)
+
+        self._transport.write(text + b"\r\n")
+
+    def quit(self, reason: Optional[str] = None) -> None:
         """Quit the IRC connection with an optional reason"""
         if not self._quitting:
             self._quitting = True
             if reason:
-                self.send("QUIT {}".format(reason))
+                self.send(f"QUIT {reason}")
             else:
                 self.send("QUIT")
 
-    def connection_made(self, transport: 'Transport') -> None:
+    def connection_made(self, transport: "asyncio.BaseTransport") -> None:
         """Called by the event loop when the connection has been established"""
-        self._transport = transport
+        if not self.server:
+            msg = "Server not set during connection_made()"
+            raise ValueError(msg)
+
+        self._transport = cast(asyncio.Transport, transport)
         self._connected = True
         self._connected_future.set_result(None)
         del self._connected_future
         self.send("CAP LS 302")
         if self.server.password:
-            self.send("PASS {}".format(self.server.password))
-        self.send("NICK {}".format(self.nick))
-        self.send("USER {} 0 * :{}".format(self.user, self.realname))
+            self.send(f"PASS {self.server.password}")
+
+        self.send(f"NICK {self.nick}")
+        self.send(f"USER {self.user} 0 * :{self.realname}")
 
-    def connection_lost(self, exc) -> None:
+    def connection_lost(self, exc: Optional[Exception]) -> None:
         """Connection to the IRC server has been lost"""
         self._transport = None
         self._connected = False
         if not self._quitting:
             self._connected_future = self.loop.create_future()
             asyncio.run_coroutine_threadsafe(self.connect(), self.loop)
         else:
             self.quit_future.set_result(None)
 
     def data_received(self, data: bytes) -> None:
         """Called by the event loop when data has been read from the socket"""
         self._buff += data
-        while b'\r\n' in self._buff:
-            raw_line, self._buff = self._buff.split(b'\r\n', 1)
+        while b"\r\n" in self._buff:
+            raw_line, self._buff = self._buff.split(b"\r\n", 1)
             message = Message.parse(raw_line)
             for trigger, func in self.handlers.values():
-                if trigger in (message.command, '*'):
+                if trigger in (message.command, "*"):
                     self.loop.create_task(func(self, message))
 
     @property
     def user(self) -> str:
         """The username used for this connection"""
         return self._user or self.nick
 
@@ -358,10 +505,10 @@
 
     @property
     def connected(self) -> bool:
         """Whether or not the connection is still active"""
         return self._connected
 
     @property
-    def server(self) -> Optional['ConnectedServer']:
+    def server(self) -> Optional["ConnectedServer"]:
         """The current server object"""
         return self._server
```

### Comparing `async-irc-0.1.8/asyncirc/server.py` & `async_irc-0.2.0/asyncirc/server.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,71 @@
-# coding=utf-8
 """
 Server objects used for different stages in the connect process
 to store contextual data
 """
+
 import asyncio
 import ssl
-from typing import Dict, Optional, Tuple
+from typing import TYPE_CHECKING, Any, Callable, Dict, Optional, Tuple, TypeVar
 
-from irclib.parser import Cap
+if TYPE_CHECKING:
+    from irclib.parser import Cap
 
 __all__ = (
-    'BaseServer',
-    'Server',
-    'BasicIPServer',
-    'BasicUNIXServer',
-    'ConnectedServer',
-    'BadAttribute',
+    "BaseServer",
+    "Server",
+    "BasicIPServer",
+    "BasicUNIXServer",
+    "ConnectedServer",
 )
 
+_ProtoT = TypeVar("_ProtoT", bound=asyncio.Protocol)
+
 
 class BaseServer:
     def __init__(
         self,
         *,
-        password: str = None,
+        password: Optional[str] = None,
         is_ssl: bool = False,
-        ssl_ctx: ssl.SSLContext = None,
-        certpath: str = None,
+        ssl_ctx: Optional[ssl.SSLContext] = None,
+        certpath: Optional[str] = None,
     ):
         if is_ssl:
             if ssl_ctx is None:
                 ssl_ctx = ssl.create_default_context()
 
             if certpath:
                 ssl_ctx.load_cert_chain(certpath)
 
-            self.ssl_ctx = ssl_ctx
+            self.ssl_ctx: Optional[ssl.SSLContext] = ssl_ctx
         else:
             self.ssl_ctx = None
 
         self.password = password
 
     @property
-    def is_ssl(self):
+    def is_ssl(self) -> bool:
         return self.ssl_ctx is not None
 
-    async def connect(self, protocol_factory, *, loop=None, **kwargs):
+    async def connect(
+        self,
+        protocol_factory: Callable[[], _ProtoT],
+        *,
+        loop: Optional[asyncio.AbstractEventLoop] = None,
+        **kwargs: Any,
+    ) -> Tuple[asyncio.Transport, _ProtoT]:
         raise NotImplementedError
 
-    async def do_connect(self, protocol_factory, *, loop=None):
+    async def do_connect(
+        self,
+        protocol_factory: Callable[[], _ProtoT],
+        *,
+        loop: Optional[asyncio.AbstractEventLoop] = None,
+    ) -> Tuple[asyncio.Transport, _ProtoT]:
         return await self.connect(protocol_factory, loop=loop, ssl=self.ssl_ctx)
 
     def __str__(self) -> str:
         raise NotImplementedError
 
 
 class BasicIPServer(BaseServer):
@@ -60,110 +73,106 @@
 
     def __init__(
         self,
         *,
         host: str,
         port: int,
         is_ssl: bool = False,
-        password: str = None,
-        ssl_ctx: ssl.SSLContext = None,
-        certpath: str = None,
+        password: Optional[str] = None,
+        ssl_ctx: Optional[ssl.SSLContext] = None,
+        certpath: Optional[str] = None,
     ) -> None:
         super().__init__(
             password=password, is_ssl=is_ssl, ssl_ctx=ssl_ctx, certpath=certpath
         )
+
         self.host = host
         self.port = port
 
-    async def connect(self, protocol_factory, *, loop=None, **kwargs):
+    async def connect(
+        self,
+        protocol_factory: Callable[[], _ProtoT],
+        *,
+        loop: Optional[asyncio.AbstractEventLoop] = None,
+        **kwargs: Any,
+    ) -> Tuple[asyncio.Transport, _ProtoT]:
         if loop is None:
             loop = asyncio.get_event_loop()
 
         return await loop.create_connection(
             protocol_factory, self.host, self.port, **kwargs
         )
 
     def __str__(self) -> str:
         if self.is_ssl:
-            return "{}:+{}".format(self.host, self.port)
+            return f"{self.host}:+{self.port}"
 
-        return "{}:{}".format(self.host, self.port)
+        return f"{self.host}:{self.port}"
 
 
 class BasicUNIXServer(BaseServer):
     def __init__(
         self,
         *,
         path: str,
         is_ssl: bool = False,
-        password: str = None,
-        ssl_ctx: ssl.SSLContext = None,
-        certpath: str = None,
+        password: Optional[str] = None,
+        ssl_ctx: Optional[ssl.SSLContext] = None,
+        certpath: Optional[str] = None,
     ) -> None:
         super().__init__(
             is_ssl=is_ssl, password=password, ssl_ctx=ssl_ctx, certpath=certpath
         )
         self.path = path
 
-    async def connect(self, protocol_factory, *, loop=None, **kwargs):
+    async def connect(
+        self,
+        protocol_factory: Callable[[], _ProtoT],
+        *,
+        loop: Optional[asyncio.AbstractEventLoop] = None,
+        **kwargs: Any,
+    ) -> Tuple[asyncio.Transport, _ProtoT]:
         if loop is None:
             loop = asyncio.get_event_loop()
 
-        return await loop.create_unix_connection(protocol_factory, self.path, **kwargs)
+        return await loop.create_unix_connection(
+            protocol_factory, self.path, **kwargs
+        )
 
     def __str__(self) -> str:
         if self.is_ssl:
-            return "{} (ssl)".format(self.path)
+            return f"{self.path} (ssl)"
 
         return self.path
 
 
 class Server(BasicIPServer):
     """Represents a server to connect to"""
 
     def __init__(
-        self, host: str, port: int, is_ssl: bool = False, password: str = None
-    ):
+        self,
+        host: str,
+        port: int,
+        is_ssl: bool = False,
+        password: Optional[str] = None,
+    ) -> None:
         super().__init__(host=host, port=port, is_ssl=is_ssl, password=password)
 
 
-class BadAttribute(AttributeError):
-    def __init__(self, obj, attr):
-        super().__init__(
-            "Incorrect base connection type ({} has no attribute {!r})".format(
-                type(obj).__name__, attr
-            )
-        )
-
-
 class ConnectedServer:
     """Represents a connected server
 
     Used to store session data like ISUPPORT tokens and enabled CAPs
     """
 
-    last_ping_sent = -1
-    last_ping_recv = -1
-    lag = -1
+    last_ping_sent: float = -1
+    last_ping_recv: float = -1
+    lag: float = -1
 
-    def __init__(self, server: 'BaseServer') -> None:
+    def __init__(self, server: "BaseServer") -> None:
         self.connection = server
         self.is_ssl = server.is_ssl
         self.password = server.password
-        self.isupport_tokens: Dict[str, str] = {}
+        self.isupport_tokens: Dict[str, Optional[str]] = {}
         self.caps: Dict[str, Tuple[Cap, Optional[bool]]] = {}
-        self.server_name = None
-        self.data = {}
-
-    @property
-    def host(self):
-        try:
-            return self.connection.host
-        except AttributeError as e:
-            raise BadAttribute(self.connection, e.args[0])
-
-    @property
-    def port(self):
-        try:
-            return self.connection.port
-        except AttributeError as e:
-            raise BadAttribute(self.connection, e.args[0])
+        self.server_name: Optional[str] = None
+        self.data: Dict[str, Any] = {}
```

### Comparing `async-irc-0.1.8/asyncirc/util/backoff.py` & `async_irc-0.2.0/asyncirc/util/backoff.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-# coding=utf-8
 """
 Provides a Delayer object for delaying repeated calls e.g. server connections
 """
 
 import asyncio
 import random
-from typing import Any, Callable
+from typing import Callable
 
-__all__ = ('AsyncDelayer',)
+__all__ = ("AsyncDelayer",)
 
 
 class AsyncDelayer:
     """Implementation of the exponential back-off algorithm for handling server reconnects
 
     Implemented as a re-entrant async context manager so it can be used like so:
     >>> import asyncio
@@ -31,18 +30,21 @@
         self._integral = integral
         self._max = 10
         self._exp = 0
         self._rand = random.Random()
         self._rand.seed()
 
     @property
-    def randfunc(self) -> Callable:
-        return self._rand.randrange if self._integral else self._rand.uniform
+    def randfunc(self) -> Callable[[int, int], float]:
+        if self._integral:
+            return self._rand.randrange
 
-    async def __aenter__(self) -> 'AsyncDelayer':
+        return self._rand.uniform
+
+    async def __aenter__(self) -> "AsyncDelayer":
         self._exp = min(self._exp + 1, self._max)
-        wait = self.randfunc(0, self._base * (2 ** self._exp))
+        wait = self.randfunc(0, self._base * (2**self._exp))
         await asyncio.sleep(wait)
         return self
 
-    async def __aexit__(self, *exc: Any) -> bool:
+    async def __aexit__(self, *exc: object) -> None:
         pass
```

