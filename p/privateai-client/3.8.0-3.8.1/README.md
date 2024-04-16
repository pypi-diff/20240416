# Comparing `tmp/privateai_client-3.8.0.tar.gz` & `tmp/privateai_client-3.8.1.tar.gz`

## Comparing `privateai_client-3.8.0.tar` & `privateai_client-3.8.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 privateai_client-3.8.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     5119 2020-02-02 00:00:00.000000 privateai_client-3.8.0/CHANGELOG.md
--rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 privateai_client-3.8.0/CONTRIBUTING.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 privateai_client-3.8.0/__init__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 privateai_client-3.8.0/requirements.dev.txt
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 privateai_client-3.8.0/requirements.txt
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 privateai_client-3.8.0/.github/pull-request-template.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 privateai_client-3.8.0/src/privateai_client/__about__.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 privateai_client-3.8.0/src/privateai_client/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 privateai_client-3.8.0/src/privateai_client/objects.py
--rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 privateai_client-3.8.0/src/privateai_client/pai_client.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 privateai_client-3.8.0/src/privateai_client/components/__init__.py
--rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 privateai_client-3.8.0/src/privateai_client/components/pai_requests.py
--rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 privateai_client-3.8.0/src/privateai_client/components/pai_responses.py
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 privateai_client-3.8.0/src/privateai_client/components/pai_uris.py
--rw-r--r--   0        0        0    29790 2020-02-02 00:00:00.000000 privateai_client-3.8.0/src/privateai_client/components/request_objects.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 privateai_client-3.8.0/src/privateai_client/tests/.env
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 privateai_client-3.8.0/src/privateai_client/tests/.env.example
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 privateai_client-3.8.0/src/privateai_client/tests/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 privateai_client-3.8.0/src/privateai_client/tests/__init__.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 privateai_client-3.8.0/src/privateai_client/tests/test_client.py
--rw-r--r--   0        0        0     6742 2020-02-02 00:00:00.000000 privateai_client-3.8.0/src/privateai_client/tests/test_integration.py
--rw-r--r--   0        0        0    45748 2020-02-02 00:00:00.000000 privateai_client-3.8.0/src/privateai_client/tests/test_request_objects.py
--rw-r--r--   0        0        0     7358 2020-02-02 00:00:00.000000 privateai_client-3.8.0/src/privateai_client/tests/test_files/simpsons_wiki.txt
--rw-r--r--   0        0        0    98054 2020-02-02 00:00:00.000000 privateai_client-3.8.0/src/privateai_client/tests/test_files/test_audio.mp3
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 privateai_client-3.8.0/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 privateai_client-3.8.0/LICENSE
--rw-r--r--   0        0        0    12634 2020-02-02 00:00:00.000000 privateai_client-3.8.0/README.md
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 privateai_client-3.8.0/pyproject.toml
--rw-r--r--   0        0        0    13487 2020-02-02 00:00:00.000000 privateai_client-3.8.0/PKG-INFO
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 privateai_client-3.8.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     5259 2020-02-02 00:00:00.000000 privateai_client-3.8.1/CHANGELOG.md
+-rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 privateai_client-3.8.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 privateai_client-3.8.1/__init__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 privateai_client-3.8.1/requirements.dev.txt
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 privateai_client-3.8.1/requirements.txt
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 privateai_client-3.8.1/.github/pull-request-template.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 privateai_client-3.8.1/src/privateai_client/__about__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 privateai_client-3.8.1/src/privateai_client/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 privateai_client-3.8.1/src/privateai_client/objects.py
+-rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 privateai_client-3.8.1/src/privateai_client/pai_client.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 privateai_client-3.8.1/src/privateai_client/components/__init__.py
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 privateai_client-3.8.1/src/privateai_client/components/pai_requests.py
+-rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 privateai_client-3.8.1/src/privateai_client/components/pai_responses.py
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 privateai_client-3.8.1/src/privateai_client/components/pai_uris.py
+-rw-r--r--   0        0        0    29837 2020-02-02 00:00:00.000000 privateai_client-3.8.1/src/privateai_client/components/request_objects.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 privateai_client-3.8.1/src/privateai_client/tests/.env
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 privateai_client-3.8.1/src/privateai_client/tests/.env.example
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 privateai_client-3.8.1/src/privateai_client/tests/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 privateai_client-3.8.1/src/privateai_client/tests/__init__.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 privateai_client-3.8.1/src/privateai_client/tests/test_client.py
+-rw-r--r--   0        0        0     7009 2020-02-02 00:00:00.000000 privateai_client-3.8.1/src/privateai_client/tests/test_integration.py
+-rw-r--r--   0        0        0    46246 2020-02-02 00:00:00.000000 privateai_client-3.8.1/src/privateai_client/tests/test_request_objects.py
+-rw-r--r--   0        0        0     7358 2020-02-02 00:00:00.000000 privateai_client-3.8.1/src/privateai_client/tests/test_files/simpsons_wiki.txt
+-rw-r--r--   0        0        0    98054 2020-02-02 00:00:00.000000 privateai_client-3.8.1/src/privateai_client/tests/test_files/test_audio.mp3
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 privateai_client-3.8.1/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 privateai_client-3.8.1/LICENSE
+-rw-r--r--   0        0        0    12634 2020-02-02 00:00:00.000000 privateai_client-3.8.1/README.md
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 privateai_client-3.8.1/pyproject.toml
+-rw-r--r--   0        0        0    13487 2020-02-02 00:00:00.000000 privateai_client-3.8.1/PKG-INFO
```

### Comparing `privateai_client-3.8.0/CHANGELOG.md` & `privateai_client-3.8.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,23 @@
 
 ### Added
 
 ### Changed
 
 ### Fixed
 
