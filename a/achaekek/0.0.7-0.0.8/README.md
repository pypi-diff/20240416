# Comparing `tmp/achaekek-0.0.7.tar.gz` & `tmp/achaekek-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "achaekek-0.0.7.tar", max compression
+gzip compressed data, was "achaekek-0.0.8.tar", max compression
```

## Comparing `achaekek-0.0.7.tar` & `achaekek-0.0.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       40 2023-12-22 22:07:17.463779 achaekek-0.0.7/README.md
--rw-r--r--   0        0        0       24 2023-12-30 22:38:59.631229 achaekek-0.0.7/achaekek/__init__.py
--rw-r--r--   0        0        0     6280 2023-12-31 12:28:17.872202 achaekek-0.0.7/achaekek/achaekek.py
--rw-r--r--   0        0        0     8446 2024-02-12 01:37:46.955714 achaekek-0.0.7/achaekek/request_types.py
--rw-r--r--   0        0        0      332 2024-02-12 01:38:10.469859 achaekek-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      463 1970-01-01 00:00:00.000000 achaekek-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       40 2024-02-21 17:40:51.693421 achaekek-0.0.8/README.md
+-rw-r--r--   0        0        0       24 2024-02-21 17:40:51.693421 achaekek-0.0.8/achaekek/__init__.py
+-rw-r--r--   0        0        0     6280 2024-02-22 00:31:14.020626 achaekek-0.0.8/achaekek/achaekek.py
+-rw-r--r--   0        0        0     8854 2024-02-22 00:36:29.303289 achaekek-0.0.8/achaekek/request_types.py
+-rw-r--r--   0        0        0      332 2024-04-16 19:30:22.656304 achaekek-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 achaekek-0.0.8/PKG-INFO
```

### Comparing `achaekek-0.0.7/achaekek/achaekek.py` & `achaekek-0.0.8/achaekek/achaekek.py`

 * *Files identical despite different names*

### Comparing `achaekek-0.0.7/achaekek/request_types.py` & `achaekek-0.0.8/achaekek/request_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,16 @@
     description: str | tuple[str, DescriptionFormat] = None
     visibility: Literal["public", "unlisted"] = None
     groupIds: list[str] = None
     extraLiquidity: int = None
 
     def to_json(self):
         """
-        Converts the create market request dataclass to a JSON dictionary suitable for sending as a request to the Manifold API, reformatting the close time and description as needed.
+        Converts the create market request dataclass to a JSON dictionary suitable for sending as a request to the
+        Manifold API, reformatting the close time and description as needed.
 
         Returns
         -------
         json: dict[str, Any]
             The JSON dictionary to be sent as a request.
         """
         json = {k: v for k, v in self.__dict__.items() if v is not None}
@@ -69,14 +70,22 @@
 class CreateMultipleChoiceMarket(_CreateMarket):
     question: str
     answers: list[str]
     addAnswersMode: Literal["DISABLED", "ONLY_CREATORS", "ANYONE"]
     outcomeType: OutcomeType = field(default=OutcomeType.MULTIPLE_CHOICE)
     shouldAnswersSumToOne: bool = True
 
+    def to_json(self):
+        dictionary = super().to_json()
+        if "addAnswersMode" in dictionary:
+            dictionary["addAnswersMode"] = dictionary["addAnswersMode"].value
+        if "shouldAnswersSumToOne" in dictionary and dictionary["shouldAnswersSumToOne"]:
+            del dictionary["shouldAnswersSumToOne"]
+        return dictionary
+
 
 @dataclass
 class CreatePollMarket(_CreateMarket):
     answers: list[str]
     outcomeType: OutcomeType = field(default=OutcomeType.POLL)
 
 
@@ -106,14 +115,15 @@
     contractId: str
     outcome: Literal["YES", "NO"] = field(default="YES")
     limitprob: float = None
     expiresAt: datetime = None
 
     def to_json(self):
         json = super.to_json()
+        json["outcome"] = json["outcome"].value
         if "limitprob" in json:
             json["limitprob"] = round(json["limitprob"], 2)
         if "expiresAt" in json:
             json["expiresAt"] = int(time.mktime(self.expiresAt.timetuple()) * 1000)
         return json
```

