# Comparing `tmp/retell_sdk-3.5.0.tar.gz` & `tmp/retell_sdk-3.6.0.tar.gz`

## Comparing `retell_sdk-3.5.0.tar` & `retell_sdk-3.6.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/__init__.py
--rw-r--r--   0        0        0    64275 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_base_client.py
--rw-r--r--   0        0        0    15337 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_constants.py
--rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_files.py
--rw-r--r--   0        0        0    22489 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_qs.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_resource.py
--rw-r--r--   0        0        0    28375 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_response.py
--rw-r--r--   0        0        0    10100 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_streaming.py
--rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_types.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/py.typed
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_utils/__init__.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_utils/_logs.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_utils/_typing.py
--rw-r--r--   0        0        0    11105 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/lib/.keep
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/resources/__init__.py
--rw-r--r--   0        0        0    42897 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/resources/agent.py
--rw-r--r--   0        0        0    25014 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/resources/call.py
--rw-r--r--   0        0        0    25717 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/resources/llm.py
--rw-r--r--   0        0        0    17883 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/resources/phone_number.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/__init__.py
--rw-r--r--   0        0        0     5336 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/agent_create_params.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/agent_list_response.py
--rw-r--r--   0        0        0     5663 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/agent_response.py
--rw-r--r--   0        0        0     5306 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/agent_update_params.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/call_create_params.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/call_list_params.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/call_list_response.py
--rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/call_register_params.py
--rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/call_response.py
--rw-r--r--   0        0        0    17570 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/llm_create_params.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/llm_list_response.py
--rw-r--r--   0        0        0    17657 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/llm_response.py
--rw-r--r--   0        0        0    17570 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/llm_update_params.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/phone_number_create_params.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/phone_number_list_response.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/phone_number_response.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/phone_number_update_params.py
--rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/register_call_response.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell_ai/lib/.keep
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell_sdk/lib/.keep
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/toddlzt/lib/.keep
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/.gitignore
--rw-r--r--   0        0        0    11336 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/LICENSE
--rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/pyproject.toml
--rw-r--r--   0        0        0    11998 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/PKG-INFO
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/__init__.py
+-rw-r--r--   0        0        0    64275 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_base_client.py
+-rw-r--r--   0        0        0    15337 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_constants.py
+-rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_files.py
+-rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_qs.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_resource.py
+-rw-r--r--   0        0        0    28375 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_response.py
+-rw-r--r--   0        0        0    10100 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_streaming.py
+-rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_types.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/py.typed
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_utils/__init__.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_utils/_typing.py
+-rw-r--r--   0        0        0    11105 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/lib/.keep
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/resources/__init__.py
+-rw-r--r--   0        0        0    42897 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/resources/agent.py
+-rw-r--r--   0        0        0    25014 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/resources/call.py
+-rw-r--r--   0        0        0    26571 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/resources/llm.py
+-rw-r--r--   0        0        0    17883 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/resources/phone_number.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/__init__.py
+-rw-r--r--   0        0        0     5336 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/agent_create_params.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/agent_list_response.py
+-rw-r--r--   0        0        0     5663 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/agent_response.py
+-rw-r--r--   0        0        0     5306 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/agent_update_params.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/call_create_params.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/call_list_params.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/call_list_response.py
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/call_register_params.py
+-rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/call_response.py
+-rw-r--r--   0        0        0    17703 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/llm_create_params.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/llm_list_response.py
+-rw-r--r--   0        0        0    17807 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/llm_response.py
+-rw-r--r--   0        0        0    17703 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/llm_update_params.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/phone_number_create_params.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/phone_number_list_response.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/phone_number_response.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/phone_number_update_params.py
+-rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/register_call_response.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell_ai/lib/.keep
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell_sdk/lib/.keep
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/toddlzt/lib/.keep
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/.gitignore
+-rw-r--r--   0        0        0    11336 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/LICENSE
+-rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/pyproject.toml
+-rw-r--r--   0        0        0    11945 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/PKG-INFO
```

### Comparing `retell_sdk-3.5.0/src/retell/__init__.py` & `retell_sdk-3.6.0/src/retell/__init__.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.5.0/src/retell/_base_client.py` & `retell_sdk-3.6.0/src/retell/_base_client.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.5.0/src/retell/_client.py` & `retell_sdk-3.6.0/src/retell/_client.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.5.0/src/retell/_compat.py` & `retell_sdk-3.6.0/src/retell/_compat.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.5.0/src/retell/_exceptions.py` & `retell_sdk-3.6.0/src/retell/_exceptions.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.5.0/src/retell/_files.py` & `retell_sdk-3.6.0/src/retell/_files.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.5.0/src/retell/_models.py` & `retell_sdk-3.6.0/src/retell/_models.py`

 * *Files 15% similar despite different names*

```diff
@@ -86,14 +86,87 @@
         def model_fields_set(self) -> set[str]:
             # a forwards-compat shim for pydantic v2
             return self.__fields_set__  # type: ignore
 
         class Config(pydantic.BaseConfig):  # pyright: ignore[reportDeprecated]
             extra: Any = pydantic.Extra.allow  # type: ignore
 