+## [3.8.1] - 2024-04-16
+
+### Added
+- Added marker_langauge options to processed text to enable new features in 3.8
+
+### Changed
+
+### Fixed
+
 ## [3.8.0] - 2024-03-27
 
 ### Added
 - Added support for the "enable_pdf_text_layer" PDFOption
 
 ### Changed
```

### Comparing `privateai_client-3.8.0/CONTRIBUTING.md` & `privateai_client-3.8.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `privateai_client-3.8.0/src/privateai_client/objects.py` & `privateai_client-3.8.1/src/privateai_client/objects.py`

 * *Files identical despite different names*

### Comparing `privateai_client-3.8.0/src/privateai_client/pai_client.py` & `privateai_client-3.8.1/src/privateai_client/pai_client.py`

 * *Files identical despite different names*

### Comparing `privateai_client-3.8.0/src/privateai_client/components/pai_requests.py` & `privateai_client-3.8.1/src/privateai_client/components/pai_requests.py`

 * *Files identical despite different names*

### Comparing `privateai_client-3.8.0/src/privateai_client/components/pai_responses.py` & `privateai_client-3.8.1/src/privateai_client/components/pai_responses.py`

 * *Files identical despite different names*

### Comparing `privateai_client-3.8.0/src/privateai_client/components/pai_uris.py` & `privateai_client-3.8.1/src/privateai_client/components/pai_uris.py`

 * *Files identical despite different names*

### Comparing `privateai_client-3.8.0/src/privateai_client/components/request_objects.py` & `privateai_client-3.8.1/src/privateai_client/components/request_objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,17 +8,15 @@
         for key, value in self.__dict__.items():
             if value in [None, [], {}]:
                 continue
             name = key if key[0] != "_" else key[1:]
             if self._issubclass(value):
                 dict_obj[name] = value.to_dict()
             elif type(value) is list:
-                dict_obj[name] = [
-                    row.to_dict() if self._issubclass(row) else row for row in value
-                ]
+                dict_obj[name] = [row.to_dict() if self._issubclass(row) else row for row in value]
             elif not key.startswith("__") and not callable(key):
                 dict_obj[name] = value
         return dict_obj
 
     def _issubclass(self, obj):
         return inspect.isclass(type(obj)) and issubclass(type(obj), BaseRequestObject)
 
