# Comparing `tmp/quickfix-py-0.0.1.tar.gz` & `tmp/quickfix_py-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickfix-py-0.0.1.tar", last modified: Tue Apr  9 22:47:38 2024, max compression
+gzip compressed data, was "quickfix_py-0.0.2.tar", last modified: Tue Apr 16 07:48:49 2024, max compression
```

## Comparing `quickfix-py-0.0.1.tar` & `quickfix_py-0.0.2.tar`

### file list

```diff
@@ -1,207 +1,207 @@
-drwxr-xr-x   0 pablo.carballo   (503) staff       (20)        0 2024-04-09 22:47:38.640121 quickfix-py-0.0.1/
-drwxr-xr-x   0 pablo.carballo   (503) staff       (20)        0 2024-04-09 22:47:38.624028 quickfix-py-0.0.1/C++/
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     6691 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/Acceptor.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     3729 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/Acceptor.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)      331 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/Allocator.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     5200 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/Application.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     2140 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/DOMDocument.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    22844 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/DataDictionary.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    20038 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/DataDictionary.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     2181 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/DataDictionaryProvider.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     2373 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/DataDictionaryProvider.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     3117 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/DatabaseConnectionID.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     2207 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/DatabaseConnectionPool.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     4286 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/Dictionary.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     2885 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/Dictionary.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     2047 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/Event.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     1148 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/Except.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     8134 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/Exceptions.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    27475 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/Field.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     2854 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/FieldConvertors.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    19814 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/FieldConvertors.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     6389 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/FieldMap.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    10722 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/FieldMap.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     1447 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/FieldNumbers.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     1649 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/FieldTypes.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    24445 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/FieldTypes.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)      922 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/Fields.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     5167 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/FileLog.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     3105 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/FileLog.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    10171 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/FileStore.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     3945 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/FileStore.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)      230 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/FixCommonFields.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)   309036 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/FixFieldNumbers.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)   281876 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/FixFields.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)   303490 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/FixValues.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     1678 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/Group.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     2091 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/Group.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     2511 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/HostDetailsProvider.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)      888 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/HostDetailsProvider.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     3492 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/HtmlBuilder.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    23865 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/HttpConnection.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     2730 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/HttpConnection.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     5376 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/HttpMessage.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     3199 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/HttpMessage.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     1328 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/HttpParser.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     1398 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/HttpParser.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     3604 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/HttpServer.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     2113 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/HttpServer.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     7798 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/Initiator.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     4429 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/Initiator.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     2082 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/Log.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     4631 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/Log.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    19241 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/Message.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    14434 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/Message.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     7198 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/MessageCracker.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     2261 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/MessageSorters.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     4304 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/MessageSorters.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     4432 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/MessageStore.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     5559 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/MessageStore.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     2490 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/Mutex.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     4708 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/MySQLConnection.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     7790 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/MySQLLog.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     4566 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/MySQLLog.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    11943 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/MySQLStore.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     4693 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/MySQLStore.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     1353 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/NullStore.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     2932 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/NullStore.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     6273 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/OdbcConnection.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     6871 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/OdbcLog.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     3252 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/OdbcLog.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    11771 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/OdbcStore.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     3635 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/OdbcStore.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     2720 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/PUGIXML_DOMDocument.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     2052 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/PUGIXML_DOMDocument.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     2584 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/Parser.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     1519 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/Parser.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     4164 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/PostgreSQLConnection.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     7825 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/PostgreSQLLog.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     4672 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/PostgreSQLLog.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    12099 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/PostgreSQLStore.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     4854 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/PostgreSQLStore.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     1541 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/Queue.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)  5668830 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/QuickfixPython.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     2544 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/QuickfixPython.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     1168 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/Responder.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    13450 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/SSLSocketAcceptor.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     7357 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/SSLSocketAcceptor.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    13332 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/SSLSocketConnection.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     7953 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/SSLSocketConnection.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    17612 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/SSLSocketInitiator.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     7919 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/SSLSocketInitiator.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    46590 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/Session.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    12406 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/Session.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    10939 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/SessionFactory.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     2810 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/SessionFactory.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     4681 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/SessionID.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     5491 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/SessionSettings.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    12106 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/SessionSettings.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     7907 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/SessionState.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     4446 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/Settings.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     1488 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/Settings.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     6842 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/SharedArray.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     6256 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/SocketAcceptor.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     2464 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/SocketAcceptor.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     5900 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/SocketConnection.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     2604 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/SocketConnection.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     3521 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/SocketConnector.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     2150 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/SocketConnector.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     6370 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/SocketInitiator.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     2418 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/SocketInitiator.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)      877 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/SocketMonitor.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     6304 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/SocketMonitor_UNIX.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     2946 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/SocketMonitor_UNIX.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     6393 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/SocketMonitor_WIN32.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     2745 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/SocketMonitor_WIN32.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     4721 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/SocketServer.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     2918 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/SocketServer.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    14450 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/ThreadedSSLSocketAcceptor.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     8192 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/ThreadedSSLSocketAcceptor.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    11641 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/ThreadedSSLSocketConnection.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     7023 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/ThreadedSSLSocketConnection.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    13186 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/ThreadedSSLSocketInitiator.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     7506 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/ThreadedSSLSocketInitiator.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     7086 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/ThreadedSocketAcceptor.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     3022 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/ThreadedSocketAcceptor.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     5367 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/ThreadedSocketConnection.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     2359 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/ThreadedSocketConnection.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     6085 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/ThreadedSocketInitiator.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     2432 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/ThreadedSocketInitiator.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     7918 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/TimeRange.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     8179 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/TimeRange.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    14921 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/Utility.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     7186 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/Utility.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    44399 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/UtilitySSL.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    11104 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/UtilitySSL.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     3440 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/Values.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)      174 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/config-all.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)      131 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/config.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     4898 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/config_unix.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)      357 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/config_windows.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    22917 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/dirent_windows.h
-drwxr-xr-x   0 pablo.carballo   (503) staff       (20)        0 2024-04-09 22:47:38.629139 quickfix-py-0.0.1/C++/double-conversion/
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    27312 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/double-conversion/bignum-dtoa.cc
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     4318 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/double-conversion/bignum-dtoa.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    23111 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/double-conversion/bignum.cc
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     5495 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/double-conversion/bignum.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     8507 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/double-conversion/cached-powers.cc
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     3027 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/double-conversion/cached-powers.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     2510 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/double-conversion/diy-fp.cc
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     4104 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/double-conversion/diy-fp.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    32649 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/double-conversion/double-conversion.cc
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    26509 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/double-conversion/double-conversion.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    31124 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/double-conversion/fast-dtoa.cc
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     4082 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/double-conversion/fast-dtoa.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    15102 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/double-conversion/fixed-dtoa.cc
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     2788 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/double-conversion/fixed-dtoa.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    13526 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/double-conversion/ieee.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    21057 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/double-conversion/strtod.cc
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     2227 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/double-conversion/strtod.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    12363 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/double-conversion/utils.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     1562 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/index.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     2747 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/pugiconfig.hpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)   277537 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/pugixml.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    47424 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/pugixml.hpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     7385 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/scope_guard.hpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)      289 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/stdafx.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)      801 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/stdafx.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     7991 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/stdint_msvc.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)      108 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/strptime.h
-drwxr-xr-x   0 pablo.carballo   (503) staff       (20)        0 2024-04-09 22:47:38.630210 quickfix-py-0.0.1/C++/swig/
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     6022 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/swig/MySQLStubs.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     6322 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/swig/PostgreSQLStubs.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     4063 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/swig/SSLStubs.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)      250 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/C++/swig/Utility.h
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     2073 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/LICENSE
--rw-r--r--   0 pablo.carballo   (503) staff       (20)       89 2024-04-08 15:08:28.000000 quickfix-py-0.0.1/MANIFEST.in
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     2869 2024-04-09 22:47:38.639844 quickfix-py-0.0.1/PKG-INFO
--rw-r--r--   0 pablo.carballo   (503) staff       (20)       32 2024-04-09 08:14:31.000000 quickfix-py-0.0.1/README.md
--rw-r--r--   0 pablo.carballo   (503) staff       (20)  1833879 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/quickfix.py
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     4825 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/quickfix40.py
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     6232 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/quickfix41.py
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    21580 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/quickfix42.py
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    64741 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/quickfix43.py
--rw-r--r--   0 pablo.carballo   (503) staff       (20)   262984 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/quickfix44.py
--rw-r--r--   0 pablo.carballo   (503) staff       (20)   381100 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/quickfix50.py
--rw-r--r--   0 pablo.carballo   (503) staff       (20)   450461 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/quickfix50sp1.py
--rw-r--r--   0 pablo.carballo   (503) staff       (20)  8975693 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/quickfix50sp2.py
-drwxr-xr-x   0 pablo.carballo   (503) staff       (20)        0 2024-04-09 22:47:38.639480 quickfix-py-0.0.1/quickfix_py.egg-info/
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     2869 2024-04-09 22:47:38.000000 quickfix-py-0.0.1/quickfix_py.egg-info/PKG-INFO
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     4229 2024-04-09 22:47:38.000000 quickfix-py-0.0.1/quickfix_py.egg-info/SOURCES.txt
--rw-r--r--   0 pablo.carballo   (503) staff       (20)        1 2024-04-09 22:47:38.000000 quickfix-py-0.0.1/quickfix_py.egg-info/dependency_links.txt
--rw-r--r--   0 pablo.carballo   (503) staff       (20)      125 2024-04-09 22:47:38.000000 quickfix-py-0.0.1/quickfix_py.egg-info/top_level.txt
--rw-r--r--   0 pablo.carballo   (503) staff       (20)     1129 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/quickfixt11.py
--rw-r--r--   0 pablo.carballo   (503) staff       (20)       38 2024-04-09 22:47:38.640176 quickfix-py-0.0.1/setup.cfg
--rwxr-xr-x   0 pablo.carballo   (503) staff       (20)     3209 2024-04-09 21:31:31.000000 quickfix-py-0.0.1/setup.py
-drwxr-xr-x   0 pablo.carballo   (503) staff       (20)        0 2024-04-09 22:47:38.639046 quickfix-py-0.0.1/spec/
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    37257 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/spec/FIX40.xml
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    57978 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/spec/FIX41.xml
--rw-r--r--   0 pablo.carballo   (503) staff       (20)   129260 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/spec/FIX42.xml
--rw-r--r--   0 pablo.carballo   (503) staff       (20)   204358 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/spec/FIX43.xml
--rw-r--r--   0 pablo.carballo   (503) staff       (20)   315395 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/spec/FIX44.xml
--rw-r--r--   0 pablo.carballo   (503) staff       (20)   393213 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/spec/FIX50.xml
--rw-r--r--   0 pablo.carballo   (503) staff       (20)   464464 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/spec/FIX50SP1.xml
--rw-r--r--   0 pablo.carballo   (503) staff       (20)  1471310 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/spec/FIX50SP2.xml
--rw-r--r--   0 pablo.carballo   (503) staff       (20)    11927 2024-04-09 21:44:18.000000 quickfix-py-0.0.1/spec/FIXT11.xml
--rw-r--r--   0 pablo.carballo   (503) staff       (20)       81 2024-04-08 15:08:28.000000 quickfix-py-0.0.1/test_std_shared_ptr.cpp
--rw-r--r--   0 pablo.carballo   (503) staff       (20)       90 2024-04-08 15:08:28.000000 quickfix-py-0.0.1/test_std_tr1_shared_ptr.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:48:49.023977 quickfix_py-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:48:49.015977 quickfix_py-0.0.2/C++/
+-rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/Acceptor.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/Acceptor.h
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/Allocator.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/Application.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/DOMDocument.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22844 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/DataDictionary.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    20038 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/DataDictionary.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/DataDictionaryProvider.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/DataDictionaryProvider.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/DatabaseConnectionID.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/DatabaseConnectionPool.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/Dictionary.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/Dictionary.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/Event.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/Except.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/Exceptions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    27475 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/Field.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/FieldConvertors.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19814 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/FieldConvertors.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/FieldMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10722 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/FieldMap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/FieldNumbers.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/FieldTypes.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    24445 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/FieldTypes.h
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/Fields.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/FileLog.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/FileLog.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/FileStore.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/FileStore.h
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/FixCommonFields.h
+-rw-r--r--   0 runner    (1001) docker     (127)   309036 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/FixFieldNumbers.h
+-rw-r--r--   0 runner    (1001) docker     (127)   281876 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/FixFields.h
+-rw-r--r--   0 runner    (1001) docker     (127)   303490 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/FixValues.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/Group.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/Group.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/HostDetailsProvider.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/HostDetailsProvider.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/HtmlBuilder.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23865 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/HttpConnection.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/HttpConnection.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/HttpMessage.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/HttpMessage.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/HttpParser.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/HttpParser.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/HttpServer.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/HttpServer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/Initiator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/Initiator.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/Log.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/Log.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19241 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/Message.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14434 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/Message.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/MessageCracker.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/MessageSorters.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/MessageSorters.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/MessageStore.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/MessageStore.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/Mutex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/MySQLConnection.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/MySQLLog.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/MySQLLog.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11943 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/MySQLStore.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/MySQLStore.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/NullStore.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/NullStore.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/OdbcConnection.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/OdbcLog.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/OdbcLog.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11771 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/OdbcStore.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/OdbcStore.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/PUGIXML_DOMDocument.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/PUGIXML_DOMDocument.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/Parser.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/Parser.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/PostgreSQLConnection.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7825 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/PostgreSQLLog.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/PostgreSQLLog.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12099 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/PostgreSQLStore.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/PostgreSQLStore.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/Queue.h
+-rw-r--r--   0 runner    (1001) docker     (127)  5668830 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/QuickfixPython.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/QuickfixPython.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/Responder.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13450 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/SSLSocketAcceptor.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/SSLSocketAcceptor.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13332 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/SSLSocketConnection.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7953 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/SSLSocketConnection.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17612 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/SSLSocketInitiator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7919 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/SSLSocketInitiator.h
+-rw-r--r--   0 runner    (1001) docker     (127)    46590 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/Session.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12406 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/Session.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10939 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/SessionFactory.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/SessionFactory.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/SessionID.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/SessionSettings.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12106 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/SessionSettings.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/SessionState.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/Settings.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/Settings.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/SharedArray.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/SocketAcceptor.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/SocketAcceptor.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5900 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/SocketConnection.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/SocketConnection.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/SocketConnector.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/SocketConnector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/SocketInitiator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/SocketInitiator.h
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/SocketMonitor.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/SocketMonitor_UNIX.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/SocketMonitor_UNIX.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6393 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/SocketMonitor_WIN32.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/SocketMonitor_WIN32.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/SocketServer.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/SocketServer.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14450 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/ThreadedSSLSocketAcceptor.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/ThreadedSSLSocketAcceptor.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/ThreadedSSLSocketConnection.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/ThreadedSSLSocketConnection.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13186 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/ThreadedSSLSocketInitiator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/ThreadedSSLSocketInitiator.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/ThreadedSocketAcceptor.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/ThreadedSocketAcceptor.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/ThreadedSocketConnection.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/ThreadedSocketConnection.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6085 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/ThreadedSocketInitiator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/ThreadedSocketInitiator.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/TimeRange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8179 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/TimeRange.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14921 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/Utility.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7186 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/Utility.h
+-rw-r--r--   0 runner    (1001) docker     (127)    44224 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/UtilitySSL.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11104 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/UtilitySSL.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/Values.h
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/config-all.h
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/config_unix.h
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/config_windows.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22917 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/dirent_windows.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:48:49.015977 quickfix_py-0.0.2/C++/double-conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)    27312 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/double-conversion/bignum-dtoa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/double-conversion/bignum-dtoa.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23111 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/double-conversion/bignum.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/double-conversion/bignum.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/double-conversion/cached-powers.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/double-conversion/cached-powers.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/double-conversion/diy-fp.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/double-conversion/diy-fp.h
+-rw-r--r--   0 runner    (1001) docker     (127)    32649 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/double-conversion/double-conversion.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    26509 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/double-conversion/double-conversion.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31124 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/double-conversion/fast-dtoa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/double-conversion/fast-dtoa.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15102 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/double-conversion/fixed-dtoa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/double-conversion/fixed-dtoa.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13526 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/double-conversion/ieee.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21057 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/double-conversion/strtod.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/double-conversion/strtod.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12363 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/double-conversion/utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/index.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/pugiconfig.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)   277537 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/pugixml.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    47424 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/pugixml.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/scope_guard.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/stdafx.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/stdafx.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7991 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/stdint_msvc.h
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/strptime.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:48:49.015977 quickfix_py-0.0.2/C++/swig/
+-rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/swig/MySQLStubs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/swig/PostgreSQLStubs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/swig/SSLStubs.h
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/C++/swig/Utility.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-04-16 07:48:49.023977 quickfix_py-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)  1833879 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/quickfix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/quickfix40.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/quickfix41.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21580 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/quickfix42.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64741 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/quickfix43.py
+-rw-r--r--   0 runner    (1001) docker     (127)   262984 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/quickfix44.py
+-rw-r--r--   0 runner    (1001) docker     (127)   381100 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/quickfix50.py
+-rw-r--r--   0 runner    (1001) docker     (127)   450461 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/quickfix50sp1.py
+-rw-r--r--   0 runner    (1001) docker     (127)  8975693 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/quickfix50sp2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:48:49.023977 quickfix_py-0.0.2/quickfix_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-04-16 07:48:48.000000 quickfix_py-0.0.2/quickfix_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-16 07:48:48.000000 quickfix_py-0.0.2/quickfix_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 07:48:48.000000 quickfix_py-0.0.2/quickfix_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-16 07:48:48.000000 quickfix_py-0.0.2/quickfix_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/quickfixt11.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 07:48:49.023977 quickfix_py-0.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3307 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:48:49.023977 quickfix_py-0.0.2/spec/
+-rw-r--r--   0 runner    (1001) docker     (127)    37257 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/spec/FIX40.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    57978 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/spec/FIX41.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   129260 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/spec/FIX42.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   204358 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/spec/FIX43.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   315395 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/spec/FIX44.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   393213 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/spec/FIX50.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   464464 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/spec/FIX50SP1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  1471310 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/spec/FIX50SP2.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    11927 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/spec/FIXT11.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/test_std_shared_ptr.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-16 07:48:45.000000 quickfix_py-0.0.2/test_std_tr1_shared_ptr.cpp
```

### Comparing `quickfix-py-0.0.1/C++/Acceptor.cpp` & `quickfix_py-0.0.2/C++/Acceptor.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/Acceptor.h` & `quickfix_py-0.0.2/C++/Acceptor.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/Application.h` & `quickfix_py-0.0.2/C++/Application.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/DOMDocument.h` & `quickfix_py-0.0.2/C++/DOMDocument.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/DataDictionary.cpp` & `quickfix_py-0.0.2/C++/DataDictionary.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/DataDictionary.h` & `quickfix_py-0.0.2/C++/DataDictionary.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/DataDictionaryProvider.cpp` & `quickfix_py-0.0.2/C++/DataDictionaryProvider.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/DataDictionaryProvider.h` & `quickfix_py-0.0.2/C++/DataDictionaryProvider.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/DatabaseConnectionID.h` & `quickfix_py-0.0.2/C++/DatabaseConnectionID.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/DatabaseConnectionPool.h` & `quickfix_py-0.0.2/C++/DatabaseConnectionPool.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/Dictionary.cpp` & `quickfix_py-0.0.2/C++/Dictionary.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/Dictionary.h` & `quickfix_py-0.0.2/C++/Dictionary.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/Event.h` & `quickfix_py-0.0.2/C++/Event.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/Except.h` & `quickfix_py-0.0.2/C++/Except.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/Exceptions.h` & `quickfix_py-0.0.2/C++/Exceptions.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/Field.h` & `quickfix_py-0.0.2/C++/Field.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/FieldConvertors.cpp` & `quickfix_py-0.0.2/C++/FieldConvertors.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/FieldConvertors.h` & `quickfix_py-0.0.2/C++/FieldConvertors.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/FieldMap.cpp` & `quickfix_py-0.0.2/C++/FieldMap.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/FieldMap.h` & `quickfix_py-0.0.2/C++/FieldMap.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/FieldNumbers.h` & `quickfix_py-0.0.2/C++/FieldNumbers.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/FieldTypes.cpp` & `quickfix_py-0.0.2/C++/FieldTypes.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/FieldTypes.h` & `quickfix_py-0.0.2/C++/FieldTypes.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/Fields.h` & `quickfix_py-0.0.2/C++/Fields.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/FileLog.cpp` & `quickfix_py-0.0.2/C++/FileLog.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/FileLog.h` & `quickfix_py-0.0.2/C++/FileLog.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/FileStore.cpp` & `quickfix_py-0.0.2/C++/FileStore.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/FileStore.h` & `quickfix_py-0.0.2/C++/FileStore.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/FixFieldNumbers.h` & `quickfix_py-0.0.2/C++/FixFieldNumbers.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/FixFields.h` & `quickfix_py-0.0.2/C++/FixFields.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/FixValues.h` & `quickfix_py-0.0.2/C++/FixValues.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/Group.cpp` & `quickfix_py-0.0.2/C++/Group.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/Group.h` & `quickfix_py-0.0.2/C++/Group.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/HostDetailsProvider.cpp` & `quickfix_py-0.0.2/C++/HostDetailsProvider.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/HostDetailsProvider.h` & `quickfix_py-0.0.2/C++/HostDetailsProvider.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/HtmlBuilder.h` & `quickfix_py-0.0.2/C++/HtmlBuilder.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/HttpConnection.cpp` & `quickfix_py-0.0.2/C++/HttpConnection.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/HttpConnection.h` & `quickfix_py-0.0.2/C++/HttpConnection.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/HttpMessage.cpp` & `quickfix_py-0.0.2/C++/HttpMessage.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/HttpMessage.h` & `quickfix_py-0.0.2/C++/HttpMessage.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/HttpParser.cpp` & `quickfix_py-0.0.2/C++/HttpParser.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/HttpParser.h` & `quickfix_py-0.0.2/C++/HttpParser.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/HttpServer.cpp` & `quickfix_py-0.0.2/C++/HttpServer.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/HttpServer.h` & `quickfix_py-0.0.2/C++/HttpServer.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/Initiator.cpp` & `quickfix_py-0.0.2/C++/Initiator.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/Initiator.h` & `quickfix_py-0.0.2/C++/Initiator.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/Log.cpp` & `quickfix_py-0.0.2/C++/Log.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/Log.h` & `quickfix_py-0.0.2/C++/Log.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/Message.cpp` & `quickfix_py-0.0.2/C++/Message.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/Message.h` & `quickfix_py-0.0.2/C++/Message.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/MessageCracker.h` & `quickfix_py-0.0.2/C++/MessageCracker.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/MessageSorters.cpp` & `quickfix_py-0.0.2/C++/MessageSorters.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/MessageSorters.h` & `quickfix_py-0.0.2/C++/MessageSorters.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/MessageStore.cpp` & `quickfix_py-0.0.2/C++/MessageStore.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/MessageStore.h` & `quickfix_py-0.0.2/C++/MessageStore.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/Mutex.h` & `quickfix_py-0.0.2/C++/Mutex.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/MySQLConnection.h` & `quickfix_py-0.0.2/C++/MySQLConnection.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/MySQLLog.cpp` & `quickfix_py-0.0.2/C++/MySQLLog.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/MySQLLog.h` & `quickfix_py-0.0.2/C++/MySQLLog.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/MySQLStore.cpp` & `quickfix_py-0.0.2/C++/MySQLStore.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/MySQLStore.h` & `quickfix_py-0.0.2/C++/MySQLStore.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/NullStore.cpp` & `quickfix_py-0.0.2/C++/NullStore.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/NullStore.h` & `quickfix_py-0.0.2/C++/NullStore.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/OdbcConnection.h` & `quickfix_py-0.0.2/C++/OdbcConnection.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/OdbcLog.cpp` & `quickfix_py-0.0.2/C++/OdbcLog.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/OdbcLog.h` & `quickfix_py-0.0.2/C++/OdbcLog.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/OdbcStore.cpp` & `quickfix_py-0.0.2/C++/OdbcStore.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/OdbcStore.h` & `quickfix_py-0.0.2/C++/OdbcStore.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/PUGIXML_DOMDocument.cpp` & `quickfix_py-0.0.2/C++/PUGIXML_DOMDocument.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/PUGIXML_DOMDocument.h` & `quickfix_py-0.0.2/C++/PUGIXML_DOMDocument.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/Parser.cpp` & `quickfix_py-0.0.2/C++/Parser.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/Parser.h` & `quickfix_py-0.0.2/C++/Parser.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/PostgreSQLConnection.h` & `quickfix_py-0.0.2/C++/PostgreSQLConnection.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/PostgreSQLLog.cpp` & `quickfix_py-0.0.2/C++/PostgreSQLLog.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/PostgreSQLLog.h` & `quickfix_py-0.0.2/C++/PostgreSQLLog.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/PostgreSQLStore.cpp` & `quickfix_py-0.0.2/C++/PostgreSQLStore.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/PostgreSQLStore.h` & `quickfix_py-0.0.2/C++/PostgreSQLStore.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/Queue.h` & `quickfix_py-0.0.2/C++/Queue.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/QuickfixPython.cpp` & `quickfix_py-0.0.2/C++/QuickfixPython.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/QuickfixPython.h` & `quickfix_py-0.0.2/C++/QuickfixPython.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/Responder.h` & `quickfix_py-0.0.2/C++/Responder.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/SSLSocketAcceptor.cpp` & `quickfix_py-0.0.2/C++/SSLSocketAcceptor.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/SSLSocketAcceptor.h` & `quickfix_py-0.0.2/C++/SSLSocketAcceptor.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/SSLSocketConnection.cpp` & `quickfix_py-0.0.2/C++/SSLSocketConnection.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/SSLSocketConnection.h` & `quickfix_py-0.0.2/C++/SSLSocketConnection.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/SSLSocketInitiator.cpp` & `quickfix_py-0.0.2/C++/SSLSocketInitiator.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/SSLSocketInitiator.h` & `quickfix_py-0.0.2/C++/SSLSocketInitiator.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/Session.cpp` & `quickfix_py-0.0.2/C++/Session.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/Session.h` & `quickfix_py-0.0.2/C++/Session.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/SessionFactory.cpp` & `quickfix_py-0.0.2/C++/SessionFactory.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/SessionFactory.h` & `quickfix_py-0.0.2/C++/SessionFactory.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/SessionID.h` & `quickfix_py-0.0.2/C++/SessionID.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/SessionSettings.cpp` & `quickfix_py-0.0.2/C++/SessionSettings.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/SessionSettings.h` & `quickfix_py-0.0.2/C++/SessionSettings.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/SessionState.h` & `quickfix_py-0.0.2/C++/SessionState.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/Settings.cpp` & `quickfix_py-0.0.2/C++/Settings.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/Settings.h` & `quickfix_py-0.0.2/C++/Settings.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/SharedArray.h` & `quickfix_py-0.0.2/C++/SharedArray.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/SocketAcceptor.cpp` & `quickfix_py-0.0.2/C++/SocketAcceptor.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/SocketAcceptor.h` & `quickfix_py-0.0.2/C++/SocketAcceptor.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/SocketConnection.cpp` & `quickfix_py-0.0.2/C++/SocketConnection.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/SocketConnection.h` & `quickfix_py-0.0.2/C++/SocketConnection.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/SocketConnector.cpp` & `quickfix_py-0.0.2/C++/SocketConnector.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/SocketConnector.h` & `quickfix_py-0.0.2/C++/SocketConnector.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/SocketInitiator.cpp` & `quickfix_py-0.0.2/C++/SocketInitiator.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/SocketInitiator.h` & `quickfix_py-0.0.2/C++/SocketInitiator.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/SocketMonitor.h` & `quickfix_py-0.0.2/C++/SocketMonitor.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/SocketMonitor_UNIX.cpp` & `quickfix_py-0.0.2/C++/SocketMonitor_UNIX.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/SocketMonitor_UNIX.h` & `quickfix_py-0.0.2/C++/SocketMonitor_UNIX.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/SocketMonitor_WIN32.cpp` & `quickfix_py-0.0.2/C++/SocketMonitor_WIN32.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/SocketMonitor_WIN32.h` & `quickfix_py-0.0.2/C++/SocketMonitor_WIN32.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/SocketServer.cpp` & `quickfix_py-0.0.2/C++/SocketServer.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/SocketServer.h` & `quickfix_py-0.0.2/C++/SocketServer.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/ThreadedSSLSocketAcceptor.cpp` & `quickfix_py-0.0.2/C++/ThreadedSSLSocketAcceptor.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/ThreadedSSLSocketAcceptor.h` & `quickfix_py-0.0.2/C++/ThreadedSSLSocketAcceptor.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/ThreadedSSLSocketConnection.cpp` & `quickfix_py-0.0.2/C++/ThreadedSSLSocketConnection.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/ThreadedSSLSocketConnection.h` & `quickfix_py-0.0.2/C++/ThreadedSSLSocketConnection.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/ThreadedSSLSocketInitiator.cpp` & `quickfix_py-0.0.2/C++/ThreadedSSLSocketInitiator.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/ThreadedSSLSocketInitiator.h` & `quickfix_py-0.0.2/C++/ThreadedSSLSocketInitiator.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/ThreadedSocketAcceptor.cpp` & `quickfix_py-0.0.2/C++/ThreadedSocketAcceptor.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/ThreadedSocketAcceptor.h` & `quickfix_py-0.0.2/C++/ThreadedSocketAcceptor.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/ThreadedSocketConnection.cpp` & `quickfix_py-0.0.2/C++/ThreadedSocketConnection.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/ThreadedSocketConnection.h` & `quickfix_py-0.0.2/C++/ThreadedSocketConnection.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/ThreadedSocketInitiator.cpp` & `quickfix_py-0.0.2/C++/ThreadedSocketInitiator.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/ThreadedSocketInitiator.h` & `quickfix_py-0.0.2/C++/ThreadedSocketInitiator.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/TimeRange.cpp` & `quickfix_py-0.0.2/C++/TimeRange.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/TimeRange.h` & `quickfix_py-0.0.2/C++/TimeRange.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/Utility.cpp` & `quickfix_py-0.0.2/C++/Utility.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/Utility.h` & `quickfix_py-0.0.2/C++/Utility.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/UtilitySSL.cpp` & `quickfix_py-0.0.2/C++/UtilitySSL.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1411,35 +1411,27 @@
   {
     errStr.assign("Unable to determine list of available CA certificates "
                   "for client authentication");
     return false;
   }
   SSL_CTX_set_client_CA_list(ctx, caList);
 
