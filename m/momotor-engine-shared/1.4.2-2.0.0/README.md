# Comparing `tmp/momotor-engine-shared-1.4.2.tar.gz` & `tmp/momotor_engine_shared-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "momotor-engine-shared-1.4.2.tar", last modified: Fri Jun 10 09:25:54 2022, max compression
+gzip compressed data, was "momotor_engine_shared-2.0.0.tar", last modified: Tue Apr 16 07:45:28 2024, max compression
```

## Comparing `momotor-engine-shared-1.4.2.tar` & `momotor_engine_shared-2.0.0.tar`

### file list

```diff
@@ -1,34 +1,63 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 09:25:54.000000 momotor-engine-shared-1.4.2/
--rw-r--r--   0 root         (0) root         (0)     1710 2022-06-10 09:25:54.000000 momotor-engine-shared-1.4.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      680 2022-06-10 09:25:36.000000 momotor-engine-shared-1.4.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2022-06-10 09:25:54.000000 momotor-engine-shared-1.4.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2103 2022-06-10 09:25:36.000000 momotor-engine-shared-1.4.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 09:25:54.000000 momotor-engine-shared-1.4.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 09:25:54.000000 momotor-engine-shared-1.4.2/src/momotor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 09:25:54.000000 momotor-engine-shared-1.4.2/src/momotor/shared/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-10 09:25:36.000000 momotor-engine-shared-1.4.2/src/momotor/shared/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      998 2022-06-10 09:25:36.000000 momotor-engine-shared-1.4.2/src/momotor/shared/doc.py
--rw-rw-rw-   0 root         (0) root         (0)      915 2022-06-10 09:25:36.000000 momotor-engine-shared-1.4.2/src/momotor/shared/exlock.py
--rw-rw-rw-   0 root         (0) root         (0)     4451 2022-06-10 09:25:36.000000 momotor-engine-shared-1.4.2/src/momotor/shared/lockset.py
--rw-rw-rw-   0 root         (0) root         (0)    11781 2022-06-10 09:25:36.000000 momotor-engine-shared-1.4.2/src/momotor/shared/log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 09:25:54.000000 momotor-engine-shared-1.4.2/src/momotor/shared/resources/
--rw-rw-rw-   0 root         (0) root         (0)     9403 2022-06-10 09:25:36.000000 momotor-engine-shared-1.4.2/src/momotor/shared/resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      670 2022-06-10 09:25:36.000000 momotor-engine-shared-1.4.2/src/momotor/shared/resources/const.py
--rw-rw-rw-   0 root         (0) root         (0)       80 2022-06-10 09:25:36.000000 momotor-engine-shared-1.4.2/src/momotor/shared/resources/exception.py
--rw-rw-rw-   0 root         (0) root         (0)     3220 2022-06-10 09:25:36.000000 momotor-engine-shared-1.4.2/src/momotor/shared/resources/group.py
--rw-rw-rw-   0 root         (0) root         (0)     6794 2022-06-10 09:25:36.000000 momotor-engine-shared-1.4.2/src/momotor/shared/resources/item.py
--rw-rw-rw-   0 root         (0) root         (0)      557 2022-06-10 09:25:36.000000 momotor-engine-shared-1.4.2/src/momotor/shared/resources/tag.py
--rw-rw-rw-   0 root         (0) root         (0)     1789 2022-06-10 09:25:36.000000 momotor-engine-shared-1.4.2/src/momotor/shared/resources/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 09:25:54.000000 momotor-engine-shared-1.4.2/src/momotor/shared/state/
--rw-rw-rw-   0 root         (0) root         (0)       91 2022-06-10 09:25:36.000000 momotor-engine-shared-1.4.2/src/momotor/shared/state/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1386 2022-06-10 09:25:36.000000 momotor-engine-shared-1.4.2/src/momotor/shared/state/base.py
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-06-10 09:25:36.000000 momotor-engine-shared-1.4.2/src/momotor/shared/state/exception.py
--rw-rw-rw-   0 root         (0) root         (0)     2126 2022-06-10 09:25:36.000000 momotor-engine-shared-1.4.2/src/momotor/shared/state/local.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-06-10 09:25:15.000000 momotor-engine-shared-1.4.2/src/momotor/shared/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 09:25:54.000000 momotor-engine-shared-1.4.2/src/momotor_engine_shared.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1710 2022-06-10 09:25:54.000000 momotor-engine-shared-1.4.2/src/momotor_engine_shared.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      894 2022-06-10 09:25:54.000000 momotor-engine-shared-1.4.2/src/momotor_engine_shared.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-10 09:25:54.000000 momotor-engine-shared-1.4.2/src/momotor_engine_shared.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-10 09:25:54.000000 momotor-engine-shared-1.4.2/src/momotor_engine_shared.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      117 2022-06-10 09:25:54.000000 momotor-engine-shared-1.4.2/src/momotor_engine_shared.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-06-10 09:25:54.000000 momotor-engine-shared-1.4.2/src/momotor_engine_shared.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:45:28.000000 momotor_engine_shared-2.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     3247 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     3220 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/.gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:45:28.000000 momotor_engine_shared-2.0.0/.idea/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:45:28.000000 momotor_engine_shared-2.0.0/.idea/inspectionProfiles/
+-rw-rw-rw-   0 root         (0) root         (0)      174 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-rw-   0 root         (0) root         (0)      288 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/.idea/misc.xml
+-rw-rw-rw-   0 root         (0) root         (0)      294 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/.idea/modules.xml
+-rw-rw-rw-   0 root         (0) root         (0)      634 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/.idea/momotor.lib.engine-shared.iml
+-rw-rw-rw-   0 root         (0) root         (0)     9415 2024-04-16 07:45:23.000000 momotor_engine_shared-2.0.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     2492 2024-04-16 07:45:28.000000 momotor_engine_shared-2.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      680 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:45:28.000000 momotor_engine_shared-2.0.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      638 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      764 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:45:28.000000 momotor_engine_shared-2.0.0/docs/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:45:28.000000 momotor_engine_shared-2.0.0/docs/source/_static/
+-rw-rw-rw-   0 root         (0) root         (0)     6988 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/docs/source/_static/logo-text-negative.png
+-rw-rw-rw-   0 root         (0) root         (0)     6887 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/docs/source/_static/logo-text.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:45:28.000000 momotor_engine_shared-2.0.0/docs/source/_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      672 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/docs/source/_templates/projectlinks.html
+-rw-rw-rw-   0 root         (0) root         (0)     3508 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/docs/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      217 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/docs/source/doc.rst
+-rw-rw-rw-   0 root         (0) root         (0)      351 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/docs/source/exlock.rst
+-rw-rw-rw-   0 root         (0) root         (0)      459 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/docs/source/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      167 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/docs/source/log.rst
+-rw-rw-rw-   0 root         (0) root         (0)    12188 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/docs/source/resources.rst
+-rw-rw-rw-   0 root         (0) root         (0)      946 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/docs/source/state.rst
+-rw-rw-rw-   0 root         (0) root         (0)      436 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/publish-docs.sh
+-rw-rw-rw-   0 root         (0) root         (0)     2475 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      413 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/semver.sh
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 07:45:28.000000 momotor_engine_shared-2.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:45:28.000000 momotor_engine_shared-2.0.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:45:28.000000 momotor_engine_shared-2.0.0/src/momotor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:45:28.000000 momotor_engine_shared-2.0.0/src/momotor/shared/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/src/momotor/shared/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      998 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/src/momotor/shared/doc.py
+-rw-rw-rw-   0 root         (0) root         (0)      916 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/src/momotor/shared/exlock.py
+-rw-rw-rw-   0 root         (0) root         (0)     4494 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/src/momotor/shared/lockset.py
+-rw-rw-rw-   0 root         (0) root         (0)    11852 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/src/momotor/shared/log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:45:28.000000 momotor_engine_shared-2.0.0/src/momotor/shared/resources/
+-rw-rw-rw-   0 root         (0) root         (0)     9388 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/src/momotor/shared/resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      670 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/src/momotor/shared/resources/const.py
+-rw-rw-rw-   0 root         (0) root         (0)       80 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/src/momotor/shared/resources/exception.py
+-rw-rw-rw-   0 root         (0) root         (0)     3252 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/src/momotor/shared/resources/group.py
+-rw-rw-rw-   0 root         (0) root         (0)     6836 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/src/momotor/shared/resources/item.py
+-rw-rw-rw-   0 root         (0) root         (0)      557 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/src/momotor/shared/resources/tag.py
+-rw-rw-rw-   0 root         (0) root         (0)     1811 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/src/momotor/shared/resources/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:45:28.000000 momotor_engine_shared-2.0.0/src/momotor/shared/state/
+-rw-rw-rw-   0 root         (0) root         (0)       91 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/src/momotor/shared/state/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1386 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/src/momotor/shared/state/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/src/momotor/shared/state/exception.py
+-rw-rw-rw-   0 root         (0) root         (0)     2158 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/src/momotor/shared/state/local.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:45:28.000000 momotor_engine_shared-2.0.0/src/momotor_engine_shared.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2492 2024-04-16 07:45:28.000000 momotor_engine_shared-2.0.0/src/momotor_engine_shared.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1348 2024-04-16 07:45:28.000000 momotor_engine_shared-2.0.0/src/momotor_engine_shared.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 07:45:28.000000 momotor_engine_shared-2.0.0/src/momotor_engine_shared.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      332 2024-04-16 07:45:28.000000 momotor_engine_shared-2.0.0/src/momotor_engine_shared.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-16 07:45:28.000000 momotor_engine_shared-2.0.0/src/momotor_engine_shared.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:45:28.000000 momotor_engine_shared-2.0.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    14734 2024-04-16 07:44:53.000000 momotor_engine_shared-2.0.0/tests/test_resources.py
+-rw-rw-rw-   0 root         (0) root         (0)       37 2024-04-16 07:45:23.000000 momotor_engine_shared-2.0.0/version.toml
```

### Comparing `momotor-engine-shared-1.4.2/README.md` & `momotor_engine_shared-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `momotor-engine-shared-1.4.2/src/momotor/shared/doc.py` & `momotor_engine_shared-2.0.0/src/momotor/shared/doc.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-shared-1.4.2/src/momotor/shared/exlock.py` & `momotor_engine_shared-2.0.0/src/momotor/shared/exlock.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-import aiorwlock
+from __future__ import annotations
 
-import typing
+import aiorwlock
 
 
 class ExLock(aiorwlock.RWLock):
     """
     A subclass of `aiorwlock.RWLock <https://github.com/aio-libs/aiorwlock>`_
 
     An :py:class:`~momotor.shared.exlock.ExLock` maintains a pair of associated locks, one for read-only
     operations and one for writing. The read lock may be held simultaneously
     by multiple reader tasks, so long as there are no writers. The write
     lock is exclusive.
     """
 
     # noinspection PyProtectedMember
-    def get(self, exclusive: bool) -> typing.Union[aiorwlock._ReaderLock, aiorwlock._WriterLock]:
-        """ Get either the :py:attr:`reader` or :py:attr:`writer` lock, depending on the value of
-        ``exclusive``
+    def get(self, exclusive: bool) -> aiorwlock._ReaderLock | aiorwlock._WriterLock:
+        """ Get either the :py:attr:`.reader` or :py:attr:`.writer` lock, depending on the value of *exclusive*
 
-        :param exclusive: if ``False``, requests the :py:attr:`reader` lock, otherwise the :py:attr:`writer` lock
+        :param exclusive: if ``False``, requests the :py:attr:`.reader` lock, otherwise the :py:attr:`writer` lock
         :return: the requested lock
         """
         return self.writer if exclusive else self.reader