@@ -86,42 +84,34 @@
     @bleep_gain.setter
     def bleep_gain(self, var):
         if self._bleep_gain_validator(var):
             self._bleep_gain = var
 
     def _bleep_start_padding_validator(self, var):
         if type(var) is not float:
-            raise ValueError(
-                f"AudioOptions.bleep_start_padding must be of type float, but got {type(var)}"
-            )
+            raise ValueError(f"AudioOptions.bleep_start_padding must be of type float, but got {type(var)}")
         if var < 0:
             raise ValueError("AudioOptions.bleep_start_padding must be positive")
         return True
 
     def _bleep_end_padding_validator(self, var):
         if type(var) is not float:
-            raise ValueError(
-                f"AudioOptions.bleep_end_padding must be of type float, but got {type(var)}"
-            )
+            raise ValueError(f"AudioOptions.bleep_end_padding must be of type float, but got {type(var)}")
         if var < 0:
             raise ValueError("AudioOptions.bleep_end_padding must be positive")
         return True
 
     def _bleep_frequency_validator(self, var):
         if type(var) is not int and var is not None:
-            raise ValueError(
-                f"AudioOptions.bleep_frequency must be of type int or None, but got {type(var)}"
-            )
+            raise ValueError(f"AudioOptions.bleep_frequency must be of type int or None, but got {type(var)}")
         return True
 
     def _bleep_gain_validator(self, var):
         if type(var) is not int and var is not None:
-            raise ValueError(
-                f"AudioOptions.bleep_gain must be of type int or None, but got {type(var)}"
-            )
+            raise ValueError(f"AudioOptions.bleep_gain must be of type int or None, but got {type(var)}")
         return True
 
     @classmethod
     def fromdict(cls, values: dict):
         try:
             return cls._fromdict(values)
         except TypeError:
@@ -153,32 +143,28 @@
     @text.setter
     def text(self, var):
         if self._text_validator(var):
             self._text = var
 
     def _processed_text_validator(self, var):
         if type(var) is not str:
-            raise TypeError(
-                f"{var} is not valid. Entity.processed_text must be of type string"
-            )
+            raise TypeError(f"{var} is not valid. Entity.processed_text must be of type string")
         return True
 
     def _text_validator(self, var):
         if type(var) is not str:
             raise TypeError(f"{var} is not valid. Entity.text must be of type string")
         return True
 
     @classmethod
     def fromdict(cls, values: dict):
         try:
             return cls._fromdict(values)
         except TypeError:
-            raise TypeError(
-                "Entity can only accept the values 'processed_text' and 'text'"
-            )
+            raise TypeError("Entity can only accept the values 'processed_text' and 'text'")
 
 
 class EntityTypeSelector(BaseRequestObject):
     valid_types = ["DISABLE", "ENABLE"]
 
     def __init__(self, type: str, value: List[str] = []):
         if self._type_validator(type):
@@ -208,17 +194,15 @@
         return True
 
     @classmethod
     def fromdict(cls, values: dict):
         try:
             return cls._fromdict(values)
         except TypeError:
