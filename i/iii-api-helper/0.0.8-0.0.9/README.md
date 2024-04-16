# Comparing `tmp/iii_api_helper-0.0.8.tar.gz` & `tmp/iii_api_helper-0.0.9.tar.gz`

## Comparing `iii_api_helper-0.0.8.tar` & `iii_api_helper-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 iii_api_helper-0.0.8/.gitlab-ci.yml
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 iii_api_helper-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 iii_api_helper-0.0.8/icons/logo.png
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 iii_api_helper-0.0.8/src/api_helper/__init__.py
--rw-r--r--   0        0        0     4363 2020-02-02 00:00:00.000000 iii_api_helper-0.0.8/src/api_helper/application.py
--rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 iii_api_helper-0.0.8/src/api_helper/middlewares.py
--rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 iii_api_helper-0.0.8/src/api_helper/responses.py
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 iii_api_helper-0.0.8/src/api_helper/sentry.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 iii_api_helper-0.0.8/src/api_helper/config/__init__.py
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 iii_api_helper-0.0.8/src/api_helper/config/configure.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 iii_api_helper-0.0.8/src/api_helper/config/formatter.py
--rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 iii_api_helper-0.0.8/src/api_helper/config/logger.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 iii_api_helper-0.0.8/src/api_helper/errors/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 iii_api_helper-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 iii_api_helper-0.0.8/tests/application/__init__.py
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 iii_api_helper-0.0.8/tests/application/test_application.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 iii_api_helper-0.0.8/tests/config/__init__.py
--rw-r--r--   0        0        0     5981 2020-02-02 00:00:00.000000 iii_api_helper-0.0.8/tests/config/test_config_functions.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 iii_api_helper-0.0.8/tests/config/test_fastapi_config.py
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 iii_api_helper-0.0.8/tests/statics/sample_env
--rw-r--r--   0        0        0     6040 2020-02-02 00:00:00.000000 iii_api_helper-0.0.8/.gitignore
--rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 iii_api_helper-0.0.8/README.md
--rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 iii_api_helper-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 iii_api_helper-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 iii_api_helper-0.0.9/.gitlab-ci.yml
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 iii_api_helper-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 iii_api_helper-0.0.9/icons/logo.png
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 iii_api_helper-0.0.9/src/api_helper/__init__.py
+-rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 iii_api_helper-0.0.9/src/api_helper/application.py
+-rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 iii_api_helper-0.0.9/src/api_helper/middlewares.py
+-rw-r--r--   0        0        0     4120 2020-02-02 00:00:00.000000 iii_api_helper-0.0.9/src/api_helper/responses.py
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 iii_api_helper-0.0.9/src/api_helper/sentry.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 iii_api_helper-0.0.9/src/api_helper/config/__init__.py
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 iii_api_helper-0.0.9/src/api_helper/config/configure.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 iii_api_helper-0.0.9/src/api_helper/config/formatter.py
+-rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 iii_api_helper-0.0.9/src/api_helper/config/logger.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 iii_api_helper-0.0.9/src/api_helper/errors/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 iii_api_helper-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 iii_api_helper-0.0.9/tests/application/__init__.py
+-rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 iii_api_helper-0.0.9/tests/application/test_application.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 iii_api_helper-0.0.9/tests/config/__init__.py
+-rw-r--r--   0        0        0     5981 2020-02-02 00:00:00.000000 iii_api_helper-0.0.9/tests/config/test_config_functions.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 iii_api_helper-0.0.9/tests/config/test_fastapi_config.py
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 iii_api_helper-0.0.9/tests/statics/sample_env
+-rw-r--r--   0        0        0     6040 2020-02-02 00:00:00.000000 iii_api_helper-0.0.9/.gitignore
+-rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 iii_api_helper-0.0.9/README.md
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 iii_api_helper-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 iii_api_helper-0.0.9/PKG-INFO
```

### Comparing `iii_api_helper-0.0.8/.gitlab-ci.yml` & `iii_api_helper-0.0.9/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `iii_api_helper-0.0.8/icons/logo.png` & `iii_api_helper-0.0.9/icons/logo.png`

 * *Files identical despite different names*

### Comparing `iii_api_helper-0.0.8/src/api_helper/middlewares.py` & `iii_api_helper-0.0.9/src/api_helper/middlewares.py`

 * *Files identical despite different names*

### Comparing `iii_api_helper-0.0.8/src/api_helper/responses.py` & `iii_api_helper-0.0.9/src/api_helper/responses.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,17 @@
     if SQLALCHEMY_INSTALLED and isinstance(type(obj), DeclarativeMeta):
         # Return obj.__dict__ if it exists and remove the _sa_instance_state
         return {key: value for key, value in obj.__dict__.items() if not key.startswith("_")}
 
     if isinstance(obj, BaseModel):
         return obj.model_dump()
 
+    if isinstance(obj, bytes):
+        return obj.decode()
+
     raise TypeError
 
 
 class ORJSONResponse(JSONResponse):
     # Override the default JSONResponse to use orjson
     # same from fastapi.responses.ORJSONResponse
```

### Comparing `iii_api_helper-0.0.8/src/api_helper/sentry.py` & `iii_api_helper-0.0.9/src/api_helper/sentry.py`

 * *Files identical despite different names*

### Comparing `iii_api_helper-0.0.8/src/api_helper/config/configure.py` & `iii_api_helper-0.0.9/src/api_helper/config/configure.py`

 * *Files identical despite different names*

### Comparing `iii_api_helper-0.0.8/src/api_helper/config/formatter.py` & `iii_api_helper-0.0.9/src/api_helper/config/formatter.py`

 * *Files identical despite different names*

### Comparing `iii_api_helper-0.0.8/src/api_helper/config/logger.py` & `iii_api_helper-0.0.9/src/api_helper/config/logger.py`

 * *Files identical despite different names*

### Comparing `iii_api_helper-0.0.8/tests/application/test_application.py` & `iii_api_helper-0.0.9/tests/application/test_application.py`

 * *Files identical despite different names*

### Comparing `iii_api_helper-0.0.8/tests/config/test_config_functions.py` & `iii_api_helper-0.0.9/tests/config/test_config_functions.py`

 * *Files identical despite different names*

### Comparing `iii_api_helper-0.0.8/tests/config/test_fastapi_config.py` & `iii_api_helper-0.0.9/tests/config/test_fastapi_config.py`

 * *Files identical despite different names*

### Comparing `iii_api_helper-0.0.8/.gitignore` & `iii_api_helper-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `iii_api_helper-0.0.8/README.md` & `iii_api_helper-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `iii_api_helper-0.0.8/pyproject.toml` & `iii_api_helper-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iii_api_helper-0.0.8/PKG-INFO` & `iii_api_helper-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: iii-api-helper
-Version: 0.0.8
+Version: 0.0.9
 Summary: III Common FastAPI base.
 Author: allen0099
 Classifier: Framework :: AsyncIO
 Classifier: Framework :: FastAPI
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
```