+    def to_dict(
+        self,
+        *,
+        mode: Literal["json", "python"] = "python",
+        use_api_names: bool = True,
+        exclude_unset: bool = True,
+        exclude_defaults: bool = False,
+        exclude_none: bool = False,
+        warnings: bool = True,
+    ) -> dict[str, object]:
+        """Recursively generate a dictionary representation of the model, optionally specifying which fields to include or exclude.
+
+        By default, fields that were not set by the API will not be included,
+        and keys will match the API response, *not* the property names from the model.
+
+        For example, if the API responds with `"fooBar": true` but we've defined a `foo_bar: bool` property,
+        the output will use the `"fooBar"` key (unless `use_api_names=False` is passed).
+
+        Args:
+            mode:
+                If mode is 'json', the dictionary will only contain JSON serializable types. e.g. `datetime` will be turned into a string, `"2024-3-22T18:11:19.117000Z"`.
+                If mode is 'python', the dictionary may contain any Python objects. e.g. `datetime(2024, 3, 22)`
+
+            use_api_names: Whether to use the key that the API responded with or the property name. Defaults to `True`.
+            exclude_unset: Whether to exclude fields that have not been explicitly set.
+            exclude_defaults: Whether to exclude fields that are set to their default value from the output.
+            exclude_none: Whether to exclude fields that have a value of `None` from the output.
+            warnings: Whether to log warnings when invalid fields are encountered. This is only supported in Pydantic v2.
+        """
+        return self.model_dump(
+            mode=mode,
+            by_alias=use_api_names,
+            exclude_unset=exclude_unset,
+            exclude_defaults=exclude_defaults,
+            exclude_none=exclude_none,
+            warnings=warnings,
+        )
+
+    def to_json(
+        self,
+        *,
+        indent: int | None = 2,
+        use_api_names: bool = True,
+        exclude_unset: bool = True,
+        exclude_defaults: bool = False,
+        exclude_none: bool = False,
+        warnings: bool = True,
+    ) -> str:
+        """Generates a JSON string representing this model as it would be received from or sent to the API (but with indentation).
+
+        By default, fields that were not set by the API will not be included,
+        and keys will match the API response, *not* the property names from the model.
+
+        For example, if the API responds with `"fooBar": true` but we've defined a `foo_bar: bool` property,
+        the output will use the `"fooBar"` key (unless `use_api_names=False` is passed).
+
+        Args:
+            indent: Indentation to use in the JSON output. If `None` is passed, the output will be compact. Defaults to `2`
+            use_api_names: Whether to use the key that the API responded with or the property name. Defaults to `True`.
+            exclude_unset: Whether to exclude fields that have not been explicitly set.
+            exclude_defaults: Whether to exclude fields that have the default value.
+            exclude_none: Whether to exclude fields that have a value of `None`.
+            warnings: Whether to show any warnings that occurred during serialization. This is only supported in Pydantic v2.
+        """
+        return self.model_dump_json(
+            indent=indent,
+            by_alias=use_api_names,
+            exclude_unset=exclude_unset,
+            exclude_defaults=exclude_defaults,
+            exclude_none=exclude_none,
+            warnings=warnings,
+        )
+
     @override
     def __str__(self) -> str:
         # mypy complains about an invalid self arg
         return f'{self.__repr_name__()}({self.__repr_str__(", ")})'  # type: ignore[misc]
 
     # Override the 'construct' method in a way that supports recursive parsing without validation.
     # Based on https://github.com/samuelcolvin/pydantic/issues/1168#issuecomment-817742836.