-            raise TypeError(
-                "EntityTypeSelector can only accept the values 'type' and 'value'"
-            )
+            raise TypeError("EntityTypeSelector can only accept the values 'type' and 'value'")
 
 
 class File(BaseRequestObject):
     valid_content_types = [
         "application/json",
         "application/msword",
         "application/pdf",
@@ -316,25 +300,21 @@
     @property
     def pattern(self):
         return self._pattern
 
     @property
     def entity_type(self):
         if self.type != "BLOCK":
-            raise AttributeError(
-                f"FilterSelector of type {self.type} does not contain entity_type"
-            )
+            raise AttributeError(f"FilterSelector of type {self.type} does not contain entity_type")
         return self._entity_type
 
     @property
     def threshold(self):
         if self.type != "BLOCK":
-            raise AttributeError(
-                f"FilterSelector of type {self.type} does not contain threshold"
-            )
+            raise AttributeError(f"FilterSelector of type {self.type} does not contain threshold")
         return self._threshold
 
     @type.setter
     def type(self, var):
         if self._type_validator(var):
             self._type = var
 
@@ -376,29 +356,27 @@
         return True
 
     @classmethod
     def fromdict(cls, values: dict):
         try:
             return cls._fromdict(values)
         except TypeError:
-            raise TypeError(
-                "FilterSelector can only accept the values 'type' and 'pattern'"
-            )
+            raise TypeError("FilterSelector can only accept the values 'type' and 'pattern'")
 
 
 class PDFOptions(BaseRequestObject):
     default_density = 200
     default_max_resolution = 3000
     default_enable_pdf_text_layer: bool = True
 
     def __init__(
         self,
         density: int = default_density,
         max_resolution: int = default_max_resolution,
-        enable_pdf_text_layer: bool = default_enable_pdf_text_layer
+        enable_pdf_text_layer: bool = default_enable_pdf_text_layer,
     ):
         self._density = density
         self._max_resolution = max_resolution
         self._enable_pdf_text_layer = enable_pdf_text_layer
 
     @property
     def density(self):
@@ -455,48 +433,64 @@
     default_pattern = "[UNIQUE_NUMBERED_ENTITY_TYPE]"
     valid_patterns = [
         "BEST_ENTITY_TYPE",
         "ALL_ENTITY_TYPES",
         "UNIQUE_NUMBERED_ENTITY_TYPE",
         "UNIQUE_HASHED_ENTITY_TYPE",
     ]
+    default_marker_language = "en"
+    valid_marker_languages = ["auto", "en", "fr", "de", "ja", "ko", "nl", "ru", "uk"]
 
-    def __init__(self, pattern: str = default_pattern):
-        for attribute in (
-            ProcessedMaskText.attributes + ProcessedSyntheticText.attributes
-        ):
+    def __init__(self, pattern: str = default_pattern, marker_language: str = default_marker_language):
+        for attribute in ProcessedMaskText.attributes + ProcessedSyntheticText.attributes:
             delattr(self, attribute) if hasattr(self, attribute) else False
         self._type = "MARKER"
         if self._pattern_validator(pattern):
             self._pattern = pattern
+        if self._marker_language_validator(marker_language):
+            self._marker_language = marker_language
 
     @property
     def pattern(self):
         return self._pattern
 
+    @property
+    def marker_language(self):
+        return self._marker_language
+
     @pattern.setter
     def pattern(self, var):
         if self._pattern_validator(var):
             self._pattern = var
 
+    @marker_language.setter
+    def marker_language(self, var):
+        if self._marker_language_validator(var):
+            self._marker_language = var
+
     def _pattern_validator(self, var):
         if var not in self.valid_patterns and var[1:-1] not in self.valid_patterns:
             raise ValueError(
                 f"{var} is not valid. ProcessedText.pattern can only be one of the following: {', '.join(self.valid_patterns)}"
             )
         return True
 
+    def _marker_language_validator(self, var):
+        if var not in self.valid_marker_languages:
+            raise ValueError(
+                f"{var} is not valid. ProcessedText.marker_language can only be one of the following: {', '.join(self.valid_marker_languages)}"
+            )
+        return True
+
 
 class ProcessedMaskText(BaseRequestObject):
     attributes = ["_mask_character"]
 
     def __init__(self, mask_character: str = "#"):
-        for attribute in (
-            ProcessedMarkerText.attributes + ProcessedSyntheticText.attributes
-        ):
+        for attribute in ProcessedMarkerText.attributes + ProcessedSyntheticText.attributes:
             delattr(self, attribute) if hasattr(self, attribute) else False
         if self._mask_character_validator(mask_character):
             self._mask_character = mask_character
         self._type = "MASK"
 
     @property
     def mask_character(self):
@@ -505,17 +499,15 @@
     @mask_character.setter
     def mask_character(self, var):
         if self._mask_character_validator(var):
             self._mask_character = var
 
     def _mask_character_validator(self, var):
         if len(var) != 1:
-            raise ValueError(
-                f"mask_character must have only one character. {var} has {len(var)} characters."
-            )
+            raise ValueError(f"mask_character must have only one character. {var} has {len(var)} characters.")
         return True
 
 
 class ProcessedSyntheticText(BaseRequestObject):
     attributes = ["_synthetic_entity_accuracy", "_preserve_relationships"]
     valid_synthetic_accuracy_values = ["standard", "standard_multilingual"]
 
@@ -573,17 +565,15 @@
             )
 
     @classmethod
     def fromdict(cls, values: dict):
         try:
             return cls._fromdict(values)
         except TypeError:
