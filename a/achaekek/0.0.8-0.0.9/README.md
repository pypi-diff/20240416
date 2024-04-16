# Comparing `tmp/achaekek-0.0.8.tar.gz` & `tmp/achaekek-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "achaekek-0.0.8.tar", max compression
+gzip compressed data, was "achaekek-0.0.9.tar", max compression
```

## Comparing `achaekek-0.0.8.tar` & `achaekek-0.0.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       40 2024-02-21 17:40:51.693421 achaekek-0.0.8/README.md
--rw-r--r--   0        0        0       24 2024-02-21 17:40:51.693421 achaekek-0.0.8/achaekek/__init__.py
--rw-r--r--   0        0        0     6280 2024-02-22 00:31:14.020626 achaekek-0.0.8/achaekek/achaekek.py
--rw-r--r--   0        0        0     8854 2024-02-22 00:36:29.303289 achaekek-0.0.8/achaekek/request_types.py
--rw-r--r--   0        0        0      332 2024-04-16 19:30:22.656304 achaekek-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 achaekek-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       40 2024-02-21 17:40:51.693421 achaekek-0.0.9/README.md
+-rw-r--r--   0        0        0       24 2024-02-21 17:40:51.693421 achaekek-0.0.9/achaekek/__init__.py
+-rw-r--r--   0        0        0     6280 2024-02-22 00:31:14.020626 achaekek-0.0.9/achaekek/achaekek.py
+-rw-r--r--   0        0        0     8721 2024-04-16 19:56:26.220792 achaekek-0.0.9/achaekek/request_types.py
+-rw-r--r--   0        0        0      332 2024-04-16 19:56:43.301646 achaekek-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 achaekek-0.0.9/PKG-INFO
```

### Comparing `achaekek-0.0.8/achaekek/achaekek.py` & `achaekek-0.0.9/achaekek/achaekek.py`

 * *Files identical despite different names*

### Comparing `achaekek-0.0.8/achaekek/request_types.py` & `achaekek-0.0.9/achaekek/request_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,17 +72,18 @@
     answers: list[str]
     addAnswersMode: Literal["DISABLED", "ONLY_CREATORS", "ANYONE"]
     outcomeType: OutcomeType = field(default=OutcomeType.MULTIPLE_CHOICE)
     shouldAnswersSumToOne: bool = True
 
     def to_json(self):
         dictionary = super().to_json()
-        if "addAnswersMode" in dictionary:
-            dictionary["addAnswersMode"] = dictionary["addAnswersMode"].value
-        if "shouldAnswersSumToOne" in dictionary and dictionary["shouldAnswersSumToOne"]:
+        if (
+            "shouldAnswersSumToOne" in dictionary
+            and dictionary["shouldAnswersSumToOne"]
+        ):
             del dictionary["shouldAnswersSumToOne"]
         return dictionary
 
 
 @dataclass
 class CreatePollMarket(_CreateMarket):
     answers: list[str]
@@ -115,15 +116,14 @@
     contractId: str
     outcome: Literal["YES", "NO"] = field(default="YES")
     limitprob: float = None
     expiresAt: datetime = None
 
     def to_json(self):
         json = super.to_json()
-        json["outcome"] = json["outcome"].value
         if "limitprob" in json:
             json["limitprob"] = round(json["limitprob"], 2)
         if "expiresAt" in json:
             json["expiresAt"] = int(time.mktime(self.expiresAt.timetuple()) * 1000)
         return json
```

### Comparing `achaekek-0.0.8/PKG-INFO` & `achaekek-0.0.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: achaekek
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python library for the Manifold markets API.
 Author: TetraspaceW
 Author-email: holomanga@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

