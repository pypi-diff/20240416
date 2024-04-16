# Comparing `tmp/known_problems_fastapi_router-0.1.0.tar.gz` & `tmp/known_problems_fastapi_router-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "known_problems_fastapi_router-0.1.0.tar", max compression
+gzip compressed data, was "known_problems_fastapi_router-0.1.1.tar", max compression
```

## Comparing `known_problems_fastapi_router-0.1.0.tar` & `known_problems_fastapi_router-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1077 2024-04-03 13:35:15.502318 known_problems_fastapi_router-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     1140 2024-04-03 13:35:15.502318 known_problems_fastapi_router-0.1.0/README.md
--rw-r--r--   0        0        0      649 2024-04-03 13:35:15.506318 known_problems_fastapi_router-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      230 2024-04-03 13:35:15.506318 known_problems_fastapi_router-0.1.0/src/known_problems_fastapi_router/__init__.py
--rw-r--r--   0        0        0      826 2024-04-03 13:35:15.506318 known_problems_fastapi_router-0.1.0/src/known_problems_fastapi_router/exception_handlers.py
--rw-r--r--   0        0        0    34719 2024-04-03 13:35:15.506318 known_problems_fastapi_router-0.1.0/src/known_problems_fastapi_router/routing.py
--rw-r--r--   0        0        0     1270 2024-04-03 13:35:15.506318 known_problems_fastapi_router-0.1.0/src/known_problems_fastapi_router/types.py
--rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 known_problems_fastapi_router-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-04-16 08:26:20.497014 known_problems_fastapi_router-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     1140 2024-04-16 08:26:20.497014 known_problems_fastapi_router-0.1.1/README.md
+-rw-r--r--   0        0        0      649 2024-04-16 08:26:20.497014 known_problems_fastapi_router-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      230 2024-04-16 08:26:20.497014 known_problems_fastapi_router-0.1.1/src/known_problems_fastapi_router/__init__.py
+-rw-r--r--   0        0        0      826 2024-04-16 08:26:20.497014 known_problems_fastapi_router-0.1.1/src/known_problems_fastapi_router/exception_handlers.py
+-rw-r--r--   0        0        0    35069 2024-04-16 08:26:20.497014 known_problems_fastapi_router-0.1.1/src/known_problems_fastapi_router/routing.py
+-rw-r--r--   0        0        0     1270 2024-04-16 08:26:20.497014 known_problems_fastapi_router-0.1.1/src/known_problems_fastapi_router/types.py
+-rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 known_problems_fastapi_router-0.1.1/PKG-INFO
```

### Comparing `known_problems_fastapi_router-0.1.0/LICENSE.txt` & `known_problems_fastapi_router-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `known_problems_fastapi_router-0.1.0/README.md` & `known_problems_fastapi_router-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `known_problems_fastapi_router-0.1.0/pyproject.toml` & `known_problems_fastapi_router-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "known-problems-fastapi-router"
-version = "0.1.0"
+version = "0.1.1"
 description = "A known problem API router package"
 authors = [
     "Fabian Haenel <fabian.haenel@fastlane.net>",
     "Simone Renesto <simone.renesto@fastlane.net>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `known_problems_fastapi_router-0.1.0/src/known_problems_fastapi_router/exception_handlers.py` & `known_problems_fastapi_router-0.1.1/src/known_problems_fastapi_router/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `known_problems_fastapi_router-0.1.0/src/known_problems_fastapi_router/routing.py` & `known_problems_fastapi_router-0.1.1/src/known_problems_fastapi_router/routing.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
             f"| {' | '.join(row)} |" for row in rows
         )
 
     def generate_responses_dict(
         self,
         responses: Optional[Dict[Union[int, str], Dict[str, Any]]],
         known_problems: Tuple[KnownProblem, ...],
-        all_problems_response_models: Dict[int, Type[BaseModel]],
+        all_problems_response_models: Dict[int, Dict[str, Type[BaseModel]]],
     ) -> Dict[Union[int, str], Dict[str, Any]]:
         responses = responses or {}
         all_known_problems = known_problems
 
         # Map KnownError's to http status codes in preparation for
         # creating the docs tables
         docs_table_to_status_code_mapping: Dict[
@@ -137,15 +137,17 @@
                         ]
                     )
                     if description
                     else error_code_table_markdown
                 )
             else:
                 responses[known_status_code] = {
-                    "model": all_problems_response_models[known_status_code],
+                    "model": Union[
+                        *list(all_problems_response_models[known_status_code].values())
+                    ],
                     "description": error_code_table_markdown,
                 }
         return responses
 
     def add_api_route(
         self,
         path: str,
@@ -258,25 +260,27 @@
         generate_unique_id_function: Callable[[APIRoute], str] = Default(
             generate_unique_id
         ),
         known_problems: Tuple[KnownProblem, ...] = tuple(),
     ) -> Callable[[DecoratedCallable], DecoratedCallable]:
         all_known_problems = known_problems + self.common_known_problems
 
-        all_problems_response_models = {
-            known_problem.status_code: create_model(  # type: ignore
-                __model_name="KnownProblemSpec",
+        all_problems_response_models: Dict[int, Dict[str, Type[BaseModel]]] = {
+            known_problem.status_code: {} for known_problem in all_known_problems
+        }
+
+        for known_problem in all_known_problems:
+            all_problems_response_models[known_problem.status_code][known_problem.code] = create_model(  # type: ignore
+                __model_name=known_problem.code.replace("-", " ").title(),
                 __base__=KnownProblemResponse,
                 **{
                     key: known_problem.extension[key].get("typing")
                     for key in known_problem.extension.keys()
                 },
             )
-            for known_problem in all_known_problems
-        }
 
         def decorator(func: DecoratedCallable) -> DecoratedCallable:
             @functools.wraps(func)
             async def handled_func(*args, **kwargs):
                 try:
                     return (
                         await func(*args, **kwargs)
@@ -288,15 +292,17 @@
                         known_problem = next(
                             known_problem
                             for known_problem in all_known_problems
                             if known_problem.exception_class is not None
                             and isinstance(e, known_problem.exception_class)
                         )
 
-                        model = all_problems_response_models[known_problem.status_code]
+                        model = all_problems_response_models[known_problem.status_code][
+                            known_problem.code
+                        ]
 
                         instance_uri = f"{methods[0]}:{path}"
 
                         for key, value in kwargs.items():
                             instance_uri = instance_uri.replace(
                                 f"{{{key}}}", str(value)
                             )
```

### Comparing `known_problems_fastapi_router-0.1.0/src/known_problems_fastapi_router/types.py` & `known_problems_fastapi_router-0.1.1/src/known_problems_fastapi_router/types.py`

 * *Files identical despite different names*

### Comparing `known_problems_fastapi_router-0.1.0/PKG-INFO` & `known_problems_fastapi_router-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: known-problems-fastapi-router
-Version: 0.1.0
+Version: 0.1.1
 Summary: A known problem API router package
 License: MIT
 Author: Fabian Haenel
 Author-email: fabian.haenel@fastlane.net
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