```

### Comparing `momotor-engine-shared-1.4.2/src/momotor/shared/lockset.py` & `momotor_engine_shared-2.0.0/src/momotor/shared/lockset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import collections.abc
 import inspect
 import logging
 import typing
 import weakref
 from abc import abstractmethod
 
 from momotor.shared.exlock import ExLock
@@ -56,15 +57,15 @@
         await self.acquire()
 
     async def __aexit__(self, *args) -> None:
         self.release()
 
 
 class LockSetBase(typing.Generic[KT, LT]):
-    __locks: typing.MutableMapping[KT, LT]
+    __locks: collections.abc.MutableMapping[KT, LT]
 
     def __init__(self, set_name: str):
         self.set_name = set_name
         self.__locks = weakref.WeakValueDictionary()
 
     @staticmethod
     def _get_caller_name(level=2):
@@ -80,15 +81,15 @@
         else:
             return f'{package}.{frame_info.function}'
 
     @abstractmethod
     def _new_lock(self) -> LT:
         ...
 
-    def _get_or_create(self, key: KT) -> typing.Tuple[LT, bool]:
+    def _get_or_create(self, key: KT) -> tuple[LT, bool]:
         lock = self.__locks.get(key)
         if lock:
             created = False
         else:
             self.__locks[key] = lock = self._new_lock()
             created = True
 
