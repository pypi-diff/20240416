# Comparing `tmp/KUtil-jakubaugustyn-0.0.3.tar.gz` & `tmp/kutil_jakubaugustyn-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KUtil-jakubaugustyn-0.0.3.tar", last modified: Wed Feb 28 16:14:28 2024, max compression
+gzip compressed data, was "kutil_jakubaugustyn-0.0.4.tar", last modified: Tue Apr 16 10:10:39 2024, max compression
```

## Comparing `KUtil-jakubaugustyn-0.0.3.tar` & `kutil_jakubaugustyn-0.0.4.tar`

### file list

```diff
@@ -1,107 +1,120 @@
-drwxrwxrwx   0        0        0        0 2024-02-28 16:14:28.715159 KUtil-jakubaugustyn-0.0.3/
--rw-rw-rw-   0        0        0     1093 2023-12-08 14:54:39.000000 KUtil-jakubaugustyn-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1448 2024-02-28 16:14:28.713026 KUtil-jakubaugustyn-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      884 2024-02-28 16:11:38.000000 KUtil-jakubaugustyn-0.0.3/README.md
--rw-rw-rw-   0        0        0      824 2024-02-28 16:09:14.000000 KUtil-jakubaugustyn-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-28 16:14:28.716246 KUtil-jakubaugustyn-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-28 16:14:28.440999 KUtil-jakubaugustyn-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-02-28 16:14:28.710915 KUtil-jakubaugustyn-0.0.3/src/KUtil_jakubaugustyn.egg-info/
--rw-rw-rw-   0        0        0     1448 2024-02-28 16:14:28.000000 KUtil-jakubaugustyn-0.0.3/src/KUtil_jakubaugustyn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3264 2024-02-28 16:14:28.000000 KUtil-jakubaugustyn-0.0.3/src/KUtil_jakubaugustyn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-28 16:14:28.000000 KUtil-jakubaugustyn-0.0.3/src/KUtil_jakubaugustyn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-02-28 16:14:28.000000 KUtil-jakubaugustyn-0.0.3/src/KUtil_jakubaugustyn.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-02-28 16:14:28.473672 KUtil-jakubaugustyn-0.0.3/src/kutil/
--rw-rw-rw-   0        0        0      297 2023-12-26 14:15:09.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-28 16:14:28.488636 KUtil-jakubaugustyn-0.0.3/src/kutil/buffer/
--rw-rw-rw-   0        0        0     2401 2023-12-18 18:55:31.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/buffer/BidirectionalByteArray.py
--rw-rw-rw-   0        0        0     3359 2024-01-13 17:44:38.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/buffer/ByteBuffer.py
--rw-rw-rw-   0        0        0     4775 2024-01-13 15:02:52.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/buffer/DataBuffer.py
--rw-rw-rw-   0        0        0      375 2024-01-07 13:46:13.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/buffer/Serializable.py
--rw-rw-rw-   0        0        0     1268 2023-12-18 18:20:16.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/buffer/TextOutput.py
--rw-rw-rw-   0        0        0      287 2023-12-18 17:47:50.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/buffer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-28 16:14:28.495102 KUtil-jakubaugustyn-0.0.3/src/kutil/io/
--rw-rw-rw-   0        0        0      204 2024-01-30 17:04:48.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/io/__init__.py
--rw-rw-rw-   0        0        0     2983 2023-12-26 14:36:42.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/io/directory.py
--rw-rw-rw-   0        0        0     3060 2024-02-21 16:34:28.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/io/file.py
-drwxrwxrwx   0        0        0        0 2024-02-28 16:14:28.525847 KUtil-jakubaugustyn-0.0.3/src/kutil/language/
--rw-rw-rw-   0        0        0     4555 2024-02-10 16:30:18.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/language/AST.py
--rw-rw-rw-   0        0        0     5769 2024-01-13 18:03:43.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/language/BytecodeFile.py
--rw-rw-rw-   0        0        0     1608 2024-01-16 14:45:31.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/language/Compiler.py
--rw-rw-rw-   0        0        0      704 2024-01-13 11:58:11.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/language/Error.py
--rw-rw-rw-   0        0        0     1601 2024-01-16 14:49:22.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/language/Interpreter.py
--rw-rw-rw-   0        0        0     4116 2024-01-16 14:49:42.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/language/Language.py
--rw-rw-rw-   0        0        0     1441 2024-01-16 15:20:00.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/language/Lexer.py
--rw-rw-rw-   0        0        0     1797 2024-01-16 14:41:55.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/language/Options.py
--rw-rw-rw-   0        0        0     1101 2024-01-16 17:36:44.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/language/Parser.py
--rw-rw-rw-   0        0        0      625 2024-01-13 18:35:04.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/language/Stack.py
--rw-rw-rw-   0        0        0     2020 2024-01-03 18:39:33.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/language/Token.py
--rw-rw-rw-   0        0        0      389 2024-01-14 18:53:04.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/language/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-28 16:14:28.533503 KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/
--rw-rw-rw-   0        0        0     8372 2024-01-16 14:54:52.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/BrainFuck.py
--rw-rw-rw-   0        0        0      274 2024-01-14 19:45:36.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-28 16:14:28.571846 KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/javascript/
--rw-rw-rw-   0        0        0    40883 2024-02-10 17:14:05.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/javascript/JSLexer.py
--rw-rw-rw-   0        0        0     1565 2024-01-22 17:04:30.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/javascript/JSOptions.py
--rw-rw-rw-   0        0        0   142027 2024-02-11 14:35:27.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/javascript/JSParser.py
--rw-rw-rw-   0        0        0     1210 2024-01-22 17:24:55.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/javascript/Javascript.py
--rw-rw-rw-   0        0        0     1669 2024-01-21 06:51:49.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/javascript/__init__.py
--rw-rw-rw-   0        0        0     5070 2024-01-25 20:00:28.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/javascript/character.py
--rw-rw-rw-   0        0        0     3458 2024-01-16 14:12:04.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/javascript/error_handler.py
--rw-rw-rw-   0        0        0     5801 2024-01-16 15:26:49.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/javascript/messages.py
--rw-rw-rw-   0        0        0    42770 2024-02-21 12:59:35.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/javascript/nodes.py
--rw-rw-rw-   0        0        0     5251 2024-01-21 17:55:38.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/javascript/syntax.py
-drwxrwxrwx   0        0        0        0 2024-02-28 16:14:28.596860 KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/paint_tryhard/
--rw-rw-rw-   0        0        0     1074 2024-01-13 19:36:22.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/paint_tryhard/Canvas.py
--rw-rw-rw-   0        0        0     6901 2024-01-13 20:32:00.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/paint_tryhard/Employee.py
--rw-rw-rw-   0        0        0    11803 2024-01-16 14:57:34.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/paint_tryhard/PTCompiler.py
--rw-rw-rw-   0        0        0     3559 2024-01-14 19:32:22.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/paint_tryhard/PTInterpreter.py
--rw-rw-rw-   0        0        0     6072 2024-01-16 14:57:34.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/paint_tryhard/PTLexer.py
--rw-rw-rw-   0        0        0     6736 2024-01-16 14:57:34.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/paint_tryhard/PTParser.py
--rw-rw-rw-   0        0        0      636 2024-01-13 14:35:10.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/paint_tryhard/PaintTryhard.py
--rw-rw-rw-   0        0        0       65 2024-01-03 15:59:55.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/paint_tryhard/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-28 16:14:28.608941 KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/paint_tryhard/jobs/
--rw-rw-rw-   0        0        0     1628 2024-01-13 18:57:59.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/paint_tryhard/jobs/__init__.py
--rw-rw-rw-   0        0        0     2954 2024-01-13 20:30:06.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/paint_tryhard/jobs/boss.py
--rw-rw-rw-   0        0        0     2265 2024-01-13 20:30:06.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/paint_tryhard/jobs/mathematician.py
--rw-rw-rw-   0        0        0     4943 2024-01-13 20:30:06.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/paint_tryhard/jobs/painter.py
-drwxrwxrwx   0        0        0        0 2024-02-28 16:14:28.636529 KUtil-jakubaugustyn-0.0.3/src/kutil/protocol/
--rw-rw-rw-   0        0        0     1333 2024-01-07 13:47:51.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/protocol/AbstractProtocol.py
-drwxrwxrwx   0        0        0        0 2024-02-28 16:14:28.650671 KUtil-jakubaugustyn-0.0.3/src/kutil/protocol/HTTP/
--rw-rw-rw-   0        0        0     1128 2023-12-08 17:27:22.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/protocol/HTTP/HTTPHeaders.py
--rw-rw-rw-   0        0        0      310 2024-01-13 09:57:02.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/protocol/HTTP/HTTPMethod.py
--rw-rw-rw-   0        0        0     2949 2023-12-24 16:52:11.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/protocol/HTTP/HTTPRequest.py
--rw-rw-rw-   0        0        0     1806 2023-12-09 15:40:16.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/protocol/HTTP/HTTPResponse.py
--rw-rw-rw-   0        0        0      306 2023-12-09 14:59:15.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/protocol/HTTP/__init__.py
--rw-rw-rw-   0        0        0     1300 2023-12-08 17:24:06.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/protocol/HTTPConnection.py
--rw-rw-rw-   0        0        0     4964 2023-12-26 07:09:52.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/protocol/HTTPServer.py
--rw-rw-rw-   0        0        0     4323 2023-12-23 13:24:37.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/protocol/ProtocolConnection.py
--rw-rw-rw-   0        0        0     1934 2023-12-09 15:35:55.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/protocol/ProtocolServer.py
--rw-rw-rw-   0        0        0      943 2023-12-08 16:22:42.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/protocol/TCPConnection.py
--rw-rw-rw-   0        0        0      895 2023-12-25 18:55:01.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/protocol/URLSearchParams.py
-drwxrwxrwx   0        0        0        0 2024-02-28 16:14:28.658294 KUtil-jakubaugustyn-0.0.3/src/kutil/protocol/WS/
--rw-rw-rw-   0        0        0     4311 2024-01-13 09:57:02.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/protocol/WS/WSMessage.py
--rw-rw-rw-   0        0        0      136 2023-12-09 16:55:52.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/protocol/WS/__init__.py
--rw-rw-rw-   0        0        0     2544 2023-12-09 17:30:00.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/protocol/WSConnection.py
--rw-rw-rw-   0        0        0      493 2023-12-09 15:28:24.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/protocol/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-28 16:14:28.666444 KUtil-jakubaugustyn-0.0.3/src/kutil/storage/
--rw-rw-rw-   0        0        0       97 2023-12-31 13:49:32.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/storage/Cache.py
--rw-rw-rw-   0        0        0     6589 2023-12-31 13:43:35.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/storage/Config.py
--rw-rw-rw-   0        0        0       65 2023-12-26 11:19:38.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/storage/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-28 16:14:28.686410 KUtil-jakubaugustyn-0.0.3/src/kutil/storage/bon/
--rw-rw-rw-   0        0        0      250 2024-01-10 15:41:05.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/storage/bon/__init__.py
--rw-rw-rw-   0        0        0     2151 2024-02-21 16:56:37.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/storage/bon/bon.py
--rw-rw-rw-   0        0        0     2109 2024-01-10 17:02:50.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/storage/bon/converter.py
--rw-rw-rw-   0        0        0     5779 2024-02-21 16:53:13.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/storage/bon/decoder.py
--rw-rw-rw-   0        0        0     6588 2024-02-21 17:02:44.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/storage/bon/encoder.py
--rw-rw-rw-   0        0        0      761 2024-02-21 16:43:29.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/storage/bon/shared.py
-drwxrwxrwx   0        0        0        0 2024-02-28 16:14:28.693071 KUtil-jakubaugustyn-0.0.3/src/kutil/threads/
--rw-rw-rw-   0        0        0     1721 2023-12-26 07:13:22.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/threads/ThreadWaiter.py
--rw-rw-rw-   0        0        0      120 2023-12-20 15:36:57.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/threads/__init__.py
--rw-rw-rw-   0        0        0    15388 2024-02-21 16:32:56.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/typing.py
-drwxrwxrwx   0        0        0        0 2024-02-28 16:14:28.702121 KUtil-jakubaugustyn-0.0.3/src/kutil/webscraper/
--rw-rw-rw-   0        0        0    18856 2024-01-13 09:57:02.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/webscraper/MapyCZServer.py
--rw-rw-rw-   0        0        0     2397 2024-01-07 13:47:51.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/webscraper/WebScraperServer.py
--rw-rw-rw-   0        0        0      187 2023-12-23 13:37:41.000000 KUtil-jakubaugustyn-0.0.3/src/kutil/webscraper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-28 16:14:28.707767 KUtil-jakubaugustyn-0.0.3/tests/
--rw-rw-rw-   0        0        0     1400 2024-02-21 17:02:14.000000 KUtil-jakubaugustyn-0.0.3/tests/test_bon.py
--rw-rw-rw-   0        0        0     2174 2024-01-21 08:11:04.000000 KUtil-jakubaugustyn-0.0.3/tests/test_js.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:10:39.276426 kutil_jakubaugustyn-0.0.4/
+-rw-rw-rw-   0        0        0     1093 2023-12-08 14:54:39.000000 kutil_jakubaugustyn-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1374 2024-04-16 10:10:39.276426 kutil_jakubaugustyn-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      810 2024-02-28 16:16:37.000000 kutil_jakubaugustyn-0.0.4/README.md
+-rw-rw-rw-   0        0        0      824 2024-04-16 10:10:01.000000 kutil_jakubaugustyn-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-16 10:10:39.276426 kutil_jakubaugustyn-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-16 10:10:38.229646 kutil_jakubaugustyn-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-16 10:10:39.276426 kutil_jakubaugustyn-0.0.4/src/KUtil_jakubaugustyn.egg-info/
+-rw-rw-rw-   0        0        0     1374 2024-04-16 10:10:37.000000 kutil_jakubaugustyn-0.0.4/src/KUtil_jakubaugustyn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3719 2024-04-16 10:10:38.000000 kutil_jakubaugustyn-0.0.4/src/KUtil_jakubaugustyn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 10:10:37.000000 kutil_jakubaugustyn-0.0.4/src/KUtil_jakubaugustyn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-16 10:10:37.000000 kutil_jakubaugustyn-0.0.4/src/KUtil_jakubaugustyn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 10:10:38.276499 kutil_jakubaugustyn-0.0.4/src/kutil/
+-rw-rw-rw-   0        0        0      302 2024-02-28 19:22:19.000000 kutil_jakubaugustyn-0.0.4/src/kutil/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:10:38.307756 kutil_jakubaugustyn-0.0.4/src/kutil/buffer/
+-rw-rw-rw-   0        0        0     2401 2023-12-18 18:55:31.000000 kutil_jakubaugustyn-0.0.4/src/kutil/buffer/BidirectionalByteArray.py
+-rw-rw-rw-   0        0        0     4303 2024-03-25 17:59:57.000000 kutil_jakubaugustyn-0.0.4/src/kutil/buffer/ByteBuffer.py
+-rw-rw-rw-   0        0        0     5333 2024-03-02 12:29:40.000000 kutil_jakubaugustyn-0.0.4/src/kutil/buffer/DataBuffer.py
+-rw-rw-rw-   0        0        0      375 2024-01-07 13:46:13.000000 kutil_jakubaugustyn-0.0.4/src/kutil/buffer/Serializable.py
+-rw-rw-rw-   0        0        0     1268 2023-12-18 18:20:16.000000 kutil_jakubaugustyn-0.0.4/src/kutil/buffer/TextOutput.py
+-rw-rw-rw-   0        0        0      335 2024-03-02 12:31:14.000000 kutil_jakubaugustyn-0.0.4/src/kutil/buffer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:10:38.323386 kutil_jakubaugustyn-0.0.4/src/kutil/io/
+-rw-rw-rw-   0        0        0      262 2024-04-16 09:37:01.000000 kutil_jakubaugustyn-0.0.4/src/kutil/io/__init__.py
+-rw-rw-rw-   0        0        0     2983 2023-12-26 14:36:42.000000 kutil_jakubaugustyn-0.0.4/src/kutil/io/directory.py
+-rw-rw-rw-   0        0        0     3568 2024-04-16 09:35:52.000000 kutil_jakubaugustyn-0.0.4/src/kutil/io/file.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:10:38.401505 kutil_jakubaugustyn-0.0.4/src/kutil/language/
+-rw-rw-rw-   0        0        0     4560 2024-02-28 19:21:38.000000 kutil_jakubaugustyn-0.0.4/src/kutil/language/AST.py
+-rw-rw-rw-   0        0        0     5769 2024-01-13 18:03:43.000000 kutil_jakubaugustyn-0.0.4/src/kutil/language/BytecodeFile.py
+-rw-rw-rw-   0        0        0     1608 2024-01-16 14:45:31.000000 kutil_jakubaugustyn-0.0.4/src/kutil/language/Compiler.py
+-rw-rw-rw-   0        0        0      704 2024-01-13 11:58:11.000000 kutil_jakubaugustyn-0.0.4/src/kutil/language/Error.py
+-rw-rw-rw-   0        0        0     1601 2024-01-16 14:49:22.000000 kutil_jakubaugustyn-0.0.4/src/kutil/language/Interpreter.py
+-rw-rw-rw-   0        0        0     4116 2024-01-16 14:49:42.000000 kutil_jakubaugustyn-0.0.4/src/kutil/language/Language.py
+-rw-rw-rw-   0        0        0     1441 2024-01-16 15:20:00.000000 kutil_jakubaugustyn-0.0.4/src/kutil/language/Lexer.py
+-rw-rw-rw-   0        0        0     1797 2024-01-16 14:41:55.000000 kutil_jakubaugustyn-0.0.4/src/kutil/language/Options.py
+-rw-rw-rw-   0        0        0     1101 2024-01-16 17:36:44.000000 kutil_jakubaugustyn-0.0.4/src/kutil/language/Parser.py
+-rw-rw-rw-   0        0        0      625 2024-01-13 18:35:04.000000 kutil_jakubaugustyn-0.0.4/src/kutil/language/Stack.py
+-rw-rw-rw-   0        0        0     2020 2024-01-03 18:39:33.000000 kutil_jakubaugustyn-0.0.4/src/kutil/language/Token.py
+-rw-rw-rw-   0        0        0      389 2024-01-14 18:53:04.000000 kutil_jakubaugustyn-0.0.4/src/kutil/language/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:10:38.417128 kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/
+-rw-rw-rw-   0        0        0     8372 2024-01-16 14:54:52.000000 kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/BrainFuck.py
+-rw-rw-rw-   0        0        0      274 2024-01-14 19:45:36.000000 kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:10:38.479620 kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/javascript/
+-rw-rw-rw-   0        0        0    40883 2024-02-10 17:14:05.000000 kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/javascript/JSLexer.py
+-rw-rw-rw-   0        0        0     1565 2024-01-22 17:04:30.000000 kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/javascript/JSOptions.py
+-rw-rw-rw-   0        0        0   142027 2024-02-11 14:35:27.000000 kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/javascript/JSParser.py
+-rw-rw-rw-   0        0        0     1210 2024-01-22 17:24:55.000000 kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/javascript/Javascript.py
+-rw-rw-rw-   0        0        0     1669 2024-01-21 06:51:49.000000 kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/javascript/__init__.py
+-rw-rw-rw-   0        0        0     5070 2024-01-25 20:00:28.000000 kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/javascript/character.py
+-rw-rw-rw-   0        0        0     3458 2024-01-16 14:12:04.000000 kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/javascript/error_handler.py
+-rw-rw-rw-   0        0        0     5801 2024-01-16 15:26:49.000000 kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/javascript/messages.py
+-rw-rw-rw-   0        0        0    42770 2024-02-21 12:59:35.000000 kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/javascript/nodes.py
+-rw-rw-rw-   0        0        0     5251 2024-01-21 17:55:38.000000 kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/javascript/syntax.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:10:38.526480 kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/paint_tryhard/
+-rw-rw-rw-   0        0        0     1074 2024-01-13 19:36:22.000000 kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/paint_tryhard/Canvas.py
+-rw-rw-rw-   0        0        0     6901 2024-01-13 20:32:00.000000 kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/paint_tryhard/Employee.py
+-rw-rw-rw-   0        0        0    11803 2024-01-16 14:57:34.000000 kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/paint_tryhard/PTCompiler.py
+-rw-rw-rw-   0        0        0     3559 2024-01-14 19:32:22.000000 kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/paint_tryhard/PTInterpreter.py
+-rw-rw-rw-   0        0        0     6072 2024-01-16 14:57:34.000000 kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/paint_tryhard/PTLexer.py
+-rw-rw-rw-   0        0        0     6736 2024-01-16 14:57:34.000000 kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/paint_tryhard/PTParser.py
+-rw-rw-rw-   0        0        0      636 2024-01-13 14:35:10.000000 kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/paint_tryhard/PaintTryhard.py
+-rw-rw-rw-   0        0        0       65 2024-01-03 15:59:55.000000 kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/paint_tryhard/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:10:38.542105 kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/paint_tryhard/jobs/
+-rw-rw-rw-   0        0        0     1628 2024-01-13 18:57:59.000000 kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/paint_tryhard/jobs/__init__.py
+-rw-rw-rw-   0        0        0     2954 2024-01-13 20:30:06.000000 kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/paint_tryhard/jobs/boss.py
+-rw-rw-rw-   0        0        0     2265 2024-01-13 20:30:06.000000 kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/paint_tryhard/jobs/mathematician.py
+-rw-rw-rw-   0        0        0     4943 2024-01-13 20:30:06.000000 kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/paint_tryhard/jobs/painter.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:10:38.588979 kutil_jakubaugustyn-0.0.4/src/kutil/protocol/
+-rw-rw-rw-   0        0        0     1378 2024-03-02 14:21:02.000000 kutil_jakubaugustyn-0.0.4/src/kutil/protocol/AbstractProtocol.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:10:38.713971 kutil_jakubaugustyn-0.0.4/src/kutil/protocol/HTTP/
+-rw-rw-rw-   0        0        0     1216 2024-03-02 10:37:15.000000 kutil_jakubaugustyn-0.0.4/src/kutil/protocol/HTTP/HTTPHeaders.py
+-rw-rw-rw-   0        0        0      310 2024-01-13 09:57:02.000000 kutil_jakubaugustyn-0.0.4/src/kutil/protocol/HTTP/HTTPMethod.py
+-rw-rw-rw-   0        0        0     3822 2024-03-02 10:54:44.000000 kutil_jakubaugustyn-0.0.4/src/kutil/protocol/HTTP/HTTPRequest.py
+-rw-rw-rw-   0        0        0     1806 2023-12-09 15:40:16.000000 kutil_jakubaugustyn-0.0.4/src/kutil/protocol/HTTP/HTTPResponse.py
+-rw-rw-rw-   0        0        0      306 2023-12-09 14:59:15.000000 kutil_jakubaugustyn-0.0.4/src/kutil/protocol/HTTP/__init__.py
+-rw-rw-rw-   0        0        0     1261 2024-03-02 13:51:31.000000 kutil_jakubaugustyn-0.0.4/src/kutil/protocol/HTTPConnection.py
+-rw-rw-rw-   0        0        0    12459 2024-03-31 19:30:22.000000 kutil_jakubaugustyn-0.0.4/src/kutil/protocol/HTTPSConnection.py
+-rw-rw-rw-   0        0        0     5991 2024-04-15 18:47:36.000000 kutil_jakubaugustyn-0.0.4/src/kutil/protocol/HTTPServer.py
+-rw-rw-rw-   0        0        0     7923 2024-03-28 17:23:06.000000 kutil_jakubaugustyn-0.0.4/src/kutil/protocol/ProtocolConnection.py
+-rw-rw-rw-   0        0        0     2589 2024-04-15 18:47:36.000000 kutil_jakubaugustyn-0.0.4/src/kutil/protocol/ProtocolServer.py
+-rw-rw-rw-   0        0        0      944 2024-03-02 10:48:15.000000 kutil_jakubaugustyn-0.0.4/src/kutil/protocol/TCPConnection.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:10:38.901457 kutil_jakubaugustyn-0.0.4/src/kutil/protocol/TLS/
+-rw-rw-rw-   0        0        0     2388 2024-03-28 17:36:36.000000 kutil_jakubaugustyn-0.0.4/src/kutil/protocol/TLS/AlertCause.py
+-rw-rw-rw-   0        0        0     4694 2024-03-29 11:04:02.000000 kutil_jakubaugustyn-0.0.4/src/kutil/protocol/TLS/CipherSuite.py
+-rw-rw-rw-   0        0        0     5969 2024-03-29 12:13:33.000000 kutil_jakubaugustyn-0.0.4/src/kutil/protocol/TLS/ConnectionState.py
+-rw-rw-rw-   0        0        0     4200 2024-03-28 16:44:17.000000 kutil_jakubaugustyn-0.0.4/src/kutil/protocol/TLS/RawTLSRecord.py
+-rw-rw-rw-   0        0        0       65 2024-03-02 10:25:01.000000 kutil_jakubaugustyn-0.0.4/src/kutil/protocol/TLS/__init__.py
+-rw-rw-rw-   0        0        0     1851 2024-03-29 08:57:18.000000 kutil_jakubaugustyn-0.0.4/src/kutil/protocol/TLS/certificate_verifier.py
+-rw-rw-rw-   0        0        0     6240 2024-03-28 06:30:56.000000 kutil_jakubaugustyn-0.0.4/src/kutil/protocol/TLS/extensions.py
+-rw-rw-rw-   0        0        0    12644 2024-03-29 11:00:58.000000 kutil_jakubaugustyn-0.0.4/src/kutil/protocol/TLS/messages.py
+-rw-rw-rw-   0        0        0     5135 2024-03-28 05:52:47.000000 kutil_jakubaugustyn-0.0.4/src/kutil/protocol/TLS/records.py
+-rw-rw-rw-   0        0        0    13034 2024-03-28 11:30:36.000000 kutil_jakubaugustyn-0.0.4/src/kutil/protocol/TLS/tls_cryptography.py
+-rw-rw-rw-   0        0        0      918 2024-04-15 18:08:31.000000 kutil_jakubaugustyn-0.0.4/src/kutil/protocol/URLSearchParams.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:10:38.963953 kutil_jakubaugustyn-0.0.4/src/kutil/protocol/WS/
+-rw-rw-rw-   0        0        0     4311 2024-01-13 09:57:02.000000 kutil_jakubaugustyn-0.0.4/src/kutil/protocol/WS/WSMessage.py
+-rw-rw-rw-   0        0        0      136 2023-12-09 16:55:52.000000 kutil_jakubaugustyn-0.0.4/src/kutil/protocol/WS/__init__.py
+-rw-rw-rw-   0        0        0     2753 2024-03-02 14:32:31.000000 kutil_jakubaugustyn-0.0.4/src/kutil/protocol/WSConnection.py
+-rw-rw-rw-   0        0        0      628 2024-03-02 10:33:58.000000 kutil_jakubaugustyn-0.0.4/src/kutil/protocol/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:10:39.010820 kutil_jakubaugustyn-0.0.4/src/kutil/storage/
+-rw-rw-rw-   0        0        0       97 2023-12-31 13:49:32.000000 kutil_jakubaugustyn-0.0.4/src/kutil/storage/Cache.py
+-rw-rw-rw-   0        0        0     6611 2024-03-01 16:41:47.000000 kutil_jakubaugustyn-0.0.4/src/kutil/storage/Config.py
+-rw-rw-rw-   0        0        0       65 2023-12-26 11:19:38.000000 kutil_jakubaugustyn-0.0.4/src/kutil/storage/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:10:39.088940 kutil_jakubaugustyn-0.0.4/src/kutil/storage/bon/
+-rw-rw-rw-   0        0        0      250 2024-01-10 15:41:05.000000 kutil_jakubaugustyn-0.0.4/src/kutil/storage/bon/__init__.py
+-rw-rw-rw-   0        0        0     2151 2024-02-21 16:56:37.000000 kutil_jakubaugustyn-0.0.4/src/kutil/storage/bon/bon.py
+-rw-rw-rw-   0        0        0     2109 2024-01-10 17:02:50.000000 kutil_jakubaugustyn-0.0.4/src/kutil/storage/bon/converter.py
+-rw-rw-rw-   0        0        0     5779 2024-02-21 16:53:13.000000 kutil_jakubaugustyn-0.0.4/src/kutil/storage/bon/decoder.py
+-rw-rw-rw-   0        0        0     6588 2024-02-21 17:02:44.000000 kutil_jakubaugustyn-0.0.4/src/kutil/storage/bon/encoder.py
+-rw-rw-rw-   0        0        0      761 2024-02-21 16:43:29.000000 kutil_jakubaugustyn-0.0.4/src/kutil/storage/bon/shared.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:10:39.151437 kutil_jakubaugustyn-0.0.4/src/kutil/threads/
+-rw-rw-rw-   0        0        0     1721 2023-12-26 07:13:22.000000 kutil_jakubaugustyn-0.0.4/src/kutil/threads/ThreadWaiter.py
+-rw-rw-rw-   0        0        0      120 2023-12-20 15:36:57.000000 kutil_jakubaugustyn-0.0.4/src/kutil/threads/__init__.py
+-rw-rw-rw-   0        0        0    15510 2024-03-02 11:13:45.000000 kutil_jakubaugustyn-0.0.4/src/kutil/typing_help.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:10:39.213937 kutil_jakubaugustyn-0.0.4/src/kutil/webscraper/
+-rw-rw-rw-   0        0        0    24555 2024-04-16 09:56:15.000000 kutil_jakubaugustyn-0.0.4/src/kutil/webscraper/MapyCZServer.py
+-rw-rw-rw-   0        0        0     3167 2024-04-16 08:53:51.000000 kutil_jakubaugustyn-0.0.4/src/kutil/webscraper/WebScraperServer.py
+-rw-rw-rw-   0        0        0      187 2023-12-23 13:37:41.000000 kutil_jakubaugustyn-0.0.4/src/kutil/webscraper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:10:39.229560 kutil_jakubaugustyn-0.0.4/tests/
+-rw-rw-rw-   0        0        0     1400 2024-02-21 17:02:14.000000 kutil_jakubaugustyn-0.0.4/tests/test_bon.py
+-rw-rw-rw-   0        0        0      756 2024-03-02 10:48:38.000000 kutil_jakubaugustyn-0.0.4/tests/test_bytebuffer.py
+-rw-rw-rw-   0        0        0     2174 2024-01-21 08:11:04.000000 kutil_jakubaugustyn-0.0.4/tests/test_js.py
```

### Comparing `KUtil-jakubaugustyn-0.0.3/LICENSE` & `kutil_jakubaugustyn-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/PKG-INFO` & `kutil_jakubaugustyn-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KUtil-jakubaugustyn
-Version: 0.0.3
+Version: 0.0.4
 Summary: Kuba's Python Utilities
 Author-email: Jakub Augustýn <kubik.augustyn@post.cz>, Radek Augustýn <raugustyn@post.cz>
 Project-URL: Homepage, https://github.com/kubikaugustyn/KUtil
 Project-URL: Issues, https://github.com/kubikaugustyn/KUtil/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,16 +15,15 @@
 # KUtil
 
 Kuba's Python Utilities (kutil is intentional - a Czech word).
 Made for Python 3.12 and newer
 
 # Installation from PyPI
 