-  if (server)
-  {
-    if (settings.get().has(CERTIFICATE_VERIFY_LEVEL))
-      verifyLevel = (settings.get().getInt(CERTIFICATE_VERIFY_LEVEL));
-
-    if (verifyLevel != SSL_CLIENT_VERIFY_NOTSET)
-    {
-      /* configure new state */
-      int cVerify = SSL_VERIFY_NONE;
-      if (verifyLevel == SSL_CLIENT_VERIFY_REQUIRE)
-        cVerify |= SSL_VERIFY_PEER | SSL_VERIFY_FAIL_IF_NO_PEER_CERT;
-      else if (verifyLevel == SSL_CLIENT_VERIFY_OPTIONAL)
-        cVerify |= SSL_VERIFY_PEER;
+  if (settings.get().has(CERTIFICATE_VERIFY_LEVEL))
+    verifyLevel = (settings.get().getInt(CERTIFICATE_VERIFY_LEVEL));
 
-      SSL_CTX_set_verify(ctx, cVerify, callbackVerify);
-    }
-  }
-  else
+  if (verifyLevel != SSL_CLIENT_VERIFY_NOTSET)
   {
-    /* Set the certificate verification callback */
-    SSL_CTX_set_verify(ctx, SSL_VERIFY_PEER, callbackVerify);
+    /* configure new state */
+    int cVerify = SSL_VERIFY_NONE;
+    if (verifyLevel == SSL_CLIENT_VERIFY_REQUIRE)
+      cVerify |= SSL_VERIFY_PEER | SSL_VERIFY_FAIL_IF_NO_PEER_CERT;
+    else if (verifyLevel == SSL_CLIENT_VERIFY_OPTIONAL)
+      cVerify |= SSL_VERIFY_PEER;
+
+    SSL_CTX_set_verify(ctx, cVerify, callbackVerify);
   }
 
   return true;
 }
 
 X509_STORE *loadCRLInfo(SSL_CTX *ctx, const SessionSettings &settings, Log *log,
                         std::string &errStr)