@@ -111,15 +112,15 @@
             await logger.debug(
                 f'{log_label} {"created" if created else "reusing"} lock'
             )
 
             return SetLock(lock, lock, True, log_label)
 
 
-ExclusiveType = typing.Union[bool, typing.Callable[[KT, bool], typing.Coroutine[None, None, bool]]]
+ExclusiveType = typing.Union[bool, collections.abc.Callable[[KT, bool], collections.abc.Coroutine[None, None, bool]]]
 
 
 class ExLockSet(LockSetBase[KT, ExLock], typing.Generic[KT]):
     def _new_lock(self) -> ExLock:
         return ExLock()
 
     async def get(self, key: KT, exclusive: ExclusiveType, *, caller_name: str = None, log_key: str = None) -> SetLock:
```

### Comparing `momotor-engine-shared-1.4.2/src/momotor/shared/log.py` & `momotor_engine_shared-2.0.0/src/momotor/shared/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,23 @@
+from __future__ import annotations
+
+from asyncio import wrap_future
+from concurrent.futures import ThreadPoolExecutor, Future
+from logging import getLogger, Logger, DEBUG, INFO, WARNING, ERROR, CRITICAL, raiseExceptions, LogRecord
+
+import collections.abc
 import sys
 import typing
 import warnings
-from asyncio import wrap_future
-from concurrent.futures import ThreadPoolExecutor, Future
 from contextlib import asynccontextmanager, contextmanager