-            raise TypeError(
-                "ProcessedText can only accept the values 'type' and 'pattern'"
-            )
+            raise TypeError("ProcessedText can only accept the values 'type' and 'pattern'")
 
     @property
     def type(self):
         return self._type
 
     @type.setter
     def type(self, var):
@@ -690,59 +680,45 @@
             raise ValueError(
                 f"{var} is not valid. EntityDetection.accuracy can only be one of the following: {', '.join(self.valid_accuracies)}"
             )
         return True
 
     def _entity_types_validator(self, var):
         if type(var) is not list:
-            raise TypeError(
-                f"{var} is not valid. EntityDetection.entity_types can only be a list"
-            )
+            raise TypeError(f"{var} is not valid. EntityDetection.entity_types can only be a list")
         elif var and not all(isinstance(row, EntityTypeSelector) for row in var):
-            raise ValueError(
-                "EntityDetection.entity_types can only contain EntityTypeSelector objects"
-            )
+            raise ValueError("EntityDetection.entity_types can only contain EntityTypeSelector objects")
         return True
 
     def _filter_validator(self, var):
         if type(var) is not list:
-            raise ValueError(
-                f"{var} is not valid. EntityDetection.filter can only be a list"
-            )
+            raise ValueError(f"{var} is not valid. EntityDetection.filter can only be a list")
         elif var and not all(isinstance(x, FilterSelector) for x in var):
-            raise ValueError(
-                "EntityDetection.filter can only contain FilterSelector objects"
-            )
+            raise ValueError("EntityDetection.filter can only contain FilterSelector objects")
         return True
 
     def _return_entity_validator(self, var):
         if type(var) is not bool:
             raise ValueError("EntityDetection.return_entity must be of type bool")
         return True
 
     def _enable_non_max_suppression_validator(self, var):
         if type(var) is not bool:
-            raise ValueError(
-                "EntityDetection.enable_non_max_suppression must be of type bool"
-            )
+            raise ValueError("EntityDetection.enable_non_max_suppression must be of type bool")
         return True
 
     @classmethod
     def fromdict(cls, values: dict):
         try:
             initializer_dict = {}
             for key, value in values.items():
                 if key == "entity_types":
-                    initializer_dict[key] = [
-                        EntityTypeSelector.fromdict(row) for row in value
-                    ]
+                    initializer_dict[key] = [EntityTypeSelector.fromdict(row) for row in value]
                 elif key == "filter":
-                    initializer_dict[key] = [
-                        FilterSelector.fromdict(row) for row in value
-                    ]
+                    initializer_dict[key] = [FilterSelector.fromdict(row) for row in value]
                 else:
                     initializer_dict[key] = value
             return cls._fromdict(initializer_dict)
         except TypeError:
             raise TypeError(
                 "EntityDetection can only accept the values 'accuracy', 'entity_types', 'filter' and 'return_entity'"
             )
@@ -872,17 +848,15 @@
     def fromdict(cls, values: dict):
         try:
             initializer_dict = {}
             for key, value in values.items():
                 if key == "file":
                     initializer_dict[key] = File.fromdict(value)
                 elif key == "timestamps":