```

### Comparing `quickfix-py-0.0.1/C++/UtilitySSL.h` & `quickfix_py-0.0.2/C++/UtilitySSL.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/Values.h` & `quickfix_py-0.0.2/C++/Values.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/config_unix.h` & `quickfix_py-0.0.2/C++/config_unix.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/dirent_windows.h` & `quickfix_py-0.0.2/C++/dirent_windows.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/double-conversion/bignum-dtoa.cc` & `quickfix_py-0.0.2/C++/double-conversion/bignum-dtoa.cc`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/double-conversion/bignum-dtoa.h` & `quickfix_py-0.0.2/C++/double-conversion/bignum-dtoa.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/double-conversion/bignum.cc` & `quickfix_py-0.0.2/C++/double-conversion/bignum.cc`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/double-conversion/bignum.h` & `quickfix_py-0.0.2/C++/double-conversion/bignum.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/double-conversion/cached-powers.cc` & `quickfix_py-0.0.2/C++/double-conversion/cached-powers.cc`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/double-conversion/cached-powers.h` & `quickfix_py-0.0.2/C++/double-conversion/cached-powers.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/double-conversion/diy-fp.cc` & `quickfix_py-0.0.2/C++/double-conversion/diy-fp.cc`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/double-conversion/diy-fp.h` & `quickfix_py-0.0.2/C++/double-conversion/diy-fp.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/double-conversion/double-conversion.cc` & `quickfix_py-0.0.2/C++/double-conversion/double-conversion.cc`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/double-conversion/double-conversion.h` & `quickfix_py-0.0.2/C++/double-conversion/double-conversion.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/double-conversion/fast-dtoa.cc` & `quickfix_py-0.0.2/C++/double-conversion/fast-dtoa.cc`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/double-conversion/fast-dtoa.h` & `quickfix_py-0.0.2/C++/double-conversion/fast-dtoa.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/double-conversion/fixed-dtoa.cc` & `quickfix_py-0.0.2/C++/double-conversion/fixed-dtoa.cc`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/double-conversion/fixed-dtoa.h` & `quickfix_py-0.0.2/C++/double-conversion/fixed-dtoa.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/double-conversion/ieee.h` & `quickfix_py-0.0.2/C++/double-conversion/ieee.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/double-conversion/strtod.cc` & `quickfix_py-0.0.2/C++/double-conversion/strtod.cc`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/double-conversion/strtod.h` & `quickfix_py-0.0.2/C++/double-conversion/strtod.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/double-conversion/utils.h` & `quickfix_py-0.0.2/C++/double-conversion/utils.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/index.h` & `quickfix_py-0.0.2/C++/index.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/pugiconfig.hpp` & `quickfix_py-0.0.2/C++/pugiconfig.hpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/pugixml.cpp` & `quickfix_py-0.0.2/C++/pugixml.cpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/pugixml.hpp` & `quickfix_py-0.0.2/C++/pugixml.hpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/scope_guard.hpp` & `quickfix_py-0.0.2/C++/scope_guard.hpp`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/stdafx.h` & `quickfix_py-0.0.2/C++/stdafx.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/stdint_msvc.h` & `quickfix_py-0.0.2/C++/stdint_msvc.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/swig/MySQLStubs.h` & `quickfix_py-0.0.2/C++/swig/MySQLStubs.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/swig/PostgreSQLStubs.h` & `quickfix_py-0.0.2/C++/swig/PostgreSQLStubs.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/C++/swig/SSLStubs.h` & `quickfix_py-0.0.2/C++/swig/SSLStubs.h`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/LICENSE` & `quickfix_py-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/PKG-INFO` & `quickfix_py-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickfix-py
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python package for Quickfix C++, FIX (Financial Information eXchange) protocol implementation
 Home-page: https://github.com/pablodcar/quickfix-py-package
 Download-URL: https://github.com/pablodcar/quickfix-py-package
 Author-email: pablodcar@gmail.com
 Maintainer: Pablo Carballo
 Maintainer-email: pablodcar@gmail.com
 License: The QuickFIX Software License, Version 1.0