-from logging import getLogger, Logger, DEBUG, INFO, WARNING, ERROR, CRITICAL, raiseExceptions, LogRecord
 
-from typing_extensions import TypeAlias
+try:
+    from typing import TypeAlias  # py3.10+
+except ImportError:
+    from typing_extensions import TypeAlias
 
 __all__ = ['AsyncLogWrapper', 'getAsyncLogger', 'async_log_exception', 'log_exception']
 
 DEFAULT_WAIT_FOR_COMPLETION = False
 _executor = ThreadPoolExecutor(max_workers=1)
 _last_future: typing.Optional[Future] = None
 
@@ -24,18 +31,18 @@
 
     :param logger: The Python logger to wrap
     :param wait_for_completion: If `True` all logging statements will only return when the line is written to the log.
                                 If `False` will queue the line to be logged and return immediately.
                                 If `None` (default) will wait if the level of the logger is DEBUG
     """
     # noinspection PyProtectedMember
-    def __init__(self, logger: Logger, *, wait_for_completion: typing.Optional[bool] = DEFAULT_WAIT_FOR_COMPLETION):
+    def __init__(self, logger: Logger, *, wait_for_completion: bool | None = DEFAULT_WAIT_FOR_COMPLETION):
         self._logger = logger
         self._sync_log = logger._log
-        self._wait_for_completion: typing.Optional[bool] = logger.isEnabledFor(DEBUG) \
+        self._wait_for_completion: bool | None = logger.isEnabledFor(DEBUG) \
             if wait_for_completion is None else wait_for_completion
 
     @property
     def name(self):
         """ Get the name of the logger """
         return self._logger.name
 
@@ -175,30 +182,30 @@
 
     @staticmethod
     async def flush():
         """ Wait until the last submitted logging statement has completed
         """
         global _last_future
 
-        fut: typing.Optional[Future] = _last_future
+        fut: Future | None = _last_future
         _last_future = None
         if fut:
             # noinspection PyBroadException
             try:
                 await wrap_future(fut)
             except:
                 pass
 
     @staticmethod
     def flush_sync():
         """ Wait until the last submitted logging statement has completed
         """
         global _last_future
 
-        fut: typing.Optional[Future] = _last_future
+        fut: Future | None = _last_future
         _last_future = None
         if fut is not None:
             # noinspection PyBroadException
             try:
                 fut.result()
             except:
                 pass
@@ -256,17 +263,15 @@
         # Wait until all async log messages have been processed
         self.flush_sync()
 
         return self._logger
 
 
 # noinspection PyPep8Naming
-def getAsyncLogger(name, *, wait_for_completion: typing.Optional[bool] = DEFAULT_WAIT_FOR_COMPLETION) \
-        -> AsyncLogWrapper:
-
+def getAsyncLogger(name, *, wait_for_completion: bool | None = DEFAULT_WAIT_FOR_COMPLETION) -> AsyncLogWrapper:
     """ Convenience function to create an asynchronous logger.
     Creates the logger by calling :py:func:`logging.getLogger` and wraps it with
     :py:class:`~momotor.shared.log.AsyncLogWrapper`
 
     :param name: name of the logger
     :param wait_for_completion: If `True` all logging statements will only return when the line is written to the log.
                                 If `False` will queue the line to be logged and return immediately.
@@ -280,21 +285,21 @@
         iter(x)
     except TypeError:
         return False
     else:
         return True
 
 