```

### Comparing `retell_sdk-3.5.0/src/retell/_qs.py` & `retell_sdk-3.6.0/src/retell/_qs.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.5.0/src/retell/_resource.py` & `retell_sdk-3.6.0/src/retell/_resource.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.5.0/src/retell/_response.py` & `retell_sdk-3.6.0/src/retell/_response.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.5.0/src/retell/_streaming.py` & `retell_sdk-3.6.0/src/retell/_streaming.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.5.0/src/retell/_types.py` & `retell_sdk-3.6.0/src/retell/_types.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.5.0/src/retell/_utils/__init__.py` & `retell_sdk-3.6.0/src/retell/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.5.0/src/retell/_utils/_logs.py` & `retell_sdk-3.6.0/src/retell/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.5.0/src/retell/_utils/_proxy.py` & `retell_sdk-3.6.0/src/retell/_utils/_proxy.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 T = TypeVar("T")
 
 
 class LazyProxy(Generic[T], ABC):
     """Implements data methods to pretend that an instance is another instance.
 
-    This includes forwarding attribute access and othe methods.
+    This includes forwarding attribute access and other methods.
     """
 
     # Note: we have to special case proxies that themselves return proxies
     # to support using a proxy as a catch-all for any random access, e.g. `proxy.foo.bar.baz`
 
     def __getattr__(self, attr: str) -> object:
         proxied = self.__get_proxied__()
```

### Comparing `retell_sdk-3.5.0/src/retell/_utils/_sync.py` & `retell_sdk-3.6.0/src/retell/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.5.0/src/retell/_utils/_transform.py` & `retell_sdk-3.6.0/src/retell/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.5.0/src/retell/_utils/_typing.py` & `retell_sdk-3.6.0/src/retell/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.5.0/src/retell/_utils/_utils.py` & `retell_sdk-3.6.0/src/retell/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.5.0/src/retell/resources/__init__.py` & `retell_sdk-3.6.0/src/retell/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.5.0/src/retell/resources/agent.py` & `retell_sdk-3.6.0/src/retell/resources/agent.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.5.0/src/retell/resources/call.py` & `retell_sdk-3.6.0/src/retell/resources/call.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.5.0/src/retell/resources/llm.py` & `retell_sdk-3.6.0/src/retell/resources/llm.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
 from typing import Iterable, Optional