-Sadly, the name *kutil* is already used, see [#3](https://github.com/kubikaugustyn/KUtil/issues/3) for more info, but
-I sneaked it to PyPI with a different name: `KUtil-jakubaugustyn`
+Sadly, the name `kutil` is already used, but I sneaked it to PyPI with a different name: `KUtil-jakubaugustyn`
 
 ```cmd
 pip3 install KUtil-jakubaugustyn
 ```
 
 # Installation
```

### Comparing `KUtil-jakubaugustyn-0.0.3/README.md` & `kutil_jakubaugustyn-0.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # KUtil
 
 Kuba's Python Utilities (kutil is intentional - a Czech word).
 Made for Python 3.12 and newer
 
 # Installation from PyPI
 
-Sadly, the name *kutil* is already used, see [#3](https://github.com/kubikaugustyn/KUtil/issues/3) for more info, but
-I sneaked it to PyPI with a different name: `KUtil-jakubaugustyn`
+Sadly, the name `kutil` is already used, but I sneaked it to PyPI with a different name: `KUtil-jakubaugustyn`
 
 ```cmd
 pip3 install KUtil-jakubaugustyn
 ```
 
 # Installation
```

### Comparing `KUtil-jakubaugustyn-0.0.3/pyproject.toml` & `kutil_jakubaugustyn-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copied that from https://github.com/Kronuz/esprima-python/blob/master/pyproject.toml
 requires = ["setuptools>=61.0", "wheel", "setuptools_scm[toml]>=8.0"]
 build-backend = "setuptools.build_meta"
 [tool.setuptools_scm]
 
 [project]
 name = "KUtil-jakubaugustyn"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name = "Jakub Augustýn", email = "kubik.augustyn@post.cz" },
     { name = "Radek Augustýn", email = "raugustyn@post.cz" },
 ]
 description = "Kuba's Python Utilities"
 readme = "README.md"
 requires-python = ">=3.12"