-ExceptionType: TypeAlias = typing.Type[Exception]
+ExceptionType: TypeAlias = type[Exception]
 
 
 @asynccontextmanager
 async def async_log_exception(async_logger: AsyncLogWrapper, msg: str, *args,
                               reraise: bool = False,
-                              ignore: typing.Union[ExceptionType, typing.Sequence[ExceptionType], None] = None):
+                              ignore: ExceptionType | collections.abc.Sequence[ExceptionType] | None = None):
     """ An async context manager that captures exceptions, logs them, and optionally re-raises them.
 
     :param async_logger: The async logger to log the exception to
     :param msg: A message to add to the exception
     :param args: Any optional arguments for the message
     :param reraise: If `True`, the exception will be re-raised after logging
     :param ignore: An exception class, or sequence of exception classes, to ignore.
@@ -311,15 +316,15 @@
         if reraise:
             raise
 
 
 @contextmanager
 def log_exception(logger: Logger, msg: str, *args,
                   reraise: bool = False,
-                  ignore: typing.Union[ExceptionType, typing.Sequence[ExceptionType], None] = None):
+                  ignore: typing.Union[ExceptionType, collections.abc.Sequence[ExceptionType], None] = None):
     """ A context manager that captures exceptions, logs them, and optionally re-raises them.
 
     :param logger: The logger to log the exception to
     :param msg: A message to add to the exception
     :param args: Any optional arguments for the message
     :param reraise: If `True`, the exception will be re-raised after logging
     :param ignore: An exception class, or sequence of exception classes, to ignore.
```

### Comparing `momotor-engine-shared-1.4.2/src/momotor/shared/resources/__init__.py` & `momotor_engine_shared-2.0.0/src/momotor/shared/resources/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,31 @@
+from __future__ import annotations
+
 import collections
+import collections.abc
 import itertools
-import typing
 
 from .const import STRONGEST, STRONG, NEUTRAL, WEAK, WEAKEST
 from .exception import NoMatch
 from .group import ResourceGroup
 from .item import ResourceItem
 from .utils import unique_everseen, quote_str
 
-__all__ = ['NoMatch', 'Resources', "ResourceGroup"]
-
+try:
+    from typing import Self  # py3.11+
+except ImportError:
+    from typing_extensions import Self
 
-RT = typing.TypeVar('RT', bound='Resources')
+__all__ = ['NoMatch', 'Resources', "ResourceGroup"]
 
 
-def split_resources(resources: str) -> typing.Generator[typing.Tuple[str, str], None, None]:
+def split_resources(resources: str) -> collections.abc.Generator[tuple[str, str], None, None]:
     """ Split a resources string into group-name, group-definition tuples
 
-    :param resources: One or more resource definitions (either multi-line or semi-colon separated),
+    :param resources: One or more resource definitions (either multi-line or semicolon separated),
                       including group names
     :raises :py:exc:`ValueError`: if the string is an invalid resources definition
     :return: A generator yielding group-name, group definition tuples
     """
     key = None
     current = ''
     whitespace = ''
@@ -84,15 +88,15 @@
             raise ValueError("unmatched quotes")
 
         assert key is None
         assert current == ''
         assert whitespace == ''
 
 
-def combine_group(left: typing.Optional[float], right: typing.Optional[float]) -> typing.Optional[float]:
+def combine_group(left: float | None, right: float | None) -> float | None:
     """ Combine group values
 
     Returns the **weakest** match, ie. the higher numeric value.
     If one value is ``None``, returns the other value.
     """
     if left is None:
         return right