+from typing_extensions import Literal
 
 import httpx
 
 from ..types import LlmResponse, LlmListResponse, llm_create_params, llm_update_params
 from .._types import NOT_GIVEN, Body, Query, Headers, NoneType, NotGiven
 from .._utils import (
     maybe_transform,
@@ -39,14 +40,15 @@
     def create(
         self,
         *,
         begin_message: Optional[str] | NotGiven = NOT_GIVEN,
         general_prompt: Optional[str] | NotGiven = NOT_GIVEN,
         general_tools: Optional[Iterable[llm_create_params.GeneralTool]] | NotGiven = NOT_GIVEN,
         inbound_dynamic_variables_webhook_url: Optional[str] | NotGiven = NOT_GIVEN,
+        model: Literal["gpt-3.5-turbo", "gpt-4-turbo"] | NotGiven = NOT_GIVEN,
         starting_state: Optional[str] | NotGiven = NOT_GIVEN,
         states: Optional[Iterable[llm_create_params.State]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
@@ -73,14 +75,16 @@
 
               - Tools of LLM (no state) = general tools
 
           inbound_dynamic_variables_webhook_url: For inbound phone calls with Retell numbers, if this webhook is set, will POST
               to it to retrieve dynamic variables to use for the call. Without this, there's
               no way to pass dynamic variables to inbound calls of Retell numbers.
 
+          model: Select the underlying LLM. If not set, would default to gpt-3.5-turbo.
+
           starting_state: Name of the starting state. Required if states is not empty.
 
           states: States of the LLM. This is to help reduce prompt length and tool choices when
               the call can be broken into distinct states. With shorter prompts and less
               tools, the LLM can better focus and follow the rules, minimizing hallucination.
               If this field is not set, the agent would only have general prompt and general
               tools (essentially one state).
@@ -97,14 +101,15 @@
             "/create-retell-llm",
             body=maybe_transform(
                 {
                     "begin_message": begin_message,
                     "general_prompt": general_prompt,
                     "general_tools": general_tools,
                     "inbound_dynamic_variables_webhook_url": inbound_dynamic_variables_webhook_url,
+                    "model": model,
                     "starting_state": starting_state,
                     "states": states,
                 },
                 llm_create_params.LlmCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
@@ -149,14 +154,15 @@
         self,
         llm_id: str,
         *,
         begin_message: Optional[str] | NotGiven = NOT_GIVEN,
         general_prompt: Optional[str] | NotGiven = NOT_GIVEN,
         general_tools: Optional[Iterable[llm_update_params.GeneralTool]] | NotGiven = NOT_GIVEN,
         inbound_dynamic_variables_webhook_url: Optional[str] | NotGiven = NOT_GIVEN,
+        model: Literal["gpt-3.5-turbo", "gpt-4-turbo"] | NotGiven = NOT_GIVEN,
         starting_state: Optional[str] | NotGiven = NOT_GIVEN,
         states: Optional[Iterable[llm_update_params.State]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
@@ -183,14 +189,16 @@
 
               - Tools of LLM (no state) = general tools
 
           inbound_dynamic_variables_webhook_url: For inbound phone calls with Retell numbers, if this webhook is set, will POST
               to it to retrieve dynamic variables to use for the call. Without this, there's
               no way to pass dynamic variables to inbound calls of Retell numbers.
 
+          model: Select the underlying LLM. If not set, would default to gpt-3.5-turbo.
+
           starting_state: Name of the starting state. Required if states is not empty.
 
           states: States of the LLM. This is to help reduce prompt length and tool choices when
               the call can be broken into distinct states. With shorter prompts and less
               tools, the LLM can better focus and follow the rules, minimizing hallucination.
               If this field is not set, the agent would only have general prompt and general
               tools (essentially one state).
@@ -209,14 +217,15 @@
             f"/update-retell-llm/{llm_id}",
             body=maybe_transform(
                 {
                     "begin_message": begin_message,
                     "general_prompt": general_prompt,
                     "general_tools": general_tools,
                     "inbound_dynamic_variables_webhook_url": inbound_dynamic_variables_webhook_url,
+                    "model": model,
                     "starting_state": starting_state,
                     "states": states,
                 },
                 llm_update_params.LlmUpdateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
@@ -290,14 +299,15 @@
     async def create(
         self,
         *,
         begin_message: Optional[str] | NotGiven = NOT_GIVEN,
         general_prompt: Optional[str] | NotGiven = NOT_GIVEN,
         general_tools: Optional[Iterable[llm_create_params.GeneralTool]] | NotGiven = NOT_GIVEN,
         inbound_dynamic_variables_webhook_url: Optional[str] | NotGiven = NOT_GIVEN,
+        model: Literal["gpt-3.5-turbo", "gpt-4-turbo"] | NotGiven = NOT_GIVEN,
         starting_state: Optional[str] | NotGiven = NOT_GIVEN,
         states: Optional[Iterable[llm_create_params.State]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
@@ -324,14 +334,16 @@
 
               - Tools of LLM (no state) = general tools
 
           inbound_dynamic_variables_webhook_url: For inbound phone calls with Retell numbers, if this webhook is set, will POST
               to it to retrieve dynamic variables to use for the call. Without this, there's
               no way to pass dynamic variables to inbound calls of Retell numbers.
 
+          model: Select the underlying LLM. If not set, would default to gpt-3.5-turbo.
+
           starting_state: Name of the starting state. Required if states is not empty.
 
           states: States of the LLM. This is to help reduce prompt length and tool choices when
               the call can be broken into distinct states. With shorter prompts and less
               tools, the LLM can better focus and follow the rules, minimizing hallucination.
               If this field is not set, the agent would only have general prompt and general
               tools (essentially one state).
@@ -348,14 +360,15 @@
             "/create-retell-llm",
             body=await async_maybe_transform(
                 {
                     "begin_message": begin_message,
                     "general_prompt": general_prompt,
                     "general_tools": general_tools,
                     "inbound_dynamic_variables_webhook_url": inbound_dynamic_variables_webhook_url,
+                    "model": model,
                     "starting_state": starting_state,
                     "states": states,
                 },
                 llm_create_params.LlmCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
@@ -400,14 +413,15 @@
         self,
         llm_id: str,
         *,
         begin_message: Optional[str] | NotGiven = NOT_GIVEN,
         general_prompt: Optional[str] | NotGiven = NOT_GIVEN,
         general_tools: Optional[Iterable[llm_update_params.GeneralTool]] | NotGiven = NOT_GIVEN,
         inbound_dynamic_variables_webhook_url: Optional[str] | NotGiven = NOT_GIVEN,
+        model: Literal["gpt-3.5-turbo", "gpt-4-turbo"] | NotGiven = NOT_GIVEN,
         starting_state: Optional[str] | NotGiven = NOT_GIVEN,
         states: Optional[Iterable[llm_update_params.State]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
@@ -434,14 +448,16 @@
 
               - Tools of LLM (no state) = general tools
 
           inbound_dynamic_variables_webhook_url: For inbound phone calls with Retell numbers, if this webhook is set, will POST
               to it to retrieve dynamic variables to use for the call. Without this, there's
               no way to pass dynamic variables to inbound calls of Retell numbers.
 
+          model: Select the underlying LLM. If not set, would default to gpt-3.5-turbo.
+
           starting_state: Name of the starting state. Required if states is not empty.
 
           states: States of the LLM. This is to help reduce prompt length and tool choices when
               the call can be broken into distinct states. With shorter prompts and less
               tools, the LLM can better focus and follow the rules, minimizing hallucination.
               If this field is not set, the agent would only have general prompt and general
               tools (essentially one state).
@@ -460,14 +476,15 @@
             f"/update-retell-llm/{llm_id}",
             body=await async_maybe_transform(
                 {
                     "begin_message": begin_message,
                     "general_prompt": general_prompt,
                     "general_tools": general_tools,
                     "inbound_dynamic_variables_webhook_url": inbound_dynamic_variables_webhook_url,
+                    "model": model,
                     "starting_state": starting_state,
                     "states": states,
                 },
                 llm_update_params.LlmUpdateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
```

### Comparing `retell_sdk-3.5.0/src/retell/resources/phone_number.py` & `retell_sdk-3.6.0/src/retell/resources/phone_number.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.5.0/src/retell/types/__init__.py` & `retell_sdk-3.6.0/src/retell/types/__init__.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.5.0/src/retell/types/agent_create_params.py` & `retell_sdk-3.6.0/src/retell/types/agent_create_params.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.5.0/src/retell/types/agent_response.py` & `retell_sdk-3.6.0/src/retell/types/agent_response.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.5.0/src/retell/types/agent_update_params.py` & `retell_sdk-3.6.0/src/retell/types/agent_update_params.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.5.0/src/retell/types/call_create_params.py` & `retell_sdk-3.6.0/src/retell/types/call_create_params.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.5.0/src/retell/types/call_list_params.py` & `retell_sdk-3.6.0/src/retell/types/call_list_params.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.5.0/src/retell/types/call_register_params.py` & `retell_sdk-3.6.0/src/retell/types/call_register_params.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.5.0/src/retell/types/call_response.py` & `retell_sdk-3.6.0/src/retell/types/call_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,91 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from typing import Dict, List, Optional
 from typing_extensions import Literal
 
 from .._models import BaseModel
 
-__all__ = ["CallResponse", "E2eLatency", "TranscriptObject", "TranscriptObjectWord"]
+__all__ = [
+    "CallResponse",
+    "E2eLatency",
+    "LlmLatency",
+    "LlmWebsocketNetworkRttLatency",
+    "TranscriptObject",
+    "TranscriptObjectWord",
+]
 
 
 class E2eLatency(BaseModel):
     max: Optional[float] = None
-    """Maximum end to end latency in the call."""
+    """Maximum latency in the call, measured in milliseconds."""
 
     min: Optional[float] = None
-    """Minimum end to end latency in the call."""
+    """Minimum latency in the call, measured in milliseconds."""
 
     num: Optional[float] = None
-    """Number of turn change.
+    """Number of data points (number of times latency is tracked)."""
 
-    We track latency every time turn change between user and agent.
-    """
+    p50: Optional[float] = None
+    """50 percentile of latency, measured in milliseconds."""
+
+    p90: Optional[float] = None
+    """90 percentile of latency, measured in milliseconds."""
+
+    p95: Optional[float] = None
+    """95 percentile of latency, measured in milliseconds."""
+
+    p99: Optional[float] = None
+    """99 percentile of latency, measured in milliseconds."""
+
+
+class LlmLatency(BaseModel):
+    max: Optional[float] = None
+    """Maximum latency in the call, measured in milliseconds."""
+
+    min: Optional[float] = None
+    """Minimum latency in the call, measured in milliseconds."""
+
+    num: Optional[float] = None
+    """Number of data points (number of times latency is tracked)."""
+
+    p50: Optional[float] = None
+    """50 percentile of latency, measured in milliseconds."""
+
+    p90: Optional[float] = None
+    """90 percentile of latency, measured in milliseconds."""
+
+    p95: Optional[float] = None
+    """95 percentile of latency, measured in milliseconds."""
+
+    p99: Optional[float] = None
+    """99 percentile of latency, measured in milliseconds."""
+
+
+class LlmWebsocketNetworkRttLatency(BaseModel):
+    max: Optional[float] = None
+    """Maximum latency in the call, measured in milliseconds."""
+
+    min: Optional[float] = None
+    """Minimum latency in the call, measured in milliseconds."""
+
+    num: Optional[float] = None
+    """Number of data points (number of times latency is tracked)."""
 
     p50: Optional[float] = None
-    """50 percentile of end to end latency."""
+    """50 percentile of latency, measured in milliseconds."""
 
     p90: Optional[float] = None
-    """90 percentile of end to end latency."""
+    """90 percentile of latency, measured in milliseconds."""
 
     p95: Optional[float] = None
-    """95 percentile of end to end latency."""
+    """95 percentile of latency, measured in milliseconds."""
 
     p99: Optional[float] = None
-    """99 percentile of end to end latency."""
+    """99 percentile of latency, measured in milliseconds."""
 
 
 class TranscriptObjectWord(BaseModel):
     end: Optional[float] = None
     """End time of the word in the call in second.
 
     This is relative audio time, not wall time.
@@ -129,15 +179,16 @@
       - deepgram voices: 8000, 16000, 24000, 32000, 48000.
     """
 
     e2e_latency: Optional[E2eLatency] = None
     """
     End to end latency (from user stops talking to agent start talking) tracking of
     the call, available after call ends. This latency does not account for the
-    network trip time from Retell server to user frontend.
+    network trip time from Retell server to user frontend. The latency is tracked
+    every time turn change between user and agent.
     """
 
     end_call_after_silence_ms: Optional[int] = None
     """If users stay silent for a period, end the call.
 
     By default, it is set to 600,000 ms (10 min). The minimum value allowed is
     10,000 ms (10 s).
@@ -153,14 +204,28 @@
     """The caller number.
 
     This field is storage purpose only, set this if you want the call object to
     contain it so that it's easier to reference it. Not used for processing, when we
     connect to your LLM websocket server, you can then get it from the call object.
     """
 
+    llm_latency: Optional[LlmLatency] = None
+    """
+    LLM latency (from issue of LLM call to first token received) tracking of the
+    call, available after call ends. When using custom LLM. this latency includes
+    LLM websocket roundtrip time between user server and Retell server.
+    """
+
+    llm_websocket_network_rtt_latency: Optional[LlmWebsocketNetworkRttLatency] = None
+    """
+    LLM websocket roundtrip latency (between user server and Retell server) tracking
+    of the call, available after call ends. Only populated for calls using custom
+    LLM.
+    """
+
     metadata: Optional[object] = None
     """An abtriary object for storage purpose only.
 
     You can put anything here like your own id for the call, twilio SID, internal
     customer id. Not used for processing, when we connect to your LLM websocket
     server, you can then get it from the call object.
     """
```

### Comparing `retell_sdk-3.5.0/src/retell/types/llm_create_params.py` & `retell_sdk-3.6.0/src/retell/types/llm_create_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,17 @@
     inbound_dynamic_variables_webhook_url: Optional[str]
     """
     For inbound phone calls with Retell numbers, if this webhook is set, will POST
     to it to retrieve dynamic variables to use for the call. Without this, there's
     no way to pass dynamic variables to inbound calls of Retell numbers.
     """
 
+    model: Literal["gpt-3.5-turbo", "gpt-4-turbo"]
+    """Select the underlying LLM. If not set, would default to gpt-3.5-turbo."""
+
     starting_state: Optional[str]
     """Name of the starting state. Required if states is not empty."""
 
     states: Optional[Iterable[State]]
     """States of the LLM.
 
     This is to help reduce prompt length and tool choices when the call can be
```

### Comparing `retell_sdk-3.5.0/src/retell/types/llm_response.py` & `retell_sdk-3.6.0/src/retell/types/llm_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -534,14 +534,17 @@
     inbound_dynamic_variables_webhook_url: Optional[str] = None
     """
     For inbound phone calls with Retell numbers, if this webhook is set, will POST
     to it to retrieve dynamic variables to use for the call. Without this, there's
     no way to pass dynamic variables to inbound calls of Retell numbers.
     """
 
+    model: Optional[Literal["gpt-3.5-turbo", "gpt-4-turbo"]] = None
+    """Select the underlying LLM. If not set, would default to gpt-3.5-turbo."""
+
     starting_state: Optional[str] = None
     """Name of the starting state. Required if states is not empty."""
 
     states: Optional[List[State]] = None
     """States of the LLM.
 
     This is to help reduce prompt length and tool choices when the call can be
```

### Comparing `retell_sdk-3.5.0/src/retell/types/llm_update_params.py` & `retell_sdk-3.6.0/src/retell/types/llm_update_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,17 @@
     inbound_dynamic_variables_webhook_url: Optional[str]
     """
     For inbound phone calls with Retell numbers, if this webhook is set, will POST
     to it to retrieve dynamic variables to use for the call. Without this, there's
     no way to pass dynamic variables to inbound calls of Retell numbers.
     """
 
+    model: Literal["gpt-3.5-turbo", "gpt-4-turbo"]
+    """Select the underlying LLM. If not set, would default to gpt-3.5-turbo."""
+
     starting_state: Optional[str]
     """Name of the starting state. Required if states is not empty."""
 
     states: Optional[Iterable[State]]
     """States of the LLM.
 
     This is to help reduce prompt length and tool choices when the call can be
```

### Comparing `retell_sdk-3.5.0/src/retell/types/phone_number_create_params.py` & `retell_sdk-3.6.0/src/retell/types/phone_number_create_params.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.5.0/src/retell/types/phone_number_response.py` & `retell_sdk-3.6.0/src/retell/types/phone_number_response.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.5.0/src/retell/types/register_call_response.py` & `retell_sdk-3.6.0/src/retell/types/register_call_response.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.5.0/LICENSE` & `retell_sdk-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.5.0/pyproject.toml` & `retell_sdk-3.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "retell-sdk"
-version = "3.5.0"
+version = "3.6.0"
 description = "The official Python library for the retell API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Retell", email = "founders@retellai.com" },
 ]
 dependencies = [
```

### Comparing `retell_sdk-3.5.0/PKG-INFO` & `retell_sdk-3.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: retell-sdk
-Version: 3.5.0
+Version: 3.6.0
 Summary: The official Python library for the retell API
 Project-URL: Homepage, https://github.com/RetellAI/retell-python-sdk
 Project-URL: Repository, https://github.com/RetellAI/retell-python-sdk
 Author-email: Retell <founders@retellai.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
@@ -93,18 +93,18 @@
 asyncio.run(main())
 ```
 
 Functionality between the synchronous and asynchronous clients is otherwise identical.
 
 ## Using types
 
-Nested request parameters are [TypedDicts](https://docs.python.org/3/library/typing.html#typing.TypedDict). Responses are [Pydantic models](https://docs.pydantic.dev), which provide helper methods for things like:
+Nested request parameters are [TypedDicts](https://docs.python.org/3/library/typing.html#typing.TypedDict). Responses are [Pydantic models](https://docs.pydantic.dev) which also provide helper methods for things like:
 
-- Serializing back into JSON, `model.model_dump_json(indent=2, exclude_unset=True)`
-- Converting to a dictionary, `model.model_dump(exclude_unset=True)`
+- Serializing back into JSON, `model.to_json()`
+- Converting to a dictionary, `model.to_dict()`
 
 Typed requests and responses provide autocomplete and documentation within your editor. If you would like to see type errors in VS Code to help catch bugs earlier, set `python.analysis.typeCheckingMode` to `basic`.
 
 ## Handling errors
 
 When the library is unable to connect to the API (for example, due to network connection problems or a timeout), a subclass of `retell.APIConnectionError` is raised.
```

