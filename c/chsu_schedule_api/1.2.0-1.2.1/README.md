# Comparing `tmp/chsu_schedule_api-1.2.0.tar.gz` & `tmp/chsu_schedule_api-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chsu_schedule_api-1.2.0.tar", max compression
+gzip compressed data, was "chsu_schedule_api-1.2.1.tar", max compression
```

## Comparing `chsu_schedule_api-1.2.0.tar` & `chsu_schedule_api-1.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      153 2024-04-03 17:16:51.794488 chsu_schedule_api-1.2.0/chsu_schedule_api/__init__.py
--rw-r--r--   0        0        0       86 2024-04-03 17:16:51.794488 chsu_schedule_api-1.2.0/chsu_schedule_api/api/__init__.py
--rw-r--r--   0        0        0     1082 2024-04-03 17:31:25.471419 chsu_schedule_api-1.2.0/chsu_schedule_api/api/abc.py
--rw-r--r--   0        0        0     5980 2024-04-03 19:13:25.257881 chsu_schedule_api-1.2.0/chsu_schedule_api/api/api.py
--rw-r--r--   0        0        0      116 2024-04-03 17:16:51.794488 chsu_schedule_api-1.2.0/chsu_schedule_api/client/__init__.py
--rw-r--r--   0        0        0     1071 2024-04-03 17:16:51.794488 chsu_schedule_api-1.2.0/chsu_schedule_api/client/abc.py
--rw-r--r--   0        0        0     2065 2024-04-03 17:16:51.794488 chsu_schedule_api-1.2.0/chsu_schedule_api/client/aiohttp.py
--rw-r--r--   0        0        0      298 2024-04-03 17:16:51.794488 chsu_schedule_api-1.2.0/chsu_schedule_api/constants.py
--rw-r--r--   0        0        0      116 2024-04-03 17:16:51.794488 chsu_schedule_api-1.2.0/chsu_schedule_api/enums.py
--rw-r--r--   0        0        0      326 2024-04-03 18:34:26.473939 chsu_schedule_api-1.2.0/chsu_schedule_api/errors.py
--rw-r--r--   0        0        0      882 2024-04-03 17:42:51.378097 chsu_schedule_api-1.2.0/chsu_schedule_api/models/__init__.py
--rw-r--r--   0        0        0      302 2024-04-03 17:16:51.794488 chsu_schedule_api-1.2.0/chsu_schedule_api/models/auditorium.py
--rw-r--r--   0        0        0      208 2024-04-03 17:16:51.794488 chsu_schedule_api-1.2.0/chsu_schedule_api/models/base.py
--rw-r--r--   0        0        0      106 2024-04-03 17:16:51.794488 chsu_schedule_api-1.2.0/chsu_schedule_api/models/building.py
--rw-r--r--   0        0        0      411 2024-04-03 17:16:51.799035 chsu_schedule_api-1.2.0/chsu_schedule_api/models/department.py
--rw-r--r--   0        0        0      108 2024-04-03 17:16:51.799035 chsu_schedule_api-1.2.0/chsu_schedule_api/models/discipline.py
--rw-r--r--   0        0        0      356 2024-04-03 17:16:51.799035 chsu_schedule_api-1.2.0/chsu_schedule_api/models/student_group.py
--rw-r--r--   0        0        0      332 2024-04-03 17:16:51.799035 chsu_schedule_api-1.2.0/chsu_schedule_api/models/teacher.py
--rw-r--r--   0        0        0     2977 2024-04-03 19:04:29.238962 chsu_schedule_api-1.2.0/chsu_schedule_api/models/timetable.py
--rw-r--r--   0        0        0     1093 2024-04-03 17:16:51.794488 chsu_schedule_api-1.2.0/LICENSE
--rw-r--r--   0        0        0     1378 2024-04-03 19:27:47.899358 chsu_schedule_api-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2293 2024-04-03 19:16:31.736270 chsu_schedule_api-1.2.0/README.md
--rw-r--r--   0        0        0     2844 1970-01-01 00:00:00.000000 chsu_schedule_api-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      153 2024-03-28 22:56:25.487494 chsu_schedule_api-1.2.1/chsu_schedule_api/__init__.py
+-rw-r--r--   0        0        0       86 2024-03-28 22:56:25.487494 chsu_schedule_api-1.2.1/chsu_schedule_api/api/__init__.py
+-rw-r--r--   0        0        0     1082 2024-04-16 12:26:44.074722 chsu_schedule_api-1.2.1/chsu_schedule_api/api/abc.py
+-rw-r--r--   0        0        0     5980 2024-04-16 12:26:44.074722 chsu_schedule_api-1.2.1/chsu_schedule_api/api/api.py
+-rw-r--r--   0        0        0      116 2024-03-28 22:56:25.488497 chsu_schedule_api-1.2.1/chsu_schedule_api/client/__init__.py
+-rw-r--r--   0        0        0     1071 2024-03-28 22:56:25.488497 chsu_schedule_api-1.2.1/chsu_schedule_api/client/abc.py
+-rw-r--r--   0        0        0     2065 2024-03-28 22:56:25.488497 chsu_schedule_api-1.2.1/chsu_schedule_api/client/aiohttp.py
+-rw-r--r--   0        0        0      298 2024-03-28 22:56:25.488497 chsu_schedule_api-1.2.1/chsu_schedule_api/constants.py
+-rw-r--r--   0        0        0      116 2024-03-28 22:56:25.488497 chsu_schedule_api-1.2.1/chsu_schedule_api/enums.py
+-rw-r--r--   0        0        0      326 2024-04-16 12:26:44.076195 chsu_schedule_api-1.2.1/chsu_schedule_api/errors.py
+-rw-r--r--   0        0        0      882 2024-04-16 12:26:44.076195 chsu_schedule_api-1.2.1/chsu_schedule_api/models/__init__.py
+-rw-r--r--   0        0        0      302 2024-03-28 22:56:25.490518 chsu_schedule_api-1.2.1/chsu_schedule_api/models/auditorium.py
+-rw-r--r--   0        0        0      208 2024-03-29 08:16:57.081988 chsu_schedule_api-1.2.1/chsu_schedule_api/models/base.py
+-rw-r--r--   0        0        0      106 2024-03-28 22:56:25.490997 chsu_schedule_api-1.2.1/chsu_schedule_api/models/building.py
+-rw-r--r--   0        0        0      411 2024-03-28 22:56:25.490997 chsu_schedule_api-1.2.1/chsu_schedule_api/models/department.py
+-rw-r--r--   0        0        0      108 2024-03-28 22:56:25.491524 chsu_schedule_api-1.2.1/chsu_schedule_api/models/discipline.py
+-rw-r--r--   0        0        0      356 2024-03-28 22:56:25.491524 chsu_schedule_api-1.2.1/chsu_schedule_api/models/student_group.py
+-rw-r--r--   0        0        0      332 2024-03-28 22:56:25.491524 chsu_schedule_api-1.2.1/chsu_schedule_api/models/teacher.py
+-rw-r--r--   0        0        0     2975 2024-04-16 12:36:49.734085 chsu_schedule_api-1.2.1/chsu_schedule_api/models/timetable.py
+-rw-r--r--   0        0        0     1093 2024-03-28 22:56:25.486469 chsu_schedule_api-1.2.1/LICENSE
+-rw-r--r--   0        0        0     1378 2024-04-16 12:40:58.517354 chsu_schedule_api-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2293 2024-04-16 12:26:44.073501 chsu_schedule_api-1.2.1/README.md
+-rw-r--r--   0        0        0     2844 1970-01-01 00:00:00.000000 chsu_schedule_api-1.2.1/PKG-INFO
```

### Comparing `chsu_schedule_api-1.2.0/chsu_schedule_api/api/abc.py` & `chsu_schedule_api-1.2.1/chsu_schedule_api/api/abc.py`

 * *Files identical despite different names*

### Comparing `chsu_schedule_api-1.2.0/chsu_schedule_api/api/api.py` & `chsu_schedule_api-1.2.1/chsu_schedule_api/api/api.py`

 * *Files identical despite different names*

### Comparing `chsu_schedule_api-1.2.0/chsu_schedule_api/client/abc.py` & `chsu_schedule_api-1.2.1/chsu_schedule_api/client/abc.py`

 * *Files identical despite different names*

### Comparing `chsu_schedule_api-1.2.0/chsu_schedule_api/client/aiohttp.py` & `chsu_schedule_api-1.2.1/chsu_schedule_api/client/aiohttp.py`

 * *Files identical despite different names*

### Comparing `chsu_schedule_api-1.2.0/chsu_schedule_api/models/__init__.py` & `chsu_schedule_api-1.2.1/chsu_schedule_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `chsu_schedule_api-1.2.0/chsu_schedule_api/models/timetable.py` & `chsu_schedule_api-1.2.1/chsu_schedule_api/models/timetable.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     def path(self) -> str:
         """Time table path"""
 
     def _dt_to_str(self) -> None:
         if isinstance(self.from_date, datetime):
             self.from_date = self.from_date.strftime("%d.%m.%Y")
         if isinstance(self.to_date, datetime):
-            self.from_date = self.to_date.strftime("%d.%m.%Y")
+            self.to_date = self.to_date.strftime("%d.%m.%Y")
 
 
 class TitleTimeTableType(CHSUModel):
     """
     Base model for time tables
     that require pre id definition
     """
```

### Comparing `chsu_schedule_api-1.2.0/LICENSE` & `chsu_schedule_api-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chsu_schedule_api-1.2.0/pyproject.toml` & `chsu_schedule_api-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chsu_schedule_api"
-version = "1.2.0"
+version = "1.2.1"
 description = "Asynchronous API wrapper for CHSU schedule API"
 authors = ["VoVcHiC <hello@chsutech.ru>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/vovchic17/CHSUScheduleAPI"
 repository = "https://github.com/vovchic17/CHSUScheduleAPI"
 keywords = ["chsu", "schedule", "api"]
```

### Comparing `chsu_schedule_api-1.2.0/README.md` & `chsu_schedule_api-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `chsu_schedule_api-1.2.0/PKG-INFO` & `chsu_schedule_api-1.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chsu_schedule_api
-Version: 1.2.0
+Version: 1.2.1
 Summary: Asynchronous API wrapper for CHSU schedule API
 Home-page: https://github.com/vovchic17/CHSUScheduleAPI
 License: MIT
 Keywords: chsu,schedule,api
 Author: VoVcHiC
 Author-email: hello@chsutech.ru
 Requires-Python: >=3.12,<4.0
```