@@ -121,40 +125,40 @@
     * blank cell: ignore, no change in match value
 
     TODO numeric items
 
     :param definition: A dictionary of group names to resource groups
 
     """
-    def __init__(self, definition: typing.Dict[str, ResourceGroup] = None):
+    def __init__(self, definition: dict[str, ResourceGroup] = None):
         self._definition = definition or {}
 
     # Factories
 
     @classmethod
-    def from_dict(cls: typing.Type[RT], definition: typing.Dict[str, typing.Union[str, typing.Iterable[str]]]) -> RT:
+    def from_dict(cls, definition: dict[str, str | collections.abc.Iterable[str]]) -> Self:
         """ Factory to create a :py:class:`~momotor.shared.resources.Resources` object from a dict
         of group names to group string definitions """
         return cls({
             key: ResourceGroup.create(value) for key, value in definition.items()
         })
 
     @classmethod
-    def from_key_value(cls: typing.Type[RT], key: str, value: typing.Union[str, typing.Iterable[str]]) -> RT:
+    def from_key_value(cls, key: str, value: str | collections.abc.Iterable[str]) -> Self:
         """ Factory to create a :py:class:`~momotor.shared.resources.Resources` object from a key and values
 
         :param key: Group name
         :param value: Group definition string or list of strings
         """
         return cls({
             key: ResourceGroup.create(value)
         })
 
     @classmethod
-    def from_string(cls: typing.Type[RT], value: typing.Union[str, typing.Iterable[str]]) -> RT:
+    def from_string(cls, value: str | collections.abc.Iterable[str]) -> Self:
         """ Factory to create a :py:class:`~momotor.shared.resources.Resources` object from
         one or more strings
 
         :param value: A string or iterable of strings containing resource definitions including a group name
         :return: The parsed resources
         :raises: :py:exc:`ValueError` if the string is an invalid resources definition
         """
@@ -167,15 +171,15 @@
                 resources.extend(split_resources(s))
 
         return cls.union(*(
             cls.from_key_value(key, value) for key, value in resources
         ))
 
     @classmethod
-    def union(cls: typing.Type[RT], *resources: RT) -> RT:
+    def union(cls, *resources: Self) -> Self:
         """ Merge multiple :py:class:`~momotor.shared.resources.Resources` objects into a new one
 
         :returns: The merged resources
         """
 
         return cls({
             key: ResourceGroup.union(*(resource.get(key) for resource in resources))
@@ -185,23 +189,23 @@
         })
 
     # Implementation
 
     def __len__(self):
         return len(self._definition)
 
-    def group_names(self) -> typing.List[str]:
+    def group_names(self) -> list[str]:
         """ Returns a list of group names
 
         :return: group names
         """
         return list(self._definition.keys())
 
     def get(self, key: str) -> ResourceGroup:
-        """ Get the :py:class:`~momotor.shared.resources.ResourceGroup` by name
+        """ Get the :py:class:`~momotor.shared.resources.group.ResourceGroup` by name
 
         :param key: Group name
         :return: The resource group matching the group name
         """
         return self._definition.get(key, ResourceGroup())
 
     def match(self, worker_resource: "Resources") -> float:
@@ -219,19 +223,19 @@
         group_names = set(self.group_names()) | set(worker_resource.group_names())
         for name in group_names:
             group_match = self.get(name).match(worker_resource.get(name))
             match = combine_group(match, NEUTRAL if group_match is None else group_match)
 
         return NEUTRAL if match is None else match
 
-    def as_tuples(self) -> typing.Iterable[typing.Tuple[str, typing.Tuple[str]]]:
+    def as_tuples(self) -> collections.abc.Iterable[tuple[str, tuple[str]]]:
         for key, group in self._definition.items():
             yield key, group.as_str_tuple()
 