@@ -50,8 +50,12 @@
         ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT
         OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF
         SUCH DAMAGE.
         
         
 Requires-Python: >=3.11
+Description-Content-Type: text/markdown
 License-File: LICENSE
+
+
+# Python bindings for Quickfix
```

### Comparing `quickfix-py-0.0.1/quickfix.py` & `quickfix_py-0.0.2/quickfix.py`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/quickfix40.py` & `quickfix_py-0.0.2/quickfix40.py`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/quickfix41.py` & `quickfix_py-0.0.2/quickfix41.py`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/quickfix42.py` & `quickfix_py-0.0.2/quickfix42.py`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/quickfix43.py` & `quickfix_py-0.0.2/quickfix43.py`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/quickfix44.py` & `quickfix_py-0.0.2/quickfix44.py`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/quickfix50.py` & `quickfix_py-0.0.2/quickfix50.py`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/quickfix50sp1.py` & `quickfix_py-0.0.2/quickfix50sp1.py`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/quickfix50sp2.py` & `quickfix_py-0.0.2/quickfix50sp2.py`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/quickfix_py.egg-info/PKG-INFO` & `quickfix_py-0.0.2/quickfix_py.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickfix-py
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python package for Quickfix C++, FIX (Financial Information eXchange) protocol implementation
 Home-page: https://github.com/pablodcar/quickfix-py-package
 Download-URL: https://github.com/pablodcar/quickfix-py-package
 Author-email: pablodcar@gmail.com
 Maintainer: Pablo Carballo
 Maintainer-email: pablodcar@gmail.com
 License: The QuickFIX Software License, Version 1.0
@@ -50,8 +50,12 @@
         ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT
         OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF
         SUCH DAMAGE.
         
         
 Requires-Python: >=3.11
+Description-Content-Type: text/markdown
 License-File: LICENSE
+
+
+# Python bindings for Quickfix
```