-                    initializer_dict[key] = [
-                        Timestamp.fromdict(entry) for entry in value
-                    ]
+                    initializer_dict[key] = [Timestamp.fromdict(entry) for entry in value]
                 else:
                     initializer_dict[key] = value
             return cls._fromdict(initializer_dict)
         except TypeError:
             raise TypeError(
                 "BleepRequest can only accept the values 'file', 'timestamps', 'bleep_frequency', and 'bleep_gain'"
             )
@@ -903,17 +877,15 @@
 
     @classmethod
     def fromdict(cls, values: dict):
         try:
             initializer_dict = {}
             for key, value in values.items():
                 if key == "entities":
-                    initializer_dict[key] = [
-                        Entity.fromdict(entity) for entity in values[key]
-                    ]
+                    initializer_dict[key] = [Entity.fromdict(entity) for entity in values[key]]
                 else:
                     initializer_dict[key] = value
             return cls._fromdict(initializer_dict)
         except TypeError:
             raise TypeError(
                 "ReidentifyTextRequest can only accept the values 'processed_text', 'entities', 'model' and 'reidentify_sensitive_fields'"
             )
```

### Comparing `privateai_client-3.8.0/src/privateai_client/tests/test_client.py` & `privateai_client-3.8.1/src/privateai_client/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `privateai_client-3.8.0/src/privateai_client/tests/test_integration.py` & `privateai_client-3.8.1/src/privateai_client/tests/test_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,23 @@
 def test_processed_text_marker():
     client = _get_client()
     req = rq.process_text_obj(text=["Hey there!"], processed_text=rq.processed_text_obj(type="MARKER"))
     resp = client.process_text(req)
     assert resp.ok
 
 
+def test_processed_text_marker_language():
+    client = _get_client()
+    req = rq.process_text_obj(
+        text=["Hey there!"], processed_text=rq.processed_text_obj(type="MARKER", marker_language="de")
+    )
+    resp = client.process_text(req)
+    assert resp.ok
+
+
 def test_processed_text_mask():
     client = _get_client()
     req = rq.process_text_obj(text=["Hey there!"], processed_text=rq.processed_text_obj(type="MASK"))
     resp = client.process_text(req)
     assert resp.ok
```

### Comparing `privateai_client-3.8.0/src/privateai_client/tests/test_request_objects.py` & `privateai_client-3.8.1/src/privateai_client/tests/test_request_objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -387,38 +387,43 @@
 def test_processed_text_initializer():
     processed_text = ProcessedText(type="MASK", mask_character="*")
     assert processed_text.type == "MASK"
     assert processed_text.mask_character == "*"
 
 
 def test_processed_text_initialize_fromdict():
-    processed_text = ProcessedText.fromdict({"type": "MARKER", "pattern": "[UNIQUE_NUMBERED_ENTITY_TYPE]"})
+    processed_text = ProcessedText.fromdict(
+        {"type": "MARKER", "pattern": "[UNIQUE_NUMBERED_ENTITY_TYPE]", "marker_language": "fr"}
+    )
     assert processed_text.type == "MARKER"
     assert processed_text.pattern == "[UNIQUE_NUMBERED_ENTITY_TYPE]"
 
 
 def test_processed_text_invalid_initialize_fromdict():
     error_msg = "ProcessedText can only accept the values 'type' and 'pattern'"
     with pytest.raises(TypeError) as excinfo:
         ProcessedText.fromdict(
             {
                 "type": "MARKER",
                 "pattern": "[UNIQUE_NUMBERED_ENTITY_TYPE]",
+                "marker_language": "en",
                 "junk": "value",
             }
         )
     assert error_msg in str(excinfo.value)
 
 
 def test_processed_text_setters():
     processed_text = ProcessedText()
     processed_text.type = "MASK"
     processed_text.pattern = "*ALL_ENTITY_TYPES*"
+    processed_text.marker_language = "de"
     assert processed_text.type == "MASK"
     assert processed_text.pattern == "*ALL_ENTITY_TYPES*"