-    def as_str_tuples(self) -> typing.Iterable[typing.Tuple[str, str]]:
+    def as_str_tuples(self) -> collections.abc.Iterable[tuple[str, str]]:
         for key, group in self._definition.items():
             yield key, group.as_str()
 
     def as_str(self, *, multiline: bool = False, compact: bool = False) -> str:
         """ Convert these resources into a string that can be parsed back into a
         :py:class:`~momotor.shared.resources.Resources` object using
         :py:meth:`~momotor.shared.resources.Resources.from_string`
```

### Comparing `momotor-engine-shared-1.4.2/src/momotor/shared/resources/const.py` & `momotor_engine_shared-2.0.0/src/momotor/shared/resources/const.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-shared-1.4.2/src/momotor/shared/resources/group.py` & `momotor_engine_shared-2.0.0/src/momotor/shared/resources/group.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,69 +1,73 @@
+from __future__ import annotations
+
+import collections.abc
 import itertools
 import typing
 
 from .exception import NoMatch
 from .item import ResourceItem
 from .utils import unique_everseen, quote_str, escape_str
 
+try:
+    from typing import Self  # py3.11+
+except ImportError:
+    from typing_extensions import Self
 
 UNSAFE_CHARS = {',', ':', ';', '"', "'"}
 
 
 def quote_item(item: str) -> str:
     if item.startswith(' ') or item.endswith(' ') or '\t' in item or '\n' in item:
         return quote_str(item)
 
     return escape_str(item, UNSAFE_CHARS)
 
 
-def combine_item(left: typing.Optional[float], right: typing.Optional[float]) -> typing.Optional[float]:
+def combine_item(left: float | None, right: float | None) -> float | None:
     """ Combine item values
 
     Returns the **strongest** match, ie. the lower numeric value.
     If one value is ``None``, returns the other value.
     """
     if left is None:
         return right
     elif right is None:
         return left
     else:
         return min(left, right)
 
 
-RGT = typing.TypeVar('RGT', bound='ResourceGroup')
-
-
 class ResourceGroup:
     """ A group of :py:class:`~momotor.shared.resources`.
     """
-    def __init__(self, items: typing.Iterable[ResourceItem] = None):
+    def __init__(self, items: collections.abc.Iterable[ResourceItem] = None):
         self._items = tuple(items) if items is not None else tuple()
 
     # Factories
 
     @classmethod
-    def create(cls: typing.Type[RGT], value: typing.Union[str, typing.Iterable[str]]) -> RGT:
+    def create(cls, value: str | collections.abc.Iterable[str]) -> Self:
         return cls(ResourceItem.create(value))
 
     @classmethod
-    def union(cls: typing.Type[RGT], *groups: RGT) -> RGT:
+    def union(cls, *groups: Self) -> Self:
         """ Merge multiple resource groups into a new one """
         return cls(unique_everseen(itertools.chain(*(group.items for group in groups))))
 
     # Implementation
 
     def __len__(self):
         return len(self._items)
 
     @property
-    def items(self) -> typing.Tuple[ResourceItem]:
+    def items(self) -> tuple[ResourceItem]:
         return self._items
 
-    def match(self, worker_group: typing.Optional["ResourceGroup"]) -> typing.Optional[float]:
+    def match(self, worker_group: typing.Optional["ResourceGroup"]) -> float | None:
         """ Returns the match between this resource group and the provided worker's resource group
 
         :param worker_group: The worker's resource group
         :return: match value, the lower the value, the better the match is (ranges from
                  -\ :py:data:`~math.inf` to +\ :py:data:`~math.inf`)
         :raises: :py:exc:`~momotor.shared.resources.NoMatch` if there are missing or excluded tags
         """
@@ -84,12 +88,12 @@
 
         # process resources defined on the worker but not the task
         for worker_resource in unmatched:
             match = combine_item(match, worker_resource.compare_missing(worker_resource))
 
         return match
 
-    def as_str_tuple(self) -> typing.Tuple[str]:
+    def as_str_tuple(self) -> tuple[str, ...]:
         return tuple(item.as_str() for item in self._items)
 
     def as_str(self) -> str:
         return ','.join(quote_item(item) for item in self.as_str_tuple())
```

### Comparing `momotor-engine-shared-1.4.2/src/momotor/shared/resources/item.py` & `momotor_engine_shared-2.0.0/src/momotor/shared/resources/item.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,28 @@
-import typing
+from __future__ import annotations
+
+import collections.abc
 
 from .const import STRONGEST, STRONG, WEAK, WEAKEST
 from .exception import NoMatch
 
+try:
+    from typing import Self  # py3.11+
+except ImportError:
+    from typing_extensions import Self
+
 PRIO_MAPPING = {
     (True, True): STRONGEST,
     (True, False): STRONG,
     (False, True): WEAK,
     (False, False): WEAKEST,
 }
 
 
-def split_items(items: str) -> typing.Generator[str, None, None]:
+def split_items(items: str) -> collections.abc.Generator[str, None, None]:
     current = ''  # Current value being collected
     whitespace = ''  # Whitespace that might or might not be part of the value
     quote = None  # None: not inside a quoted string, otherwise the quote itself
     escape = False  # True: include next character unconditionally
 
     for c in items+',':
         if escape:
@@ -59,47 +66,44 @@
         # Unterminated quoted string
         raise ValueError("unmatched quotes")
 
     assert current == ''
     assert whitespace == ''
 
 
-RIT = typing.TypeVar('RIT', bound='ResourceItem')
-
-
 class ResourceItem:
     def __init__(self, value: str, required: bool, excluded: bool):
         if required and excluded:
             raise ValueError('cannot combine required and excluded flags')
 
         self.value = value
         self.required = required
         self.excluded = excluded
 
     @classmethod
-    def _create_item(cls: typing.Type[RIT], value) -> RIT:
+    def _create_item(cls, value) -> Self:
         from .tag import Tag
         return Tag(value)
 
     @classmethod
-    def create(cls: typing.Type[RIT], value: typing.Union[str, typing.Iterable[str]]) -> typing.Iterable[RIT]:
+    def create(cls, value: str | collections.abc.Iterable[str]) -> collections.abc.Iterable[Self]:
         if isinstance(value, str):
             for item in split_items(value):
                 if item:
                     yield cls._create_item(item)
         else:
             for element in value:
                 for item in split_items(element):
                     if item:
                         yield cls._create_item(item)
 
-    def comparable(self, worker: RIT) -> bool:
-        return type(self) == type(worker)
+    def comparable(self, worker: Self) -> bool:
+        return type(self) is type(worker)
 
-    def compare(self, worker: RIT) -> typing.Optional[float]:
+    def compare(self, worker: Self) -> float | None:
         """
             +-----------+------------------------------------------------------+----------------------------------------------------+-----------------------------------------------+
             | . worker  | required                                             | optional                                           | excluded                                      |
             | task      |                                                      |                                                    |                                               |
             +-----------+------------------------------------------------------+----------------------------------------------------+-----------------------------------------------+
             | required  | :py:data:`~momotor.shared.resources.const.STRONGEST` | :py:data:`~momotor.shared.resources.const.STRONG`  | :py:class:`~momotor.shared.resources.NoMatch` |
             +-----------+------------------------------------------------------+----------------------------------------------------+-----------------------------------------------+