### Comparing `quickfix-py-0.0.1/quickfix_py.egg-info/SOURCES.txt` & `quickfix_py-0.0.2/quickfix_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/quickfixt11.py` & `quickfix_py-0.0.2/quickfixt11.py`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/setup.py` & `quickfix_py-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 import glob
+import subprocess
 import sys
 from distutils.command.build_ext import build_ext
 from distutils.core import Extension, setup
-import subprocess
 
 
 class build_ext_subclass(build_ext):
     def build_extensions(self):
         self.compiler.define_macro("PYTHON_MAJOR_VERSION", sys.version_info[0])
         print("Testing for std::tr1::shared_ptr...")
         try:
@@ -58,22 +58,22 @@
     "-IC++/swig",
     "-DHAVE_SSL=1",
 ]
 
 ldflags = subprocess.getoutput("pkg-config --libs openssl").strip().split()
 extra_link_args = ldflags
 
-if sys.platform == 'linux': # TODO: execute command  to get openssl 
+if sys.platform == "linux":  # TODO: execute command  to get openssl
     extra_compile_args.append("-I/usr/include/openssl")
 else:
     extra_compile_args.append("-I/opt/homebrew/opt/openssl@3/include")
 
 setup(
     name="quickfix-py",
-    version="0.0.1",
+    version="0.0.2",
     python_requires=">=3.11",
     py_modules=[
         "quickfix",
         "quickfixt11",
         "quickfix40",
         "quickfix41",
         "quickfix42",
@@ -86,14 +86,16 @@
     data_files=[("share/quickfix", glob.glob("spec/FIX*.xml"))],
     author_email="pablodcar@gmail.com",
     maintainer="Pablo Carballo",
     maintainer_email="pablodcar@gmail.com",
     description="Python package for Quickfix C++, FIX (Financial Information eXchange) protocol implementation",
     url="https://github.com/pablodcar/quickfix-py-package",
     download_url="https://github.com/pablodcar/quickfix-py-package",
+    long_description=open("README.md").read(),
+    long_description_content_type="text/markdown",
     license=license,
     cmdclass={"build_ext": build_ext_subclass},
     ext_modules=[
         Extension(
             "_quickfix",
             glob.glob("C++/*.cpp"),
             include_dirs=["C++"],
```

### Comparing `quickfix-py-0.0.1/spec/FIX40.xml` & `quickfix_py-0.0.2/spec/FIX40.xml`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/spec/FIX41.xml` & `quickfix_py-0.0.2/spec/FIX41.xml`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/spec/FIX42.xml` & `quickfix_py-0.0.2/spec/FIX42.xml`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/spec/FIX43.xml` & `quickfix_py-0.0.2/spec/FIX43.xml`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/spec/FIX44.xml` & `quickfix_py-0.0.2/spec/FIX44.xml`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/spec/FIX50.xml` & `quickfix_py-0.0.2/spec/FIX50.xml`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/spec/FIX50SP1.xml` & `quickfix_py-0.0.2/spec/FIX50SP1.xml`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/spec/FIX50SP2.xml` & `quickfix_py-0.0.2/spec/FIX50SP2.xml`

 * *Files identical despite different names*

### Comparing `quickfix-py-0.0.1/spec/FIXT11.xml` & `quickfix_py-0.0.2/spec/FIXT11.xml`

 * *Files identical despite different names*