+    assert processed_text.marker_language == "de"
 
 
 def test_processed_text_type_validator():
     error_msg = "junk is not valid. ProcessedText.type can only be one of the following: "
     with pytest.raises(ValueError) as excinfo:
         ProcessedText.fromdict({"type": "junk", "pattern": "[UNIQUE_NUMBERED_ENTITY_TYPE]"})
     assert error_msg in str(excinfo.value)
@@ -427,14 +432,21 @@
 def test_processed_text_pattern_validator():
     error_msg = "junk is not valid. ProcessedText.pattern can only be one of the following: "
     with pytest.raises(ValueError) as excinfo:
         ProcessedText.fromdict({"type": "MARKER", "pattern": "junk"})
     assert error_msg in str(excinfo.value)
 
 
+def test_processed_text_marker_language_validator():
+    error_msg = "junk is not valid. ProcessedText.marker_language can only be one of the following: "
+    with pytest.raises(ValueError) as excinfo:
+        ProcessedText.fromdict({"type": "MARKER", "marker_language": "junk"})
+    assert error_msg in str(excinfo.value)
+
+
 def test_processed_text_to_dict():
     processed_text = ProcessedText(type="MASK", mask_character="*").to_dict()
     assert processed_text["type"] == "MASK"
     assert processed_text["mask_character"] == "*"
 
 
 # PDF Options Tests
@@ -449,19 +461,20 @@
     pdf_options = PDFOptions(density=300, max_resolution=500, enable_pdf_text_layer=False)
     assert pdf_options.density == 300
     assert pdf_options.max_resolution == 500
     assert pdf_options.enable_pdf_text_layer is False
 
 
 def test_pdf_options_initialize_fromdict():
-    pdf_options = PDFOptions.fromdict({"density": 300, "max_resolution": 500, 'enable_pdf_text_layer': True})
+    pdf_options = PDFOptions.fromdict({"density": 300, "max_resolution": 500, "enable_pdf_text_layer": True})
     assert pdf_options.density == 300
     assert pdf_options.max_resolution == 500
     assert pdf_options.enable_pdf_text_layer is True
 
+
 def test_pdf_options_invalid_initialize_fromdict():
     error_msg = "PDFOptions can only accept 'density', 'max_resolution' and 'enable_pdf_text_layer'"
     with pytest.raises(TypeError) as excinfo:
         PDFOptions.fromdict({"density": 300, "max_resolution": 500, "junk": "value"})
     assert error_msg in str(excinfo.value)
```

### Comparing `privateai_client-3.8.0/src/privateai_client/tests/test_files/simpsons_wiki.txt` & `privateai_client-3.8.1/src/privateai_client/tests/test_files/simpsons_wiki.txt`

 * *Files identical despite different names*

### Comparing `privateai_client-3.8.0/src/privateai_client/tests/test_files/test_audio.mp3` & `privateai_client-3.8.1/src/privateai_client/tests/test_files/test_audio.mp3`

 * *Files identical despite different names*

### Comparing `privateai_client-3.8.0/LICENSE` & `privateai_client-3.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `privateai_client-3.8.0/README.md` & `privateai_client-3.8.1/README.md`

 * *Files identical despite different names*

### Comparing `privateai_client-3.8.0/pyproject.toml` & `privateai_client-3.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `privateai_client-3.8.0/PKG-INFO` & `privateai_client-3.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: privateai_client
-Version: 3.8.0
+Version: 3.8.1
 Summary: A thin client for communicating with the Private AI de-identication API.
 Project-URL: Homepage, https://github.com/privateai/pai-thin-client/
 Project-URL: Bug Tracker, https://github.com/privateai/pai-thin-client/issues
 Project-URL: Changelog, https://github.com/privateai/pai-thin-client/blob/main/CHANGELOG.md
 Project-URL: Contributing, https://github.com/privateai/pai-thin-client/blob/main/CONTRIBUTING.md
 Author-email: Adam Guiducci <adam.guiducci@private-ai.com>, Bryan Bell-Smith <bryan.bellsmith@private-ai.com>
 License-File: LICENSE
```