@@ -116,15 +120,15 @@
                     raise NoMatch
 
             return PRIO_MAPPING[(self.required, worker.required)]
 
         return None
 
     @classmethod
-    def compare_missing(cls: typing.Type[RIT], worker: RIT) -> typing.Optional[float]:
+    def compare_missing(cls, worker: Self) -> float | None:
         """
             +----------+-----------------------------------------------+----------------------------------------------------+------------------------------------------------+
             | . worker | required                                      | optional                                           | excluded                                       |
             | task     |                                               |                                                    |                                                |
             +----------+-----------------------------------------------+----------------------------------------------------+------------------------------------------------+
             | `-`      | :py:class:`~momotor.shared.resources.NoMatch` |                                                    |                                                |
             +----------+-----------------------------------------------+----------------------------------------------------+------------------------------------------------+
```

### Comparing `momotor-engine-shared-1.4.2/src/momotor/shared/resources/tag.py` & `momotor_engine_shared-2.0.0/src/momotor/shared/resources/tag.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-shared-1.4.2/src/momotor/shared/resources/utils.py` & `momotor_engine_shared-2.0.0/src/momotor/shared/resources/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from itertools import filterfalse
+from __future__ import annotations
+
 import re
-import typing
+from itertools import filterfalse
 
 
 def unique_everseen(iterable, key=None):
     # https://docs.python.org/3.7/library/itertools.html#itertools-recipes
     """List unique elements, preserving order. Remember all elements ever seen."""
     # unique_everseen('AAAABBBCCDAABBB') --> A B C D
     # unique_everseen('ABBCcAD', str.lower) --> A B C D
@@ -21,15 +22,15 @@
                 seen_add(k)
                 yield element
 
 
 SAFE_STR_RE = re.compile(r'\w+')
 
 
-def escape_str(s: str, escape_chars: typing.Set[str] = None) -> str:
+def escape_str(s: str, escape_chars: set[str] | None = None) -> str:
     """ Return string with characters in `escape_chars` escaped.
     Uses the backslash character for escapes, so that is always escaped and does not have to be supplied
     to `escape_chars`
     """
     escape_chars = {'\\'} | (escape_chars if escape_chars else set())
 
     result = ''
```

### Comparing `momotor-engine-shared-1.4.2/src/momotor/shared/state/base.py` & `momotor_engine_shared-2.0.0/src/momotor/shared/state/base.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+import typing
 from abc import ABC
 from contextlib import asynccontextmanager
-import typing
 
 
 class StateABC(ABC):
     """ Abstract base class to implement shared locks
     """
     @asynccontextmanager
     async def get_lock(self, key: str, *, exclusive: bool = True) -> typing.AsyncContextManager[None]:
```

### Comparing `momotor-engine-shared-1.4.2/src/momotor/shared/state/local.py` & `momotor_engine_shared-2.0.0/src/momotor/shared/state/local.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
-from contextlib import asynccontextmanager
+import collections.abc
 import typing
 import weakref
+from contextlib import asynccontextmanager
 
 from momotor.shared.exlock import ExLock
 from .base import StateABC
 from ..doc import annotate_docstring
 from ..log import getAsyncLogger
 
 logger = getAsyncLogger(__name__)
@@ -17,15 +18,15 @@
 
     Uses a :py:class:`~weakref.WeakValueDictionary` of :py:class:`momotor.shared.exlock.ExLock` objects.
 
     Produces debug logging information on the ``{logger.name}`` logger
     """
     def __init__(self):
         self.__dict_lock = asyncio.Lock()
-        self.__locks: typing.MutableMapping[str, ExLock] = weakref.WeakValueDictionary()
+        self.__locks: collections.abc.MutableMapping[str, ExLock] = weakref.WeakValueDictionary()
 
     async def _get_rwlock(self, key: str, create: bool):
         async with self.__dict_lock:
             lock = self.__locks.get(key)
             if lock is None and create:
                 lock = self.__locks[key] = ExLock()
```