```

### Comparing `KUtil-jakubaugustyn-0.0.3/src/KUtil_jakubaugustyn.egg-info/PKG-INFO` & `kutil_jakubaugustyn-0.0.4/src/KUtil_jakubaugustyn.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KUtil-jakubaugustyn
-Version: 0.0.3
+Version: 0.0.4
 Summary: Kuba's Python Utilities
 Author-email: Jakub Augustýn <kubik.augustyn@post.cz>, Radek Augustýn <raugustyn@post.cz>
 Project-URL: Homepage, https://github.com/kubikaugustyn/KUtil
 Project-URL: Issues, https://github.com/kubikaugustyn/KUtil/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,16 +15,15 @@
 # KUtil
 
 Kuba's Python Utilities (kutil is intentional - a Czech word).
 Made for Python 3.12 and newer
 
 # Installation from PyPI
 
-Sadly, the name *kutil* is already used, see [#3](https://github.com/kubikaugustyn/KUtil/issues/3) for more info, but
-I sneaked it to PyPI with a different name: `KUtil-jakubaugustyn`
+Sadly, the name `kutil` is already used, but I sneaked it to PyPI with a different name: `KUtil-jakubaugustyn`
 
 ```cmd
 pip3 install KUtil-jakubaugustyn
 ```
 
 # Installation
```

### Comparing `KUtil-jakubaugustyn-0.0.3/src/KUtil_jakubaugustyn.egg-info/SOURCES.txt` & `kutil_jakubaugustyn-0.0.4/src/KUtil_jakubaugustyn.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 README.md
 pyproject.toml
 src/KUtil_jakubaugustyn.egg-info/PKG-INFO
 src/KUtil_jakubaugustyn.egg-info/SOURCES.txt
 src/KUtil_jakubaugustyn.egg-info/dependency_links.txt
 src/KUtil_jakubaugustyn.egg-info/top_level.txt
 src/kutil/__init__.py
-src/kutil/typing.py
+src/kutil/typing_help.py
 src/kutil/buffer/BidirectionalByteArray.py
 src/kutil/buffer/ByteBuffer.py
 src/kutil/buffer/DataBuffer.py
 src/kutil/buffer/Serializable.py
 src/kutil/buffer/TextOutput.py
 src/kutil/buffer/__init__.py
 src/kutil/io/__init__.py
@@ -50,26 +50,37 @@
 src/kutil/language/languages/paint_tryhard/__init__.py
 src/kutil/language/languages/paint_tryhard/jobs/__init__.py
 src/kutil/language/languages/paint_tryhard/jobs/boss.py
 src/kutil/language/languages/paint_tryhard/jobs/mathematician.py
 src/kutil/language/languages/paint_tryhard/jobs/painter.py
 src/kutil/protocol/AbstractProtocol.py
 src/kutil/protocol/HTTPConnection.py
+src/kutil/protocol/HTTPSConnection.py
 src/kutil/protocol/HTTPServer.py
 src/kutil/protocol/ProtocolConnection.py
 src/kutil/protocol/ProtocolServer.py
 src/kutil/protocol/TCPConnection.py
 src/kutil/protocol/URLSearchParams.py
 src/kutil/protocol/WSConnection.py
 src/kutil/protocol/__init__.py
 src/kutil/protocol/HTTP/HTTPHeaders.py
 src/kutil/protocol/HTTP/HTTPMethod.py
 src/kutil/protocol/HTTP/HTTPRequest.py
 src/kutil/protocol/HTTP/HTTPResponse.py
 src/kutil/protocol/HTTP/__init__.py
+src/kutil/protocol/TLS/AlertCause.py
+src/kutil/protocol/TLS/CipherSuite.py
+src/kutil/protocol/TLS/ConnectionState.py
+src/kutil/protocol/TLS/RawTLSRecord.py
+src/kutil/protocol/TLS/__init__.py
+src/kutil/protocol/TLS/certificate_verifier.py
+src/kutil/protocol/TLS/extensions.py
+src/kutil/protocol/TLS/messages.py
+src/kutil/protocol/TLS/records.py
+src/kutil/protocol/TLS/tls_cryptography.py
 src/kutil/protocol/WS/WSMessage.py
 src/kutil/protocol/WS/__init__.py
 src/kutil/storage/Cache.py
 src/kutil/storage/Config.py
 src/kutil/storage/__init__.py
 src/kutil/storage/bon/__init__.py
 src/kutil/storage/bon/bon.py
@@ -79,8 +90,9 @@
 src/kutil/storage/bon/shared.py
 src/kutil/threads/ThreadWaiter.py
 src/kutil/threads/__init__.py
 src/kutil/webscraper/MapyCZServer.py
 src/kutil/webscraper/WebScraperServer.py
 src/kutil/webscraper/__init__.py
 tests/test_bon.py
+tests/test_bytebuffer.py
 tests/test_js.py
```

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/buffer/BidirectionalByteArray.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/buffer/BidirectionalByteArray.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/buffer/ByteBuffer.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/buffer/ByteBuffer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,65 +1,77 @@
 #  -*- coding: utf-8 -*-
 __author__ = "kubik.augustyn@post.cz"
 
 import copy
 from typing import Iterable, Self
 
 
+class OutOfBoundsReadError(BaseException):
+    pass
+
+
+class OutOfBoundsUndoError(BaseException):
+    pass
+
+
 class ByteBuffer(Iterable[int]):
     data: bytearray
     pointer: int
 
     def __init__(self, dataOrLength: Iterable[int] | int = 0):
         self.data = bytearray(dataOrLength) if isinstance(dataOrLength, int) else bytearray(
             dataOrLength)
         self.pointer = 0
 
     def readByte(self) -> int:
-        self.has(1)
+        self.assertHas(1)
         self.pointer += 1
         return self.data[self.pointer - 1]
 
+    def readLastByte(self) -> int:
+        assert len(self.data) > 0
+        return self.data[-1]
+
     def read(self, amount: int) -> bytearray:
         if amount == 0:
             return bytearray()
-        self.has(amount)
+        self.assertHas(amount)
         self.pointer += amount
         return self.data[self.pointer - amount:self.pointer]
 
     def readLine(self, newLine: bytes = b"\r\n") -> bytearray:
         amount: int = self.index(newLine)
         data: bytearray = self.read(amount) if amount > 0 else bytearray()
         self.skip(len(newLine))
         return data
 
     def index(self, seq: bytes) -> int:
-        self.has(len(seq))
+        self.assertHas(len(seq))
         for i in range(len(self) - len(seq) + 1):
             if self.data[self.pointer + i:self.pointer + i + len(seq)] == seq:
                 return i
         raise IndexError
 
     def skip(self, amount: int):
         assert amount > 0
-        self.has(amount)
+        self.assertHas(amount)
         self.pointer += amount
 
     def back(self, amount: int):
         assert amount > 0
-        self.has(-amount)
+        self.assertHas(-amount)
         self.pointer -= amount
 
     def __len__(self) -> int:
         return len(self.data) - self.pointer
 
-    def readAll(self) -> bytearray:
+    def readRest(self) -> bytearray:
         if len(self) == 0:
             return bytearray(0)
-        self.has(1)
+        self.assertHas(1)
         amount = len(self)
         self.pointer += amount
         return self.data[self.pointer - amount:self.pointer]
 
     def writeByte(self, byte: int, i: int = -1) -> Self:
         if i == -1:
             self.data.append(byte)
@@ -81,27 +93,46 @@
     def reset(self, data: Iterable[int] | None = None) -> Self:
         self.resetPointer()
         self.data.clear()
         if data is not None:
             self.data.extend(data)
         return self
 
+    def resetBeforePointer(self) -> Self:
+        self.data = self.data[self.pointer:]
+        self.resetPointer()
+        return self
+
     def resetPointer(self) -> Self:
         self.pointer = 0
         return self
 
-    def has(self, amount: int) -> bool:
+    def assertHas(self, amount: int) -> bool:
         if amount == 0:
             raise ValueError("Invalid amount")
+        bytesLeft: int = len(self.data) - self.pointer
+        if amount < 0:
+            if -amount > self.pointer:
+                raise OutOfBoundsUndoError(
+                    f"Not enough bytes (going back by {-amount}, but {self.pointer} had been read)")
+        else:
+            if len(self.data) < self.pointer + amount:
+                raise OutOfBoundsReadError(
+                    f"Not enough bytes (reading {amount}, but {bytesLeft} are available)")
+        return True
+
+    def has(self, amount: int) -> bool:
+        if amount == 0:
+            return True
         if amount < 0:
             if -amount > self.pointer:
-                raise ValueError("Not enough bytes")
+                return False
         else:
             if len(self.data) < self.pointer + amount:
-                raise IndexError("Not enough bytes")
+                return False
         return True
 
     def copy(self) -> Self:
         copyBuff = ByteBuffer()
         copyBuff.data = copy.copy(self.data)
         copyBuff.pointer = self.pointer
         return copyBuff
```

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/buffer/DataBuffer.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/buffer/DataBuffer.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,18 @@
         self.buff.write(num.to_bytes(4, "big", signed=False))
         return self
 
     def writeUInt64(self, num: int) -> Self:
         self.buff.write(num.to_bytes(8, "big", signed=False))
         return self
 
+    def writeUIntN(self, num: int, byteSize: int) -> Self:
+        self.buff.write(num.to_bytes(byteSize, "big", signed=False))
+        return self
+
     def writeInt8(self, num: int) -> Self:
         # I don't want to mess with the negative stuff
         self.buff.write(num.to_bytes(1, "big", signed=True))
         return self
 
     def writeInt16(self, num: int) -> Self:
         self.buff.write(num.to_bytes(2, "big", signed=True))
@@ -44,14 +48,18 @@
         self.buff.write(num.to_bytes(4, "big", signed=True))
         return self
 
     def writeInt64(self, num: int) -> Self:
         self.buff.write(num.to_bytes(8, "big", signed=True))
         return self
 
+    def writeIntN(self, num: int, byteSize: int) -> Self:
+        self.buff.write(num.to_bytes(byteSize, "big", signed=True))
+        return self
+
     def writeUInt(self, num: int, byteSize: int) -> Self:
         if byteSize == 1:
             self.writeUInt8(num)
         elif byteSize == 2:
             self.writeUInt16(num)
         elif byteSize == 4:
             self.writeUInt32(num)
@@ -97,27 +105,33 @@
 
     def readUInt32(self) -> int:
         return int.from_bytes(self.buff.read(4), "big", signed=False)
 
     def readUInt64(self) -> int:
         return int.from_bytes(self.buff.read(8), "big", signed=False)
 
+    def readUIntN(self, byteSize: int) -> int:
+        return int.from_bytes(self.buff.read(byteSize), "big", signed=False)
+
     def readInt8(self) -> int:
         # I don't want to mess with the negative stuff
         return int.from_bytes(self.buff.read(1), "big", signed=True)
 
     def readInt16(self) -> int:
         return int.from_bytes(self.buff.read(2), "big", signed=True)
 
     def readInt32(self) -> int:
         return int.from_bytes(self.buff.read(4), "big", signed=True)
 
     def readInt64(self) -> int:
         return int.from_bytes(self.buff.read(8), "big", signed=True)
 
+    def readIntN(self, byteSize: int) -> int:
+        return int.from_bytes(self.buff.read(byteSize), "big", signed=True)
+
     def readUInt(self, byteSize: int) -> int:
         if byteSize == 1:
             return self.readUInt8()
         elif byteSize == 2:
             return self.readUInt16()
         elif byteSize == 4:
             return self.readUInt32()
```

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/buffer/TextOutput.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/buffer/TextOutput.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/io/directory.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/io/directory.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/io/file.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/io/file.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #  -*- coding: utf-8 -*-
 __author__ = "kubik.augustyn@post.cz"
 
 import json
+import os.path
 
 from kutil.buffer.ByteBuffer import ByteBuffer
-from kutil.typing import FinalStr, Final, Literal, overload
+from kutil.typing_help import FinalStr, Final, Literal, overload
 
 type OUTPUT_STR = Literal["text", "bytes", "bytearray", "json", "buffer"]
 type OUTPUT = str | bytes | bytearray | dict | ByteBuffer
 
 
 # Read file
 @overload  # https://mypy.readthedocs.io/en/latest/more_types.html#function-overloading
@@ -64,14 +65,15 @@
         raise ValueError("Bad data kind.")
     with open(path, "wb+") as f:
         f.write(content)
 
 
 # Newline stuff
 type NL_TYPE = Literal["CR", "LF", "CRLF"]
+NL_TYPES: set[str] = {"CR", "LF", "CRLF"}
 CR: FinalStr = "\r"  # Carriage return
 LF: FinalStr = "\n"  # Line feed
 CRLF: FinalStr = "\r\n"  # CRLF
 bCR: Final[bytes] = b"\r"  # Bytes carriage return
 bLF: Final[bytes] = b"\n"  # Bytes line feed
 bCRLF: Final[bytes] = b"\r\n"  # Bytes CRLF
 cCR: Final[int] = ord("\r")  # Char carriage return
@@ -93,15 +95,32 @@
         NL, bNL = LF, bLF
     elif nlType == "CRLF":
         NL, bNL = CRLF, bCRLF
     else:
         raise ValueError
 
 
+# TODO Fix config and make this possible
+# changeNewline(Config().io.newline)
+
+def splitFileExtension(path: str) -> tuple[str, str]:
+    fn, ext = os.path.splitext(os.path.basename(path))
+    return fn, ext
+
+
+def getFileName(path: str) -> str:
+    return splitFileExtension(path)[0]
+
+
+def getFileExtension(path: str) -> str:
+    return splitFileExtension(path)[1]
+
+
 __all__ = [
     "readFile", "writeFile",
     "CR", "LF", "CRLF",
     "bCR", "bLF", "bCRLF",
     "cCR", "cLF",
     "NL", "bNL",
-    "changeNewline"
+    "changeNewline",
+    "splitFileExtension", "getFileName", "getFileExtension"
 ]
```

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/language/AST.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/language/AST.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #  -*- coding: utf-8 -*-
 __author__ = "kubik.augustyn@post.cz"
 
 from enum import Enum
 from typing import Any, Iterator
-from kutil.typing import FrozenList
+from kutil.typing_help import FrozenList
 
 
 class ASTNode:
     type: Enum
     data: Any
 
     def __init__(self, type: Enum, data: Any):
```

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/language/BytecodeFile.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/language/BytecodeFile.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/language/Compiler.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/language/Compiler.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/language/Error.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/language/Error.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/language/Interpreter.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/language/Interpreter.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/language/Language.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/language/Language.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/language/Lexer.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/language/Lexer.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/language/Options.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/language/Options.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/language/Parser.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/language/Parser.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/language/Stack.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/language/Stack.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/language/Token.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/language/Token.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/BrainFuck.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/BrainFuck.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/javascript/JSLexer.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/javascript/JSLexer.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/javascript/JSOptions.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/javascript/JSOptions.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/javascript/JSParser.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/javascript/JSParser.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/javascript/Javascript.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/javascript/Javascript.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/javascript/__init__.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/javascript/__init__.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/javascript/character.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/javascript/character.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/javascript/error_handler.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/javascript/error_handler.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/javascript/messages.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/javascript/messages.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/javascript/nodes.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/javascript/nodes.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/javascript/syntax.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/javascript/syntax.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/paint_tryhard/Canvas.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/paint_tryhard/Canvas.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/paint_tryhard/Employee.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/paint_tryhard/Employee.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/paint_tryhard/PTCompiler.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/paint_tryhard/PTCompiler.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/paint_tryhard/PTInterpreter.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/paint_tryhard/PTInterpreter.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/paint_tryhard/PTLexer.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/paint_tryhard/PTLexer.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/paint_tryhard/PTParser.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/paint_tryhard/PTParser.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/paint_tryhard/PaintTryhard.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/paint_tryhard/PaintTryhard.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/paint_tryhard/jobs/__init__.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/paint_tryhard/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/paint_tryhard/jobs/boss.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/paint_tryhard/jobs/boss.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/paint_tryhard/jobs/mathematician.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/paint_tryhard/jobs/mathematician.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/language/languages/paint_tryhard/jobs/painter.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/language/languages/paint_tryhard/jobs/painter.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/protocol/AbstractProtocol.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/protocol/AbstractProtocol.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 
 from kutil.buffer import ByteBuffer
 
 
 class NeedMoreDataError(BaseException): ...
 
 
+class StopUnpacking(BaseException): ...
+
+
 class AbstractProtocol(ABC):
     name: str = "AbstractProtocol"
     connection: object
 
     def __init__(self, connection):
         from kutil.protocol.ProtocolConnection import ProtocolConnection
         if not isinstance(connection, ProtocolConnection):
```

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/protocol/HTTP/HTTPHeaders.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/protocol/HTTP/HTTPHeaders.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 
     def __eq__(self, other):
         return self.key.lower() == other.key.lower()
 
     def __str__(self):
         return self.key
 
+    def __repr__(self):
+        return f"<CaseInsensitiveKey '{self.key}'>"
+
 
 class HTTPHeaders(dict[str, str]):
     def __init__(self):
         super().__init__()
 
     def __setitem__(self, key: str, value: str):
         key = CaseInsensitiveKey(key)
@@ -30,15 +33,15 @@
     def __getitem__(self, key: str) -> str:
         key = CaseInsensitiveKey(key)
         return super().__getitem__(key)
 
     def get(self, key: str, default=None):
         key = CaseInsensitiveKey(key)
         if key not in self:
-            return
+            return default
         return super().__getitem__(key)
 
 
 if __name__ == '__main__':
     headers: HTTPHeaders = HTTPHeaders()
     headers["Sus"] = "good"
     assert headers.get("sUS") == "good"
```

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/protocol/HTTP/HTTPRequest.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/protocol/HTTP/HTTPRequest.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #  -*- coding: utf-8 -*-
 __author__ = "kubik.augustyn@post.cz"
 
+import json
+
 from kutil.buffer.ByteBuffer import ByteBuffer
 from kutil.buffer.Serializable import Serializable
 from kutil.protocol.HTTP.HTTPMethod import HTTPMethod
 from kutil.protocol.HTTP.HTTPHeaders import HTTPHeaders
 from typing import Final, Optional
 
 
@@ -24,29 +26,56 @@
     def write(self, buff: ByteBuffer):
         raise NotImplementedError
 
     def writeRest(self, buff: ByteBuffer):
         # Make sure the content-length is present and correct
         self.headers["Content-Length"] = str(len(self.body))
         for name, value in self.headers.items():
-            buff.write(self.enc(str(name))).write(self.HEADER_SEP).write(self.enc(value)).write(self.CRLF)
+            buff.write(self.enc(str(name))).write(self.HEADER_SEP).write(self.enc(value)).write(
+                self.CRLF)
         buff.write(self.CRLF)
         buff.write(self.body)
 
     def read(self, buff: ByteBuffer):
         raise NotImplementedError
 
     def readRest(self, buff: ByteBuffer):
         line: bytearray = buff.readLine(self.CRLF)
         self.headers = HTTPHeaders()
         while len(line) > 0:
-            name, value = line.split(self.HEADER_SEP)
+            name, value = line.split(self.HEADER_SEP, maxsplit=1)
             self.headers[self.dec(name)] = self.dec(value)
             line = buff.readLine(self.CRLF)
-        self.body = bytes(buff.readAll())
+        try:
+            bodySize: int = abs(int(self.headers.get("Content-Length", "0")))
+        except (ValueError, TypeError):
+            bodySize: int = 0
+        self.body = bytes(buff.read(bodySize))
+
+    @property
+    def json(self) -> dict:
+        if self.body is None or len(self.body) == 0:
+            raise ValueError("Empty body")
+        try:
+            text = HTTPThing.dec(self.body)
+        except UnicodeDecodeError as e:
+            raise ValueError("Invalid body format") from e
+
+        return json.loads(text)
+
+    @property
+    def text(self) -> str:
+        if self.body is None or len(self.body) == 0:
+            return ""
+        try:
+            text = HTTPThing.dec(self.body)
+        except UnicodeDecodeError as e:
+            raise ValueError("Invalid body format") from e
+
+        return text
 
     @staticmethod
     def enc(thing: str) -> bytes:
         return thing.encode("utf-8")
 
     @staticmethod
     def dec(thing: bytes) -> str:
@@ -60,15 +89,16 @@
     def __init__(self, method: Optional[HTTPMethod] = None, requestURI: Optional[str] = None,
                  headers: Optional[HTTPHeaders] = None, body: Optional[bytes] = None):
         super().__init__(headers, body)
         self.method = method or HTTPMethod.GET
         self.requestURI = requestURI or "/"
 
     def write(self, buff: ByteBuffer):
-        buff.write(self.method.value).write(self.SP).write(self.enc(self.requestURI)).write(self.SP).write(self.VERSION)
+        buff.write(self.method.value).write(self.SP).write(self.enc(self.requestURI)).write(
+            self.SP).write(self.VERSION)
         buff.write(self.CRLF)
         self.writeRest(buff)
 
     def read(self, buff: ByteBuffer):
         method, requestURI, version = buff.readLine(self.CRLF).split(self.SP)
         self.method = HTTPMethod(method)
         self.requestURI = self.dec(requestURI)
```

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/protocol/HTTP/HTTPResponse.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/protocol/HTTP/HTTPResponse.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/protocol/HTTPConnection.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/protocol/HTTPConnection.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,26 +6,23 @@
 from kutil.buffer.ByteBuffer import ByteBuffer
 from kutil.protocol.AbstractProtocol import AbstractProtocol, NeedMoreDataError
 from kutil.protocol.ProtocolConnection import ProtocolConnection
 from kutil.protocol.TCPConnection import TCPProtocol
 from kutil.protocol.HTTP.HTTPRequest import HTTPRequest
 from kutil.protocol.HTTP.HTTPResponse import HTTPResponse
 
-type OnHTTPDataListener = Callable[[HTTPResponse], None]
+type OnHTTPDataListener = Callable[[ProtocolConnection, HTTPResponse], None]
 
 
 class HTTPProtocol(AbstractProtocol):
     name = "HTTPProtocol"
 
     def unpackData(self, buff: ByteBuffer) -> HTTPResponse:
         resp = HTTPResponse()
-        try:
-            resp.read(buff)
-        except Exception:
-            raise NeedMoreDataError
+        resp.read(buff)  # Don't catch errors!
         return resp
 
     def unpackSubProtocol(self, buff: ByteBuffer) -> ByteBuffer:
         return buff  # Nothing lol
 
     def packData(self, data: HTTPRequest, buff: ByteBuffer):
         data.write(buff)
```

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/protocol/HTTPServer.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/protocol/HTTPServer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 #  -*- coding: utf-8 -*-
 __author__ = "kubik.augustyn@post.cz"
 
-from typing import Callable, Any
+from typing import Callable, Any, Self
+
+from kutil.typing_help import neverCall
+
 from kutil.protocol.AbstractProtocol import AbstractProtocol, NeedMoreDataError
 from kutil.buffer.ByteBuffer import ByteBuffer
 from kutil.protocol.ProtocolConnection import ProtocolConnection
 from kutil.protocol.ProtocolServer import ProtocolServer
 from kutil.protocol.TCPConnection import TCPProtocol
 from kutil.protocol.WS.WSMessage import WSMessage
 from kutil.protocol.HTTP.HTTPRequest import HTTPRequest
@@ -38,55 +41,73 @@
         data.write(buff)
 
     def packSubProtocol(self, buff: ByteBuffer):
         raise RuntimeError  # Not possible
         # pass  # Nothing lol
 
 
+class WebSocketNotAllowed(Exception):
+    pass
+
+
 class HTTPServerConnection(ProtocolConnection):
     # Note that editing the __init__ method might break the whole thing
-    onData: Callable[[HTTPRequest | WSMessage], None]
+    onData: Callable[[Self, HTTPRequest | WSMessage], None]
     didUpgradeToWS: bool
     acceptWSChecker: AcceptWSChecker
     onWebsocketEstablishment: Callable[[Any], None] | None
     wsConn: WSConnection | None
 
     def init(self):
         self.didUpgradeToWS = False
         self.acceptWSChecker = lambda x, y: False
         self.onWebsocketEstablishment = None  # Change if wanted, called with self as the argument
         self.wsConn = None
 
-    def onDataInner(self, data: HTTPRequest | WSMessage) -> bool:
-        assert isinstance(data, HTTPRequest) if not self.didUpgradeToWS else isinstance(data, WSMessage)
+    def _denyWebsocketConnection(self, notAllowedOrInvalid: bool):
+        if notAllowedOrInvalid:
+            resp: HTTPResponse = HTTPResponse(400, "Invalid protocol selected", HTTPHeaders(), b'')
+        else:
+            resp: HTTPResponse = HTTPResponse(400, "Bad request", HTTPHeaders(),
+                                              b'Invalid key header or version != 13 selected')
+        self.sendData(resp)
+        self.close(WebSocketNotAllowed())
+
+    def onDataInner(self, data: HTTPRequest | WSMessage, stoppedUnpacking: bool = False,
+                    layer: AbstractProtocol | None = None) -> bool:
+        assert isinstance(data, HTTPRequest) if not self.didUpgradeToWS else isinstance(data,
+                                                                                        WSMessage)
         if not self.didUpgradeToWS:
-            if data.headers.get("Upgrade") == "websocket" and data.headers.get("Connection") == "Upgrade":
+            if data.headers.get("Upgrade") == "websocket" and data.headers.get(
+                    "Connection") == "Upgrade":
                 if not self.acceptWSChecker(self, data):
                     # Cancel the connection if we aren't allowed to establish a WS connection
-                    self.close()
+                    self._denyWebsocketConnection(True)
                     return False
-                if data.headers.get("Sec-WebSocket-Version") != "13" or data.headers.get("Sec-WebSocket-Key") is None:
+                if data.headers.get("Sec-WebSocket-Version") != "13" or data.headers.get(
+                        "Sec-WebSocket-Key") is None:
                     # Make sure we both support v13 and we have a key
-                    self.close()
+                    self._denyWebsocketConnection(False)
                     return False
                 # print(data.headers.get("Sec-WebSocket-Key"))
                 # print(WSProtocol.createAcceptHeader(data.headers.get("Sec-WebSocket-Key")))
                 headers: HTTPHeaders = HTTPHeaders()
                 headers["Upgrade"] = "websocket"
                 headers["Connection"] = "Upgrade"
                 # headers["Sec-WebSocket-Protocol"] = "chat" - breaks stuff, although on Wikipedia
-                headers["Sec-WebSocket-Accept"] = WSProtocol.createAcceptHeader(data.headers.get("Sec-WebSocket-Key"))
+                headers["Sec-WebSocket-Accept"] = WSProtocol.createAcceptHeader(
+                    data.headers.get("Sec-WebSocket-Key"))
                 resp: HTTPResponse = HTTPResponse(101, "Switching Protocols", headers, b'')
                 self.sendData(resp)
                 self.removeProtocol(self.layers[-1])  # Remove the HTTP protocol
                 self.addProtocol(WSProtocol(self))
                 self.didUpgradeToWS = True
                 if self.onWebsocketEstablishment:
                     self.onWebsocketEstablishment(self)
-                self.wsConn = WSConnection(("", 0), [], None, self.sock)
+                self.wsConn = WSConnection(("", 0), [], neverCall, self.sock)
                 return False  # Don't call the onData with the WS request
         return True
 
     def acceptWebsocket(self, acceptWSChecker: AcceptWSChecker):
         self.acceptWSChecker = acceptWSChecker
 
     @property
@@ -96,16 +117,19 @@
         return self
 
 
 class HTTPServer(ProtocolServer):
     connectionType: type[ProtocolConnection] = HTTPServerConnection
     acceptWSChecker: AcceptWSChecker
 
-    def __init__(self, address: tuple[str, int], onConnection: Callable[[ProtocolConnection], Callable[[Any], None]]):
-        super().__init__(address, lambda conn: [TCPProtocol(conn), HTTPServerProtocol(conn)], onConnection)
+    def __init__(self, address: tuple[str, int],
+                 onConnection: Callable[[ProtocolConnection], Callable[[ProtocolConnection,
+                                                                        HTTPRequest], None]]):
+        super().__init__(address, lambda conn: [TCPProtocol(conn), HTTPServerProtocol(conn)],
+                         onConnection)
         self.acceptWSChecker = lambda x, y: False
 
     def acceptWebsocket(self, acceptWSChecker: AcceptWSChecker):
         self.acceptWSChecker = acceptWSChecker
 
     def onConnectionInner(self, conn: HTTPServerConnection) -> bool:
         conn.acceptWebsocket(self.acceptWSChecker)
```

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/protocol/TCPConnection.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/protocol/TCPConnection.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 type OnTCPDataListener = Callable[[bytes], None]
 
 
 class TCPProtocol(AbstractProtocol):
     name = "TCPProtocol"
 
     def unpackData(self, buff: ByteBuffer) -> bytes:
-        return buff.readAll()
+        return buff.readRest()
 
     def unpackSubProtocol(self, buff: ByteBuffer) -> ByteBuffer:
         return buff  # Nothing lol
 
     def packData(self, data: bytes, buff: ByteBuffer):
         buff.write(data)
```

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/protocol/URLSearchParams.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/protocol/URLSearchParams.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 class URLSearchParams:
     params: dict[str, str]
 
     def __init__(self, val: Optional[str] = None):
         self.params = {}
-        if val.startswith("?"):
+        if val.startswith("?") or val.startswith("&"):
             val = val[1:]
         if val:
             self.parse(val)
 
     def parse(self, val: str):
         self.params = {}
         for part in val.split("&"):
```

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/protocol/WS/WSMessage.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/protocol/WS/WSMessage.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/protocol/WSConnection.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/protocol/WSConnection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #  -*- coding: utf-8 -*-
 __author__ = "kubik.augustyn@post.cz"
 
 from base64 import b64encode
 from hashlib import sha1
+from typing import Any
 
 from kutil.protocol.AbstractProtocol import AbstractProtocol, NeedMoreDataError
 from kutil.buffer.ByteBuffer import ByteBuffer
-from kutil.protocol.ProtocolConnection import ProtocolConnection
+from kutil.protocol.ProtocolConnection import ProtocolConnection, ConnectionClosed
 from kutil.protocol.WS import WSMessage, WSOpcode, WSData
 
 
 class WSProtocol(AbstractProtocol):
     name = "WSProtocol"
 
     def unpackData(self, buff: ByteBuffer) -> WSMessage:
@@ -50,25 +51,27 @@
 
 class WSConnection(ProtocolConnection):
     dataBuffer: ByteBuffer
 
     def init(self):
         self.dataBuffer = ByteBuffer()
 
-    def onDataInner(self, data: WSMessage) -> bool | WSData:
+    def onDataInner(self, data: WSMessage, stoppedUnpacking: bool = False,
+                    layer: AbstractProtocol | None = None) -> bool | WSData:
         if data.opcode in (WSOpcode.BINARY_FRAME, WSOpcode.TEXT_FRAME):
             self.dataBuffer.write(data.payload.superSecretRawAccess)
             if data.isFin:
                 message: WSData = WSData(self.dataBuffer.export())
                 message.isBinary = data.opcode == WSOpcode.BINARY_FRAME
                 return message
             return False
         if data.opcode == WSOpcode.CONNECTION_CLOSE:
-            self.close()
+            self.close(ConnectionClosed())
             return False
         print("Unknown frame:", data.opcode.name)
-        self.close()
+        self.close(ValueError("Unknown frame:" + data.opcode.name))
         return False
 
 
 if __name__ == '__main__':
-    assert WSProtocol.createAcceptHeader("x3JJHMbDL1EzLkh9GBhXDw==") == "HSmrc0sMlYUkAGmm5OPpG2HaGWk="
+    assert WSProtocol.createAcceptHeader(
+        "x3JJHMbDL1EzLkh9GBhXDw==") == "HSmrc0sMlYUkAGmm5OPpG2HaGWk="
```

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/storage/Config.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/storage/Config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #  -*- coding: utf-8 -*-
 __author__ = "kubik.augustyn@post.cz"
 
 import inspect
 import os.path
 from typing import TypeVar, Optional
 
-from kutil.typing import singleton, anyattribute
+from kutil.typing_help import singleton, anyattribute
 from kutil.io.directory import getDirParent
 from kutil.io.file import readFile, writeFile
 
 TConfigEntry = TypeVar("TConfigEntry", bound="ConfigEntry")
 
 
 @anyattribute("_raw")
@@ -74,66 +74,66 @@
 class Config:
     """
     A class that holds all the configuration for your project.
     """
 
     CONFIG_FILE = "config.json"
     # https://stackoverflow.com/questions/2860153/how
-    backupConfigPath: str = getDirParent(os.path.dirname(__file__))  # C:\Users\...\KUtil\kutil
+    _backupConfigPath: str = getDirParent(os.path.dirname(__file__))  # C:\Users\...\KUtil\kutil
 
-    startDirPath: str
-    descendentConfigPaths: list[str]  # The last item is the most unlikely config to be used
-    configEntries: list[ConfigEntry]
+    _startDirPath: str
+    _descendentConfigPaths: list[str]  # The last item is the most unlikely config to be used
+    _configEntries: list[ConfigEntry]
 
     def __init__(self):
         # https://stackoverflow.com/questions/13699283/how-tf
         # get the caller's stack frame and extract its file path
         frame_info = inspect.stack()[2]  # Index 2 - __init__, @anyattribute, @singleton, <caller>
         filepath = frame_info.filename
         del frame_info  # drop the reference to the stack frame to avoid reference cycles
         # make the path absolute (optional)
-        self.startDirPath = os.path.dirname(os.path.abspath(filepath))
-        self.configEntries = []
+        self._startDirPath = os.path.dirname(os.path.abspath(filepath))
+        self._configEntries = []
 
         self._populateConfigPaths()
         # print(self.descendentConfigPaths)
 
     def _populateConfigPaths(self):
-        paths = [self.backupConfigPath]
-        path = self.startDirPath
+        paths = [self._backupConfigPath]
+        path = self._startDirPath
         try:
             while True:
                 if path not in paths:
                     paths.append(path)
                 path = getDirParent(path)
         except ValueError:
             pass
         paths.reverse()
         # Filter out non-existent paths
         paths = list(filter(lambda path: os.path.exists(self._getConfigPath(path)), paths))
         assert len(paths) > 0, f"Failed to find {self.CONFIG_FILE}"
-        self.descendentConfigPaths = paths
+        self._descendentConfigPaths = paths
 
     def _getConfigPath(self, dirPath: str) -> str:
         return os.path.join(dirPath, self.CONFIG_FILE)
 
     def _loadConfig(self, depth: int) -> ConfigEntry:
-        assert depth < len(self.descendentConfigPaths), f"No path for such deep {self.CONFIG_FILE} file"
-        if depth < len(self.configEntries):
-            return self.configEntries[depth]
-        for i, path in enumerate(self.descendentConfigPaths):
-            if i < len(self.configEntries):
+        assert depth < len(self._descendentConfigPaths), f"No path for such deep {self.CONFIG_FILE} file"
+        if depth < len(self._configEntries):
+            return self._configEntries[depth]
+        for i, path in enumerate(self._descendentConfigPaths):
+            if i < len(self._configEntries):
                 continue  # We have already loaded that one
             elif i > depth:
                 break
             raw = readFile(self._getConfigPath(path), "json")
             entry = ConfigEntry(raw, path)
-            assert i == len(self.configEntries)  # All good, just checking
-            self.configEntries.append(entry)
-        return self.configEntries[depth]
+            assert i == len(self._configEntries)  # All good, just checking
+            self._configEntries.append(entry)
+        return self._configEntries[depth]
 
     def _getSuitableEntryToRead(self, key: str) -> ConfigEntry:
         try:
             depth = 0
             while True:
                 entry = self._loadConfig(depth)
                 if key in entry:
```

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/storage/bon/bon.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/storage/bon/bon.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/storage/bon/converter.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/storage/bon/converter.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/storage/bon/decoder.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/storage/bon/decoder.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/storage/bon/encoder.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/storage/bon/encoder.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/storage/bon/shared.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/storage/bon/shared.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/threads/ThreadWaiter.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/threads/ThreadWaiter.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/typing.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/typing_help.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,16 +177,16 @@
                 else:  # Set property of any name
                     if attributeStorage is None or oldDelAttr is not None:
                         oldDelAttr(self, name)
                     else:
                         del getattr(self, attributeStorage)[name]
 
             def __repr__(self) -> str:
-                # return f"<kutil.typing.anyattribute._AnyAttributeHelper of {repr(cls)} at {hex(id(self))}>"
-                # return f"<kutil.typing.anyattribute._AnyAttributeHelper of {cls.__repr__(self)} at {hex(id(self))}>"
+                # return f"<kutil.typing_help.anyattribute._AnyAttributeHelper of {repr(cls)} at {hex(id(self))}>"
+                # return f"<kutil.typing_help.anyattribute._AnyAttributeHelper of {cls.__repr__(self)} at {hex(id(self))}>"
                 return cls.__repr__(self)
 
         # print("Updated class:", vars(_AnyAttributeHelper))
 
         # def _anyattribute(*args, **kwargs):
         #     instance = _AnyAttributeHelper(*args, **kwargs)
         # print("Instance:", vars(instance))
@@ -311,15 +311,15 @@
             return wrapper(self, *args, **kwargs)
 
         def __repr__(self):
             funcs = map(
                 lambda info: info[0].__name__ + str(inspect.signature(info[0])),
                 self.__overloads__
             )
-            return f"<kutil.typing.overload_args wrapper for {', '.join(funcs)} at {hex(id(self))}>"
+            return f"<kutil.typing_help.overload_args wrapper for {', '.join(funcs)} at {hex(id(self))}>"
 
     return ReprWrapper()
 
 
 def overload_args(fn: Callable) -> Callable:
     raise NotImplementedError("It's implemented, but not properly :-/")
     # TODO Fix it
@@ -383,12 +383,16 @@
 
     newDict: dict = {}
     for d in dicts:
         newDict.update(d)
     return newDict
 
 
+def neverCall(*args, **kwargs) -> Never:
+    raise Exception("This function should never be called")
+
+
 # dictUnion({"a": 6}, {"a": 8}, {"b": 7})
 
 
 # Additional types
 type FinalStr = Final[str]
```

### Comparing `KUtil-jakubaugustyn-0.0.3/src/kutil/webscraper/WebScraperServer.py` & `kutil_jakubaugustyn-0.0.4/src/kutil/webscraper/WebScraperServer.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,40 +24,58 @@
     def listen(self):
         self.server.listen()
 
     def onConnection(self, conn: ProtocolConnection):
         # print(conn)
         if not isinstance(conn, HTTPServerConnection):
             raise ValueError
-        castedConn: HTTPServerConnection = conn
         # print(f"On connection...")
-        return lambda data: self.onData(castedConn, data)
+        return self.onData
 
     def onData(self, conn: HTTPServerConnection, req: HTTPRequest):
         try:
             resp = self.onDataInner(conn, req)
+            assert isinstance(resp, HTTPResponse)
         except Exception as e:
             content = str(e)
             if not content:
                 content = str(type(e).__name__)
-            resp = HTTPResponse(500, "Internal server error", HTTPHeaders(), HTTPResponse.enc(content))
+            resp = HTTPResponse(500, "Internal server error", HTTPHeaders(),
+                                HTTPResponse.enc(content))
             resp.headers["Content-Type"] = "text/plain"
         # Don't close the socket if the client wants to request more data
         close = req.headers.get("Connection", "close") != "keep-alive"
         resp.headers["Access-Control-Allow-Origin"] = "*"
         WebScraperServer.sendResponse(resp, conn, close)
 
     @abstractmethod
     def onDataInner(self, conn: HTTPServerConnection, req: HTTPRequest) -> HTTPResponse:
-        return HTTPResponse(405, "Method not Allowed", HTTPHeaders(), b'This is for websocket.')
+        headers = HTTPHeaders()
+        headers["Content-Type"] = "text/html"
+        return HTTPResponse(200, "OK", headers, b'WebScraperServer - rewrite the '
+                                                b'onDataInner method to handle incoming requests')
 
     @staticmethod
     def sendResponse(resp: HTTPResponse, conn: HTTPServerConnection, close: bool = True):
         conn.sendData(resp)
         if close:
             conn.close()
 
     @staticmethod
     def badRequest() -> HTTPResponse:
         headers: HTTPHeaders = HTTPHeaders()
         headers["Content-Type"] = "text/html"
         return HTTPResponse(400, "Bad request", headers, b'<h1>A bad request.</h1>')
+
+    @staticmethod
+    def badMethod() -> HTTPResponse:
+        headers: HTTPHeaders = HTTPHeaders()
+        headers["Content-Type"] = "text/html"
+        return HTTPResponse(405, "Method not allowed", headers,
+                            b'<h1>The requested method is not allowed.</h1>')
+
+    @staticmethod
+    def internalError() -> HTTPResponse:
+        headers: HTTPHeaders = HTTPHeaders()
+        headers["Content-Type"] = "text/html"
+        return HTTPResponse(500, "Internal server error", headers,
+                            b'<h1>An internal server error has occured.</h1>')
```

### Comparing `KUtil-jakubaugustyn-0.0.3/tests/test_bon.py` & `kutil_jakubaugustyn-0.0.4/tests/test_bon.py`

 * *Files identical despite different names*

### Comparing `KUtil-jakubaugustyn-0.0.3/tests/test_js.py` & `kutil_jakubaugustyn-0.0.4/tests/test_js.py`

 * *Files identical despite different names*

