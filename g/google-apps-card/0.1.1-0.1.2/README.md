# Comparing `tmp/google-apps-card-0.1.1.tar.gz` & `tmp/google-apps-card-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-apps-card-0.1.1.tar", last modified: Tue Mar  5 18:49:16 2024, max compression
+gzip compressed data, was "google-apps-card-0.1.2.tar", last modified: Tue Apr 16 13:42:06 2024, max compression
```

## Comparing `google-apps-card-0.1.1.tar` & `google-apps-card-0.1.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:49:16.302035 google-apps-card-0.1.1/
--rw-rw-r--   0 root         (0)     1003    11358 2024-03-05 18:46:00.000000 google-apps-card-0.1.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2024-03-05 18:46:00.000000 google-apps-card-0.1.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5046 2024-03-05 18:49:16.302035 google-apps-card-0.1.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3694 2024-03-05 18:46:00.000000 google-apps-card-0.1.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:49:16.294032 google-apps-card-0.1.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:49:16.294032 google-apps-card-0.1.1/google/apps/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:49:16.298033 google-apps-card-0.1.1/google/apps/card/
--rw-rw-r--   0 root         (0)     1003     1437 2024-03-05 18:46:00.000000 google-apps-card-0.1.1/google/apps/card/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2024-03-05 18:46:00.000000 google-apps-card-0.1.1/google/apps/card/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       77 2024-03-05 18:46:00.000000 google-apps-card-0.1.1/google/apps/card/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:49:16.298033 google-apps-card-0.1.1/google/apps/card_v1/
--rw-rw-r--   0 root         (0)     1003     1421 2024-03-05 18:46:00.000000 google-apps-card-0.1.1/google/apps/card_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      227 2024-03-05 18:46:00.000000 google-apps-card-0.1.1/google/apps/card_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-03-05 18:46:00.000000 google-apps-card-0.1.1/google/apps/card_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       77 2024-03-05 18:46:00.000000 google-apps-card-0.1.1/google/apps/card_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:49:16.298033 google-apps-card-0.1.1/google/apps/card_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:00.000000 google-apps-card-0.1.1/google/apps/card_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:49:16.298033 google-apps-card-0.1.1/google/apps/card_v1/types/
--rw-rw-r--   0 root         (0)     1003     1305 2024-03-05 18:46:00.000000 google-apps-card-0.1.1/google/apps/card_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003   101400 2024-03-05 18:46:00.000000 google-apps-card-0.1.1/google/apps/card_v1/types/card.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:49:16.302035 google-apps-card-0.1.1/google_apps_card.egg-info/
--rw-r--r--   0 root         (0)     1003     5046 2024-03-05 18:49:16.000000 google-apps-card-0.1.1/google_apps_card.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003      762 2024-03-05 18:49:16.000000 google-apps-card-0.1.1/google_apps_card.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-05 18:49:16.000000 google-apps-card-0.1.1/google_apps_card.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-05 18:49:16.000000 google-apps-card-0.1.1/google_apps_card.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      305 2024-03-05 18:49:16.000000 google-apps-card-0.1.1/google_apps_card.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-03-05 18:49:16.000000 google-apps-card-0.1.1/google_apps_card.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2024-03-05 18:49:16.302035 google-apps-card-0.1.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3147 2024-03-05 18:46:00.000000 google-apps-card-0.1.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:49:16.302035 google-apps-card-0.1.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:00.000000 google-apps-card-0.1.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:49:16.302035 google-apps-card-0.1.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:00.000000 google-apps-card-0.1.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:49:16.302035 google-apps-card-0.1.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:00.000000 google-apps-card-0.1.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:49:16.302035 google-apps-card-0.1.1/tests/unit/gapic/card_v1/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:00.000000 google-apps-card-0.1.1/tests/unit/gapic/card_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      754 2024-03-05 18:46:00.000000 google-apps-card-0.1.1/tests/unit/gapic/card_v1/test_card.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 13:42:06.400358 google-apps-card-0.1.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-04-16 13:39:06.000000 google-apps-card-0.1.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2024-04-16 13:39:06.000000 google-apps-card-0.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5046 2024-04-16 13:42:06.400358 google-apps-card-0.1.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3694 2024-04-16 13:39:06.000000 google-apps-card-0.1.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 13:42:06.392357 google-apps-card-0.1.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 13:42:06.392357 google-apps-card-0.1.2/google/apps/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 13:42:06.396358 google-apps-card-0.1.2/google/apps/card/
+-rw-rw-r--   0 root         (0)     1003     1475 2024-04-16 13:39:06.000000 google-apps-card-0.1.2/google/apps/card/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2024-04-16 13:39:06.000000 google-apps-card-0.1.2/google/apps/card/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       77 2024-04-16 13:39:06.000000 google-apps-card-0.1.2/google/apps/card/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 13:42:06.396358 google-apps-card-0.1.2/google/apps/card_v1/
+-rw-rw-r--   0 root         (0)     1003     1459 2024-04-16 13:39:06.000000 google-apps-card-0.1.2/google/apps/card_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      227 2024-04-16 13:39:06.000000 google-apps-card-0.1.2/google/apps/card_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-04-16 13:39:06.000000 google-apps-card-0.1.2/google/apps/card_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       77 2024-04-16 13:39:06.000000 google-apps-card-0.1.2/google/apps/card_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 13:42:06.396358 google-apps-card-0.1.2/google/apps/card_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-16 13:39:06.000000 google-apps-card-0.1.2/google/apps/card_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 13:42:06.396358 google-apps-card-0.1.2/google/apps/card_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1343 2024-04-16 13:39:06.000000 google-apps-card-0.1.2/google/apps/card_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003   106228 2024-04-16 13:39:06.000000 google-apps-card-0.1.2/google/apps/card_v1/types/card.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 13:42:06.396358 google-apps-card-0.1.2/google_apps_card.egg-info/
+-rw-r--r--   0 root         (0)     1003     5046 2024-04-16 13:42:06.000000 google-apps-card-0.1.2/google_apps_card.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003      762 2024-04-16 13:42:06.000000 google-apps-card-0.1.2/google_apps_card.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-16 13:42:06.000000 google-apps-card-0.1.2/google_apps_card.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-16 13:42:06.000000 google-apps-card-0.1.2/google_apps_card.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      305 2024-04-16 13:42:06.000000 google-apps-card-0.1.2/google_apps_card.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-04-16 13:42:06.000000 google-apps-card-0.1.2/google_apps_card.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2024-04-16 13:42:06.400358 google-apps-card-0.1.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3147 2024-04-16 13:39:06.000000 google-apps-card-0.1.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 13:42:06.396358 google-apps-card-0.1.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-16 13:39:06.000000 google-apps-card-0.1.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 13:42:06.396358 google-apps-card-0.1.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-16 13:39:06.000000 google-apps-card-0.1.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 13:42:06.396358 google-apps-card-0.1.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-16 13:39:06.000000 google-apps-card-0.1.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 13:42:06.400358 google-apps-card-0.1.2/tests/unit/gapic/card_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-16 13:39:06.000000 google-apps-card-0.1.2/tests/unit/gapic/card_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      754 2024-04-16 13:39:06.000000 google-apps-card-0.1.2/tests/unit/gapic/card_v1/test_card.py
```

### Comparing `google-apps-card-0.1.1/LICENSE` & `google-apps-card-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-apps-card-0.1.1/MANIFEST.in` & `google-apps-card-0.1.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-apps-card-0.1.1/PKG-INFO` & `google-apps-card-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-apps-card
-Version: 0.1.1
+Version: 0.1.2
 Summary: Google Apps Card API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-apps-card
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-apps-card-0.1.1/README.rst` & `google-apps-card-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `google-apps-card-0.1.1/google/apps/card/__init__.py` & `google-apps-card-0.1.2/google/apps/card_v1/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from google.apps.card import gapic_version as package_version
+from google.apps.card_v1 import gapic_version as package_version
 
 __version__ = package_version.__version__
 
 
-from google.apps.card_v1.types.card import (
+from .types.card import (
     Action,
     BorderStyle,
     Button,
     ButtonList,
     Card,
     Columns,
     DateTimePicker,
     DecoratedText,
     Divider,
     Grid,
     Icon,
     Image,
     ImageComponent,
     ImageCropStyle,
+    MaterialIcon,
     OnClick,
     OpenLink,
     SelectionInput,
     Suggestions,
     TextInput,
     TextParagraph,
     Widget,
@@ -53,14 +54,15 @@
     "DecoratedText",
     "Divider",
     "Grid",
     "Icon",
     "Image",
     "ImageComponent",
     "ImageCropStyle",
+    "MaterialIcon",
     "OnClick",
     "OpenLink",
     "SelectionInput",
     "Suggestions",
     "TextInput",
     "TextParagraph",
     "Widget",
```

### Comparing `google-apps-card-0.1.1/google/apps/card/gapic_version.py` & `google-apps-card-0.1.2/google/apps/card/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.1"  # {x-release-please-version}
+__version__ = "0.1.2"  # {x-release-please-version}
```

### Comparing `google-apps-card-0.1.1/google/apps/card_v1/__init__.py` & `google-apps-card-0.1.2/google/apps/card/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from google.apps.card_v1 import gapic_version as package_version
+from google.apps.card import gapic_version as package_version
 
 __version__ = package_version.__version__
 
 
-from .types.card import (
+from google.apps.card_v1.types.card import (
     Action,
     BorderStyle,
     Button,
     ButtonList,
     Card,
     Columns,
     DateTimePicker,
     DecoratedText,
     Divider,
     Grid,
     Icon,
     Image,
     ImageComponent,
     ImageCropStyle,
+    MaterialIcon,
     OnClick,
     OpenLink,
     SelectionInput,
     Suggestions,
     TextInput,
     TextParagraph,
     Widget,
@@ -53,14 +54,15 @@
     "DecoratedText",
     "Divider",
     "Grid",
     "Icon",
     "Image",
     "ImageComponent",
     "ImageCropStyle",
+    "MaterialIcon",
     "OnClick",
     "OpenLink",
     "SelectionInput",
     "Suggestions",
     "TextInput",
     "TextParagraph",
     "Widget",
```

### Comparing `google-apps-card-0.1.1/google/apps/card_v1/gapic_version.py` & `google-apps-card-0.1.2/google/apps/card_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.1"  # {x-release-please-version}
+__version__ = "0.1.2"  # {x-release-please-version}
```

### Comparing `google-apps-card-0.1.1/google/apps/card_v1/services/__init__.py` & `google-apps-card-0.1.2/google/apps/card_v1/services/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-apps-card-0.1.1/google/apps/card_v1/types/__init__.py` & `google-apps-card-0.1.2/google/apps/card_v1/types/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -24,14 +24,15 @@
     DecoratedText,
     Divider,
     Grid,
     Icon,
     Image,
     ImageComponent,
     ImageCropStyle,
+    MaterialIcon,
     OnClick,
     OpenLink,
     SelectionInput,
     Suggestions,
     TextInput,
     TextParagraph,
     Widget,
@@ -48,14 +49,15 @@
     "DecoratedText",
     "Divider",
     "Grid",
     "Icon",
     "Image",
     "ImageComponent",
     "ImageCropStyle",
+    "MaterialIcon",
     "OnClick",
     "OpenLink",
     "SelectionInput",
     "Suggestions",
     "TextInput",
     "TextParagraph",
     "Widget",
```

### Comparing `google-apps-card-0.1.1/google/apps/card_v1/types/card.py` & `google-apps-card-0.1.2/google/apps/card_v1/types/card.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
 00000010: 662d 3820 2d2a 2d0a 2320 436f 7079 7269  f-8 -*-.# Copyri
-00000020: 6768 7420 3230 3233 2047 6f6f 676c 6520  ght 2023 Google 
+00000020: 6768 7420 3230 3234 2047 6f6f 676c 6520  ght 2024 Google 
 00000030: 4c4c 430a 230a 2320 4c69 6365 6e73 6564  LLC.#.# Licensed
 00000040: 2075 6e64 6572 2074 6865 2041 7061 6368   under the Apach
 00000050: 6520 4c69 6365 6e73 652c 2056 6572 7369  e License, Versi
 00000060: 6f6e 2032 2e30 2028 7468 6520 224c 6963  on 2.0 (the "Lic
 00000070: 656e 7365 2229 3b0a 2320 796f 7520 6d61  ense");.# you ma
 00000080: 7920 6e6f 7420 7573 6520 7468 6973 2066  y not use this f
 00000090: 696c 6520 6578 6365 7074 2069 6e20 636f  ile except in co
@@ -64,6275 +64,6577 @@
 000003f0: 222c 0a20 2020 2020 2020 2022 4275 7474  ",.        "Butt
 00000400: 6f6e 4c69 7374 222c 0a20 2020 2020 2020  onList",.       
 00000410: 2022 5365 6c65 6374 696f 6e49 6e70 7574   "SelectionInput
 00000420: 222c 0a20 2020 2020 2020 2022 4461 7465  ",.        "Date
 00000430: 5469 6d65 5069 636b 6572 222c 0a20 2020  TimePicker",.   
 00000440: 2020 2020 2022 4275 7474 6f6e 222c 0a20       "Button",. 
 00000450: 2020 2020 2020 2022 4963 6f6e 222c 0a20         "Icon",. 
-00000460: 2020 2020 2020 2022 496d 6167 6543 726f         "ImageCro
-00000470: 7053 7479 6c65 222c 0a20 2020 2020 2020  pStyle",.       
-00000480: 2022 426f 7264 6572 5374 796c 6522 2c0a   "BorderStyle",.
-00000490: 2020 2020 2020 2020 2249 6d61 6765 436f          "ImageCo
-000004a0: 6d70 6f6e 656e 7422 2c0a 2020 2020 2020  mponent",.      
-000004b0: 2020 2247 7269 6422 2c0a 2020 2020 2020    "Grid",.      
-000004c0: 2020 2243 6f6c 756d 6e73 222c 0a20 2020    "Columns",.   
-000004d0: 2020 2020 2022 4f6e 436c 6963 6b22 2c0a       "OnClick",.
-000004e0: 2020 2020 2020 2020 224f 7065 6e4c 696e          "OpenLin
-000004f0: 6b22 2c0a 2020 2020 2020 2020 2241 6374  k",.        "Act
-00000500: 696f 6e22 2c0a 2020 2020 7d2c 0a29 0a0a  ion",.    },.)..
-00000510: 0a63 6c61 7373 2043 6172 6428 7072 6f74  .class Card(prot
-00000520: 6f2e 4d65 7373 6167 6529 3a0a 2020 2020  o.Message):.    
-00000530: 7222 2222 4120 6361 7264 2069 6e74 6572  r"""A card inter
-00000540: 6661 6365 2064 6973 706c 6179 6564 2069  face displayed i
-00000550: 6e20 6120 476f 6f67 6c65 2043 6861 7420  n a Google Chat 
-00000560: 6d65 7373 6167 6520 6f72 2047 6f6f 676c  message or Googl
-00000570: 650a 2020 2020 576f 726b 7370 6163 6520  e.    Workspace 
-00000580: 4164 642d 6f6e 2e0a 0a20 2020 2043 6172  Add-on...    Car
-00000590: 6473 2073 7570 706f 7274 2061 2064 6566  ds support a def
-000005a0: 696e 6564 206c 6179 6f75 742c 2069 6e74  ined layout, int
-000005b0: 6572 6163 7469 7665 2055 4920 656c 656d  eractive UI elem
-000005c0: 656e 7473 206c 696b 650a 2020 2020 6275  ents like.    bu
-000005d0: 7474 6f6e 732c 2061 6e64 2072 6963 6820  ttons, and rich 
-000005e0: 6d65 6469 6120 6c69 6b65 2069 6d61 6765  media like image
-000005f0: 732e 2055 7365 2063 6172 6473 2074 6f20  s. Use cards to 
-00000600: 7072 6573 656e 7420 6465 7461 696c 6564  present detailed
-00000610: 0a20 2020 2069 6e66 6f72 6d61 7469 6f6e  .    information
-00000620: 2c20 6761 7468 6572 2069 6e66 6f72 6d61  , gather informa
-00000630: 7469 6f6e 2066 726f 6d20 7573 6572 732c  tion from users,
-00000640: 2061 6e64 2067 7569 6465 2075 7365 7273   and guide users
-00000650: 2074 6f20 7461 6b65 0a20 2020 2061 206e   to take.    a n
-00000660: 6578 7420 7374 6570 2e0a 0a20 2020 2060  ext step...    `
-00000670: 4361 7264 2062 7569 6c64 6572 203c 6874  Card builder <ht
-00000680: 7470 733a 2f2f 6164 646f 6e73 2e67 7375  tps://addons.gsu
-00000690: 6974 652e 676f 6f67 6c65 2e63 6f6d 2f75  ite.google.com/u
-000006a0: 696b 6974 2f62 7569 6c64 6572 3e60 5f5f  ikit/builder>`__
-000006b0: 0a0a 2020 2020 546f 206c 6561 726e 2068  ..    To learn h
-000006c0: 6f77 2074 6f20 6275 696c 6420 6361 7264  ow to build card
-000006d0: 732c 2073 6565 2074 6865 2066 6f6c 6c6f  s, see the follo
-000006e0: 7769 6e67 2064 6f63 756d 656e 7461 7469  wing documentati
-000006f0: 6f6e 3a0a 0a20 2020 202d 2020 466f 7220  on:..    -  For 
-00000700: 476f 6f67 6c65 2043 6861 7420 6170 7073  Google Chat apps
-00000710: 2c20 7365 6520 6044 6573 6967 6e20 6479  , see `Design dy
-00000720: 6e61 6d69 632c 2069 6e74 6572 6163 7469  namic, interacti
-00000730: 7665 2c20 616e 640a 2020 2020 2020 2063  ve, and.       c
-00000740: 6f6e 7369 7374 656e 7420 5549 7320 7769  onsistent UIs wi
-00000750: 7468 0a20 2020 2020 2020 6361 7264 7320  th.       cards 
+00000460: 2020 2020 2020 2022 4d61 7465 7269 616c         "Material
+00000470: 4963 6f6e 222c 0a20 2020 2020 2020 2022  Icon",.        "
+00000480: 496d 6167 6543 726f 7053 7479 6c65 222c  ImageCropStyle",
+00000490: 0a20 2020 2020 2020 2022 426f 7264 6572  .        "Border
+000004a0: 5374 796c 6522 2c0a 2020 2020 2020 2020  Style",.        
+000004b0: 2249 6d61 6765 436f 6d70 6f6e 656e 7422  "ImageComponent"
+000004c0: 2c0a 2020 2020 2020 2020 2247 7269 6422  ,.        "Grid"
+000004d0: 2c0a 2020 2020 2020 2020 2243 6f6c 756d  ,.        "Colum
+000004e0: 6e73 222c 0a20 2020 2020 2020 2022 4f6e  ns",.        "On
+000004f0: 436c 6963 6b22 2c0a 2020 2020 2020 2020  Click",.        
+00000500: 224f 7065 6e4c 696e 6b22 2c0a 2020 2020  "OpenLink",.    
+00000510: 2020 2020 2241 6374 696f 6e22 2c0a 2020      "Action",.  
+00000520: 2020 7d2c 0a29 0a0a 0a63 6c61 7373 2043    },.)...class C
+00000530: 6172 6428 7072 6f74 6f2e 4d65 7373 6167  ard(proto.Messag
+00000540: 6529 3a0a 2020 2020 7222 2222 4120 6361  e):.    r"""A ca
+00000550: 7264 2069 6e74 6572 6661 6365 2064 6973  rd interface dis
+00000560: 706c 6179 6564 2069 6e20 6120 476f 6f67  played in a Goog
+00000570: 6c65 2043 6861 7420 6d65 7373 6167 6520  le Chat message 
+00000580: 6f72 2047 6f6f 676c 650a 2020 2020 576f  or Google.    Wo
+00000590: 726b 7370 6163 6520 4164 642d 6f6e 2e0a  rkspace Add-on..
+000005a0: 0a20 2020 2043 6172 6473 2073 7570 706f  .    Cards suppo
+000005b0: 7274 2061 2064 6566 696e 6564 206c 6179  rt a defined lay
+000005c0: 6f75 742c 2069 6e74 6572 6163 7469 7665  out, interactive
+000005d0: 2055 4920 656c 656d 656e 7473 206c 696b   UI elements lik
+000005e0: 650a 2020 2020 6275 7474 6f6e 732c 2061  e.    buttons, a
+000005f0: 6e64 2072 6963 6820 6d65 6469 6120 6c69  nd rich media li
+00000600: 6b65 2069 6d61 6765 732e 2055 7365 2063  ke images. Use c
+00000610: 6172 6473 2074 6f20 7072 6573 656e 7420  ards to present 
+00000620: 6465 7461 696c 6564 0a20 2020 2069 6e66  detailed.    inf
+00000630: 6f72 6d61 7469 6f6e 2c20 6761 7468 6572  ormation, gather
+00000640: 2069 6e66 6f72 6d61 7469 6f6e 2066 726f   information fro
+00000650: 6d20 7573 6572 732c 2061 6e64 2067 7569  m users, and gui
+00000660: 6465 2075 7365 7273 2074 6f20 7461 6b65  de users to take
+00000670: 0a20 2020 2061 206e 6578 7420 7374 6570  .    a next step
+00000680: 2e0a 0a20 2020 2060 4361 7264 2062 7569  ...    `Card bui
+00000690: 6c64 6572 203c 6874 7470 733a 2f2f 6164  lder <https://ad
+000006a0: 646f 6e73 2e67 7375 6974 652e 676f 6f67  dons.gsuite.goog
+000006b0: 6c65 2e63 6f6d 2f75 696b 6974 2f62 7569  le.com/uikit/bui
+000006c0: 6c64 6572 3e60 5f5f 0a0a 2020 2020 546f  lder>`__..    To
+000006d0: 206c 6561 726e 2068 6f77 2074 6f20 6275   learn how to bu
+000006e0: 696c 6420 6361 7264 732c 2073 6565 2074  ild cards, see t
+000006f0: 6865 2066 6f6c 6c6f 7769 6e67 2064 6f63  he following doc
+00000700: 756d 656e 7461 7469 6f6e 3a0a 0a20 2020  umentation:..   
+00000710: 202d 2020 466f 7220 476f 6f67 6c65 2043   -  For Google C
+00000720: 6861 7420 6170 7073 2c20 7365 6520 6044  hat apps, see `D
+00000730: 6573 6967 6e20 7468 6520 636f 6d70 6f6e  esign the compon
+00000740: 656e 7473 206f 6620 6120 6361 7264 206f  ents of a card o
+00000750: 720a 2020 2020 2020 2064 6961 6c6f 6720  r.       dialog 
 00000760: 3c68 7474 7073 3a2f 2f64 6576 656c 6f70  <https://develop
-00000770: 6572 732e 676f 6f67 6c65 2e63 6f6d 2f63  ers.google.com/c
-00000780: 6861 742f 7569 3e60 5f5f 2e0a 2020 2020  hat/ui>`__..    
-00000790: 2d20 2046 6f72 2047 6f6f 676c 6520 576f  -  For Google Wo
-000007a0: 726b 7370 6163 6520 4164 642d 6f6e 732c  rkspace Add-ons,
-000007b0: 2073 6565 2060 4361 7264 2d62 6173 6564   see `Card-based
-000007c0: 0a20 2020 2020 2020 696e 7465 7266 6163  .       interfac
-000007d0: 6573 203c 6874 7470 733a 2f2f 6465 7665  es <https://deve
-000007e0: 6c6f 7065 7273 2e67 6f6f 676c 652e 636f  lopers.google.co
-000007f0: 6d2f 6170 7073 2d73 6372 6970 742f 6164  m/apps-script/ad
-00000800: 642d 6f6e 732f 636f 6e63 6570 7473 2f63  d-ons/concepts/c
-00000810: 6172 6473 3e60 5f5f 2e0a 0a20 2020 202a  ards>`__...    *
-00000820: 2a45 7861 6d70 6c65 3a20 4361 7264 206d  *Example: Card m
-00000830: 6573 7361 6765 2066 6f72 2061 2047 6f6f  essage for a Goo
-00000840: 676c 6520 4368 6174 2061 7070 2a2a 0a0a  gle Chat app**..
-00000850: 2020 2020 7c45 7861 6d70 6c65 2063 6f6e      |Example con
-00000860: 7461 6374 2063 6172 647c 0a0a 2020 2020  tact card|..    
-00000870: 546f 2063 7265 6174 6520 7468 6520 7361  To create the sa
-00000880: 6d70 6c65 2063 6172 6420 6d65 7373 6167  mple card messag
-00000890: 6520 696e 2047 6f6f 676c 6520 4368 6174  e in Google Chat
-000008a0: 2c20 7573 6520 7468 6520 666f 6c6c 6f77  , use the follow
-000008b0: 696e 670a 2020 2020 4a53 4f4e 3a0a 0a20  ing.    JSON:.. 
-000008c0: 2020 203a 3a0a 0a20 2020 2020 2020 7b0a     ::..       {.
-000008d0: 2020 2020 2020 2020 2022 6361 7264 7356           "cardsV
-000008e0: 3222 3a20 5b0a 2020 2020 2020 2020 2020  2": [.          
-000008f0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00000900: 2263 6172 6449 6422 3a20 2275 6e69 7175  "cardId": "uniqu
-00000910: 652d 6361 7264 2d69 6422 2c0a 2020 2020  e-card-id",.    
-00000920: 2020 2020 2020 2020 2022 6361 7264 223a           "card":
-00000930: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00000940: 2020 2268 6561 6465 7222 3a20 7b0a 2020    "header": {.  
-00000950: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000960: 7469 746c 6522 3a20 2253 6173 6861 222c  title": "Sasha",
-00000970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000980: 2020 2273 7562 7469 746c 6522 3a20 2253    "subtitle": "S
-00000990: 6f66 7477 6172 6520 456e 6769 6e65 6572  oftware Engineer
-000009a0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-000009b0: 2020 2020 2269 6d61 6765 5572 6c22 3a0a      "imageUrl":.
-000009c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009d0: 2022 6874 7470 733a 2f2f 6465 7665 6c6f   "https://develo
-000009e0: 7065 7273 2e67 6f6f 676c 652e 636f 6d2f  pers.google.com/
-000009f0: 6368 6174 2f69 6d61 6765 732f 7175 6963  chat/images/quic
-00000a00: 6b73 7461 7274 2d61 7070 2d61 7661 7461  kstart-app-avata
-00000a10: 722e 706e 6722 2c0a 2020 2020 2020 2020  r.png",.        
-00000a20: 2020 2020 2020 2020 2022 696d 6167 6554           "imageT
-00000a30: 7970 6522 3a20 2243 4952 434c 4522 2c0a  ype": "CIRCLE",.
-00000a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a50: 2022 696d 6167 6541 6c74 5465 7874 223a   "imageAltText":
-00000a60: 2022 4176 6174 6172 2066 6f72 2053 6173   "Avatar for Sas
-00000a70: 6861 222c 0a20 2020 2020 2020 2020 2020  ha",.           
-00000a80: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-00000a90: 2020 2020 2020 2273 6563 7469 6f6e 7322        "sections"
-00000aa0: 3a20 5b0a 2020 2020 2020 2020 2020 2020  : [.            
-00000ab0: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
-00000ac0: 2020 2020 2020 2020 2020 2268 6561 6465            "heade
-00000ad0: 7222 3a20 2243 6f6e 7461 6374 2049 6e66  r": "Contact Inf
-00000ae0: 6f22 2c0a 2020 2020 2020 2020 2020 2020  o",.            
-00000af0: 2020 2020 2020 2022 636f 6c6c 6170 7369         "collapsi
-00000b00: 626c 6522 3a20 7472 7565 2c0a 2020 2020  ble": true,.    
-00000b10: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000b20: 756e 636f 6c6c 6170 7369 626c 6557 6964  uncollapsibleWid
-00000b30: 6765 7473 436f 756e 7422 3a20 312c 0a20  getsCount": 1,. 
-00000b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b50: 2020 2277 6964 6765 7473 223a 205b 0a20    "widgets": [. 
-00000b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b70: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-00000b80: 2020 2020 2020 2020 2020 2020 2022 6465               "de
-00000b90: 636f 7261 7465 6454 6578 7422 3a20 7b0a  coratedText": {.
+00000770: 6572 732e 676f 6f67 6c65 2e63 6f6d 2f77  ers.google.com/w
+00000780: 6f72 6b73 7061 6365 2f63 6861 742f 6465  orkspace/chat/de
+00000790: 7369 676e 2d63 6f6d 706f 6e65 6e74 732d  sign-components-
+000007a0: 6361 7264 2d64 6961 6c6f 673e 605f 5f2e  card-dialog>`__.
+000007b0: 0a20 2020 202d 2020 466f 7220 476f 6f67  .    -  For Goog
+000007c0: 6c65 2057 6f72 6b73 7061 6365 2041 6464  le Workspace Add
+000007d0: 2d6f 6e73 2c20 7365 6520 6043 6172 642d  -ons, see `Card-
+000007e0: 6261 7365 640a 2020 2020 2020 2069 6e74  based.       int
+000007f0: 6572 6661 6365 7320 3c68 7474 7073 3a2f  erfaces <https:/
+00000800: 2f64 6576 656c 6f70 6572 732e 676f 6f67  /developers.goog
+00000810: 6c65 2e63 6f6d 2f61 7070 732d 7363 7269  le.com/apps-scri
+00000820: 7074 2f61 6464 2d6f 6e73 2f63 6f6e 6365  pt/add-ons/conce
+00000830: 7074 732f 6361 7264 733e 605f 5f2e 0a0a  pts/cards>`__...
+00000840: 2020 2020 2a2a 4578 616d 706c 653a 2043      **Example: C
+00000850: 6172 6420 6d65 7373 6167 6520 666f 7220  ard message for 
+00000860: 6120 476f 6f67 6c65 2043 6861 7420 6170  a Google Chat ap
+00000870: 702a 2a0a 0a20 2020 207c 4578 616d 706c  p**..    |Exampl
+00000880: 6520 636f 6e74 6163 7420 6361 7264 7c0a  e contact card|.
+00000890: 0a20 2020 2054 6f20 6372 6561 7465 2074  .    To create t
+000008a0: 6865 2073 616d 706c 6520 6361 7264 206d  he sample card m
+000008b0: 6573 7361 6765 2069 6e20 476f 6f67 6c65  essage in Google
+000008c0: 2043 6861 742c 2075 7365 2074 6865 2066   Chat, use the f
+000008d0: 6f6c 6c6f 7769 6e67 0a20 2020 204a 534f  ollowing.    JSO
+000008e0: 4e3a 0a0a 2020 2020 3a3a 0a0a 2020 2020  N:..    ::..    
+000008f0: 2020 207b 0a20 2020 2020 2020 2020 2263     {.         "c
+00000900: 6172 6473 5632 223a 205b 0a20 2020 2020  ardsV2": [.     
+00000910: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00000920: 2020 2020 2022 6361 7264 4964 223a 2022       "cardId": "
+00000930: 756e 6971 7565 2d63 6172 642d 6964 222c  unique-card-id",
+00000940: 0a20 2020 2020 2020 2020 2020 2020 2263  .             "c
+00000950: 6172 6422 3a20 7b0a 2020 2020 2020 2020  ard": {.        
+00000960: 2020 2020 2020 2022 6865 6164 6572 223a         "header":
+00000970: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00000980: 2020 2020 2022 7469 746c 6522 3a20 2253       "title": "S
+00000990: 6173 6861 222c 0a20 2020 2020 2020 2020  asha",.         
+000009a0: 2020 2020 2020 2020 2022 7375 6274 6974           "subtit
+000009b0: 6c65 223a 2022 536f 6674 7761 7265 2045  le": "Software E
+000009c0: 6e67 696e 6565 7222 2c0a 2020 2020 2020  ngineer",.      
+000009d0: 2020 2020 2020 2020 2020 2020 2269 6d61              "ima
+000009e0: 6765 5572 6c22 3a0a 2020 2020 2020 2020  geUrl":.        
+000009f0: 2020 2020 2020 2020 2020 2268 7474 7073            "https
+00000a00: 3a2f 2f64 6576 656c 6f70 6572 732e 676f  ://developers.go
+00000a10: 6f67 6c65 2e63 6f6d 2f77 6f72 6b73 7061  ogle.com/workspa
+00000a20: 6365 2f63 6861 742f 696d 6167 6573 2f71  ce/chat/images/q
+00000a30: 7569 636b 7374 6172 742d 6170 702d 6176  uickstart-app-av
+00000a40: 6174 6172 2e70 6e67 222c 0a20 2020 2020  atar.png",.     
+00000a50: 2020 2020 2020 2020 2020 2020 2022 696d               "im
+00000a60: 6167 6554 7970 6522 3a20 2243 4952 434c  ageType": "CIRCL
+00000a70: 4522 2c0a 2020 2020 2020 2020 2020 2020  E",.            
+00000a80: 2020 2020 2020 2269 6d61 6765 416c 7454        "imageAltT
+00000a90: 6578 7422 3a20 2241 7661 7461 7220 666f  ext": "Avatar fo
+00000aa0: 7220 5361 7368 6122 0a20 2020 2020 2020  r Sasha".       
+00000ab0: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+00000ac0: 2020 2020 2020 2020 2020 2020 2273 6563              "sec
+00000ad0: 7469 6f6e 7322 3a20 5b0a 2020 2020 2020  tions": [.      
+00000ae0: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
+00000af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b00: 2020 2268 6561 6465 7222 3a20 2243 6f6e    "header": "Con
+00000b10: 7461 6374 2049 6e66 6f22 2c0a 2020 2020  tact Info",.    
+00000b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b30: 2263 6f6c 6c61 7073 6962 6c65 223a 2074  "collapsible": t
+00000b40: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+00000b50: 2020 2020 2020 2020 2022 756e 636f 6c6c           "uncoll
+00000b60: 6170 7369 626c 6557 6964 6765 7473 436f  apsibleWidgetsCo
+00000b70: 756e 7422 3a20 312c 0a20 2020 2020 2020  unt": 1,.       
+00000b80: 2020 2020 2020 2020 2020 2020 2022 7769               "wi
+00000b90: 6467 6574 7322 3a20 5b0a 2020 2020 2020  dgets": [.      
 00000ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000bb0: 2020 2020 2020 2020 2022 7374 6172 7449           "startI
-00000bc0: 636f 6e22 3a20 7b0a 2020 2020 2020 2020  con": {.        
-00000bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000be0: 2020 2022 6b6e 6f77 6e49 636f 6e22 3a20     "knownIcon": 
-00000bf0: 2245 4d41 494c 222c 0a20 2020 2020 2020  "EMAIL",.       
-00000c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c10: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-00000c20: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-00000c30: 6578 7422 3a20 2273 6173 6861 4065 7861  ext": "sasha@exa
-00000c40: 6d70 6c65 2e63 6f6d 222c 0a20 2020 2020  mple.com",.     
-00000c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c60: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
-00000c70: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00000c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c90: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00000ca0: 2020 2020 2020 2020 2020 2264 6563 6f72            "decor
-00000cb0: 6174 6564 5465 7874 223a 207b 0a20 2020  atedText": {.   
+00000bb0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00000bc0: 2020 2020 2020 2020 2020 2264 6563 6f72            "decor
+00000bd0: 6174 6564 5465 7874 223a 207b 0a20 2020  atedText": {.   
+00000be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000bf0: 2020 2020 2020 2022 7374 6172 7449 636f         "startIco
+00000c00: 6e22 3a20 7b0a 2020 2020 2020 2020 2020  n": {.          
+00000c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c20: 2020 226b 6e6f 776e 4963 6f6e 223a 2022    "knownIcon": "
+00000c30: 454d 4149 4c22 0a20 2020 2020 2020 2020  EMAIL".         
+00000c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c50: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
+00000c60: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+00000c70: 6578 7422 3a20 2273 6173 6861 4065 7861  ext": "sasha@exa
+00000c80: 6d70 6c65 2e63 6f6d 220a 2020 2020 2020  mple.com".      
+00000c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ca0: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
+00000cb0: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
 00000cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000cd0: 2020 2020 2020 2273 7461 7274 4963 6f6e        "startIcon
-00000ce0: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-00000cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d00: 226b 6e6f 776e 4963 6f6e 223a 2022 5045  "knownIcon": "PE
-00000d10: 5253 4f4e 222c 0a20 2020 2020 2020 2020  RSON",.         
-00000d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d30: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-00000d40: 2020 2020 2020 2020 2020 2020 2274 6578              "tex
-00000d50: 7422 3a20 223c 666f 6e74 2063 6f6c 6f72  t": "<font color
-00000d60: 3d5c 2223 3830 6532 3765 5c22 3e4f 6e6c  =\"#80e27e\">Onl
-00000d70: 696e 653c 2f66 6f6e 743e 222c 0a20 2020  ine</font>",.   
+00000cd0: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
+00000ce0: 2020 2020 2020 2020 2020 2020 2022 6465               "de
+00000cf0: 636f 7261 7465 6454 6578 7422 3a20 7b0a  coratedText": {.
+00000d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d10: 2020 2020 2020 2020 2020 2273 7461 7274            "start
+00000d20: 4963 6f6e 223a 207b 0a20 2020 2020 2020  Icon": {.       
+00000d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d40: 2020 2020 2022 6b6e 6f77 6e49 636f 6e22       "knownIcon"
+00000d50: 3a20 2250 4552 534f 4e22 0a20 2020 2020  : "PERSON".     
+00000d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d70: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
 00000d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d90: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-00000da0: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-00000db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000dc0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-00000dd0: 2020 2020 2020 2020 2020 2020 2022 6465               "de
-00000de0: 636f 7261 7465 6454 6578 7422 3a20 7b0a  coratedText": {.
-00000df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e00: 2020 2020 2020 2020 2022 7374 6172 7449           "startI
-00000e10: 636f 6e22 3a20 7b0a 2020 2020 2020 2020  con": {.        
-00000e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e30: 2020 2022 6b6e 6f77 6e49 636f 6e22 3a20     "knownIcon": 
-00000e40: 2250 484f 4e45 222c 0a20 2020 2020 2020  "PHONE",.       
-00000e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e60: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-00000e70: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-00000e80: 6578 7422 3a20 222b 3120 2835 3535 2920  ext": "+1 (555) 
-00000e90: 3535 352d 3132 3334 222c 0a20 2020 2020  555-1234",.     
-00000ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000eb0: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
-00000ec0: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00000ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ee0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00000ef0: 2020 2020 2020 2020 2020 2262 7574 746f            "butto
-00000f00: 6e4c 6973 7422 3a20 7b0a 2020 2020 2020  nList": {.      
-00000f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f20: 2020 2022 6275 7474 6f6e 7322 3a20 5b0a     "buttons": [.
+00000d90: 2020 2274 6578 7422 3a20 223c 666f 6e74    "text": "<font
+00000da0: 2063 6f6c 6f72 3d5c 2223 3830 6532 3765   color=\"#80e27e
+00000db0: 5c22 3e4f 6e6c 696e 653c 2f66 6f6e 743e  \">Online</font>
+00000dc0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00000dd0: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00000de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000df0: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
+00000e00: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
+00000e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e20: 2020 2020 2022 6465 636f 7261 7465 6454       "decoratedT
+00000e30: 6578 7422 3a20 7b0a 2020 2020 2020 2020  ext": {.        
+00000e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e50: 2020 2273 7461 7274 4963 6f6e 223a 207b    "startIcon": {
+00000e60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000e70: 2020 2020 2020 2020 2020 2020 2022 6b6e               "kn
+00000e80: 6f77 6e49 636f 6e22 3a20 2250 484f 4e45  ownIcon": "PHONE
+00000e90: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00000ea0: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+00000eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ec0: 2020 2020 2020 2020 2022 7465 7874 223a           "text":
+00000ed0: 2022 2b31 2028 3535 3529 2035 3535 2d31   "+1 (555) 555-1
+00000ee0: 3233 3422 0a20 2020 2020 2020 2020 2020  234".           
+00000ef0: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
+00000f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f10: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00000f20: 2020 2020 2020 2020 2020 2020 2020 7b0a                {.
 00000f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f40: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
-00000f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f60: 2020 2020 2020 2020 2020 2274 6578 7422            "text"
-00000f70: 3a20 2253 6861 7265 222c 0a20 2020 2020  : "Share",.     
+00000f40: 2020 2020 2020 2020 2262 7574 746f 6e4c          "buttonL
+00000f50: 6973 7422 3a20 7b0a 2020 2020 2020 2020  ist": {.        
+00000f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f70: 2020 2262 7574 746f 6e73 223a 205b 0a20    "buttons": [. 
 00000f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f90: 2020 2020 2020 2020 226f 6e43 6c69 636b          "onClick
-00000fa0: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-00000fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fc0: 2020 2020 226f 7065 6e4c 696e 6b22 3a20      "openLink": 
-00000fd0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00000fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ff0: 2020 2022 7572 6c22 3a20 2268 7474 7073     "url": "https
-00001000: 3a2f 2f65 7861 6d70 6c65 2e63 6f6d 2f73  ://example.com/s
-00001010: 6861 7265 222c 0a20 2020 2020 2020 2020  hare",.         
-00001020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001030: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00001040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001050: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
-00001060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001070: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-00001080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001090: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-000010a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000010b0: 7465 7874 223a 2022 4564 6974 222c 0a20  text": "Edit",. 
-000010c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010d0: 2020 2020 2020 2020 2020 2020 226f 6e43              "onC
-000010e0: 6c69 636b 223a 207b 0a20 2020 2020 2020  lick": {.       
+00000f90: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
+00000fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000fb0: 2020 2020 2020 2020 2020 2022 7465 7874             "text
+00000fc0: 223a 2022 5368 6172 6522 2c0a 2020 2020  ": "Share",.    
+00000fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000fe0: 2020 2020 2020 2020 2020 226f 6e43 6c69            "onCli
+00000ff0: 636b 223a 207b 0a20 2020 2020 2020 2020  ck": {.         
+00001000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001010: 2020 2020 2020 226f 7065 6e4c 696e 6b22        "openLink"
+00001020: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00001030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001040: 2020 2020 2020 2275 726c 223a 2022 6874        "url": "ht
+00001050: 7470 733a 2f2f 6578 616d 706c 652e 636f  tps://example.co
+00001060: 6d2f 7368 6172 6522 0a20 2020 2020 2020  m/share".       
+00001070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001080: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00001090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010a0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+000010b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010c0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+000010d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010e0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
 000010f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001100: 2020 2020 2020 2020 2261 6374 696f 6e22          "action"
-00001110: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00001100: 2020 2020 2020 2274 6578 7422 3a20 2245        "text": "E
+00001110: 6469 7422 2c0a 2020 2020 2020 2020 2020  dit",.          
 00001120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001130: 2020 2020 2022 6675 6e63 7469 6f6e 223a       "function":
-00001140: 2022 676f 546f 5669 6577 222c 0a20 2020   "goToView",.   
+00001130: 2020 2020 226f 6e43 6c69 636b 223a 207b      "onClick": {
+00001140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00001150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001160: 2020 2020 2020 2020 2020 2020 2020 2270                "p
-00001170: 6172 616d 6574 6572 7322 3a20 5b0a 2020  arameters": [.  
-00001180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011a0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00001160: 2022 6163 7469 6f6e 223a 207b 0a20 2020   "action": {.   
+00001170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001180: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001190: 6675 6e63 7469 6f6e 223a 2022 676f 546f  function": "goTo
+000011a0: 5669 6577 222c 0a20 2020 2020 2020 2020  View",.         
 000011b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011c0: 2020 2020 2020 2020 226b 6579 223a 2022          "key": "
-000011d0: 7669 6577 5479 7065 222c 0a20 2020 2020  viewType",.     
+000011c0: 2020 2020 2020 2020 2022 7061 7261 6d65           "parame
+000011d0: 7465 7273 223a 205b 0a20 2020 2020 2020  ters": [.       
 000011e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001200: 2276 616c 7565 223a 2022 4544 4954 222c  "value": "EDIT",
-00001210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001230: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
+000011f0: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
+00001200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001220: 2020 2020 2022 6b65 7922 3a20 2276 6965       "key": "vie
+00001230: 7754 7970 6522 2c0a 2020 2020 2020 2020  wType",.        
 00001240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001250: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
-00001260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001270: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00001250: 2020 2020 2020 2020 2020 2020 2020 2276                "v
+00001260: 616c 7565 223a 2022 4544 4954 220a 2020  alue": "EDIT".  
+00001270: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001290: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00001290: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
 000012a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012b0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+000012b0: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
 000012c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012d0: 205d 2c0a 2020 2020 2020 2020 2020 2020   ],.            
-000012e0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-000012f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001300: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-00001310: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
-00001320: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-00001330: 2020 2020 2020 2020 2020 2020 2020 5d2c                ],
-00001340: 0a20 2020 2020 2020 2020 2020 2020 7d2c  .             },
-00001350: 0a20 2020 2020 2020 2020 2020 7d0a 2020  .           }.  
-00001360: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
-00001370: 207d 0a0a 2020 2020 2e2e 207c 4578 616d   }..    .. |Exam
-00001380: 706c 6520 636f 6e74 6163 7420 6361 7264  ple contact card
-00001390: 7c20 696d 6167 653a 3a20 6874 7470 733a  | image:: https:
-000013a0: 2f2f 6465 7665 6c6f 7065 7273 2e67 6f6f  //developers.goo
-000013b0: 676c 652e 636f 6d2f 6368 6174 2f69 6d61  gle.com/chat/ima
-000013c0: 6765 732f 6361 7264 5f61 7069 5f72 6566  ges/card_api_ref
-000013d0: 6572 656e 6365 2e70 6e67 0a0a 2020 2020  erence.png..    
-000013e0: 4174 7472 6962 7574 6573 3a0a 2020 2020  Attributes:.    
-000013f0: 2020 2020 6865 6164 6572 2028 676f 6f67      header (goog
-00001400: 6c65 2e61 7070 732e 6361 7264 5f76 312e  le.apps.card_v1.
-00001410: 7479 7065 732e 4361 7264 2e43 6172 6448  types.Card.CardH
-00001420: 6561 6465 7229 3a0a 2020 2020 2020 2020  eader):.        
-00001430: 2020 2020 5468 6520 6865 6164 6572 206f      The header o
-00001440: 6620 7468 6520 6361 7264 2e20 4120 6865  f the card. A he
-00001450: 6164 6572 2075 7375 616c 6c79 0a20 2020  ader usually.   
-00001460: 2020 2020 2020 2020 2063 6f6e 7461 696e           contain
-00001470: 7320 6120 6c65 6164 696e 6720 696d 6167  s a leading imag
-00001480: 6520 616e 6420 6120 7469 746c 652e 2048  e and a title. H
-00001490: 6561 6465 7273 0a20 2020 2020 2020 2020  eaders.         
-000014a0: 2020 2061 6c77 6179 7320 6170 7065 6172     always appear
-000014b0: 2061 7420 7468 6520 746f 7020 6f66 2061   at the top of a
-000014c0: 2063 6172 642e 0a20 2020 2020 2020 2073   card..        s
-000014d0: 6563 7469 6f6e 7320 284d 7574 6162 6c65  ections (Mutable
-000014e0: 5365 7175 656e 6365 5b67 6f6f 676c 652e  Sequence[google.
-000014f0: 6170 7073 2e63 6172 645f 7631 2e74 7970  apps.card_v1.typ
-00001500: 6573 2e43 6172 642e 5365 6374 696f 6e5d  es.Card.Section]
-00001510: 293a 0a20 2020 2020 2020 2020 2020 2043  ):.            C
-00001520: 6f6e 7461 696e 7320 6120 636f 6c6c 6563  ontains a collec
-00001530: 7469 6f6e 206f 6620 7769 6467 6574 732e  tion of widgets.
-00001540: 2045 6163 6820 7365 6374 696f 6e20 6861   Each section ha
-00001550: 7320 6974 7320 6f77 6e2c 0a20 2020 2020  s its own,.     
-00001560: 2020 2020 2020 206f 7074 696f 6e61 6c20         optional 
-00001570: 6865 6164 6572 2e20 5365 6374 696f 6e73  header. Sections
-00001580: 2061 7265 2076 6973 7561 6c6c 7920 7365   are visually se
-00001590: 7061 7261 7465 6420 6279 2061 206c 696e  parated by a lin
-000015a0: 650a 2020 2020 2020 2020 2020 2020 6469  e.            di
-000015b0: 7669 6465 722e 2046 6f72 2061 6e20 6578  vider. For an ex
-000015c0: 616d 706c 6520 696e 2047 6f6f 676c 6520  ample in Google 
-000015d0: 4368 6174 2061 7070 732c 2073 6565 2060  Chat apps, see `
-000015e0: 4361 7264 0a20 2020 2020 2020 2020 2020  Card.           
-000015f0: 2073 6563 7469 6f6e 203c 6874 7470 733a   section <https:
-00001600: 2f2f 6465 7665 6c6f 7065 7273 2e67 6f6f  //developers.goo
-00001610: 676c 652e 636f 6d2f 6368 6174 2f75 692f  gle.com/chat/ui/
-00001620: 7769 6467 6574 732f 6361 7264 2d73 6563  widgets/card-sec
-00001630: 7469 6f6e 3e60 5f5f 2e0a 2020 2020 2020  tion>`__..      
-00001640: 2020 7365 6374 696f 6e5f 6469 7669 6465    section_divide
-00001650: 725f 7374 796c 6520 2867 6f6f 676c 652e  r_style (google.
-00001660: 6170 7073 2e63 6172 645f 7631 2e74 7970  apps.card_v1.typ
-00001670: 6573 2e43 6172 642e 4469 7669 6465 7253  es.Card.DividerS
-00001680: 7479 6c65 293a 0a20 2020 2020 2020 2020  tyle):.         
-00001690: 2020 2054 6865 2064 6976 6964 6572 2073     The divider s
-000016a0: 7479 6c65 2062 6574 7765 656e 2073 6563  tyle between sec
-000016b0: 7469 6f6e 732e 0a20 2020 2020 2020 2063  tions..        c
-000016c0: 6172 645f 6163 7469 6f6e 7320 284d 7574  ard_actions (Mut
-000016d0: 6162 6c65 5365 7175 656e 6365 5b67 6f6f  ableSequence[goo
-000016e0: 676c 652e 6170 7073 2e63 6172 645f 7631  gle.apps.card_v1
-000016f0: 2e74 7970 6573 2e43 6172 642e 4361 7264  .types.Card.Card
-00001700: 4163 7469 6f6e 5d29 3a0a 2020 2020 2020  Action]):.      
-00001710: 2020 2020 2020 5468 6520 6361 7264 2773        The card's
-00001720: 2061 6374 696f 6e73 2e20 4163 7469 6f6e   actions. Action
-00001730: 7320 6172 6520 6164 6465 6420 746f 2074  s are added to t
-00001740: 6865 2063 6172 6427 7320 746f 6f6c 6261  he card's toolba
-00001750: 720a 2020 2020 2020 2020 2020 2020 6d65  r.            me
-00001760: 6e75 2e0a 0a20 2020 2020 2020 2020 2020  nu...           
-00001770: 2060 476f 6f67 6c65 2057 6f72 6b73 7061   `Google Workspa
-00001780: 6365 0a20 2020 2020 2020 2020 2020 2041  ce.            A
-00001790: 6464 2d6f 6e73 203c 6874 7470 733a 2f2f  dd-ons <https://
-000017a0: 6465 7665 6c6f 7065 7273 2e67 6f6f 676c  developers.googl
-000017b0: 652e 636f 6d2f 776f 726b 7370 6163 652f  e.com/workspace/
-000017c0: 6164 642d 6f6e 733e 605f 5f3a 0a0a 2020  add-ons>`__:..  
-000017d0: 2020 2020 2020 2020 2020 466f 7220 6578            For ex
-000017e0: 616d 706c 652c 2074 6865 2066 6f6c 6c6f  ample, the follo
-000017f0: 7769 6e67 204a 534f 4e20 636f 6e73 7472  wing JSON constr
-00001800: 7563 7473 2061 2063 6172 6420 6163 7469  ucts a card acti
-00001810: 6f6e 0a20 2020 2020 2020 2020 2020 206d  on.            m
-00001820: 656e 7520 7769 7468 2060 6053 6574 7469  enu with ``Setti
-00001830: 6e67 7360 6020 616e 6420 6060 5365 6e64  ngs`` and ``Send
-00001840: 2046 6565 6462 6163 6b60 6020 6f70 7469   Feedback`` opti
-00001850: 6f6e 733a 0a0a 2020 2020 2020 2020 2020  ons:..          
-00001860: 2020 3a3a 0a0a 2020 2020 2020 2020 2020    ::..          
-00001870: 2020 2020 2022 6361 7264 5f61 6374 696f       "card_actio
-00001880: 6e73 223a 205b 0a20 2020 2020 2020 2020  ns": [.         
-00001890: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-000018a0: 2020 2020 2020 2020 2020 2020 2022 6163               "ac
-000018b0: 7469 6f6e 4c61 6265 6c22 3a20 2253 6574  tionLabel": "Set
-000018c0: 7469 6e67 7322 2c0a 2020 2020 2020 2020  tings",.        
-000018d0: 2020 2020 2020 2020 2020 2022 6f6e 436c             "onCl
-000018e0: 6963 6b22 3a20 7b0a 2020 2020 2020 2020  ick": {.        
-000018f0: 2020 2020 2020 2020 2020 2020 2022 6163               "ac
-00001900: 7469 6f6e 223a 207b 0a20 2020 2020 2020  tion": {.       
-00001910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001920: 2266 756e 6374 696f 6e4e 616d 6522 3a20  "functionName": 
-00001930: 2267 6f54 6f56 6965 7722 2c0a 2020 2020  "goToView",.    
-00001940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001950: 2020 2022 7061 7261 6d65 7465 7273 223a     "parameters":
-00001960: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
-00001970: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
-00001980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001990: 2020 2020 2020 2020 2022 6b65 7922 3a20           "key": 
-000019a0: 2276 6965 7754 7970 6522 2c0a 2020 2020  "viewType",.    
-000019b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019c0: 2020 2020 2020 2022 7661 6c75 6522 3a20         "value": 
-000019d0: 2253 4554 5449 4e47 220a 2020 2020 2020  "SETTING".      
-000019e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019f0: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
-00001a00: 2020 2020 2020 2020 2020 205d 2c0a 2020             ],.  
-00001a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a20: 2020 2020 2022 6c6f 6164 496e 6469 6361       "loadIndica
-00001a30: 746f 7222 3a20 224c 6f61 6449 6e64 6963  tor": "LoadIndic
-00001a40: 6174 6f72 2e53 5049 4e4e 4552 220a 2020  ator.SPINNER".  
-00001a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a60: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
-00001a70: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00001a80: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
-00001a90: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00001aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001ab0: 2020 2020 2261 6374 696f 6e4c 6162 656c      "actionLabel
-00001ac0: 223a 2022 5365 6e64 2046 6565 6462 6163  ": "Send Feedbac
-00001ad0: 6b22 2c0a 2020 2020 2020 2020 2020 2020  k",.            
-00001ae0: 2020 2020 2020 2022 6f6e 436c 6963 6b22         "onClick"
-00001af0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-00001b00: 2020 2020 2020 2020 2022 6f70 656e 4c69           "openLi
-00001b10: 6e6b 223a 207b 0a20 2020 2020 2020 2020  nk": {.         
-00001b20: 2020 2020 2020 2020 2020 2020 2020 2275                "u
-00001b30: 726c 223a 2022 6874 7470 733a 2f2f 6578  rl": "https://ex
-00001b40: 616d 706c 652e 636f 6d2f 6665 6564 6261  ample.com/feedba
-00001b50: 636b 220a 2020 2020 2020 2020 2020 2020  ck".            
-00001b60: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00001b70: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
-00001b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b90: 207d 0a20 2020 2020 2020 2020 2020 2020   }.             
-00001ba0: 2020 5d0a 2020 2020 2020 2020 6e61 6d65    ].        name
-00001bb0: 2028 7374 7229 3a0a 2020 2020 2020 2020   (str):.        
-00001bc0: 2020 2020 4e61 6d65 206f 6620 7468 6520      Name of the 
-00001bd0: 6361 7264 2e20 5573 6564 2061 7320 6120  card. Used as a 
-00001be0: 6361 7264 2069 6465 6e74 6966 6965 7220  card identifier 
-00001bf0: 696e 2063 6172 640a 2020 2020 2020 2020  in card.        
-00001c00: 2020 2020 6e61 7669 6761 7469 6f6e 2e0a      navigation..
-00001c10: 0a20 2020 2020 2020 2020 2020 2060 476f  .            `Go
-00001c20: 6f67 6c65 2057 6f72 6b73 7061 6365 0a20  ogle Workspace. 
-00001c30: 2020 2020 2020 2020 2020 2041 6464 2d6f             Add-o
-00001c40: 6e73 203c 6874 7470 733a 2f2f 6465 7665  ns <https://deve
-00001c50: 6c6f 7065 7273 2e67 6f6f 676c 652e 636f  lopers.google.co
-00001c60: 6d2f 776f 726b 7370 6163 652f 6164 642d  m/workspace/add-
-00001c70: 6f6e 733e 605f 5f3a 0a20 2020 2020 2020  ons>`__:.       
-00001c80: 2066 6978 6564 5f66 6f6f 7465 7220 2867   fixed_footer (g
-00001c90: 6f6f 676c 652e 6170 7073 2e63 6172 645f  oogle.apps.card_
-00001ca0: 7631 2e74 7970 6573 2e43 6172 642e 4361  v1.types.Card.Ca
-00001cb0: 7264 4669 7865 6446 6f6f 7465 7229 3a0a  rdFixedFooter):.
-00001cc0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00001cd0: 6669 7865 6420 666f 6f74 6572 2073 686f  fixed footer sho
-00001ce0: 776e 2061 7420 7468 6520 626f 7474 6f6d  wn at the bottom
-00001cf0: 206f 6620 7468 6973 2063 6172 642e 0a0a   of this card...
-00001d00: 2020 2020 2020 2020 2020 2020 5365 7474              Sett
-00001d10: 696e 6720 6060 6669 7865 6446 6f6f 7465  ing ``fixedFoote
-00001d20: 7260 6020 7769 7468 6f75 7420 7370 6563  r`` without spec
-00001d30: 6966 7969 6e67 2061 0a20 2020 2020 2020  ifying a.       
-00001d40: 2020 2020 2060 6070 7269 6d61 7279 4275       ``primaryBu
-00001d50: 7474 6f6e 6060 206f 7220 6120 6060 7365  tton`` or a ``se
-00001d60: 636f 6e64 6172 7942 7574 746f 6e60 6020  condaryButton`` 
-00001d70: 6361 7573 6573 2061 6e20 6572 726f 722e  causes an error.
-00001d80: 0a20 2020 2020 2020 2020 2020 2046 6f72  .            For
-00001d90: 2043 6861 7420 6170 7073 2c20 796f 7520   Chat apps, you 
-00001da0: 6361 6e20 7573 6520 6669 7865 6420 666f  can use fixed fo
-00001db0: 6f74 6572 7320 696e 0a20 2020 2020 2020  oters in.       
-00001dc0: 2020 2020 2060 6469 616c 6f67 7320 3c68       `dialogs <h
-00001dd0: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
-00001de0: 732e 676f 6f67 6c65 2e63 6f6d 2f63 6861  s.google.com/cha
-00001df0: 742f 686f 772d 746f 732f 6469 616c 6f67  t/how-tos/dialog
-00001e00: 733e 605f 5f2c 0a20 2020 2020 2020 2020  s>`__,.         
-00001e10: 2020 2062 7574 206e 6f74 2060 6361 7264     but not `card
-00001e20: 0a20 2020 2020 2020 2020 2020 206d 6573  .            mes
-00001e30: 7361 6765 7320 3c68 7474 7073 3a2f 2f64  sages <https://d
-00001e40: 6576 656c 6f70 6572 732e 676f 6f67 6c65  evelopers.google
-00001e50: 2e63 6f6d 2f63 6861 742f 6170 692f 6775  .com/chat/api/gu
-00001e60: 6964 6573 2f76 312f 6d65 7373 6167 6573  ides/v1/messages
-00001e70: 2f63 7265 6174 6523 6372 6561 7465 3e60  /create#create>`
-00001e80: 5f5f 2e0a 0a20 2020 2020 2020 2020 2020  __...           
-00001e90: 2060 476f 6f67 6c65 2057 6f72 6b73 7061   `Google Workspa
-00001ea0: 6365 2041 6464 2d6f 6e73 2061 6e64 2043  ce Add-ons and C
-00001eb0: 6861 740a 2020 2020 2020 2020 2020 2020  hat.            
-00001ec0: 6170 7073 203c 6874 7470 733a 2f2f 6465  apps <https://de
-00001ed0: 7665 6c6f 7065 7273 2e67 6f6f 676c 652e  velopers.google.
-00001ee0: 636f 6d2f 776f 726b 7370 6163 652f 6578  com/workspace/ex
-00001ef0: 7465 6e64 3e60 5f5f 3a0a 2020 2020 2020  tend>`__:.      
-00001f00: 2020 6469 7370 6c61 795f 7374 796c 6520    display_style 
-00001f10: 2867 6f6f 676c 652e 6170 7073 2e63 6172  (google.apps.car
-00001f20: 645f 7631 2e74 7970 6573 2e43 6172 642e  d_v1.types.Card.
-00001f30: 4469 7370 6c61 7953 7479 6c65 293a 0a20  DisplayStyle):. 
-00001f40: 2020 2020 2020 2020 2020 2049 6e20 476f             In Go
-00001f50: 6f67 6c65 2057 6f72 6b73 7061 6365 2041  ogle Workspace A
-00001f60: 6464 2d6f 6e73 2c20 7365 7473 2074 6865  dd-ons, sets the
-00001f70: 2064 6973 706c 6179 2070 726f 7065 7274   display propert
-00001f80: 6965 7320 6f66 0a20 2020 2020 2020 2020  ies of.         
-00001f90: 2020 2074 6865 2060 6070 6565 6b43 6172     the ``peekCar
-00001fa0: 6448 6561 6465 7260 602e 0a0a 2020 2020  dHeader``...    
-00001fb0: 2020 2020 2020 2020 6047 6f6f 676c 6520          `Google 
-00001fc0: 576f 726b 7370 6163 650a 2020 2020 2020  Workspace.      
-00001fd0: 2020 2020 2020 4164 642d 6f6e 7320 3c68        Add-ons <h
-00001fe0: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
-00001ff0: 732e 676f 6f67 6c65 2e63 6f6d 2f77 6f72  s.google.com/wor
-00002000: 6b73 7061 6365 2f61 6464 2d6f 6e73 3e60  kspace/add-ons>`
-00002010: 5f5f 3a0a 2020 2020 2020 2020 7065 656b  __:.        peek
-00002020: 5f63 6172 645f 6865 6164 6572 2028 676f  _card_header (go
-00002030: 6f67 6c65 2e61 7070 732e 6361 7264 5f76  ogle.apps.card_v
-00002040: 312e 7479 7065 732e 4361 7264 2e43 6172  1.types.Card.Car
-00002050: 6448 6561 6465 7229 3a0a 2020 2020 2020  dHeader):.      
-00002060: 2020 2020 2020 5768 656e 2064 6973 706c        When displ
-00002070: 6179 696e 6720 636f 6e74 6578 7475 616c  aying contextual
-00002080: 2063 6f6e 7465 6e74 2c20 7468 6520 7065   content, the pe
-00002090: 656b 2063 6172 6420 6865 6164 6572 0a20  ek card header. 
-000020a0: 2020 2020 2020 2020 2020 2061 6374 7320             acts 
-000020b0: 6173 2061 2070 6c61 6365 686f 6c64 6572  as a placeholder
-000020c0: 2073 6f20 7468 6174 2074 6865 2075 7365   so that the use
-000020d0: 7220 6361 6e20 6e61 7669 6761 7465 2066  r can navigate f
-000020e0: 6f72 7761 7264 0a20 2020 2020 2020 2020  orward.         
-000020f0: 2020 2062 6574 7765 656e 2074 6865 2068     between the h
-00002100: 6f6d 6570 6167 6520 6361 7264 7320 616e  omepage cards an
-00002110: 6420 7468 6520 636f 6e74 6578 7475 616c  d the contextual
-00002120: 2063 6172 6473 2e0a 0a20 2020 2020 2020   cards...       
-00002130: 2020 2020 2060 476f 6f67 6c65 2057 6f72       `Google Wor
-00002140: 6b73 7061 6365 0a20 2020 2020 2020 2020  kspace.         
-00002150: 2020 2041 6464 2d6f 6e73 203c 6874 7470     Add-ons <http
-00002160: 733a 2f2f 6465 7665 6c6f 7065 7273 2e67  s://developers.g
-00002170: 6f6f 676c 652e 636f 6d2f 776f 726b 7370  oogle.com/worksp
-00002180: 6163 652f 6164 642d 6f6e 733e 605f 5f3a  ace/add-ons>`__:
-00002190: 0a20 2020 2022 2222 0a0a 2020 2020 636c  .    """..    cl
-000021a0: 6173 7320 4469 7669 6465 7253 7479 6c65  ass DividerStyle
-000021b0: 2870 726f 746f 2e45 6e75 6d29 3a0a 2020  (proto.Enum):.  
-000021c0: 2020 2020 2020 7222 2222 5468 6520 6469        r"""The di
-000021d0: 7669 6465 7220 7374 796c 6520 6f66 2061  vider style of a
-000021e0: 2063 6172 642e 2043 7572 7265 6e74 6c79   card. Currently
-000021f0: 206f 6e6c 7920 7573 6564 2066 6f72 2064   only used for d
-00002200: 6976 6964 6572 730a 2020 2020 2020 2020  ividers.        
-00002210: 6265 7477 6565 6e73 2063 6172 6420 7365  betweens card se
-00002220: 6374 696f 6e73 2e0a 0a20 2020 2020 2020  ctions...       
-00002230: 2060 476f 6f67 6c65 2057 6f72 6b73 7061   `Google Workspa
-00002240: 6365 2041 6464 2d6f 6e73 2061 6e64 2043  ce Add-ons and C
-00002250: 6861 740a 2020 2020 2020 2020 6170 7073  hat.        apps
-00002260: 203c 6874 7470 733a 2f2f 6465 7665 6c6f   <https://develo
-00002270: 7065 7273 2e67 6f6f 676c 652e 636f 6d2f  pers.google.com/
-00002280: 776f 726b 7370 6163 652f 6578 7465 6e64  workspace/extend
-00002290: 3e60 5f5f 3a0a 0a20 2020 2020 2020 2056  >`__:..        V
-000022a0: 616c 7565 733a 0a20 2020 2020 2020 2020  alues:.         
-000022b0: 2020 2044 4956 4944 4552 5f53 5459 4c45     DIVIDER_STYLE
-000022c0: 5f55 4e53 5045 4349 4649 4544 2028 3029  _UNSPECIFIED (0)
-000022d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000022e0: 2020 446f 6e27 7420 7573 652e 2055 6e73    Don't use. Uns
-000022f0: 7065 6369 6669 6564 2e0a 2020 2020 2020  pecified..      
-00002300: 2020 2020 2020 534f 4c49 445f 4449 5649        SOLID_DIVI
-00002310: 4445 5220 2831 293a 0a20 2020 2020 2020  DER (1):.       
-00002320: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
-00002330: 206f 7074 696f 6e2e 2052 656e 6465 7220   option. Render 
-00002340: 6120 736f 6c69 6420 6469 7669 6465 720a  a solid divider.
-00002350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002360: 6265 7477 6565 6e20 7365 6374 696f 6e73  between sections
-00002370: 2e0a 2020 2020 2020 2020 2020 2020 4e4f  ..            NO
-00002380: 5f44 4956 4944 4552 2028 3229 3a0a 2020  _DIVIDER (2):.  
-00002390: 2020 2020 2020 2020 2020 2020 2020 4966                If
-000023a0: 2073 6574 2c20 6e6f 2064 6976 6964 6572   set, no divider
-000023b0: 2069 7320 7265 6e64 6572 6564 2062 6574   is rendered bet
-000023c0: 7765 656e 0a20 2020 2020 2020 2020 2020  ween.           
-000023d0: 2020 2020 2073 6563 7469 6f6e 732e 0a20       sections.. 
-000023e0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000023f0: 2020 2044 4956 4944 4552 5f53 5459 4c45     DIVIDER_STYLE
-00002400: 5f55 4e53 5045 4349 4649 4544 203d 2030  _UNSPECIFIED = 0
-00002410: 0a20 2020 2020 2020 2053 4f4c 4944 5f44  .        SOLID_D
-00002420: 4956 4944 4552 203d 2031 0a20 2020 2020  IVIDER = 1.     
-00002430: 2020 204e 4f5f 4449 5649 4445 5220 3d20     NO_DIVIDER = 
-00002440: 320a 0a20 2020 2063 6c61 7373 2044 6973  2..    class Dis
-00002450: 706c 6179 5374 796c 6528 7072 6f74 6f2e  playStyle(proto.
-00002460: 456e 756d 293a 0a20 2020 2020 2020 2072  Enum):.        r
-00002470: 2222 2249 6e20 476f 6f67 6c65 2057 6f72  """In Google Wor
-00002480: 6b73 7061 6365 2041 6464 2d6f 6e73 2c20  kspace Add-ons, 
-00002490: 6465 7465 726d 696e 6573 2068 6f77 2061  determines how a
-000024a0: 2063 6172 6420 6973 2064 6973 706c 6179   card is display
-000024b0: 6564 2e0a 0a20 2020 2020 2020 2060 476f  ed...        `Go
-000024c0: 6f67 6c65 2057 6f72 6b73 7061 6365 0a20  ogle Workspace. 
-000024d0: 2020 2020 2020 2041 6464 2d6f 6e73 203c         Add-ons <
-000024e0: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
-000024f0: 7273 2e67 6f6f 676c 652e 636f 6d2f 776f  rs.google.com/wo
-00002500: 726b 7370 6163 652f 6164 642d 6f6e 733e  rkspace/add-ons>
-00002510: 605f 5f3a 0a0a 2020 2020 2020 2020 5661  `__:..        Va
-00002520: 6c75 6573 3a0a 2020 2020 2020 2020 2020  lues:.          
-00002530: 2020 4449 5350 4c41 595f 5354 594c 455f    DISPLAY_STYLE_
-00002540: 554e 5350 4543 4946 4945 4420 2830 293a  UNSPECIFIED (0):
-00002550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002560: 2044 6f6e 2774 2075 7365 2e20 556e 7370   Don't use. Unsp
-00002570: 6563 6966 6965 642e 0a20 2020 2020 2020  ecified..       
-00002580: 2020 2020 2050 4545 4b20 2831 293a 0a20       PEEK (1):. 
-00002590: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-000025a0: 6865 2068 6561 6465 7220 6f66 2074 6865  he header of the
-000025b0: 2063 6172 6420 6170 7065 6172 7320 6174   card appears at
-000025c0: 2074 6865 2062 6f74 746f 6d0a 2020 2020   the bottom.    
-000025d0: 2020 2020 2020 2020 2020 2020 6f66 2074              of t
-000025e0: 6865 2073 6964 6562 6172 2c20 7061 7274  he sidebar, part
-000025f0: 6961 6c6c 7920 636f 7665 7269 6e67 2074  ially covering t
-00002600: 6865 2063 7572 7265 6e74 0a20 2020 2020  he current.     
-00002610: 2020 2020 2020 2020 2020 2074 6f70 2063             top c
-00002620: 6172 6420 6f66 2074 6865 2073 7461 636b  ard of the stack
-00002630: 2e20 436c 6963 6b69 6e67 2074 6865 2068  . Clicking the h
-00002640: 6561 6465 7220 706f 7073 0a20 2020 2020  eader pops.     
-00002650: 2020 2020 2020 2020 2020 2074 6865 2063             the c
-00002660: 6172 6420 696e 746f 2074 6865 2063 6172  ard into the car
-00002670: 6420 7374 6163 6b2e 2049 6620 7468 6520  d stack. If the 
-00002680: 6361 7264 2068 6173 206e 6f0a 2020 2020  card has no.    
-00002690: 2020 2020 2020 2020 2020 2020 6865 6164              head
-000026a0: 6572 2c20 6120 6765 6e65 7261 7465 6420  er, a generated 
-000026b0: 6865 6164 6572 2069 7320 7573 6564 2069  header is used i
-000026c0: 6e73 7465 6164 2e0a 2020 2020 2020 2020  nstead..        
-000026d0: 2020 2020 5245 504c 4143 4520 2832 293a      REPLACE (2):
-000026e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000026f0: 2044 6566 6175 6c74 2076 616c 7565 2e20   Default value. 
-00002700: 5468 6520 6361 7264 2069 7320 7368 6f77  The card is show
-00002710: 6e20 6279 2072 6570 6c61 6369 6e67 0a20  n by replacing. 
-00002720: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00002730: 6865 2076 6965 7720 6f66 2074 6865 2074  he view of the t
-00002740: 6f70 2063 6172 6420 696e 2074 6865 2063  op card in the c
-00002750: 6172 6420 7374 6163 6b2e 0a20 2020 2020  ard stack..     
-00002760: 2020 2022 2222 0a20 2020 2020 2020 2044     """.        D
-00002770: 4953 504c 4159 5f53 5459 4c45 5f55 4e53  ISPLAY_STYLE_UNS
-00002780: 5045 4349 4649 4544 203d 2030 0a20 2020  PECIFIED = 0.   
-00002790: 2020 2020 2050 4545 4b20 3d20 310a 2020       PEEK = 1.  
-000027a0: 2020 2020 2020 5245 504c 4143 4520 3d20        REPLACE = 
-000027b0: 320a 0a20 2020 2063 6c61 7373 2043 6172  2..    class Car
-000027c0: 6448 6561 6465 7228 7072 6f74 6f2e 4d65  dHeader(proto.Me
-000027d0: 7373 6167 6529 3a0a 2020 2020 2020 2020  ssage):.        
-000027e0: 7222 2222 5265 7072 6573 656e 7473 2061  r"""Represents a
-000027f0: 2063 6172 6420 6865 6164 6572 2e20 466f   card header. Fo
-00002800: 7220 616e 2065 7861 6d70 6c65 2069 6e20  r an example in 
-00002810: 476f 6f67 6c65 2043 6861 7420 6170 7073  Google Chat apps
-00002820: 2c20 7365 650a 2020 2020 2020 2020 6043  , see.        `C
-00002830: 6172 640a 2020 2020 2020 2020 6865 6164  ard.        head
-00002840: 6572 203c 6874 7470 733a 2f2f 6465 7665  er <https://deve
-00002850: 6c6f 7065 7273 2e67 6f6f 676c 652e 636f  lopers.google.co
-00002860: 6d2f 6368 6174 2f75 692f 7769 6467 6574  m/chat/ui/widget
-00002870: 732f 6361 7264 2d68 6561 6465 723e 605f  s/card-header>`_
-00002880: 5f2e 0a0a 2020 2020 2020 2020 6047 6f6f  _...        `Goo
-00002890: 676c 6520 576f 726b 7370 6163 6520 4164  gle Workspace Ad
-000028a0: 642d 6f6e 7320 616e 6420 4368 6174 0a20  d-ons and Chat. 
-000028b0: 2020 2020 2020 2061 7070 7320 3c68 7474         apps <htt
-000028c0: 7073 3a2f 2f64 6576 656c 6f70 6572 732e  ps://developers.
-000028d0: 676f 6f67 6c65 2e63 6f6d 2f77 6f72 6b73  google.com/works
-000028e0: 7061 6365 2f65 7874 656e 643e 605f 5f3a  pace/extend>`__:
-000028f0: 0a0a 2020 2020 2020 2020 4174 7472 6962  ..        Attrib
-00002900: 7574 6573 3a0a 2020 2020 2020 2020 2020  utes:.          
-00002910: 2020 7469 746c 6520 2873 7472 293a 0a20    title (str):. 
-00002920: 2020 2020 2020 2020 2020 2020 2020 2052                 R
-00002930: 6571 7569 7265 642e 2054 6865 2074 6974  equired. The tit
-00002940: 6c65 206f 6620 7468 6520 6361 7264 2068  le of the card h
-00002950: 6561 6465 722e 0a20 2020 2020 2020 2020  eader..         
-00002960: 2020 2020 2020 2054 6865 2068 6561 6465         The heade
-00002970: 7220 6861 7320 6120 6669 7865 6420 6865  r has a fixed he
-00002980: 6967 6874 3a20 6966 2062 6f74 6820 610a  ight: if both a.
-00002990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029a0: 7469 746c 6520 616e 6420 7375 6274 6974  title and subtit
-000029b0: 6c65 2061 7265 2073 7065 6369 6669 6564  le are specified
-000029c0: 2c20 6561 6368 2074 616b 6573 2075 700a  , each takes up.
-000029d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029e0: 6f6e 6520 6c69 6e65 2e20 4966 206f 6e6c  one line. If onl
-000029f0: 7920 7468 6520 7469 746c 6520 6973 2073  y the title is s
-00002a00: 7065 6369 6669 6564 2c20 6974 0a20 2020  pecified, it.   
-00002a10: 2020 2020 2020 2020 2020 2020 2074 616b               tak
-00002a20: 6573 2075 7020 626f 7468 206c 696e 6573  es up both lines
-00002a30: 2e0a 2020 2020 2020 2020 2020 2020 7375  ..            su
-00002a40: 6274 6974 6c65 2028 7374 7229 3a0a 2020  btitle (str):.  
-00002a50: 2020 2020 2020 2020 2020 2020 2020 5468                Th
-00002a60: 6520 7375 6274 6974 6c65 206f 6620 7468  e subtitle of th
-00002a70: 6520 6361 7264 2068 6561 6465 722e 2049  e card header. I
-00002a80: 6620 7370 6563 6966 6965 642c 2061 7070  f specified, app
-00002a90: 6561 7273 206f 6e0a 2020 2020 2020 2020  ears on.        
-00002aa0: 2020 2020 2020 2020 6974 7320 6f77 6e20          its own 
-00002ab0: 6c69 6e65 2062 656c 6f77 2074 6865 2060  line below the `
-00002ac0: 6074 6974 6c65 6060 2e0a 2020 2020 2020  `title``..      
-00002ad0: 2020 2020 2020 696d 6167 655f 7479 7065        image_type
-00002ae0: 2028 676f 6f67 6c65 2e61 7070 732e 6361   (google.apps.ca
-00002af0: 7264 5f76 312e 7479 7065 732e 5769 6467  rd_v1.types.Widg
-00002b00: 6574 2e49 6d61 6765 5479 7065 293a 0a20  et.ImageType):. 
-00002b10: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-00002b20: 6865 2073 6861 7065 2075 7365 6420 746f  he shape used to
-00002b30: 2063 726f 7020 7468 6520 696d 6167 652e   crop the image.
-00002b40: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002b50: 2020 6047 6f6f 676c 6520 576f 726b 7370    `Google Worksp
-00002b60: 6163 6520 4164 642d 6f6e 7320 616e 6420  ace Add-ons and 
-00002b70: 4368 6174 0a20 2020 2020 2020 2020 2020  Chat.           
-00002b80: 2020 2020 2061 7070 7320 3c68 7474 7073       apps <https
-00002b90: 3a2f 2f64 6576 656c 6f70 6572 732e 676f  ://developers.go
-00002ba0: 6f67 6c65 2e63 6f6d 2f77 6f72 6b73 7061  ogle.com/workspa
-00002bb0: 6365 2f65 7874 656e 643e 605f 5f3a 0a20  ce/extend>`__:. 
-00002bc0: 2020 2020 2020 2020 2020 2069 6d61 6765             image
-00002bd0: 5f75 726c 2028 7374 7229 3a0a 2020 2020  _url (str):.    
-00002be0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00002bf0: 4854 5450 5320 5552 4c20 6f66 2074 6865  HTTPS URL of the
-00002c00: 2069 6d61 6765 2069 6e20 7468 6520 6361   image in the ca
-00002c10: 7264 0a20 2020 2020 2020 2020 2020 2020  rd.             
-00002c20: 2020 2068 6561 6465 722e 0a20 2020 2020     header..     
-00002c30: 2020 2020 2020 2069 6d61 6765 5f61 6c74         image_alt
-00002c40: 5f74 6578 7420 2873 7472 293a 0a20 2020  _text (str):.   
-00002c50: 2020 2020 2020 2020 2020 2020 2054 6865               The
-00002c60: 2061 6c74 6572 6e61 7469 7665 2074 6578   alternative tex
-00002c70: 7420 6f66 2074 6869 7320 696d 6167 6520  t of this image 
-00002c80: 7468 6174 2773 0a20 2020 2020 2020 2020  that's.         
-00002c90: 2020 2020 2020 2075 7365 6420 666f 7220         used for 
-00002ca0: 6163 6365 7373 6962 696c 6974 792e 0a20  accessibility.. 
-00002cb0: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
-00002cc0: 2020 2020 7469 746c 653a 2073 7472 203d      title: str =
-00002cd0: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
-00002ce0: 2020 2020 2020 2020 2020 7072 6f74 6f2e            proto.
-00002cf0: 5354 5249 4e47 2c0a 2020 2020 2020 2020  STRING,.        
-00002d00: 2020 2020 6e75 6d62 6572 3d31 2c0a 2020      number=1,.  
-00002d10: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00002d20: 7375 6274 6974 6c65 3a20 7374 7220 3d20  subtitle: str = 
-00002d30: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
-00002d40: 2020 2020 2020 2020 2070 726f 746f 2e53           proto.S
-00002d50: 5452 494e 472c 0a20 2020 2020 2020 2020  TRING,.         
-00002d60: 2020 206e 756d 6265 723d 322c 0a20 2020     number=2,.   
-00002d70: 2020 2020 2029 0a20 2020 2020 2020 2069       ).        i
-00002d80: 6d61 6765 5f74 7970 653a 2022 5769 6467  mage_type: "Widg
-00002d90: 6574 2e49 6d61 6765 5479 7065 2220 3d20  et.ImageType" = 
-00002da0: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
-00002db0: 2020 2020 2020 2020 2070 726f 746f 2e45           proto.E
-00002dc0: 4e55 4d2c 0a20 2020 2020 2020 2020 2020  NUM,.           
-00002dd0: 206e 756d 6265 723d 332c 0a20 2020 2020   number=3,.     
-00002de0: 2020 2020 2020 2065 6e75 6d3d 2257 6964         enum="Wid
-00002df0: 6765 742e 496d 6167 6554 7970 6522 2c0a  get.ImageType",.
-00002e00: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00002e10: 2020 696d 6167 655f 7572 6c3a 2073 7472    image_url: str
-00002e20: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
-00002e30: 2020 2020 2020 2020 2020 2020 7072 6f74              prot
-00002e40: 6f2e 5354 5249 4e47 2c0a 2020 2020 2020  o.STRING,.      
-00002e50: 2020 2020 2020 6e75 6d62 6572 3d34 2c0a        number=4,.
-00002e60: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00002e70: 2020 696d 6167 655f 616c 745f 7465 7874    image_alt_text
-00002e80: 3a20 7374 7220 3d20 7072 6f74 6f2e 4669  : str = proto.Fi
-00002e90: 656c 6428 0a20 2020 2020 2020 2020 2020  eld(.           
-00002ea0: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
-00002eb0: 2020 2020 2020 2020 2020 206e 756d 6265             numbe
-00002ec0: 723d 352c 0a20 2020 2020 2020 2029 0a0a  r=5,.        )..
-00002ed0: 2020 2020 636c 6173 7320 5365 6374 696f      class Sectio
-00002ee0: 6e28 7072 6f74 6f2e 4d65 7373 6167 6529  n(proto.Message)
-00002ef0: 3a0a 2020 2020 2020 2020 7222 2222 4120  :.        r"""A 
-00002f00: 7365 6374 696f 6e20 636f 6e74 6169 6e73  section contains
-00002f10: 2061 2063 6f6c 6c65 6374 696f 6e20 6f66   a collection of
-00002f20: 2077 6964 6765 7473 2074 6861 7420 6172   widgets that ar
-00002f30: 6520 7265 6e64 6572 6564 0a20 2020 2020  e rendered.     
-00002f40: 2020 2076 6572 7469 6361 6c6c 7920 696e     vertically in
-00002f50: 2074 6865 206f 7264 6572 2074 6861 7420   the order that 
-00002f60: 7468 6579 2772 6520 7370 6563 6966 6965  they're specifie
-00002f70: 642e 0a0a 2020 2020 2020 2020 6047 6f6f  d...        `Goo
-00002f80: 676c 6520 576f 726b 7370 6163 6520 4164  gle Workspace Ad
-00002f90: 642d 6f6e 7320 616e 6420 4368 6174 0a20  d-ons and Chat. 
-00002fa0: 2020 2020 2020 2061 7070 7320 3c68 7474         apps <htt
-00002fb0: 7073 3a2f 2f64 6576 656c 6f70 6572 732e  ps://developers.
-00002fc0: 676f 6f67 6c65 2e63 6f6d 2f77 6f72 6b73  google.com/works
-00002fd0: 7061 6365 2f65 7874 656e 643e 605f 5f3a  pace/extend>`__:
-00002fe0: 0a0a 2020 2020 2020 2020 4174 7472 6962  ..        Attrib
-00002ff0: 7574 6573 3a0a 2020 2020 2020 2020 2020  utes:.          
-00003000: 2020 6865 6164 6572 2028 7374 7229 3a0a    header (str):.
-00003010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003020: 5465 7874 2074 6861 7420 6170 7065 6172  Text that appear
-00003030: 7320 6174 2074 6865 2074 6f70 206f 6620  s at the top of 
-00003040: 6120 7365 6374 696f 6e2e 2053 7570 706f  a section. Suppo
-00003050: 7274 7320 7369 6d70 6c65 0a20 2020 2020  rts simple.     
-00003060: 2020 2020 2020 2020 2020 2048 544d 4c20             HTML 
-00003070: 666f 726d 6174 7465 6420 7465 7874 2e20  formatted text. 
-00003080: 466f 7220 6d6f 7265 2069 6e66 6f72 6d61  For more informa
-00003090: 7469 6f6e 2061 626f 7574 2066 6f72 6d61  tion about forma
-000030a0: 7474 696e 670a 2020 2020 2020 2020 2020  tting.          
-000030b0: 2020 2020 2020 7465 7874 2c20 7365 6520        text, see 
-000030c0: 6046 6f72 6d61 7474 696e 6720 7465 7874  `Formatting text
-000030d0: 2069 6e20 476f 6f67 6c65 2043 6861 740a   in Google Chat.
-000030e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030f0: 6170 7073 203c 6874 7470 733a 2f2f 6465  apps <https://de
-00003100: 7665 6c6f 7065 7273 2e67 6f6f 676c 652e  velopers.google.
-00003110: 636f 6d2f 6368 6174 2f66 6f72 6d61 742d  com/chat/format-
-00003120: 6d65 7373 6167 6573 2363 6172 642d 666f  messages#card-fo
-00003130: 726d 6174 7469 6e67 3e60 5f5f 0a20 2020  rmatting>`__.   
-00003140: 2020 2020 2020 2020 2020 2020 2061 6e64               and
-00003150: 2060 466f 726d 6174 7469 6e67 2074 6578   `Formatting tex
-00003160: 7420 696e 2047 6f6f 676c 6520 576f 726b  t in Google Work
-00003170: 7370 6163 650a 2020 2020 2020 2020 2020  space.          
-00003180: 2020 2020 2020 4164 642d 6f6e 7320 3c68        Add-ons <h
-00003190: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
-000031a0: 732e 676f 6f67 6c65 2e63 6f6d 2f61 7070  s.google.com/app
-000031b0: 732d 7363 7269 7074 2f61 6464 2d6f 6e73  s-script/add-ons
-000031c0: 2f63 6f6e 6365 7074 732f 7769 6467 6574  /concepts/widget
-000031d0: 7323 7465 7874 5f66 6f72 6d61 7474 696e  s#text_formattin
-000031e0: 673e 605f 5f2e 0a20 2020 2020 2020 2020  g>`__..         
-000031f0: 2020 2077 6964 6765 7473 2028 4d75 7461     widgets (Muta
-00003200: 626c 6553 6571 7565 6e63 655b 676f 6f67  bleSequence[goog
-00003210: 6c65 2e61 7070 732e 6361 7264 5f76 312e  le.apps.card_v1.
-00003220: 7479 7065 732e 5769 6467 6574 5d29 3a0a  types.Widget]):.
-00003230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003240: 416c 6c20 7468 6520 7769 6467 6574 7320  All the widgets 
-00003250: 696e 2074 6865 2073 6563 7469 6f6e 2e0a  in the section..
-00003260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003270: 4d75 7374 2063 6f6e 7461 696e 2061 7420  Must contain at 
-00003280: 6c65 6173 7420 6f6e 6520 7769 6467 6574  least one widget
-00003290: 2e0a 2020 2020 2020 2020 2020 2020 636f  ..            co
-000032a0: 6c6c 6170 7369 626c 6520 2862 6f6f 6c29  llapsible (bool)
-000032b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000032c0: 2020 496e 6469 6361 7465 7320 7768 6574    Indicates whet
-000032d0: 6865 7220 7468 6973 2073 6563 7469 6f6e  her this section
-000032e0: 2069 7320 636f 6c6c 6170 7369 626c 652e   is collapsible.
-000032f0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003300: 2020 436f 6c6c 6170 7369 626c 6520 7365    Collapsible se
-00003310: 6374 696f 6e73 2068 6964 6520 736f 6d65  ctions hide some
-00003320: 206f 7220 616c 6c20 7769 6467 6574 732c   or all widgets,
-00003330: 2062 7574 2075 7365 7273 2063 616e 0a20   but users can. 
-00003340: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00003350: 7870 616e 6420 7468 6520 7365 6374 696f  xpand the sectio
-00003360: 6e20 746f 2072 6576 6561 6c20 7468 6520  n to reveal the 
-00003370: 6869 6464 656e 2077 6964 6765 7473 2062  hidden widgets b
-00003380: 7920 636c 6963 6b69 6e67 0a20 2020 2020  y clicking.     
-00003390: 2020 2020 2020 2020 2020 202a 2a53 686f             **Sho
-000033a0: 7720 6d6f 7265 2a2a 2e20 5573 6572 7320  w more**. Users 
-000033b0: 6361 6e20 6869 6465 2074 6865 2077 6964  can hide the wid
-000033c0: 6765 7473 2061 6761 696e 2062 7920 636c  gets again by cl
-000033d0: 6963 6b69 6e67 0a20 2020 2020 2020 2020  icking.         
-000033e0: 2020 2020 2020 202a 2a53 686f 7720 6c65         **Show le
-000033f0: 7373 2a2a 2e0a 0a20 2020 2020 2020 2020  ss**...         
-00003400: 2020 2020 2020 2054 6f20 6465 7465 726d         To determ
-00003410: 696e 6520 7768 6963 6820 7769 6467 6574  ine which widget
-00003420: 7320 6172 6520 6869 6464 656e 2c20 7370  s are hidden, sp
-00003430: 6563 6966 790a 2020 2020 2020 2020 2020  ecify.          
-00003440: 2020 2020 2020 6060 756e 636f 6c6c 6170        ``uncollap
-00003450: 7369 626c 6557 6964 6765 7473 436f 756e  sibleWidgetsCoun
-00003460: 7460 602e 0a20 2020 2020 2020 2020 2020  t``..           
-00003470: 2075 6e63 6f6c 6c61 7073 6962 6c65 5f77   uncollapsible_w
-00003480: 6964 6765 7473 5f63 6f75 6e74 2028 696e  idgets_count (in
-00003490: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
-000034a0: 2020 2020 5468 6520 6e75 6d62 6572 206f      The number o
-000034b0: 6620 756e 636f 6c6c 6170 7369 626c 6520  f uncollapsible 
-000034c0: 7769 6467 6574 7320 7768 6963 6820 7265  widgets which re
-000034d0: 6d61 696e 2076 6973 6962 6c65 0a20 2020  main visible.   
-000034e0: 2020 2020 2020 2020 2020 2020 2065 7665               eve
-000034f0: 6e20 7768 656e 2061 2073 6563 7469 6f6e  n when a section
-00003500: 2069 7320 636f 6c6c 6170 7365 642e 0a0a   is collapsed...
-00003510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003520: 466f 7220 6578 616d 706c 652c 2077 6865  For example, whe
-00003530: 6e20 6120 7365 6374 696f 6e20 636f 6e74  n a section cont
-00003540: 6169 6e73 2066 6976 6520 7769 6467 6574  ains five widget
-00003550: 7320 616e 6420 7468 650a 2020 2020 2020  s and the.      
-00003560: 2020 2020 2020 2020 2020 6060 756e 636f            ``unco
-00003570: 6c6c 6170 7369 626c 6557 6964 6765 7473  llapsibleWidgets
-00003580: 436f 756e 7460 6020 6973 2073 6574 2074  Count`` is set t
-00003590: 6f20 6060 3260 602c 2074 6865 2066 6972  o ``2``, the fir
-000035a0: 7374 2074 776f 0a20 2020 2020 2020 2020  st two.         
-000035b0: 2020 2020 2020 2077 6964 6765 7473 2061         widgets a
-000035c0: 7265 2061 6c77 6179 7320 7368 6f77 6e20  re always shown 
-000035d0: 616e 6420 7468 6520 6c61 7374 2074 6872  and the last thr
-000035e0: 6565 2061 7265 2063 6f6c 6c61 7073 6564  ee are collapsed
-000035f0: 2062 790a 2020 2020 2020 2020 2020 2020   by.            
-00003600: 2020 2020 6465 6661 756c 742e 2054 6865      default. The
-00003610: 2060 6075 6e63 6f6c 6c61 7073 6962 6c65   ``uncollapsible
-00003620: 5769 6467 6574 7343 6f75 6e74 6060 2069  WidgetsCount`` i
-00003630: 7320 7461 6b65 6e20 696e 746f 0a20 2020  s taken into.   
-00003640: 2020 2020 2020 2020 2020 2020 2061 6363               acc
-00003650: 6f75 6e74 206f 6e6c 7920 7768 656e 2060  ount only when `
-00003660: 6063 6f6c 6c61 7073 6962 6c65 6060 2069  `collapsible`` i
-00003670: 7320 6060 7472 7565 6060 2e0a 2020 2020  s ``true``..    
-00003680: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
-00003690: 2068 6561 6465 723a 2073 7472 203d 2070   header: str = p
-000036a0: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
-000036b0: 2020 2020 2020 2020 7072 6f74 6f2e 5354          proto.ST
-000036c0: 5249 4e47 2c0a 2020 2020 2020 2020 2020  RING,.          
-000036d0: 2020 6e75 6d62 6572 3d31 2c0a 2020 2020    number=1,.    
-000036e0: 2020 2020 290a 2020 2020 2020 2020 7769      ).        wi
-000036f0: 6467 6574 733a 204d 7574 6162 6c65 5365  dgets: MutableSe
-00003700: 7175 656e 6365 5b22 5769 6467 6574 225d  quence["Widget"]
-00003710: 203d 2070 726f 746f 2e52 6570 6561 7465   = proto.Repeate
-00003720: 6446 6965 6c64 280a 2020 2020 2020 2020  dField(.        
-00003730: 2020 2020 7072 6f74 6f2e 4d45 5353 4147      proto.MESSAG
-00003740: 452c 0a20 2020 2020 2020 2020 2020 206e  E,.            n
-00003750: 756d 6265 723d 322c 0a20 2020 2020 2020  umber=2,.       
-00003760: 2020 2020 206d 6573 7361 6765 3d22 5769       message="Wi
-00003770: 6467 6574 222c 0a20 2020 2020 2020 2029  dget",.        )
-00003780: 0a20 2020 2020 2020 2063 6f6c 6c61 7073  .        collaps
-00003790: 6962 6c65 3a20 626f 6f6c 203d 2070 726f  ible: bool = pro
-000037a0: 746f 2e46 6965 6c64 280a 2020 2020 2020  to.Field(.      
-000037b0: 2020 2020 2020 7072 6f74 6f2e 424f 4f4c        proto.BOOL
-000037c0: 2c0a 2020 2020 2020 2020 2020 2020 6e75  ,.            nu
-000037d0: 6d62 6572 3d35 2c0a 2020 2020 2020 2020  mber=5,.        
-000037e0: 290a 2020 2020 2020 2020 756e 636f 6c6c  ).        uncoll
-000037f0: 6170 7369 626c 655f 7769 6467 6574 735f  apsible_widgets_
-00003800: 636f 756e 743a 2069 6e74 203d 2070 726f  count: int = pro
-00003810: 746f 2e46 6965 6c64 280a 2020 2020 2020  to.Field(.      
-00003820: 2020 2020 2020 7072 6f74 6f2e 494e 5433        proto.INT3
-00003830: 322c 0a20 2020 2020 2020 2020 2020 206e  2,.            n
-00003840: 756d 6265 723d 362c 0a20 2020 2020 2020  umber=6,.       
-00003850: 2029 0a0a 2020 2020 636c 6173 7320 4361   )..    class Ca
-00003860: 7264 4163 7469 6f6e 2870 726f 746f 2e4d  rdAction(proto.M
-00003870: 6573 7361 6765 293a 0a20 2020 2020 2020  essage):.       
-00003880: 2072 2222 2241 2063 6172 6420 6163 7469   r"""A card acti
-00003890: 6f6e 2069 7320 7468 6520 6163 7469 6f6e  on is the action
-000038a0: 2061 7373 6f63 6961 7465 6420 7769 7468   associated with
-000038b0: 2074 6865 2063 6172 642e 2046 6f72 2065   the card. For e
-000038c0: 7861 6d70 6c65 2c0a 2020 2020 2020 2020  xample,.        
-000038d0: 616e 2069 6e76 6f69 6365 2063 6172 6420  an invoice card 
-000038e0: 6d69 6768 7420 696e 636c 7564 6520 6163  might include ac
-000038f0: 7469 6f6e 7320 7375 6368 2061 7320 6465  tions such as de
-00003900: 6c65 7465 2069 6e76 6f69 6365 2c20 656d  lete invoice, em
-00003910: 6169 6c0a 2020 2020 2020 2020 696e 766f  ail.        invo
-00003920: 6963 652c 206f 7220 6f70 656e 2074 6865  ice, or open the
-00003930: 2069 6e76 6f69 6365 2069 6e20 6120 6272   invoice in a br
-00003940: 6f77 7365 722e 0a0a 2020 2020 2020 2020  owser...        
-00003950: 6047 6f6f 676c 6520 576f 726b 7370 6163  `Google Workspac
-00003960: 650a 2020 2020 2020 2020 4164 642d 6f6e  e.        Add-on
-00003970: 7320 3c68 7474 7073 3a2f 2f64 6576 656c  s <https://devel
-00003980: 6f70 6572 732e 676f 6f67 6c65 2e63 6f6d  opers.google.com
-00003990: 2f77 6f72 6b73 7061 6365 2f61 6464 2d6f  /workspace/add-o
-000039a0: 6e73 3e60 5f5f 3a0a 0a20 2020 2020 2020  ns>`__:..       
-000039b0: 2041 7474 7269 6275 7465 733a 0a20 2020   Attributes:.   
-000039c0: 2020 2020 2020 2020 2061 6374 696f 6e5f           action_
-000039d0: 6c61 6265 6c20 2873 7472 293a 0a20 2020  label (str):.   
-000039e0: 2020 2020 2020 2020 2020 2020 2054 6865               The
-000039f0: 206c 6162 656c 2074 6861 7420 6469 7370   label that disp
-00003a00: 6c61 7973 2061 7320 7468 6520 6163 7469  lays as the acti
-00003a10: 6f6e 206d 656e 750a 2020 2020 2020 2020  on menu.        
-00003a20: 2020 2020 2020 2020 6974 656d 2e0a 2020          item..  
-00003a30: 2020 2020 2020 2020 2020 6f6e 5f63 6c69            on_cli
-00003a40: 636b 2028 676f 6f67 6c65 2e61 7070 732e  ck (google.apps.
-00003a50: 6361 7264 5f76 312e 7479 7065 732e 4f6e  card_v1.types.On
-00003a60: 436c 6963 6b29 3a0a 2020 2020 2020 2020  Click):.        
-00003a70: 2020 2020 2020 2020 5468 6520 6060 6f6e          The ``on
-00003a80: 436c 6963 6b60 6020 6163 7469 6f6e 2066  Click`` action f
-00003a90: 6f72 2074 6869 7320 6163 7469 6f6e 2069  or this action i
-00003aa0: 7465 6d2e 0a20 2020 2020 2020 2022 2222  tem..        """
-00003ab0: 0a0a 2020 2020 2020 2020 6163 7469 6f6e  ..        action
-00003ac0: 5f6c 6162 656c 3a20 7374 7220 3d20 7072  _label: str = pr
-00003ad0: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
-00003ae0: 2020 2020 2020 2070 726f 746f 2e53 5452         proto.STR
-00003af0: 494e 472c 0a20 2020 2020 2020 2020 2020  ING,.           
-00003b00: 206e 756d 6265 723d 312c 0a20 2020 2020   number=1,.     
-00003b10: 2020 2029 0a20 2020 2020 2020 206f 6e5f     ).        on_
-00003b20: 636c 6963 6b3a 2022 4f6e 436c 6963 6b22  click: "OnClick"
-00003b30: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
-00003b40: 2020 2020 2020 2020 2020 2020 7072 6f74              prot
-00003b50: 6f2e 4d45 5353 4147 452c 0a20 2020 2020  o.MESSAGE,.     
-00003b60: 2020 2020 2020 206e 756d 6265 723d 322c         number=2,
-00003b70: 0a20 2020 2020 2020 2020 2020 206d 6573  .            mes
-00003b80: 7361 6765 3d22 4f6e 436c 6963 6b22 2c0a  sage="OnClick",.
-00003b90: 2020 2020 2020 2020 290a 0a20 2020 2063          )..    c
-00003ba0: 6c61 7373 2043 6172 6446 6978 6564 466f  lass CardFixedFo
-00003bb0: 6f74 6572 2870 726f 746f 2e4d 6573 7361  oter(proto.Messa
-00003bc0: 6765 293a 0a20 2020 2020 2020 2072 2222  ge):.        r""
-00003bd0: 2241 2070 6572 7369 7374 656e 7420 2873  "A persistent (s
-00003be0: 7469 636b 7929 2066 6f6f 7465 7220 7468  ticky) footer th
-00003bf0: 6174 2074 6861 7420 6170 7065 6172 7320  at that appears 
-00003c00: 6174 2074 6865 2062 6f74 746f 6d20 6f66  at the bottom of
-00003c10: 2074 6865 0a20 2020 2020 2020 2063 6172   the.        car
-00003c20: 642e 0a0a 2020 2020 2020 2020 5365 7474  d...        Sett
-00003c30: 696e 6720 6060 6669 7865 6446 6f6f 7465  ing ``fixedFoote
-00003c40: 7260 6020 7769 7468 6f75 7420 7370 6563  r`` without spec
-00003c50: 6966 7969 6e67 2061 2060 6070 7269 6d61  ifying a ``prima
-00003c60: 7279 4275 7474 6f6e 6060 206f 7220 610a  ryButton`` or a.
-00003c70: 2020 2020 2020 2020 6060 7365 636f 6e64          ``second
-00003c80: 6172 7942 7574 746f 6e60 6020 6361 7573  aryButton`` caus
-00003c90: 6573 2061 6e20 6572 726f 722e 0a0a 2020  es an error...  
-00003ca0: 2020 2020 2020 466f 7220 4368 6174 2061        For Chat a
-00003cb0: 7070 732c 2079 6f75 2063 616e 2075 7365  pps, you can use
-00003cc0: 2066 6978 6564 2066 6f6f 7465 7273 2069   fixed footers i
-00003cd0: 6e0a 2020 2020 2020 2020 6064 6961 6c6f  n.        `dialo
-00003ce0: 6773 203c 6874 7470 733a 2f2f 6465 7665  gs <https://deve
-00003cf0: 6c6f 7065 7273 2e67 6f6f 676c 652e 636f  lopers.google.co
-00003d00: 6d2f 6368 6174 2f68 6f77 2d74 6f73 2f64  m/chat/how-tos/d
-00003d10: 6961 6c6f 6773 3e60 5f5f 2c0a 2020 2020  ialogs>`__,.    
-00003d20: 2020 2020 6275 7420 6e6f 7420 6063 6172      but not `car
-00003d30: 640a 2020 2020 2020 2020 6d65 7373 6167  d.        messag
-00003d40: 6573 203c 6874 7470 733a 2f2f 6465 7665  es <https://deve
-00003d50: 6c6f 7065 7273 2e67 6f6f 676c 652e 636f  lopers.google.co
-00003d60: 6d2f 6368 6174 2f61 7069 2f67 7569 6465  m/chat/api/guide
-00003d70: 732f 7631 2f6d 6573 7361 6765 732f 6372  s/v1/messages/cr
-00003d80: 6561 7465 2363 7265 6174 653e 605f 5f2e  eate#create>`__.
-00003d90: 0a20 2020 2020 2020 2046 6f72 2061 6e20  .        For an 
-00003da0: 6578 616d 706c 6520 696e 2047 6f6f 676c  example in Googl
-00003db0: 6520 4368 6174 2061 7070 732c 2073 6565  e Chat apps, see
-00003dc0: 2060 4361 7264 0a20 2020 2020 2020 2066   `Card.        f
-00003dd0: 6f6f 7465 7220 3c68 7474 7073 3a2f 2f64  ooter <https://d
-00003de0: 6576 656c 6f70 6572 732e 676f 6f67 6c65  evelopers.google
-00003df0: 2e63 6f6d 2f63 6861 742f 7569 2f77 6964  .com/chat/ui/wid
-00003e00: 6765 7473 2f63 6172 642d 6669 7865 642d  gets/card-fixed-
-00003e10: 666f 6f74 6572 3e60 5f5f 2e0a 0a20 2020  footer>`__...   
-00003e20: 2020 2020 2060 476f 6f67 6c65 2057 6f72       `Google Wor
-00003e30: 6b73 7061 6365 2041 6464 2d6f 6e73 2061  kspace Add-ons a
-00003e40: 6e64 2043 6861 740a 2020 2020 2020 2020  nd Chat.        
-00003e50: 6170 7073 203c 6874 7470 733a 2f2f 6465  apps <https://de
-00003e60: 7665 6c6f 7065 7273 2e67 6f6f 676c 652e  velopers.google.
-00003e70: 636f 6d2f 776f 726b 7370 6163 652f 6578  com/workspace/ex
-00003e80: 7465 6e64 3e60 5f5f 3a0a 0a20 2020 2020  tend>`__:..     
-00003e90: 2020 2041 7474 7269 6275 7465 733a 0a20     Attributes:. 
-00003ea0: 2020 2020 2020 2020 2020 2070 7269 6d61             prima
-00003eb0: 7279 5f62 7574 746f 6e20 2867 6f6f 676c  ry_button (googl
-00003ec0: 652e 6170 7073 2e63 6172 645f 7631 2e74  e.apps.card_v1.t
-00003ed0: 7970 6573 2e42 7574 746f 6e29 3a0a 2020  ypes.Button):.  
-00003ee0: 2020 2020 2020 2020 2020 2020 2020 5468                Th
-00003ef0: 6520 7072 696d 6172 7920 6275 7474 6f6e  e primary button
-00003f00: 206f 6620 7468 6520 6669 7865 6420 666f   of the fixed fo
-00003f10: 6f74 6572 2e20 5468 650a 2020 2020 2020  oter. The.      
-00003f20: 2020 2020 2020 2020 2020 6275 7474 6f6e            button
-00003f30: 206d 7573 7420 6265 2061 2074 6578 7420   must be a text 
-00003f40: 6275 7474 6f6e 2077 6974 6820 7465 7874  button with text
-00003f50: 2061 6e64 2063 6f6c 6f72 0a20 2020 2020   and color.     
-00003f60: 2020 2020 2020 2020 2020 2073 6574 2e0a             set..
-00003f70: 2020 2020 2020 2020 2020 2020 7365 636f              seco
-00003f80: 6e64 6172 795f 6275 7474 6f6e 2028 676f  ndary_button (go
-00003f90: 6f67 6c65 2e61 7070 732e 6361 7264 5f76  ogle.apps.card_v
-00003fa0: 312e 7479 7065 732e 4275 7474 6f6e 293a  1.types.Button):
-00003fb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003fc0: 2054 6865 2073 6563 6f6e 6461 7279 2062   The secondary b
-00003fd0: 7574 746f 6e20 6f66 2074 6865 2066 6978  utton of the fix
-00003fe0: 6564 2066 6f6f 7465 722e 2054 6865 2062  ed footer. The b
-00003ff0: 7574 746f 6e20 6d75 7374 2062 650a 2020  utton must be.  
-00004000: 2020 2020 2020 2020 2020 2020 2020 6120                a 
-00004010: 7465 7874 2062 7574 746f 6e20 7769 7468  text button with
-00004020: 2074 6578 7420 616e 6420 636f 6c6f 7220   text and color 
-00004030: 7365 742e 2049 660a 2020 2020 2020 2020  set. If.        
-00004040: 2020 2020 2020 2020 6060 7365 636f 6e64          ``second
-00004050: 6172 7942 7574 746f 6e60 6020 6973 2073  aryButton`` is s
-00004060: 6574 2c20 796f 7520 6d75 7374 2061 6c73  et, you must als
-00004070: 6f20 7365 740a 2020 2020 2020 2020 2020  o set.          
-00004080: 2020 2020 2020 6060 7072 696d 6172 7942        ``primaryB
-00004090: 7574 746f 6e60 602e 0a20 2020 2020 2020  utton``..       
-000040a0: 2022 2222 0a0a 2020 2020 2020 2020 7072   """..        pr
-000040b0: 696d 6172 795f 6275 7474 6f6e 3a20 2242  imary_button: "B
-000040c0: 7574 746f 6e22 203d 2070 726f 746f 2e46  utton" = proto.F
-000040d0: 6965 6c64 280a 2020 2020 2020 2020 2020  ield(.          
-000040e0: 2020 7072 6f74 6f2e 4d45 5353 4147 452c    proto.MESSAGE,
-000040f0: 0a20 2020 2020 2020 2020 2020 206e 756d  .            num
-00004100: 6265 723d 312c 0a20 2020 2020 2020 2020  ber=1,.         
-00004110: 2020 206d 6573 7361 6765 3d22 4275 7474     message="Butt
-00004120: 6f6e 222c 0a20 2020 2020 2020 2029 0a20  on",.        ). 
-00004130: 2020 2020 2020 2073 6563 6f6e 6461 7279         secondary
-00004140: 5f62 7574 746f 6e3a 2022 4275 7474 6f6e  _button: "Button
-00004150: 2220 3d20 7072 6f74 6f2e 4669 656c 6428  " = proto.Field(
-00004160: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-00004170: 746f 2e4d 4553 5341 4745 2c0a 2020 2020  to.MESSAGE,.    
-00004180: 2020 2020 2020 2020 6e75 6d62 6572 3d32          number=2
-00004190: 2c0a 2020 2020 2020 2020 2020 2020 6d65  ,.            me
-000041a0: 7373 6167 653d 2242 7574 746f 6e22 2c0a  ssage="Button",.
-000041b0: 2020 2020 2020 2020 290a 0a20 2020 2068          )..    h
-000041c0: 6561 6465 723a 2043 6172 6448 6561 6465  eader: CardHeade
-000041d0: 7220 3d20 7072 6f74 6f2e 4669 656c 6428  r = proto.Field(
-000041e0: 0a20 2020 2020 2020 2070 726f 746f 2e4d  .        proto.M
-000041f0: 4553 5341 4745 2c0a 2020 2020 2020 2020  ESSAGE,.        
+000012d0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+000012e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012f0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00001300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001310: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00001320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001330: 2020 5d0a 2020 2020 2020 2020 2020 2020    ].            
+00001340: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00001350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001360: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
+00001370: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
+00001380: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
+00001390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013a0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+000013b0: 7d0a 2020 2020 2020 2020 2020 207d 0a20  }.           }. 
+000013c0: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
+000013d0: 207d 0a0a 2020 2020 2e2e 207c 4578 616d   }..    .. |Exam
+000013e0: 706c 6520 636f 6e74 6163 7420 6361 7264  ple contact card
+000013f0: 7c20 696d 6167 653a 3a20 6874 7470 733a  | image:: https:
+00001400: 2f2f 6465 7665 6c6f 7065 7273 2e67 6f6f  //developers.goo
+00001410: 676c 652e 636f 6d2f 776f 726b 7370 6163  gle.com/workspac
+00001420: 652f 6368 6174 2f69 6d61 6765 732f 6361  e/chat/images/ca
+00001430: 7264 5f61 7069 5f72 6566 6572 656e 6365  rd_api_reference
+00001440: 2e70 6e67 0a0a 2020 2020 4174 7472 6962  .png..    Attrib
+00001450: 7574 6573 3a0a 2020 2020 2020 2020 6865  utes:.        he
+00001460: 6164 6572 2028 676f 6f67 6c65 2e61 7070  ader (google.app
+00001470: 732e 6361 7264 5f76 312e 7479 7065 732e  s.card_v1.types.
+00001480: 4361 7264 2e43 6172 6448 6561 6465 7229  Card.CardHeader)
+00001490: 3a0a 2020 2020 2020 2020 2020 2020 5468  :.            Th
+000014a0: 6520 6865 6164 6572 206f 6620 7468 6520  e header of the 
+000014b0: 6361 7264 2e20 4120 6865 6164 6572 2075  card. A header u
+000014c0: 7375 616c 6c79 0a20 2020 2020 2020 2020  sually.         
+000014d0: 2020 2063 6f6e 7461 696e 7320 6120 6c65     contains a le
+000014e0: 6164 696e 6720 696d 6167 6520 616e 6420  ading image and 
+000014f0: 6120 7469 746c 652e 2048 6561 6465 7273  a title. Headers
+00001500: 0a20 2020 2020 2020 2020 2020 2061 6c77  .            alw
+00001510: 6179 7320 6170 7065 6172 2061 7420 7468  ays appear at th
+00001520: 6520 746f 7020 6f66 2061 2063 6172 642e  e top of a card.
+00001530: 0a20 2020 2020 2020 2073 6563 7469 6f6e  .        section
+00001540: 7320 284d 7574 6162 6c65 5365 7175 656e  s (MutableSequen
+00001550: 6365 5b67 6f6f 676c 652e 6170 7073 2e63  ce[google.apps.c
+00001560: 6172 645f 7631 2e74 7970 6573 2e43 6172  ard_v1.types.Car
+00001570: 642e 5365 6374 696f 6e5d 293a 0a20 2020  d.Section]):.   
+00001580: 2020 2020 2020 2020 2043 6f6e 7461 696e           Contain
+00001590: 7320 6120 636f 6c6c 6563 7469 6f6e 206f  s a collection o
+000015a0: 6620 7769 6467 6574 732e 2045 6163 6820  f widgets. Each 
+000015b0: 7365 6374 696f 6e20 6861 7320 6974 7320  section has its 
+000015c0: 6f77 6e2c 0a20 2020 2020 2020 2020 2020  own,.           
+000015d0: 206f 7074 696f 6e61 6c20 6865 6164 6572   optional header
+000015e0: 2e20 5365 6374 696f 6e73 2061 7265 2076  . Sections are v
+000015f0: 6973 7561 6c6c 7920 7365 7061 7261 7465  isually separate
+00001600: 6420 6279 2061 206c 696e 650a 2020 2020  d by a line.    
+00001610: 2020 2020 2020 2020 6469 7669 6465 722e          divider.
+00001620: 2046 6f72 2061 6e20 6578 616d 706c 6520   For an example 
+00001630: 696e 2047 6f6f 676c 6520 4368 6174 2061  in Google Chat a
+00001640: 7070 732c 2073 6565 2060 4465 6669 6e65  pps, see `Define
+00001650: 2061 0a20 2020 2020 2020 2020 2020 2073   a.            s
+00001660: 6563 7469 6f6e 206f 6620 610a 2020 2020  ection of a.    
+00001670: 2020 2020 2020 2020 6361 7264 203c 6874          card <ht
+00001680: 7470 733a 2f2f 6465 7665 6c6f 7065 7273  tps://developers
+00001690: 2e67 6f6f 676c 652e 636f 6d2f 776f 726b  .google.com/work
+000016a0: 7370 6163 652f 6368 6174 2f64 6573 6967  space/chat/desig
+000016b0: 6e2d 636f 6d70 6f6e 656e 7473 2d63 6172  n-components-car
+000016c0: 642d 6469 616c 6f67 2364 6566 696e 655f  d-dialog#define_
+000016d0: 615f 7365 6374 696f 6e5f 6f66 5f61 5f63  a_section_of_a_c
+000016e0: 6172 643e 605f 5f2e 0a20 2020 2020 2020  ard>`__..       
+000016f0: 2073 6563 7469 6f6e 5f64 6976 6964 6572   section_divider
+00001700: 5f73 7479 6c65 2028 676f 6f67 6c65 2e61  _style (google.a
+00001710: 7070 732e 6361 7264 5f76 312e 7479 7065  pps.card_v1.type
+00001720: 732e 4361 7264 2e44 6976 6964 6572 5374  s.Card.DividerSt
+00001730: 796c 6529 3a0a 2020 2020 2020 2020 2020  yle):.          
+00001740: 2020 5468 6520 6469 7669 6465 7220 7374    The divider st
+00001750: 796c 6520 6265 7477 6565 6e20 7365 6374  yle between sect
+00001760: 696f 6e73 2e0a 2020 2020 2020 2020 6361  ions..        ca
+00001770: 7264 5f61 6374 696f 6e73 2028 4d75 7461  rd_actions (Muta
+00001780: 626c 6553 6571 7565 6e63 655b 676f 6f67  bleSequence[goog
+00001790: 6c65 2e61 7070 732e 6361 7264 5f76 312e  le.apps.card_v1.
+000017a0: 7479 7065 732e 4361 7264 2e43 6172 6441  types.Card.CardA
+000017b0: 6374 696f 6e5d 293a 0a20 2020 2020 2020  ction]):.       
+000017c0: 2020 2020 2054 6865 2063 6172 6427 7320       The card's 
+000017d0: 6163 7469 6f6e 732e 2041 6374 696f 6e73  actions. Actions
+000017e0: 2061 7265 2061 6464 6564 2074 6f20 7468   are added to th
+000017f0: 6520 6361 7264 2773 2074 6f6f 6c62 6172  e card's toolbar
+00001800: 0a20 2020 2020 2020 2020 2020 206d 656e  .            men
+00001810: 752e 0a0a 2020 2020 2020 2020 2020 2020  u...            
+00001820: 6047 6f6f 676c 6520 576f 726b 7370 6163  `Google Workspac
+00001830: 650a 2020 2020 2020 2020 2020 2020 4164  e.            Ad
+00001840: 642d 6f6e 7320 3c68 7474 7073 3a2f 2f64  d-ons <https://d
+00001850: 6576 656c 6f70 6572 732e 676f 6f67 6c65  evelopers.google
+00001860: 2e63 6f6d 2f77 6f72 6b73 7061 6365 2f61  .com/workspace/a
+00001870: 6464 2d6f 6e73 3e60 5f5f 3a0a 0a20 2020  dd-ons>`__:..   
+00001880: 2020 2020 2020 2020 2046 6f72 2065 7861           For exa
+00001890: 6d70 6c65 2c20 7468 6520 666f 6c6c 6f77  mple, the follow
+000018a0: 696e 6720 4a53 4f4e 2063 6f6e 7374 7275  ing JSON constru
+000018b0: 6374 7320 6120 6361 7264 2061 6374 696f  cts a card actio
+000018c0: 6e0a 2020 2020 2020 2020 2020 2020 6d65  n.            me
+000018d0: 6e75 2077 6974 6820 6060 5365 7474 696e  nu with ``Settin
+000018e0: 6773 6060 2061 6e64 2060 6053 656e 6420  gs`` and ``Send 
+000018f0: 4665 6564 6261 636b 6060 206f 7074 696f  Feedback`` optio
+00001900: 6e73 3a0a 0a20 2020 2020 2020 2020 2020  ns:..           
+00001910: 203a 3a0a 0a20 2020 2020 2020 2020 2020   ::..           
+00001920: 2020 2020 2263 6172 645f 6163 7469 6f6e      "card_action
+00001930: 7322 3a20 5b0a 2020 2020 2020 2020 2020  s": [.          
+00001940: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00001950: 2020 2020 2020 2020 2020 2020 2261 6374              "act
+00001960: 696f 6e4c 6162 656c 223a 2022 5365 7474  ionLabel": "Sett
+00001970: 696e 6773 222c 0a20 2020 2020 2020 2020  ings",.         
+00001980: 2020 2020 2020 2020 2020 226f 6e43 6c69            "onCli
+00001990: 636b 223a 207b 0a20 2020 2020 2020 2020  ck": {.         
+000019a0: 2020 2020 2020 2020 2020 2020 2261 6374              "act
+000019b0: 696f 6e22 3a20 7b0a 2020 2020 2020 2020  ion": {.        
+000019c0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000019d0: 6675 6e63 7469 6f6e 4e61 6d65 223a 2022  functionName": "
+000019e0: 676f 546f 5669 6577 222c 0a20 2020 2020  goToView",.     
+000019f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a00: 2020 2270 6172 616d 6574 6572 7322 3a20    "parameters": 
+00001a10: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+00001a20: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
+00001a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a40: 2020 2020 2020 2020 226b 6579 223a 2022          "key": "
+00001a50: 7669 6577 5479 7065 222c 0a20 2020 2020  viewType",.     
+00001a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a70: 2020 2020 2020 2276 616c 7565 223a 2022        "value": "
+00001a80: 5345 5454 494e 4722 0a20 2020 2020 2020  SETTING".       
+00001a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001aa0: 207d 0a20 2020 2020 2020 2020 2020 2020   }.             
+00001ab0: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
+00001ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ad0: 2020 2020 226c 6f61 6449 6e64 6963 6174      "loadIndicat
+00001ae0: 6f72 223a 2022 4c6f 6164 496e 6469 6361  or": "LoadIndica
+00001af0: 746f 722e 5350 494e 4e45 5222 0a20 2020  tor.SPINNER".   
+00001b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b10: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
+00001b20: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00001b30: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
+00001b40: 2020 2020 2020 2020 2020 2020 2020 7b0a                {.
+00001b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b60: 2020 2022 6163 7469 6f6e 4c61 6265 6c22     "actionLabel"
+00001b70: 3a20 2253 656e 6420 4665 6564 6261 636b  : "Send Feedback
+00001b80: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00001b90: 2020 2020 2020 226f 6e43 6c69 636b 223a        "onClick":
+00001ba0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00001bb0: 2020 2020 2020 2020 226f 7065 6e4c 696e          "openLin
+00001bc0: 6b22 3a20 7b0a 2020 2020 2020 2020 2020  k": {.          
+00001bd0: 2020 2020 2020 2020 2020 2020 2022 7572               "ur
+00001be0: 6c22 3a20 2268 7474 7073 3a2f 2f65 7861  l": "https://exa
+00001bf0: 6d70 6c65 2e63 6f6d 2f66 6565 6462 6163  mple.com/feedbac
+00001c00: 6b22 0a20 2020 2020 2020 2020 2020 2020  k".             
+00001c10: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00001c20: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
+00001c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c40: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00001c50: 205d 0a20 2020 2020 2020 206e 616d 6520   ].        name 
+00001c60: 2873 7472 293a 0a20 2020 2020 2020 2020  (str):.         
+00001c70: 2020 204e 616d 6520 6f66 2074 6865 2063     Name of the c
+00001c80: 6172 642e 2055 7365 6420 6173 2061 2063  ard. Used as a c
+00001c90: 6172 6420 6964 656e 7469 6669 6572 2069  ard identifier i
+00001ca0: 6e20 6361 7264 0a20 2020 2020 2020 2020  n card.         
+00001cb0: 2020 206e 6176 6967 6174 696f 6e2e 0a0a     navigation...
+00001cc0: 2020 2020 2020 2020 2020 2020 6047 6f6f              `Goo
+00001cd0: 676c 6520 576f 726b 7370 6163 650a 2020  gle Workspace.  
+00001ce0: 2020 2020 2020 2020 2020 4164 642d 6f6e            Add-on
+00001cf0: 7320 3c68 7474 7073 3a2f 2f64 6576 656c  s <https://devel
+00001d00: 6f70 6572 732e 676f 6f67 6c65 2e63 6f6d  opers.google.com
+00001d10: 2f77 6f72 6b73 7061 6365 2f61 6464 2d6f  /workspace/add-o
+00001d20: 6e73 3e60 5f5f 3a0a 2020 2020 2020 2020  ns>`__:.        
+00001d30: 6669 7865 645f 666f 6f74 6572 2028 676f  fixed_footer (go
+00001d40: 6f67 6c65 2e61 7070 732e 6361 7264 5f76  ogle.apps.card_v
+00001d50: 312e 7479 7065 732e 4361 7264 2e43 6172  1.types.Card.Car
+00001d60: 6446 6978 6564 466f 6f74 6572 293a 0a20  dFixedFooter):. 
+00001d70: 2020 2020 2020 2020 2020 2054 6865 2066             The f
+00001d80: 6978 6564 2066 6f6f 7465 7220 7368 6f77  ixed footer show
+00001d90: 6e20 6174 2074 6865 2062 6f74 746f 6d20  n at the bottom 
+00001da0: 6f66 2074 6869 7320 6361 7264 2e0a 0a20  of this card... 
+00001db0: 2020 2020 2020 2020 2020 2053 6574 7469             Setti
+00001dc0: 6e67 2060 6066 6978 6564 466f 6f74 6572  ng ``fixedFooter
+00001dd0: 6060 2077 6974 686f 7574 2073 7065 6369  `` without speci
+00001de0: 6679 696e 6720 610a 2020 2020 2020 2020  fying a.        
+00001df0: 2020 2020 6060 7072 696d 6172 7942 7574      ``primaryBut
+00001e00: 746f 6e60 6020 6f72 2061 2060 6073 6563  ton`` or a ``sec
+00001e10: 6f6e 6461 7279 4275 7474 6f6e 6060 2063  ondaryButton`` c
+00001e20: 6175 7365 7320 616e 2065 7272 6f72 2e0a  auses an error..
+00001e30: 2020 2020 2020 2020 2020 2020 466f 7220              For 
+00001e40: 4368 6174 2061 7070 732c 2079 6f75 2063  Chat apps, you c
+00001e50: 616e 2075 7365 2066 6978 6564 2066 6f6f  an use fixed foo
+00001e60: 7465 7273 2069 6e0a 2020 2020 2020 2020  ters in.        
+00001e70: 2020 2020 6064 6961 6c6f 6773 203c 6874      `dialogs <ht
+00001e80: 7470 733a 2f2f 6465 7665 6c6f 7065 7273  tps://developers
+00001e90: 2e67 6f6f 676c 652e 636f 6d2f 776f 726b  .google.com/work
+00001ea0: 7370 6163 652f 6368 6174 2f64 6961 6c6f  space/chat/dialo
+00001eb0: 6773 3e60 5f5f 2c0a 2020 2020 2020 2020  gs>`__,.        
+00001ec0: 2020 2020 6275 7420 6e6f 7420 6063 6172      but not `car
+00001ed0: 640a 2020 2020 2020 2020 2020 2020 6d65  d.            me
+00001ee0: 7373 6167 6573 203c 6874 7470 733a 2f2f  ssages <https://
+00001ef0: 6465 7665 6c6f 7065 7273 2e67 6f6f 676c  developers.googl
+00001f00: 652e 636f 6d2f 776f 726b 7370 6163 652f  e.com/workspace/
+00001f10: 6368 6174 2f63 7265 6174 652d 6d65 7373  chat/create-mess
+00001f20: 6167 6573 2363 7265 6174 653e 605f 5f2e  ages#create>`__.
+00001f30: 0a0a 2020 2020 2020 2020 2020 2020 6047  ..            `G
+00001f40: 6f6f 676c 6520 576f 726b 7370 6163 6520  oogle Workspace 
+00001f50: 4164 642d 6f6e 7320 616e 6420 4368 6174  Add-ons and Chat
+00001f60: 0a20 2020 2020 2020 2020 2020 2061 7070  .            app
+00001f70: 7320 3c68 7474 7073 3a2f 2f64 6576 656c  s <https://devel
+00001f80: 6f70 6572 732e 676f 6f67 6c65 2e63 6f6d  opers.google.com
+00001f90: 2f77 6f72 6b73 7061 6365 2f65 7874 656e  /workspace/exten
+00001fa0: 643e 605f 5f3a 0a20 2020 2020 2020 2064  d>`__:.        d
+00001fb0: 6973 706c 6179 5f73 7479 6c65 2028 676f  isplay_style (go
+00001fc0: 6f67 6c65 2e61 7070 732e 6361 7264 5f76  ogle.apps.card_v
+00001fd0: 312e 7479 7065 732e 4361 7264 2e44 6973  1.types.Card.Dis
+00001fe0: 706c 6179 5374 796c 6529 3a0a 2020 2020  playStyle):.    
+00001ff0: 2020 2020 2020 2020 496e 2047 6f6f 676c          In Googl
+00002000: 6520 576f 726b 7370 6163 6520 4164 642d  e Workspace Add-
+00002010: 6f6e 732c 2073 6574 7320 7468 6520 6469  ons, sets the di
+00002020: 7370 6c61 7920 7072 6f70 6572 7469 6573  splay properties
+00002030: 206f 660a 2020 2020 2020 2020 2020 2020   of.            
+00002040: 7468 6520 6060 7065 656b 4361 7264 4865  the ``peekCardHe
+00002050: 6164 6572 6060 2e0a 0a20 2020 2020 2020  ader``...       
+00002060: 2020 2020 2060 476f 6f67 6c65 2057 6f72       `Google Wor
+00002070: 6b73 7061 6365 0a20 2020 2020 2020 2020  kspace.         
+00002080: 2020 2041 6464 2d6f 6e73 203c 6874 7470     Add-ons <http
+00002090: 733a 2f2f 6465 7665 6c6f 7065 7273 2e67  s://developers.g
+000020a0: 6f6f 676c 652e 636f 6d2f 776f 726b 7370  oogle.com/worksp
+000020b0: 6163 652f 6164 642d 6f6e 733e 605f 5f3a  ace/add-ons>`__:
+000020c0: 0a20 2020 2020 2020 2070 6565 6b5f 6361  .        peek_ca
+000020d0: 7264 5f68 6561 6465 7220 2867 6f6f 676c  rd_header (googl
+000020e0: 652e 6170 7073 2e63 6172 645f 7631 2e74  e.apps.card_v1.t
+000020f0: 7970 6573 2e43 6172 642e 4361 7264 4865  ypes.Card.CardHe
+00002100: 6164 6572 293a 0a20 2020 2020 2020 2020  ader):.         
+00002110: 2020 2057 6865 6e20 6469 7370 6c61 7969     When displayi
+00002120: 6e67 2063 6f6e 7465 7874 7561 6c20 636f  ng contextual co
+00002130: 6e74 656e 742c 2074 6865 2070 6565 6b20  ntent, the peek 
+00002140: 6361 7264 2068 6561 6465 720a 2020 2020  card header.    
+00002150: 2020 2020 2020 2020 6163 7473 2061 7320          acts as 
+00002160: 6120 706c 6163 6568 6f6c 6465 7220 736f  a placeholder so
+00002170: 2074 6861 7420 7468 6520 7573 6572 2063   that the user c
+00002180: 616e 206e 6176 6967 6174 6520 666f 7277  an navigate forw
+00002190: 6172 640a 2020 2020 2020 2020 2020 2020  ard.            
+000021a0: 6265 7477 6565 6e20 7468 6520 686f 6d65  between the home
+000021b0: 7061 6765 2063 6172 6473 2061 6e64 2074  page cards and t
+000021c0: 6865 2063 6f6e 7465 7874 7561 6c20 6361  he contextual ca
+000021d0: 7264 732e 0a0a 2020 2020 2020 2020 2020  rds...          
+000021e0: 2020 6047 6f6f 676c 6520 576f 726b 7370    `Google Worksp
+000021f0: 6163 650a 2020 2020 2020 2020 2020 2020  ace.            
+00002200: 4164 642d 6f6e 7320 3c68 7474 7073 3a2f  Add-ons <https:/
+00002210: 2f64 6576 656c 6f70 6572 732e 676f 6f67  /developers.goog
+00002220: 6c65 2e63 6f6d 2f77 6f72 6b73 7061 6365  le.com/workspace
+00002230: 2f61 6464 2d6f 6e73 3e60 5f5f 3a0a 2020  /add-ons>`__:.  
+00002240: 2020 2222 220a 0a20 2020 2063 6c61 7373    """..    class
+00002250: 2044 6976 6964 6572 5374 796c 6528 7072   DividerStyle(pr
+00002260: 6f74 6f2e 456e 756d 293a 0a20 2020 2020  oto.Enum):.     
+00002270: 2020 2072 2222 2254 6865 2064 6976 6964     r"""The divid
+00002280: 6572 2073 7479 6c65 206f 6620 6120 6361  er style of a ca
+00002290: 7264 2e20 4375 7272 656e 746c 7920 6f6e  rd. Currently on
+000022a0: 6c79 2075 7365 6420 666f 7220 6469 7669  ly used for divi
+000022b0: 6465 7273 0a20 2020 2020 2020 2062 6574  ders.        bet
+000022c0: 7765 656e 7320 6361 7264 2073 6563 7469  weens card secti
+000022d0: 6f6e 732e 0a0a 2020 2020 2020 2020 6047  ons...        `G
+000022e0: 6f6f 676c 6520 576f 726b 7370 6163 6520  oogle Workspace 
+000022f0: 4164 642d 6f6e 7320 616e 6420 4368 6174  Add-ons and Chat
+00002300: 0a20 2020 2020 2020 2061 7070 7320 3c68  .        apps <h
+00002310: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
+00002320: 732e 676f 6f67 6c65 2e63 6f6d 2f77 6f72  s.google.com/wor
+00002330: 6b73 7061 6365 2f65 7874 656e 643e 605f  kspace/extend>`_
+00002340: 5f3a 0a0a 2020 2020 2020 2020 5661 6c75  _:..        Valu
+00002350: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+00002360: 4449 5649 4445 525f 5354 594c 455f 554e  DIVIDER_STYLE_UN
+00002370: 5350 4543 4946 4945 4420 2830 293a 0a20  SPECIFIED (0):. 
+00002380: 2020 2020 2020 2020 2020 2020 2020 2044                 D
+00002390: 6f6e 2774 2075 7365 2e20 556e 7370 6563  on't use. Unspec
+000023a0: 6966 6965 642e 0a20 2020 2020 2020 2020  ified..         
+000023b0: 2020 2053 4f4c 4944 5f44 4956 4944 4552     SOLID_DIVIDER
+000023c0: 2028 3129 3a0a 2020 2020 2020 2020 2020   (1):.          
+000023d0: 2020 2020 2020 4465 6661 756c 7420 6f70        Default op
+000023e0: 7469 6f6e 2e20 5265 6e64 6572 2061 2073  tion. Render a s
+000023f0: 6f6c 6964 2064 6976 6964 6572 0a20 2020  olid divider.   
+00002400: 2020 2020 2020 2020 2020 2020 2062 6574               bet
+00002410: 7765 656e 2073 6563 7469 6f6e 732e 0a20  ween sections.. 
+00002420: 2020 2020 2020 2020 2020 204e 4f5f 4449             NO_DI
+00002430: 5649 4445 5220 2832 293a 0a20 2020 2020  VIDER (2):.     
+00002440: 2020 2020 2020 2020 2020 2049 6620 7365             If se
+00002450: 742c 206e 6f20 6469 7669 6465 7220 6973  t, no divider is
+00002460: 2072 656e 6465 7265 6420 6265 7477 6565   rendered betwee
+00002470: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
+00002480: 2020 7365 6374 696f 6e73 2e0a 2020 2020    sections..    
+00002490: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000024a0: 4449 5649 4445 525f 5354 594c 455f 554e  DIVIDER_STYLE_UN
+000024b0: 5350 4543 4946 4945 4420 3d20 300a 2020  SPECIFIED = 0.  
+000024c0: 2020 2020 2020 534f 4c49 445f 4449 5649        SOLID_DIVI
+000024d0: 4445 5220 3d20 310a 2020 2020 2020 2020  DER = 1.        
+000024e0: 4e4f 5f44 4956 4944 4552 203d 2032 0a0a  NO_DIVIDER = 2..
+000024f0: 2020 2020 636c 6173 7320 4469 7370 6c61      class Displa
+00002500: 7953 7479 6c65 2870 726f 746f 2e45 6e75  yStyle(proto.Enu
+00002510: 6d29 3a0a 2020 2020 2020 2020 7222 2222  m):.        r"""
+00002520: 496e 2047 6f6f 676c 6520 576f 726b 7370  In Google Worksp
+00002530: 6163 6520 4164 642d 6f6e 732c 2064 6574  ace Add-ons, det
+00002540: 6572 6d69 6e65 7320 686f 7720 6120 6361  ermines how a ca
+00002550: 7264 2069 7320 6469 7370 6c61 7965 642e  rd is displayed.
+00002560: 0a0a 2020 2020 2020 2020 6047 6f6f 676c  ..        `Googl
+00002570: 6520 576f 726b 7370 6163 650a 2020 2020  e Workspace.    
+00002580: 2020 2020 4164 642d 6f6e 7320 3c68 7474      Add-ons <htt
+00002590: 7073 3a2f 2f64 6576 656c 6f70 6572 732e  ps://developers.
+000025a0: 676f 6f67 6c65 2e63 6f6d 2f77 6f72 6b73  google.com/works
+000025b0: 7061 6365 2f61 6464 2d6f 6e73 3e60 5f5f  pace/add-ons>`__
+000025c0: 3a0a 0a20 2020 2020 2020 2056 616c 7565  :..        Value
+000025d0: 733a 0a20 2020 2020 2020 2020 2020 2044  s:.            D
+000025e0: 4953 504c 4159 5f53 5459 4c45 5f55 4e53  ISPLAY_STYLE_UNS
+000025f0: 5045 4349 4649 4544 2028 3029 3a0a 2020  PECIFIED (0):.  
+00002600: 2020 2020 2020 2020 2020 2020 2020 446f                Do
+00002610: 6e27 7420 7573 652e 2055 6e73 7065 6369  n't use. Unspeci
+00002620: 6669 6564 2e0a 2020 2020 2020 2020 2020  fied..          
+00002630: 2020 5045 454b 2028 3129 3a0a 2020 2020    PEEK (1):.    
+00002640: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+00002650: 6865 6164 6572 206f 6620 7468 6520 6361  header of the ca
+00002660: 7264 2061 7070 6561 7273 2061 7420 7468  rd appears at th
+00002670: 6520 626f 7474 6f6d 0a20 2020 2020 2020  e bottom.       
+00002680: 2020 2020 2020 2020 206f 6620 7468 6520           of the 
+00002690: 7369 6465 6261 722c 2070 6172 7469 616c  sidebar, partial
+000026a0: 6c79 2063 6f76 6572 696e 6720 7468 6520  ly covering the 
+000026b0: 6375 7272 656e 740a 2020 2020 2020 2020  current.        
+000026c0: 2020 2020 2020 2020 746f 7020 6361 7264          top card
+000026d0: 206f 6620 7468 6520 7374 6163 6b2e 2043   of the stack. C
+000026e0: 6c69 636b 696e 6720 7468 6520 6865 6164  licking the head
+000026f0: 6572 2070 6f70 730a 2020 2020 2020 2020  er pops.        
+00002700: 2020 2020 2020 2020 7468 6520 6361 7264          the card
+00002710: 2069 6e74 6f20 7468 6520 6361 7264 2073   into the card s
+00002720: 7461 636b 2e20 4966 2074 6865 2063 6172  tack. If the car
+00002730: 6420 6861 7320 6e6f 0a20 2020 2020 2020  d has no.       
+00002740: 2020 2020 2020 2020 2068 6561 6465 722c           header,
+00002750: 2061 2067 656e 6572 6174 6564 2068 6561   a generated hea
+00002760: 6465 7220 6973 2075 7365 6420 696e 7374  der is used inst
+00002770: 6561 642e 0a20 2020 2020 2020 2020 2020  ead..           
+00002780: 2052 4550 4c41 4345 2028 3229 3a0a 2020   REPLACE (2):.  
+00002790: 2020 2020 2020 2020 2020 2020 2020 4465                De
+000027a0: 6661 756c 7420 7661 6c75 652e 2054 6865  fault value. The
+000027b0: 2063 6172 6420 6973 2073 686f 776e 2062   card is shown b
+000027c0: 7920 7265 706c 6163 696e 670a 2020 2020  y replacing.    
+000027d0: 2020 2020 2020 2020 2020 2020 7468 6520              the 
+000027e0: 7669 6577 206f 6620 7468 6520 746f 7020  view of the top 
+000027f0: 6361 7264 2069 6e20 7468 6520 6361 7264  card in the card
+00002800: 2073 7461 636b 2e0a 2020 2020 2020 2020   stack..        
+00002810: 2222 220a 2020 2020 2020 2020 4449 5350  """.        DISP
+00002820: 4c41 595f 5354 594c 455f 554e 5350 4543  LAY_STYLE_UNSPEC
+00002830: 4946 4945 4420 3d20 300a 2020 2020 2020  IFIED = 0.      
+00002840: 2020 5045 454b 203d 2031 0a20 2020 2020    PEEK = 1.     
+00002850: 2020 2052 4550 4c41 4345 203d 2032 0a0a     REPLACE = 2..
+00002860: 2020 2020 636c 6173 7320 4361 7264 4865      class CardHe
+00002870: 6164 6572 2870 726f 746f 2e4d 6573 7361  ader(proto.Messa
+00002880: 6765 293a 0a20 2020 2020 2020 2072 2222  ge):.        r""
+00002890: 2252 6570 7265 7365 6e74 7320 6120 6361  "Represents a ca
+000028a0: 7264 2068 6561 6465 722e 2046 6f72 2061  rd header. For a
+000028b0: 6e20 6578 616d 706c 6520 696e 2047 6f6f  n example in Goo
+000028c0: 676c 6520 4368 6174 2061 7070 732c 2073  gle Chat apps, s
+000028d0: 6565 0a20 2020 2020 2020 2060 4164 6420  ee.        `Add 
+000028e0: 610a 2020 2020 2020 2020 6865 6164 6572  a.        header
+000028f0: 203c 6874 7470 733a 2f2f 6465 7665 6c6f   <https://develo
+00002900: 7065 7273 2e67 6f6f 676c 652e 636f 6d2f  pers.google.com/
+00002910: 776f 726b 7370 6163 652f 6368 6174 2f64  workspace/chat/d
+00002920: 6573 6967 6e2d 636f 6d70 6f6e 656e 7473  esign-components
+00002930: 2d63 6172 642d 6469 616c 6f67 2361 6464  -card-dialog#add
+00002940: 5f61 5f68 6561 6465 723e 605f 5f2e 0a0a  _a_header>`__...
+00002950: 2020 2020 2020 2020 6047 6f6f 676c 6520          `Google 
+00002960: 576f 726b 7370 6163 6520 4164 642d 6f6e  Workspace Add-on
+00002970: 7320 616e 6420 4368 6174 0a20 2020 2020  s and Chat.     
+00002980: 2020 2061 7070 7320 3c68 7474 7073 3a2f     apps <https:/
+00002990: 2f64 6576 656c 6f70 6572 732e 676f 6f67  /developers.goog
+000029a0: 6c65 2e63 6f6d 2f77 6f72 6b73 7061 6365  le.com/workspace
+000029b0: 2f65 7874 656e 643e 605f 5f3a 0a0a 2020  /extend>`__:..  
+000029c0: 2020 2020 2020 4174 7472 6962 7574 6573        Attributes
+000029d0: 3a0a 2020 2020 2020 2020 2020 2020 7469  :.            ti
+000029e0: 746c 6520 2873 7472 293a 0a20 2020 2020  tle (str):.     
+000029f0: 2020 2020 2020 2020 2020 2052 6571 7569             Requi
+00002a00: 7265 642e 2054 6865 2074 6974 6c65 206f  red. The title o
+00002a10: 6620 7468 6520 6361 7264 2068 6561 6465  f the card heade
+00002a20: 722e 0a20 2020 2020 2020 2020 2020 2020  r..             
+00002a30: 2020 2054 6865 2068 6561 6465 7220 6861     The header ha
+00002a40: 7320 6120 6669 7865 6420 6865 6967 6874  s a fixed height
+00002a50: 3a20 6966 2062 6f74 6820 610a 2020 2020  : if both a.    
+00002a60: 2020 2020 2020 2020 2020 2020 7469 746c              titl
+00002a70: 6520 616e 6420 7375 6274 6974 6c65 2061  e and subtitle a
+00002a80: 7265 2073 7065 6369 6669 6564 2c20 6561  re specified, ea
+00002a90: 6368 2074 616b 6573 2075 700a 2020 2020  ch takes up.    
+00002aa0: 2020 2020 2020 2020 2020 2020 6f6e 6520              one 
+00002ab0: 6c69 6e65 2e20 4966 206f 6e6c 7920 7468  line. If only th
+00002ac0: 6520 7469 746c 6520 6973 2073 7065 6369  e title is speci
+00002ad0: 6669 6564 2c20 6974 0a20 2020 2020 2020  fied, it.       
+00002ae0: 2020 2020 2020 2020 2074 616b 6573 2075           takes u
+00002af0: 7020 626f 7468 206c 696e 6573 2e0a 2020  p both lines..  
+00002b00: 2020 2020 2020 2020 2020 7375 6274 6974            subtit
+00002b10: 6c65 2028 7374 7229 3a0a 2020 2020 2020  le (str):.      
+00002b20: 2020 2020 2020 2020 2020 5468 6520 7375            The su
+00002b30: 6274 6974 6c65 206f 6620 7468 6520 6361  btitle of the ca
+00002b40: 7264 2068 6561 6465 722e 2049 6620 7370  rd header. If sp
+00002b50: 6563 6966 6965 642c 2061 7070 6561 7273  ecified, appears
+00002b60: 206f 6e0a 2020 2020 2020 2020 2020 2020   on.            
+00002b70: 2020 2020 6974 7320 6f77 6e20 6c69 6e65      its own line
+00002b80: 2062 656c 6f77 2074 6865 2060 6074 6974   below the ``tit
+00002b90: 6c65 6060 2e0a 2020 2020 2020 2020 2020  le``..          
+00002ba0: 2020 696d 6167 655f 7479 7065 2028 676f    image_type (go
+00002bb0: 6f67 6c65 2e61 7070 732e 6361 7264 5f76  ogle.apps.card_v
+00002bc0: 312e 7479 7065 732e 5769 6467 6574 2e49  1.types.Widget.I
+00002bd0: 6d61 6765 5479 7065 293a 0a20 2020 2020  mageType):.     
+00002be0: 2020 2020 2020 2020 2020 2054 6865 2073             The s
+00002bf0: 6861 7065 2075 7365 6420 746f 2063 726f  hape used to cro
+00002c00: 7020 7468 6520 696d 6167 652e 0a0a 2020  p the image...  
+00002c10: 2020 2020 2020 2020 2020 2020 2020 6047                `G
+00002c20: 6f6f 676c 6520 576f 726b 7370 6163 6520  oogle Workspace 
+00002c30: 4164 642d 6f6e 7320 616e 6420 4368 6174  Add-ons and Chat
+00002c40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002c50: 2061 7070 7320 3c68 7474 7073 3a2f 2f64   apps <https://d
+00002c60: 6576 656c 6f70 6572 732e 676f 6f67 6c65  evelopers.google
+00002c70: 2e63 6f6d 2f77 6f72 6b73 7061 6365 2f65  .com/workspace/e
+00002c80: 7874 656e 643e 605f 5f3a 0a20 2020 2020  xtend>`__:.     
+00002c90: 2020 2020 2020 2069 6d61 6765 5f75 726c         image_url
+00002ca0: 2028 7374 7229 3a0a 2020 2020 2020 2020   (str):.        
+00002cb0: 2020 2020 2020 2020 5468 6520 4854 5450          The HTTP
+00002cc0: 5320 5552 4c20 6f66 2074 6865 2069 6d61  S URL of the ima
+00002cd0: 6765 2069 6e20 7468 6520 6361 7264 0a20  ge in the card. 
+00002ce0: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+00002cf0: 6561 6465 722e 0a20 2020 2020 2020 2020  eader..         
+00002d00: 2020 2069 6d61 6765 5f61 6c74 5f74 6578     image_alt_tex
+00002d10: 7420 2873 7472 293a 0a20 2020 2020 2020  t (str):.       
+00002d20: 2020 2020 2020 2020 2054 6865 2061 6c74           The alt
+00002d30: 6572 6e61 7469 7665 2074 6578 7420 6f66  ernative text of
+00002d40: 2074 6869 7320 696d 6167 6520 7468 6174   this image that
+00002d50: 2773 0a20 2020 2020 2020 2020 2020 2020  's.             
+00002d60: 2020 2075 7365 6420 666f 7220 6163 6365     used for acce
+00002d70: 7373 6962 696c 6974 792e 0a20 2020 2020  ssibility..     
+00002d80: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+00002d90: 7469 746c 653a 2073 7472 203d 2070 726f  title: str = pro
+00002da0: 746f 2e46 6965 6c64 280a 2020 2020 2020  to.Field(.      
+00002db0: 2020 2020 2020 7072 6f74 6f2e 5354 5249        proto.STRI
+00002dc0: 4e47 2c0a 2020 2020 2020 2020 2020 2020  NG,.            
+00002dd0: 6e75 6d62 6572 3d31 2c0a 2020 2020 2020  number=1,.      
+00002de0: 2020 290a 2020 2020 2020 2020 7375 6274    ).        subt
+00002df0: 6974 6c65 3a20 7374 7220 3d20 7072 6f74  itle: str = prot
+00002e00: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+00002e10: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
+00002e20: 472c 0a20 2020 2020 2020 2020 2020 206e  G,.            n
+00002e30: 756d 6265 723d 322c 0a20 2020 2020 2020  umber=2,.       
+00002e40: 2029 0a20 2020 2020 2020 2069 6d61 6765   ).        image
+00002e50: 5f74 7970 653a 2022 5769 6467 6574 2e49  _type: "Widget.I
+00002e60: 6d61 6765 5479 7065 2220 3d20 7072 6f74  mageType" = prot
+00002e70: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+00002e80: 2020 2020 2070 726f 746f 2e45 4e55 4d2c       proto.ENUM,
+00002e90: 0a20 2020 2020 2020 2020 2020 206e 756d  .            num
+00002ea0: 6265 723d 332c 0a20 2020 2020 2020 2020  ber=3,.         
+00002eb0: 2020 2065 6e75 6d3d 2257 6964 6765 742e     enum="Widget.
+00002ec0: 496d 6167 6554 7970 6522 2c0a 2020 2020  ImageType",.    
+00002ed0: 2020 2020 290a 2020 2020 2020 2020 696d      ).        im
+00002ee0: 6167 655f 7572 6c3a 2073 7472 203d 2070  age_url: str = p
+00002ef0: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
+00002f00: 2020 2020 2020 2020 7072 6f74 6f2e 5354          proto.ST
+00002f10: 5249 4e47 2c0a 2020 2020 2020 2020 2020  RING,.          
+00002f20: 2020 6e75 6d62 6572 3d34 2c0a 2020 2020    number=4,.    
+00002f30: 2020 2020 290a 2020 2020 2020 2020 696d      ).        im
+00002f40: 6167 655f 616c 745f 7465 7874 3a20 7374  age_alt_text: st
+00002f50: 7220 3d20 7072 6f74 6f2e 4669 656c 6428  r = proto.Field(
+00002f60: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
+00002f70: 746f 2e53 5452 494e 472c 0a20 2020 2020  to.STRING,.     
+00002f80: 2020 2020 2020 206e 756d 6265 723d 352c         number=5,
+00002f90: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00002fa0: 636c 6173 7320 5365 6374 696f 6e28 7072  class Section(pr
+00002fb0: 6f74 6f2e 4d65 7373 6167 6529 3a0a 2020  oto.Message):.  
+00002fc0: 2020 2020 2020 7222 2222 4120 7365 6374        r"""A sect
+00002fd0: 696f 6e20 636f 6e74 6169 6e73 2061 2063  ion contains a c
+00002fe0: 6f6c 6c65 6374 696f 6e20 6f66 2077 6964  ollection of wid
+00002ff0: 6765 7473 2074 6861 7420 6172 6520 7265  gets that are re
+00003000: 6e64 6572 6564 0a20 2020 2020 2020 2076  ndered.        v
+00003010: 6572 7469 6361 6c6c 7920 696e 2074 6865  ertically in the
+00003020: 206f 7264 6572 2074 6861 7420 7468 6579   order that they
+00003030: 2772 6520 7370 6563 6966 6965 642e 0a0a  're specified...
+00003040: 2020 2020 2020 2020 6047 6f6f 676c 6520          `Google 
+00003050: 576f 726b 7370 6163 6520 4164 642d 6f6e  Workspace Add-on
+00003060: 7320 616e 6420 4368 6174 0a20 2020 2020  s and Chat.     
+00003070: 2020 2061 7070 7320 3c68 7474 7073 3a2f     apps <https:/
+00003080: 2f64 6576 656c 6f70 6572 732e 676f 6f67  /developers.goog
+00003090: 6c65 2e63 6f6d 2f77 6f72 6b73 7061 6365  le.com/workspace
+000030a0: 2f65 7874 656e 643e 605f 5f3a 0a0a 2020  /extend>`__:..  
+000030b0: 2020 2020 2020 4174 7472 6962 7574 6573        Attributes
+000030c0: 3a0a 2020 2020 2020 2020 2020 2020 6865  :.            he
+000030d0: 6164 6572 2028 7374 7229 3a0a 2020 2020  ader (str):.    
+000030e0: 2020 2020 2020 2020 2020 2020 5465 7874              Text
+000030f0: 2074 6861 7420 6170 7065 6172 7320 6174   that appears at
+00003100: 2074 6865 2074 6f70 206f 6620 6120 7365   the top of a se
+00003110: 6374 696f 6e2e 2053 7570 706f 7274 7320  ction. Supports 
+00003120: 7369 6d70 6c65 0a20 2020 2020 2020 2020  simple.         
+00003130: 2020 2020 2020 2048 544d 4c20 666f 726d         HTML form
+00003140: 6174 7465 6420 7465 7874 2e20 466f 7220  atted text. For 
+00003150: 6d6f 7265 2069 6e66 6f72 6d61 7469 6f6e  more information
+00003160: 2061 626f 7574 2066 6f72 6d61 7474 696e   about formattin
+00003170: 670a 2020 2020 2020 2020 2020 2020 2020  g.              
+00003180: 2020 7465 7874 2c20 7365 6520 6046 6f72    text, see `For
+00003190: 6d61 7474 696e 6720 7465 7874 2069 6e20  matting text in 
+000031a0: 476f 6f67 6c65 2043 6861 740a 2020 2020  Google Chat.    
+000031b0: 2020 2020 2020 2020 2020 2020 6170 7073              apps
+000031c0: 203c 6874 7470 733a 2f2f 6465 7665 6c6f   <https://develo
+000031d0: 7065 7273 2e67 6f6f 676c 652e 636f 6d2f  pers.google.com/
+000031e0: 776f 726b 7370 6163 652f 6368 6174 2f66  workspace/chat/f
+000031f0: 6f72 6d61 742d 6d65 7373 6167 6573 2363  ormat-messages#c
+00003200: 6172 642d 666f 726d 6174 7469 6e67 3e60  ard-formatting>`
+00003210: 5f5f 0a20 2020 2020 2020 2020 2020 2020  __.             
+00003220: 2020 2061 6e64 2060 466f 726d 6174 7469     and `Formatti
+00003230: 6e67 2074 6578 7420 696e 2047 6f6f 676c  ng text in Googl
+00003240: 6520 576f 726b 7370 6163 650a 2020 2020  e Workspace.    
+00003250: 2020 2020 2020 2020 2020 2020 4164 642d              Add-
+00003260: 6f6e 7320 3c68 7474 7073 3a2f 2f64 6576  ons <https://dev
+00003270: 656c 6f70 6572 732e 676f 6f67 6c65 2e63  elopers.google.c
+00003280: 6f6d 2f61 7070 732d 7363 7269 7074 2f61  om/apps-script/a
+00003290: 6464 2d6f 6e73 2f63 6f6e 6365 7074 732f  dd-ons/concepts/
+000032a0: 7769 6467 6574 7323 7465 7874 5f66 6f72  widgets#text_for
+000032b0: 6d61 7474 696e 673e 605f 5f2e 0a20 2020  matting>`__..   
+000032c0: 2020 2020 2020 2020 2077 6964 6765 7473           widgets
+000032d0: 2028 4d75 7461 626c 6553 6571 7565 6e63   (MutableSequenc
+000032e0: 655b 676f 6f67 6c65 2e61 7070 732e 6361  e[google.apps.ca
+000032f0: 7264 5f76 312e 7479 7065 732e 5769 6467  rd_v1.types.Widg
+00003300: 6574 5d29 3a0a 2020 2020 2020 2020 2020  et]):.          
+00003310: 2020 2020 2020 416c 6c20 7468 6520 7769        All the wi
+00003320: 6467 6574 7320 696e 2074 6865 2073 6563  dgets in the sec
+00003330: 7469 6f6e 2e0a 2020 2020 2020 2020 2020  tion..          
+00003340: 2020 2020 2020 4d75 7374 2063 6f6e 7461        Must conta
+00003350: 696e 2061 7420 6c65 6173 7420 6f6e 6520  in at least one 
+00003360: 7769 6467 6574 2e0a 2020 2020 2020 2020  widget..        
+00003370: 2020 2020 636f 6c6c 6170 7369 626c 6520      collapsible 
+00003380: 2862 6f6f 6c29 3a0a 2020 2020 2020 2020  (bool):.        
+00003390: 2020 2020 2020 2020 496e 6469 6361 7465          Indicate
+000033a0: 7320 7768 6574 6865 7220 7468 6973 2073  s whether this s
+000033b0: 6563 7469 6f6e 2069 7320 636f 6c6c 6170  ection is collap
+000033c0: 7369 626c 652e 0a0a 2020 2020 2020 2020  sible...        
+000033d0: 2020 2020 2020 2020 436f 6c6c 6170 7369          Collapsi
+000033e0: 626c 6520 7365 6374 696f 6e73 2068 6964  ble sections hid
+000033f0: 6520 736f 6d65 206f 7220 616c 6c20 7769  e some or all wi
+00003400: 6467 6574 732c 2062 7574 2075 7365 7273  dgets, but users
+00003410: 2063 616e 0a20 2020 2020 2020 2020 2020   can.           
+00003420: 2020 2020 2065 7870 616e 6420 7468 6520       expand the 
+00003430: 7365 6374 696f 6e20 746f 2072 6576 6561  section to revea
+00003440: 6c20 7468 6520 6869 6464 656e 2077 6964  l the hidden wid
+00003450: 6765 7473 2062 7920 636c 6963 6b69 6e67  gets by clicking
+00003460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003470: 202a 2a53 686f 7720 6d6f 7265 2a2a 2e20   **Show more**. 
+00003480: 5573 6572 7320 6361 6e20 6869 6465 2074  Users can hide t
+00003490: 6865 2077 6964 6765 7473 2061 6761 696e  he widgets again
+000034a0: 2062 7920 636c 6963 6b69 6e67 0a20 2020   by clicking.   
+000034b0: 2020 2020 2020 2020 2020 2020 202a 2a53               **S
+000034c0: 686f 7720 6c65 7373 2a2a 2e0a 0a20 2020  how less**...   
+000034d0: 2020 2020 2020 2020 2020 2020 2054 6f20               To 
+000034e0: 6465 7465 726d 696e 6520 7768 6963 6820  determine which 
+000034f0: 7769 6467 6574 7320 6172 6520 6869 6464  widgets are hidd
+00003500: 656e 2c20 7370 6563 6966 790a 2020 2020  en, specify.    
+00003510: 2020 2020 2020 2020 2020 2020 6060 756e              ``un
+00003520: 636f 6c6c 6170 7369 626c 6557 6964 6765  collapsibleWidge
+00003530: 7473 436f 756e 7460 602e 0a20 2020 2020  tsCount``..     
+00003540: 2020 2020 2020 2075 6e63 6f6c 6c61 7073         uncollaps
+00003550: 6962 6c65 5f77 6964 6765 7473 5f63 6f75  ible_widgets_cou
+00003560: 6e74 2028 696e 7429 3a0a 2020 2020 2020  nt (int):.      
+00003570: 2020 2020 2020 2020 2020 5468 6520 6e75            The nu
+00003580: 6d62 6572 206f 6620 756e 636f 6c6c 6170  mber of uncollap
+00003590: 7369 626c 6520 7769 6467 6574 7320 7768  sible widgets wh
+000035a0: 6963 6820 7265 6d61 696e 2076 6973 6962  ich remain visib
+000035b0: 6c65 0a20 2020 2020 2020 2020 2020 2020  le.             
+000035c0: 2020 2065 7665 6e20 7768 656e 2061 2073     even when a s
+000035d0: 6563 7469 6f6e 2069 7320 636f 6c6c 6170  ection is collap
+000035e0: 7365 642e 0a0a 2020 2020 2020 2020 2020  sed...          
+000035f0: 2020 2020 2020 466f 7220 6578 616d 706c        For exampl
+00003600: 652c 2077 6865 6e20 6120 7365 6374 696f  e, when a sectio
+00003610: 6e20 636f 6e74 6169 6e73 2066 6976 6520  n contains five 
+00003620: 7769 6467 6574 7320 616e 6420 7468 650a  widgets and the.
+00003630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003640: 6060 756e 636f 6c6c 6170 7369 626c 6557  ``uncollapsibleW
+00003650: 6964 6765 7473 436f 756e 7460 6020 6973  idgetsCount`` is
+00003660: 2073 6574 2074 6f20 6060 3260 602c 2074   set to ``2``, t
+00003670: 6865 2066 6972 7374 2074 776f 0a20 2020  he first two.   
+00003680: 2020 2020 2020 2020 2020 2020 2077 6964               wid
+00003690: 6765 7473 2061 7265 2061 6c77 6179 7320  gets are always 
+000036a0: 7368 6f77 6e20 616e 6420 7468 6520 6c61  shown and the la
+000036b0: 7374 2074 6872 6565 2061 7265 2063 6f6c  st three are col
+000036c0: 6c61 7073 6564 2062 790a 2020 2020 2020  lapsed by.      
+000036d0: 2020 2020 2020 2020 2020 6465 6661 756c            defaul
+000036e0: 742e 2054 6865 2060 6075 6e63 6f6c 6c61  t. The ``uncolla
+000036f0: 7073 6962 6c65 5769 6467 6574 7343 6f75  psibleWidgetsCou
+00003700: 6e74 6060 2069 7320 7461 6b65 6e20 696e  nt`` is taken in
+00003710: 746f 0a20 2020 2020 2020 2020 2020 2020  to.             
+00003720: 2020 2061 6363 6f75 6e74 206f 6e6c 7920     account only 
+00003730: 7768 656e 2060 6063 6f6c 6c61 7073 6962  when ``collapsib
+00003740: 6c65 6060 2069 7320 6060 7472 7565 6060  le`` is ``true``
+00003750: 2e0a 2020 2020 2020 2020 2222 220a 0a20  ..        """.. 
+00003760: 2020 2020 2020 2068 6561 6465 723a 2073         header: s
+00003770: 7472 203d 2070 726f 746f 2e46 6965 6c64  tr = proto.Field
+00003780: 280a 2020 2020 2020 2020 2020 2020 7072  (.            pr
+00003790: 6f74 6f2e 5354 5249 4e47 2c0a 2020 2020  oto.STRING,.    
+000037a0: 2020 2020 2020 2020 6e75 6d62 6572 3d31          number=1
+000037b0: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+000037c0: 2020 2020 7769 6467 6574 733a 204d 7574      widgets: Mut
+000037d0: 6162 6c65 5365 7175 656e 6365 5b22 5769  ableSequence["Wi
+000037e0: 6467 6574 225d 203d 2070 726f 746f 2e52  dget"] = proto.R
+000037f0: 6570 6561 7465 6446 6965 6c64 280a 2020  epeatedField(.  
+00003800: 2020 2020 2020 2020 2020 7072 6f74 6f2e            proto.
+00003810: 4d45 5353 4147 452c 0a20 2020 2020 2020  MESSAGE,.       
+00003820: 2020 2020 206e 756d 6265 723d 322c 0a20       number=2,. 
+00003830: 2020 2020 2020 2020 2020 206d 6573 7361             messa
+00003840: 6765 3d22 5769 6467 6574 222c 0a20 2020  ge="Widget",.   
+00003850: 2020 2020 2029 0a20 2020 2020 2020 2063       ).        c
+00003860: 6f6c 6c61 7073 6962 6c65 3a20 626f 6f6c  ollapsible: bool
+00003870: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
+00003880: 2020 2020 2020 2020 2020 2020 7072 6f74              prot
+00003890: 6f2e 424f 4f4c 2c0a 2020 2020 2020 2020  o.BOOL,.        
+000038a0: 2020 2020 6e75 6d62 6572 3d35 2c0a 2020      number=5,.  
+000038b0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+000038c0: 756e 636f 6c6c 6170 7369 626c 655f 7769  uncollapsible_wi
+000038d0: 6467 6574 735f 636f 756e 743a 2069 6e74  dgets_count: int
+000038e0: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
+000038f0: 2020 2020 2020 2020 2020 2020 7072 6f74              prot
+00003900: 6f2e 494e 5433 322c 0a20 2020 2020 2020  o.INT32,.       
+00003910: 2020 2020 206e 756d 6265 723d 362c 0a20       number=6,. 
+00003920: 2020 2020 2020 2029 0a0a 2020 2020 636c         )..    cl
+00003930: 6173 7320 4361 7264 4163 7469 6f6e 2870  ass CardAction(p
+00003940: 726f 746f 2e4d 6573 7361 6765 293a 0a20  roto.Message):. 
+00003950: 2020 2020 2020 2072 2222 2241 2063 6172         r"""A car
+00003960: 6420 6163 7469 6f6e 2069 7320 7468 6520  d action is the 
+00003970: 6163 7469 6f6e 2061 7373 6f63 6961 7465  action associate
+00003980: 6420 7769 7468 2074 6865 2063 6172 642e  d with the card.
+00003990: 2046 6f72 2065 7861 6d70 6c65 2c0a 2020   For example,.  
+000039a0: 2020 2020 2020 616e 2069 6e76 6f69 6365        an invoice
+000039b0: 2063 6172 6420 6d69 6768 7420 696e 636c   card might incl
+000039c0: 7564 6520 6163 7469 6f6e 7320 7375 6368  ude actions such
+000039d0: 2061 7320 6465 6c65 7465 2069 6e76 6f69   as delete invoi
+000039e0: 6365 2c20 656d 6169 6c0a 2020 2020 2020  ce, email.      
+000039f0: 2020 696e 766f 6963 652c 206f 7220 6f70    invoice, or op
+00003a00: 656e 2074 6865 2069 6e76 6f69 6365 2069  en the invoice i
+00003a10: 6e20 6120 6272 6f77 7365 722e 0a0a 2020  n a browser...  
+00003a20: 2020 2020 2020 6047 6f6f 676c 6520 576f        `Google Wo
+00003a30: 726b 7370 6163 650a 2020 2020 2020 2020  rkspace.        
+00003a40: 4164 642d 6f6e 7320 3c68 7474 7073 3a2f  Add-ons <https:/
+00003a50: 2f64 6576 656c 6f70 6572 732e 676f 6f67  /developers.goog
+00003a60: 6c65 2e63 6f6d 2f77 6f72 6b73 7061 6365  le.com/workspace
+00003a70: 2f61 6464 2d6f 6e73 3e60 5f5f 3a0a 0a20  /add-ons>`__:.. 
+00003a80: 2020 2020 2020 2041 7474 7269 6275 7465         Attribute
+00003a90: 733a 0a20 2020 2020 2020 2020 2020 2061  s:.            a
+00003aa0: 6374 696f 6e5f 6c61 6265 6c20 2873 7472  ction_label (str
+00003ab0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00003ac0: 2020 2054 6865 206c 6162 656c 2074 6861     The label tha
+00003ad0: 7420 6469 7370 6c61 7973 2061 7320 7468  t displays as th
+00003ae0: 6520 6163 7469 6f6e 206d 656e 750a 2020  e action menu.  
+00003af0: 2020 2020 2020 2020 2020 2020 2020 6974                it
+00003b00: 656d 2e0a 2020 2020 2020 2020 2020 2020  em..            
+00003b10: 6f6e 5f63 6c69 636b 2028 676f 6f67 6c65  on_click (google
+00003b20: 2e61 7070 732e 6361 7264 5f76 312e 7479  .apps.card_v1.ty
+00003b30: 7065 732e 4f6e 436c 6963 6b29 3a0a 2020  pes.OnClick):.  
+00003b40: 2020 2020 2020 2020 2020 2020 2020 5468                Th
+00003b50: 6520 6060 6f6e 436c 6963 6b60 6020 6163  e ``onClick`` ac
+00003b60: 7469 6f6e 2066 6f72 2074 6869 7320 6163  tion for this ac
+00003b70: 7469 6f6e 2069 7465 6d2e 0a20 2020 2020  tion item..     
+00003b80: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+00003b90: 6163 7469 6f6e 5f6c 6162 656c 3a20 7374  action_label: st
+00003ba0: 7220 3d20 7072 6f74 6f2e 4669 656c 6428  r = proto.Field(
+00003bb0: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
+00003bc0: 746f 2e53 5452 494e 472c 0a20 2020 2020  to.STRING,.     
+00003bd0: 2020 2020 2020 206e 756d 6265 723d 312c         number=1,
+00003be0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+00003bf0: 2020 206f 6e5f 636c 6963 6b3a 2022 4f6e     on_click: "On
+00003c00: 436c 6963 6b22 203d 2070 726f 746f 2e46  Click" = proto.F
+00003c10: 6965 6c64 280a 2020 2020 2020 2020 2020  ield(.          
+00003c20: 2020 7072 6f74 6f2e 4d45 5353 4147 452c    proto.MESSAGE,
+00003c30: 0a20 2020 2020 2020 2020 2020 206e 756d  .            num
+00003c40: 6265 723d 322c 0a20 2020 2020 2020 2020  ber=2,.         
+00003c50: 2020 206d 6573 7361 6765 3d22 4f6e 436c     message="OnCl
+00003c60: 6963 6b22 2c0a 2020 2020 2020 2020 290a  ick",.        ).
+00003c70: 0a20 2020 2063 6c61 7373 2043 6172 6446  .    class CardF
+00003c80: 6978 6564 466f 6f74 6572 2870 726f 746f  ixedFooter(proto
+00003c90: 2e4d 6573 7361 6765 293a 0a20 2020 2020  .Message):.     
+00003ca0: 2020 2072 2222 2241 2070 6572 7369 7374     r"""A persist
+00003cb0: 656e 7420 2873 7469 636b 7929 2066 6f6f  ent (sticky) foo
+00003cc0: 7465 7220 7468 6174 2074 6861 7420 6170  ter that that ap
+00003cd0: 7065 6172 7320 6174 2074 6865 2062 6f74  pears at the bot
+00003ce0: 746f 6d20 6f66 2074 6865 0a20 2020 2020  tom of the.     
+00003cf0: 2020 2063 6172 642e 0a0a 2020 2020 2020     card...      
+00003d00: 2020 5365 7474 696e 6720 6060 6669 7865    Setting ``fixe
+00003d10: 6446 6f6f 7465 7260 6020 7769 7468 6f75  dFooter`` withou
+00003d20: 7420 7370 6563 6966 7969 6e67 2061 2060  t specifying a `
+00003d30: 6070 7269 6d61 7279 4275 7474 6f6e 6060  `primaryButton``
+00003d40: 206f 7220 610a 2020 2020 2020 2020 6060   or a.        ``
+00003d50: 7365 636f 6e64 6172 7942 7574 746f 6e60  secondaryButton`
+00003d60: 6020 6361 7573 6573 2061 6e20 6572 726f  ` causes an erro
+00003d70: 722e 0a0a 2020 2020 2020 2020 466f 7220  r...        For 
+00003d80: 4368 6174 2061 7070 732c 2079 6f75 2063  Chat apps, you c
+00003d90: 616e 2075 7365 2066 6978 6564 2066 6f6f  an use fixed foo
+00003da0: 7465 7273 2069 6e0a 2020 2020 2020 2020  ters in.        
+00003db0: 6064 6961 6c6f 6773 203c 6874 7470 733a  `dialogs <https:
+00003dc0: 2f2f 6465 7665 6c6f 7065 7273 2e67 6f6f  //developers.goo
+00003dd0: 676c 652e 636f 6d2f 776f 726b 7370 6163  gle.com/workspac
+00003de0: 652f 6368 6174 2f64 6961 6c6f 6773 3e60  e/chat/dialogs>`
+00003df0: 5f5f 2c0a 2020 2020 2020 2020 6275 7420  __,.        but 
+00003e00: 6e6f 7420 6063 6172 640a 2020 2020 2020  not `card.      
+00003e10: 2020 6d65 7373 6167 6573 203c 6874 7470    messages <http
+00003e20: 733a 2f2f 6465 7665 6c6f 7065 7273 2e67  s://developers.g
+00003e30: 6f6f 676c 652e 636f 6d2f 776f 726b 7370  oogle.com/worksp
+00003e40: 6163 652f 6368 6174 2f63 7265 6174 652d  ace/chat/create-
+00003e50: 6d65 7373 6167 6573 2363 7265 6174 653e  messages#create>
+00003e60: 605f 5f2e 0a20 2020 2020 2020 2046 6f72  `__..        For
+00003e70: 2061 6e20 6578 616d 706c 6520 696e 2047   an example in G
+00003e80: 6f6f 676c 6520 4368 6174 2061 7070 732c  oogle Chat apps,
+00003e90: 2073 6565 2060 4164 6420 6120 7065 7273   see `Add a pers
+00003ea0: 6973 7465 6e74 0a20 2020 2020 2020 2066  istent.        f
+00003eb0: 6f6f 7465 7220 3c68 7474 7073 3a2f 2f64  ooter <https://d
+00003ec0: 6576 656c 6f70 6572 732e 676f 6f67 6c65  evelopers.google
+00003ed0: 2e63 6f6d 2f77 6f72 6b73 7061 6365 2f63  .com/workspace/c
+00003ee0: 6861 742f 6465 7369 676e 2d63 6f6d 706f  hat/design-compo
+00003ef0: 6e65 6e74 732d 6361 7264 2d64 6961 6c6f  nents-card-dialo
+00003f00: 6723 6164 645f 615f 7065 7273 6973 7465  g#add_a_persiste
+00003f10: 6e74 5f66 6f6f 7465 723e 605f 5f2e 0a0a  nt_footer>`__...
+00003f20: 2020 2020 2020 2020 6047 6f6f 676c 6520          `Google 
+00003f30: 576f 726b 7370 6163 6520 4164 642d 6f6e  Workspace Add-on
+00003f40: 7320 616e 6420 4368 6174 0a20 2020 2020  s and Chat.     
+00003f50: 2020 2061 7070 7320 3c68 7474 7073 3a2f     apps <https:/
+00003f60: 2f64 6576 656c 6f70 6572 732e 676f 6f67  /developers.goog
+00003f70: 6c65 2e63 6f6d 2f77 6f72 6b73 7061 6365  le.com/workspace
+00003f80: 2f65 7874 656e 643e 605f 5f3a 0a0a 2020  /extend>`__:..  
+00003f90: 2020 2020 2020 4174 7472 6962 7574 6573        Attributes
+00003fa0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+00003fb0: 696d 6172 795f 6275 7474 6f6e 2028 676f  imary_button (go
+00003fc0: 6f67 6c65 2e61 7070 732e 6361 7264 5f76  ogle.apps.card_v
+00003fd0: 312e 7479 7065 732e 4275 7474 6f6e 293a  1.types.Button):
+00003fe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003ff0: 2054 6865 2070 7269 6d61 7279 2062 7574   The primary but
+00004000: 746f 6e20 6f66 2074 6865 2066 6978 6564  ton of the fixed
+00004010: 2066 6f6f 7465 722e 2054 6865 0a20 2020   footer. The.   
+00004020: 2020 2020 2020 2020 2020 2020 2062 7574               but
+00004030: 746f 6e20 6d75 7374 2062 6520 6120 7465  ton must be a te
+00004040: 7874 2062 7574 746f 6e20 7769 7468 2074  xt button with t
+00004050: 6578 7420 616e 6420 636f 6c6f 720a 2020  ext and color.  
+00004060: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00004070: 742e 0a20 2020 2020 2020 2020 2020 2073  t..            s
+00004080: 6563 6f6e 6461 7279 5f62 7574 746f 6e20  econdary_button 
+00004090: 2867 6f6f 676c 652e 6170 7073 2e63 6172  (google.apps.car
+000040a0: 645f 7631 2e74 7970 6573 2e42 7574 746f  d_v1.types.Butto
+000040b0: 6e29 3a0a 2020 2020 2020 2020 2020 2020  n):.            
+000040c0: 2020 2020 5468 6520 7365 636f 6e64 6172      The secondar
+000040d0: 7920 6275 7474 6f6e 206f 6620 7468 6520  y button of the 
+000040e0: 6669 7865 6420 666f 6f74 6572 2e20 5468  fixed footer. Th
+000040f0: 6520 6275 7474 6f6e 206d 7573 7420 6265  e button must be
+00004100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004110: 2061 2074 6578 7420 6275 7474 6f6e 2077   a text button w
+00004120: 6974 6820 7465 7874 2061 6e64 2063 6f6c  ith text and col
+00004130: 6f72 2073 6574 2e20 4966 0a20 2020 2020  or set. If.     
+00004140: 2020 2020 2020 2020 2020 2060 6073 6563             ``sec
+00004150: 6f6e 6461 7279 4275 7474 6f6e 6060 2069  ondaryButton`` i
+00004160: 7320 7365 742c 2079 6f75 206d 7573 7420  s set, you must 
+00004170: 616c 736f 2073 6574 0a20 2020 2020 2020  also set.       
+00004180: 2020 2020 2020 2020 2060 6070 7269 6d61           ``prima
+00004190: 7279 4275 7474 6f6e 6060 2e0a 2020 2020  ryButton``..    
+000041a0: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+000041b0: 2070 7269 6d61 7279 5f62 7574 746f 6e3a   primary_button:
+000041c0: 2022 4275 7474 6f6e 2220 3d20 7072 6f74   "Button" = prot
+000041d0: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+000041e0: 2020 2020 2070 726f 746f 2e4d 4553 5341       proto.MESSA
+000041f0: 4745 2c0a 2020 2020 2020 2020 2020 2020  GE,.            
 00004200: 6e75 6d62 6572 3d31 2c0a 2020 2020 2020  number=1,.      
-00004210: 2020 6d65 7373 6167 653d 4361 7264 4865    message=CardHe
-00004220: 6164 6572 2c0a 2020 2020 290a 2020 2020  ader,.    ).    
-00004230: 7365 6374 696f 6e73 3a20 4d75 7461 626c  sections: Mutabl
-00004240: 6553 6571 7565 6e63 655b 5365 6374 696f  eSequence[Sectio
-00004250: 6e5d 203d 2070 726f 746f 2e52 6570 6561  n] = proto.Repea
-00004260: 7465 6446 6965 6c64 280a 2020 2020 2020  tedField(.      
-00004270: 2020 7072 6f74 6f2e 4d45 5353 4147 452c    proto.MESSAGE,
-00004280: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
-00004290: 322c 0a20 2020 2020 2020 206d 6573 7361  2,.        messa
-000042a0: 6765 3d53 6563 7469 6f6e 2c0a 2020 2020  ge=Section,.    
-000042b0: 290a 2020 2020 7365 6374 696f 6e5f 6469  ).    section_di
-000042c0: 7669 6465 725f 7374 796c 653a 2044 6976  vider_style: Div
-000042d0: 6964 6572 5374 796c 6520 3d20 7072 6f74  iderStyle = prot
-000042e0: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-000042f0: 2070 726f 746f 2e45 4e55 4d2c 0a20 2020   proto.ENUM,.   
-00004300: 2020 2020 206e 756d 6265 723d 392c 0a20       number=9,. 
-00004310: 2020 2020 2020 2065 6e75 6d3d 4469 7669         enum=Divi
-00004320: 6465 7253 7479 6c65 2c0a 2020 2020 290a  derStyle,.    ).
-00004330: 2020 2020 6361 7264 5f61 6374 696f 6e73      card_actions
-00004340: 3a20 4d75 7461 626c 6553 6571 7565 6e63  : MutableSequenc
-00004350: 655b 4361 7264 4163 7469 6f6e 5d20 3d20  e[CardAction] = 
-00004360: 7072 6f74 6f2e 5265 7065 6174 6564 4669  proto.RepeatedFi
-00004370: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
-00004380: 746f 2e4d 4553 5341 4745 2c0a 2020 2020  to.MESSAGE,.    
-00004390: 2020 2020 6e75 6d62 6572 3d33 2c0a 2020      number=3,.  
-000043a0: 2020 2020 2020 6d65 7373 6167 653d 4361        message=Ca
-000043b0: 7264 4163 7469 6f6e 2c0a 2020 2020 290a  rdAction,.    ).
-000043c0: 2020 2020 6e61 6d65 3a20 7374 7220 3d20      name: str = 
-000043d0: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
-000043e0: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
-000043f0: 472c 0a20 2020 2020 2020 206e 756d 6265  G,.        numbe
-00004400: 723d 342c 0a20 2020 2029 0a20 2020 2066  r=4,.    ).    f
-00004410: 6978 6564 5f66 6f6f 7465 723a 2043 6172  ixed_footer: Car
-00004420: 6446 6978 6564 466f 6f74 6572 203d 2070  dFixedFooter = p
-00004430: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
-00004440: 2020 2020 7072 6f74 6f2e 4d45 5353 4147      proto.MESSAG
-00004450: 452c 0a20 2020 2020 2020 206e 756d 6265  E,.        numbe
-00004460: 723d 352c 0a20 2020 2020 2020 206d 6573  r=5,.        mes
-00004470: 7361 6765 3d43 6172 6446 6978 6564 466f  sage=CardFixedFo
-00004480: 6f74 6572 2c0a 2020 2020 290a 2020 2020  oter,.    ).    
-00004490: 6469 7370 6c61 795f 7374 796c 653a 2044  display_style: D
-000044a0: 6973 706c 6179 5374 796c 6520 3d20 7072  isplayStyle = pr
-000044b0: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
-000044c0: 2020 2070 726f 746f 2e45 4e55 4d2c 0a20     proto.ENUM,. 
-000044d0: 2020 2020 2020 206e 756d 6265 723d 362c         number=6,
-000044e0: 0a20 2020 2020 2020 2065 6e75 6d3d 4469  .        enum=Di
-000044f0: 7370 6c61 7953 7479 6c65 2c0a 2020 2020  splayStyle,.    
-00004500: 290a 2020 2020 7065 656b 5f63 6172 645f  ).    peek_card_
-00004510: 6865 6164 6572 3a20 4361 7264 4865 6164  header: CardHead
-00004520: 6572 203d 2070 726f 746f 2e46 6965 6c64  er = proto.Field
-00004530: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
-00004540: 4d45 5353 4147 452c 0a20 2020 2020 2020  MESSAGE,.       
-00004550: 206e 756d 6265 723d 372c 0a20 2020 2020   number=7,.     
-00004560: 2020 206d 6573 7361 6765 3d43 6172 6448     message=CardH
-00004570: 6561 6465 722c 0a20 2020 2029 0a0a 0a63  eader,.    )...c
-00004580: 6c61 7373 2057 6964 6765 7428 7072 6f74  lass Widget(prot
-00004590: 6f2e 4d65 7373 6167 6529 3a0a 2020 2020  o.Message):.    
-000045a0: 7222 2222 4561 6368 2063 6172 6420 6973  r"""Each card is
-000045b0: 206d 6164 6520 7570 206f 6620 7769 6467   made up of widg
-000045c0: 6574 732e 0a0a 2020 2020 4120 7769 6467  ets...    A widg
-000045d0: 6574 2069 7320 6120 636f 6d70 6f73 6974  et is a composit
-000045e0: 6520 6f62 6a65 6374 2074 6861 7420 6361  e object that ca
-000045f0: 6e20 7265 7072 6573 656e 7420 6f6e 6520  n represent one 
-00004600: 6f66 2074 6578 742c 0a20 2020 2069 6d61  of text,.    ima
-00004610: 6765 732c 2062 7574 746f 6e73 2c20 616e  ges, buttons, an
-00004620: 6420 6f74 6865 7220 6f62 6a65 6374 2074  d other object t
-00004630: 7970 6573 2e0a 0a20 2020 2054 6869 7320  ypes...    This 
-00004640: 6d65 7373 6167 6520 6861 7320 606f 6e65  message has `one
-00004650: 6f66 605f 2066 6965 6c64 7320 286d 7574  of`_ fields (mut
-00004660: 7561 6c6c 7920 6578 636c 7573 6976 6520  ually exclusive 
-00004670: 6669 656c 6473 292e 0a20 2020 2046 6f72  fields)..    For
-00004680: 2065 6163 6820 6f6e 656f 662c 2061 7420   each oneof, at 
-00004690: 6d6f 7374 206f 6e65 206d 656d 6265 7220  most one member 
-000046a0: 6669 656c 6420 6361 6e20 6265 2073 6574  field can be set
-000046b0: 2061 7420 7468 6520 7361 6d65 2074 696d   at the same tim
-000046c0: 652e 0a20 2020 2053 6574 7469 6e67 2061  e..    Setting a
-000046d0: 6e79 206d 656d 6265 7220 6f66 2074 6865  ny member of the
-000046e0: 206f 6e65 6f66 2061 7574 6f6d 6174 6963   oneof automatic
-000046f0: 616c 6c79 2063 6c65 6172 7320 616c 6c20  ally clears all 
-00004700: 6f74 6865 720a 2020 2020 6d65 6d62 6572  other.    member
-00004710: 732e 0a0a 2020 2020 2e2e 205f 6f6e 656f  s...    .. _oneo
-00004720: 663a 2068 7474 7073 3a2f 2f70 726f 746f  f: https://proto
-00004730: 2d70 6c75 732d 7079 7468 6f6e 2e72 6561  -plus-python.rea
-00004740: 6474 6865 646f 6373 2e69 6f2f 656e 2f73  dthedocs.io/en/s
-00004750: 7461 626c 652f 6669 656c 6473 2e68 746d  table/fields.htm
-00004760: 6c23 6f6e 656f 6673 2d6d 7574 7561 6c6c  l#oneofs-mutuall
-00004770: 792d 6578 636c 7573 6976 652d 6669 656c  y-exclusive-fiel
-00004780: 6473 0a0a 2020 2020 4174 7472 6962 7574  ds..    Attribut
-00004790: 6573 3a0a 2020 2020 2020 2020 7465 7874  es:.        text
-000047a0: 5f70 6172 6167 7261 7068 2028 676f 6f67  _paragraph (goog
-000047b0: 6c65 2e61 7070 732e 6361 7264 5f76 312e  le.apps.card_v1.
-000047c0: 7479 7065 732e 5465 7874 5061 7261 6772  types.TextParagr
-000047d0: 6170 6829 3a0a 2020 2020 2020 2020 2020  aph):.          
-000047e0: 2020 4469 7370 6c61 7973 2061 2074 6578    Displays a tex
-000047f0: 7420 7061 7261 6772 6170 682e 2053 7570  t paragraph. Sup
-00004800: 706f 7274 7320 7369 6d70 6c65 2048 544d  ports simple HTM
-00004810: 4c20 666f 726d 6174 7465 640a 2020 2020  L formatted.    
-00004820: 2020 2020 2020 2020 7465 7874 2e20 466f          text. Fo
-00004830: 7220 6d6f 7265 2069 6e66 6f72 6d61 7469  r more informati
-00004840: 6f6e 2061 626f 7574 2066 6f72 6d61 7474  on about formatt
-00004850: 696e 6720 7465 7874 2c20 7365 650a 2020  ing text, see.  
-00004860: 2020 2020 2020 2020 2020 6046 6f72 6d61            `Forma
-00004870: 7474 696e 6720 7465 7874 2069 6e20 476f  tting text in Go
-00004880: 6f67 6c65 2043 6861 740a 2020 2020 2020  ogle Chat.      
-00004890: 2020 2020 2020 6170 7073 203c 6874 7470        apps <http
-000048a0: 733a 2f2f 6465 7665 6c6f 7065 7273 2e67  s://developers.g
-000048b0: 6f6f 676c 652e 636f 6d2f 6368 6174 2f66  oogle.com/chat/f
-000048c0: 6f72 6d61 742d 6d65 7373 6167 6573 2363  ormat-messages#c
-000048d0: 6172 642d 666f 726d 6174 7469 6e67 3e60  ard-formatting>`
-000048e0: 5f5f 0a20 2020 2020 2020 2020 2020 2061  __.            a
-000048f0: 6e64 2060 466f 726d 6174 7469 6e67 2074  nd `Formatting t
-00004900: 6578 7420 696e 2047 6f6f 676c 6520 576f  ext in Google Wo
-00004910: 726b 7370 6163 650a 2020 2020 2020 2020  rkspace.        
-00004920: 2020 2020 4164 642d 6f6e 7320 3c68 7474      Add-ons <htt
-00004930: 7073 3a2f 2f64 6576 656c 6f70 6572 732e  ps://developers.
-00004940: 676f 6f67 6c65 2e63 6f6d 2f61 7070 732d  google.com/apps-
-00004950: 7363 7269 7074 2f61 6464 2d6f 6e73 2f63  script/add-ons/c
-00004960: 6f6e 6365 7074 732f 7769 6467 6574 7323  oncepts/widgets#
-00004970: 7465 7874 5f66 6f72 6d61 7474 696e 673e  text_formatting>
-00004980: 605f 5f2e 0a0a 2020 2020 2020 2020 2020  `__...          
-00004990: 2020 466f 7220 6578 616d 706c 652c 2074    For example, t
-000049a0: 6865 2066 6f6c 6c6f 7769 6e67 204a 534f  he following JSO
-000049b0: 4e20 6372 6561 7465 7320 6120 626f 6c64  N creates a bold
-000049c0: 6564 2074 6578 743a 0a0a 2020 2020 2020  ed text:..      
-000049d0: 2020 2020 2020 3a3a 0a0a 2020 2020 2020        ::..      
-000049e0: 2020 2020 2020 2020 2022 7465 7874 5061           "textPa
-000049f0: 7261 6772 6170 6822 3a20 7b0a 2020 2020  ragraph": {.    
-00004a00: 2020 2020 2020 2020 2020 2020 2022 7465               "te
-00004a10: 7874 223a 2022 2020 3c62 3e62 6f6c 6420  xt": "  <b>bold 
-00004a20: 7465 7874 3c2f 623e 220a 2020 2020 2020  text</b>".      
-00004a30: 2020 2020 2020 2020 207d 0a0a 2020 2020           }..    
-00004a40: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
-00004a50: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
-00004a60: 6620 606f 6e65 6f66 605f 2060 6064 6174  f `oneof`_ ``dat
-00004a70: 6160 602e 0a20 2020 2020 2020 2069 6d61  a``..        ima
-00004a80: 6765 2028 676f 6f67 6c65 2e61 7070 732e  ge (google.apps.
-00004a90: 6361 7264 5f76 312e 7479 7065 732e 496d  card_v1.types.Im
-00004aa0: 6167 6529 3a0a 2020 2020 2020 2020 2020  age):.          
-00004ab0: 2020 4469 7370 6c61 7973 2061 6e20 696d    Displays an im
-00004ac0: 6167 652e 0a0a 2020 2020 2020 2020 2020  age...          
-00004ad0: 2020 466f 7220 6578 616d 706c 652c 2074    For example, t
-00004ae0: 6865 2066 6f6c 6c6f 7769 6e67 204a 534f  he following JSO
-00004af0: 4e20 6372 6561 7465 7320 616e 2069 6d61  N creates an ima
-00004b00: 6765 2077 6974 680a 2020 2020 2020 2020  ge with.        
-00004b10: 2020 2020 616c 7465 726e 6174 6976 6520      alternative 
-00004b20: 7465 7874 3a0a 0a20 2020 2020 2020 2020  text:..         
-00004b30: 2020 203a 3a0a 0a20 2020 2020 2020 2020     ::..         
-00004b40: 2020 2020 2020 2269 6d61 6765 223a 207b        "image": {
-00004b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004b60: 2020 2269 6d61 6765 5572 6c22 3a0a 2020    "imageUrl":.  
-00004b70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00004b80: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
-00004b90: 7273 2e67 6f6f 676c 652e 636f 6d2f 6368  rs.google.com/ch
-00004ba0: 6174 2f69 6d61 6765 732f 7175 6963 6b73  at/images/quicks
-00004bb0: 7461 7274 2d61 7070 2d61 7661 7461 722e  tart-app-avatar.
-00004bc0: 706e 6722 2c0a 2020 2020 2020 2020 2020  png",.          
-00004bd0: 2020 2020 2020 2022 616c 7454 6578 7422         "altText"
-00004be0: 3a20 2243 6861 7420 6170 7020 6176 6174  : "Chat app avat
-00004bf0: 6172 220a 2020 2020 2020 2020 2020 2020  ar".            
-00004c00: 2020 207d 0a0a 2020 2020 2020 2020 2020     }..          
-00004c10: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
-00004c20: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
-00004c30: 6f66 605f 2060 6064 6174 6160 602e 0a20  of`_ ``data``.. 
-00004c40: 2020 2020 2020 2064 6563 6f72 6174 6564         decorated
-00004c50: 5f74 6578 7420 2867 6f6f 676c 652e 6170  _text (google.ap
-00004c60: 7073 2e63 6172 645f 7631 2e74 7970 6573  ps.card_v1.types
-00004c70: 2e44 6563 6f72 6174 6564 5465 7874 293a  .DecoratedText):
-00004c80: 0a20 2020 2020 2020 2020 2020 2044 6973  .            Dis
-00004c90: 706c 6179 7320 6120 6465 636f 7261 7465  plays a decorate
-00004ca0: 6420 7465 7874 2069 7465 6d2e 0a0a 2020  d text item...  
-00004cb0: 2020 2020 2020 2020 2020 466f 7220 6578            For ex
-00004cc0: 616d 706c 652c 2074 6865 2066 6f6c 6c6f  ample, the follo
-00004cd0: 7769 6e67 204a 534f 4e20 6372 6561 7465  wing JSON create
-00004ce0: 7320 6120 6465 636f 7261 7465 6420 7465  s a decorated te
-00004cf0: 7874 0a20 2020 2020 2020 2020 2020 2077  xt.            w
-00004d00: 6964 6765 7420 7368 6f77 696e 6720 656d  idget showing em
-00004d10: 6169 6c20 6164 6472 6573 733a 0a0a 2020  ail address:..  
-00004d20: 2020 2020 2020 2020 2020 3a3a 0a0a 2020            ::..  
-00004d30: 2020 2020 2020 2020 2020 2020 2022 6465               "de
-00004d40: 636f 7261 7465 6454 6578 7422 3a20 7b0a  coratedText": {.
-00004d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d60: 2022 6963 6f6e 223a 207b 0a20 2020 2020   "icon": {.     
-00004d70: 2020 2020 2020 2020 2020 2020 2020 226b                "k
-00004d80: 6e6f 776e 4963 6f6e 223a 2022 454d 4149  nownIcon": "EMAI
-00004d90: 4c22 0a20 2020 2020 2020 2020 2020 2020  L".             
-00004da0: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-00004db0: 2020 2020 2020 2020 2274 6f70 4c61 6265          "topLabe
-00004dc0: 6c22 3a20 2245 6d61 696c 2041 6464 7265  l": "Email Addre
-00004dd0: 7373 222c 0a20 2020 2020 2020 2020 2020  ss",.           
-00004de0: 2020 2020 2020 2274 6578 7422 3a20 2273        "text": "s
-00004df0: 6173 6861 4065 7861 6d70 6c65 2e63 6f6d  asha@example.com
-00004e00: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00004e10: 2020 2020 2262 6f74 746f 6d4c 6162 656c      "bottomLabel
-00004e20: 223a 2022 5468 6973 2069 7320 6120 6e65  ": "This is a ne
-00004e30: 7720 456d 6169 6c20 6164 6472 6573 7321  w Email address!
-00004e40: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00004e50: 2020 2020 2273 7769 7463 6843 6f6e 7472      "switchContr
-00004e60: 6f6c 223a 207b 0a20 2020 2020 2020 2020  ol": {.         
-00004e70: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
-00004e80: 3a20 2268 6173 5f73 656e 645f 7765 6c63  : "has_send_welc
-00004e90: 6f6d 655f 656d 6169 6c5f 746f 5f73 6173  ome_email_to_sas
-00004ea0: 6861 222c 0a20 2020 2020 2020 2020 2020  ha",.           
-00004eb0: 2020 2020 2020 2020 2273 656c 6563 7465          "selecte
-00004ec0: 6422 3a20 6661 6c73 652c 0a20 2020 2020  d": false,.     
-00004ed0: 2020 2020 2020 2020 2020 2020 2020 2263                "c
-00004ee0: 6f6e 7472 6f6c 5479 7065 223a 2022 4348  ontrolType": "CH
-00004ef0: 4543 4b42 4f58 220a 2020 2020 2020 2020  ECKBOX".        
-00004f00: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00004f10: 2020 2020 2020 2020 2020 7d0a 0a20 2020            }..   
-00004f20: 2020 2020 2020 2020 2054 6869 7320 6669           This fi
-00004f30: 656c 6420 6973 2061 206d 656d 6265 7220  eld is a member 
-00004f40: 6f66 2060 6f6e 656f 6660 5f20 6060 6461  of `oneof`_ ``da
-00004f50: 7461 6060 2e0a 2020 2020 2020 2020 6275  ta``..        bu
-00004f60: 7474 6f6e 5f6c 6973 7420 2867 6f6f 676c  tton_list (googl
-00004f70: 652e 6170 7073 2e63 6172 645f 7631 2e74  e.apps.card_v1.t
-00004f80: 7970 6573 2e42 7574 746f 6e4c 6973 7429  ypes.ButtonList)
-00004f90: 3a0a 2020 2020 2020 2020 2020 2020 4120  :.            A 
-00004fa0: 6c69 7374 206f 6620 6275 7474 6f6e 732e  list of buttons.
-00004fb0: 0a0a 2020 2020 2020 2020 2020 2020 466f  ..            Fo
-00004fc0: 7220 6578 616d 706c 652c 2074 6865 2066  r example, the f
-00004fd0: 6f6c 6c6f 7769 6e67 204a 534f 4e20 6372  ollowing JSON cr
-00004fe0: 6561 7465 7320 7477 6f20 6275 7474 6f6e  eates two button
-00004ff0: 732e 2054 6865 0a20 2020 2020 2020 2020  s. The.         
-00005000: 2020 2066 6972 7374 2069 7320 6120 626c     first is a bl
-00005010: 7565 2074 6578 7420 6275 7474 6f6e 2061  ue text button a
-00005020: 6e64 2074 6865 2073 6563 6f6e 6420 6973  nd the second is
-00005030: 2061 6e20 696d 6167 650a 2020 2020 2020   an image.      
-00005040: 2020 2020 2020 6275 7474 6f6e 2074 6861        button tha
-00005050: 7420 6f70 656e 7320 6120 6c69 6e6b 3a0a  t opens a link:.
-00005060: 0a20 2020 2020 2020 2020 2020 203a 3a0a  .            ::.
-00005070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005080: 2262 7574 746f 6e4c 6973 7422 3a20 7b0a  "buttonList": {.
-00005090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000050a0: 2022 6275 7474 6f6e 7322 3a20 5b0a 2020   "buttons": [.  
-000050b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000050c0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-000050d0: 2020 2020 2020 2020 2274 6578 7422 3a20          "text": 
-000050e0: 2245 6469 7422 2c0a 2020 2020 2020 2020  "Edit",.        
-000050f0: 2020 2020 2020 2020 2020 2020 2022 636f               "co
-00005100: 6c6f 7222 3a20 7b0a 2020 2020 2020 2020  lor": {.        
-00005110: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00005120: 7265 6422 3a20 302c 0a20 2020 2020 2020  red": 0,.       
-00005130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005140: 2267 7265 656e 223a 2030 2c0a 2020 2020  "green": 0,.    
-00005150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005160: 2020 2022 626c 7565 223a 2031 2c0a 2020     "blue": 1,.  
-00005170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005180: 2020 2020 2022 616c 7068 6122 3a20 310a       "alpha": 1.
-00005190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051a0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-000051b0: 2020 2020 2020 2020 2020 2020 2022 6469               "di
-000051c0: 7361 626c 6564 223a 2074 7275 652c 0a20  sabled": true,. 
-000051d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051e0: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-000051f0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-00005200: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00005210: 6963 6f6e 223a 207b 0a20 2020 2020 2020  icon": {.       
+00004210: 2020 2020 2020 6d65 7373 6167 653d 2242        message="B
+00004220: 7574 746f 6e22 2c0a 2020 2020 2020 2020  utton",.        
+00004230: 290a 2020 2020 2020 2020 7365 636f 6e64  ).        second
+00004240: 6172 795f 6275 7474 6f6e 3a20 2242 7574  ary_button: "But
+00004250: 746f 6e22 203d 2070 726f 746f 2e46 6965  ton" = proto.Fie
+00004260: 6c64 280a 2020 2020 2020 2020 2020 2020  ld(.            
+00004270: 7072 6f74 6f2e 4d45 5353 4147 452c 0a20  proto.MESSAGE,. 
+00004280: 2020 2020 2020 2020 2020 206e 756d 6265             numbe
+00004290: 723d 322c 0a20 2020 2020 2020 2020 2020  r=2,.           
+000042a0: 206d 6573 7361 6765 3d22 4275 7474 6f6e   message="Button
+000042b0: 222c 0a20 2020 2020 2020 2029 0a0a 2020  ",.        )..  
+000042c0: 2020 6865 6164 6572 3a20 4361 7264 4865    header: CardHe
+000042d0: 6164 6572 203d 2070 726f 746f 2e46 6965  ader = proto.Fie
+000042e0: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
+000042f0: 6f2e 4d45 5353 4147 452c 0a20 2020 2020  o.MESSAGE,.     
+00004300: 2020 206e 756d 6265 723d 312c 0a20 2020     number=1,.   
+00004310: 2020 2020 206d 6573 7361 6765 3d43 6172       message=Car
+00004320: 6448 6561 6465 722c 0a20 2020 2029 0a20  dHeader,.    ). 
+00004330: 2020 2073 6563 7469 6f6e 733a 204d 7574     sections: Mut
+00004340: 6162 6c65 5365 7175 656e 6365 5b53 6563  ableSequence[Sec
+00004350: 7469 6f6e 5d20 3d20 7072 6f74 6f2e 5265  tion] = proto.Re
+00004360: 7065 6174 6564 4669 656c 6428 0a20 2020  peatedField(.   
+00004370: 2020 2020 2070 726f 746f 2e4d 4553 5341       proto.MESSA
+00004380: 4745 2c0a 2020 2020 2020 2020 6e75 6d62  GE,.        numb
+00004390: 6572 3d32 2c0a 2020 2020 2020 2020 6d65  er=2,.        me
+000043a0: 7373 6167 653d 5365 6374 696f 6e2c 0a20  ssage=Section,. 
+000043b0: 2020 2029 0a20 2020 2073 6563 7469 6f6e     ).    section
+000043c0: 5f64 6976 6964 6572 5f73 7479 6c65 3a20  _divider_style: 
+000043d0: 4469 7669 6465 7253 7479 6c65 203d 2070  DividerStyle = p
+000043e0: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
+000043f0: 2020 2020 7072 6f74 6f2e 454e 554d 2c0a      proto.ENUM,.
+00004400: 2020 2020 2020 2020 6e75 6d62 6572 3d39          number=9
+00004410: 2c0a 2020 2020 2020 2020 656e 756d 3d44  ,.        enum=D
+00004420: 6976 6964 6572 5374 796c 652c 0a20 2020  ividerStyle,.   
+00004430: 2029 0a20 2020 2063 6172 645f 6163 7469   ).    card_acti
+00004440: 6f6e 733a 204d 7574 6162 6c65 5365 7175  ons: MutableSequ
+00004450: 656e 6365 5b43 6172 6441 6374 696f 6e5d  ence[CardAction]
+00004460: 203d 2070 726f 746f 2e52 6570 6561 7465   = proto.Repeate
+00004470: 6446 6965 6c64 280a 2020 2020 2020 2020  dField(.        
+00004480: 7072 6f74 6f2e 4d45 5353 4147 452c 0a20  proto.MESSAGE,. 
+00004490: 2020 2020 2020 206e 756d 6265 723d 332c         number=3,
+000044a0: 0a20 2020 2020 2020 206d 6573 7361 6765  .        message
+000044b0: 3d43 6172 6441 6374 696f 6e2c 0a20 2020  =CardAction,.   
+000044c0: 2029 0a20 2020 206e 616d 653a 2073 7472   ).    name: str
+000044d0: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
+000044e0: 2020 2020 2020 2020 7072 6f74 6f2e 5354          proto.ST
+000044f0: 5249 4e47 2c0a 2020 2020 2020 2020 6e75  RING,.        nu
+00004500: 6d62 6572 3d34 2c0a 2020 2020 290a 2020  mber=4,.    ).  
+00004510: 2020 6669 7865 645f 666f 6f74 6572 3a20    fixed_footer: 
+00004520: 4361 7264 4669 7865 6446 6f6f 7465 7220  CardFixedFooter 
+00004530: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
+00004540: 2020 2020 2020 2070 726f 746f 2e4d 4553         proto.MES
+00004550: 5341 4745 2c0a 2020 2020 2020 2020 6e75  SAGE,.        nu
+00004560: 6d62 6572 3d35 2c0a 2020 2020 2020 2020  mber=5,.        
+00004570: 6d65 7373 6167 653d 4361 7264 4669 7865  message=CardFixe
+00004580: 6446 6f6f 7465 722c 0a20 2020 2029 0a20  dFooter,.    ). 
+00004590: 2020 2064 6973 706c 6179 5f73 7479 6c65     display_style
+000045a0: 3a20 4469 7370 6c61 7953 7479 6c65 203d  : DisplayStyle =
+000045b0: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
+000045c0: 2020 2020 2020 7072 6f74 6f2e 454e 554d        proto.ENUM
+000045d0: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
+000045e0: 3d36 2c0a 2020 2020 2020 2020 656e 756d  =6,.        enum
+000045f0: 3d44 6973 706c 6179 5374 796c 652c 0a20  =DisplayStyle,. 
+00004600: 2020 2029 0a20 2020 2070 6565 6b5f 6361     ).    peek_ca
+00004610: 7264 5f68 6561 6465 723a 2043 6172 6448  rd_header: CardH
+00004620: 6561 6465 7220 3d20 7072 6f74 6f2e 4669  eader = proto.Fi
+00004630: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
+00004640: 746f 2e4d 4553 5341 4745 2c0a 2020 2020  to.MESSAGE,.    
+00004650: 2020 2020 6e75 6d62 6572 3d37 2c0a 2020      number=7,.  
+00004660: 2020 2020 2020 6d65 7373 6167 653d 4361        message=Ca
+00004670: 7264 4865 6164 6572 2c0a 2020 2020 290a  rdHeader,.    ).
+00004680: 0a0a 636c 6173 7320 5769 6467 6574 2870  ..class Widget(p
+00004690: 726f 746f 2e4d 6573 7361 6765 293a 0a20  roto.Message):. 
+000046a0: 2020 2072 2222 2245 6163 6820 6361 7264     r"""Each card
+000046b0: 2069 7320 6d61 6465 2075 7020 6f66 2077   is made up of w
+000046c0: 6964 6765 7473 2e0a 0a20 2020 2041 2077  idgets...    A w
+000046d0: 6964 6765 7420 6973 2061 2063 6f6d 706f  idget is a compo
+000046e0: 7369 7465 206f 626a 6563 7420 7468 6174  site object that
+000046f0: 2063 616e 2072 6570 7265 7365 6e74 206f   can represent o
+00004700: 6e65 206f 6620 7465 7874 2c0a 2020 2020  ne of text,.    
+00004710: 696d 6167 6573 2c20 6275 7474 6f6e 732c  images, buttons,
+00004720: 2061 6e64 206f 7468 6572 206f 626a 6563   and other objec
+00004730: 7420 7479 7065 732e 0a0a 2020 2020 5468  t types...    Th
+00004740: 6973 206d 6573 7361 6765 2068 6173 2060  is message has `
+00004750: 6f6e 656f 6660 5f20 6669 656c 6473 2028  oneof`_ fields (
+00004760: 6d75 7475 616c 6c79 2065 7863 6c75 7369  mutually exclusi
+00004770: 7665 2066 6965 6c64 7329 2e0a 2020 2020  ve fields)..    
+00004780: 466f 7220 6561 6368 206f 6e65 6f66 2c20  For each oneof, 
+00004790: 6174 206d 6f73 7420 6f6e 6520 6d65 6d62  at most one memb
+000047a0: 6572 2066 6965 6c64 2063 616e 2062 6520  er field can be 
+000047b0: 7365 7420 6174 2074 6865 2073 616d 6520  set at the same 
+000047c0: 7469 6d65 2e0a 2020 2020 5365 7474 696e  time..    Settin
+000047d0: 6720 616e 7920 6d65 6d62 6572 206f 6620  g any member of 
+000047e0: 7468 6520 6f6e 656f 6620 6175 746f 6d61  the oneof automa
+000047f0: 7469 6361 6c6c 7920 636c 6561 7273 2061  tically clears a
+00004800: 6c6c 206f 7468 6572 0a20 2020 206d 656d  ll other.    mem
+00004810: 6265 7273 2e0a 0a20 2020 202e 2e20 5f6f  bers...    .. _o
+00004820: 6e65 6f66 3a20 6874 7470 733a 2f2f 7072  neof: https://pr
+00004830: 6f74 6f2d 706c 7573 2d70 7974 686f 6e2e  oto-plus-python.
+00004840: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
+00004850: 6e2f 7374 6162 6c65 2f66 6965 6c64 732e  n/stable/fields.
+00004860: 6874 6d6c 236f 6e65 6f66 732d 6d75 7475  html#oneofs-mutu
+00004870: 616c 6c79 2d65 7863 6c75 7369 7665 2d66  ally-exclusive-f
+00004880: 6965 6c64 730a 0a20 2020 2041 7474 7269  ields..    Attri
+00004890: 6275 7465 733a 0a20 2020 2020 2020 2074  butes:.        t
+000048a0: 6578 745f 7061 7261 6772 6170 6820 2867  ext_paragraph (g
+000048b0: 6f6f 676c 652e 6170 7073 2e63 6172 645f  oogle.apps.card_
+000048c0: 7631 2e74 7970 6573 2e54 6578 7450 6172  v1.types.TextPar
+000048d0: 6167 7261 7068 293a 0a20 2020 2020 2020  agraph):.       
+000048e0: 2020 2020 2044 6973 706c 6179 7320 6120       Displays a 
+000048f0: 7465 7874 2070 6172 6167 7261 7068 2e20  text paragraph. 
+00004900: 5375 7070 6f72 7473 2073 696d 706c 6520  Supports simple 
+00004910: 4854 4d4c 2066 6f72 6d61 7474 6564 0a20  HTML formatted. 
+00004920: 2020 2020 2020 2020 2020 2074 6578 742e             text.
+00004930: 2046 6f72 206d 6f72 6520 696e 666f 726d   For more inform
+00004940: 6174 696f 6e20 6162 6f75 7420 666f 726d  ation about form
+00004950: 6174 7469 6e67 2074 6578 742c 2073 6565  atting text, see
+00004960: 0a20 2020 2020 2020 2020 2020 2060 466f  .            `Fo
+00004970: 726d 6174 7469 6e67 2074 6578 7420 696e  rmatting text in
+00004980: 2047 6f6f 676c 6520 4368 6174 0a20 2020   Google Chat.   
+00004990: 2020 2020 2020 2020 2061 7070 7320 3c68           apps <h
+000049a0: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
+000049b0: 732e 676f 6f67 6c65 2e63 6f6d 2f77 6f72  s.google.com/wor
+000049c0: 6b73 7061 6365 2f63 6861 742f 666f 726d  kspace/chat/form
+000049d0: 6174 2d6d 6573 7361 6765 7323 6361 7264  at-messages#card
+000049e0: 2d66 6f72 6d61 7474 696e 673e 605f 5f0a  -formatting>`__.
+000049f0: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+00004a00: 6046 6f72 6d61 7474 696e 6720 7465 7874  `Formatting text
+00004a10: 2069 6e20 476f 6f67 6c65 2057 6f72 6b73   in Google Works
+00004a20: 7061 6365 0a20 2020 2020 2020 2020 2020  pace.           
+00004a30: 2041 6464 2d6f 6e73 203c 6874 7470 733a   Add-ons <https:
+00004a40: 2f2f 6465 7665 6c6f 7065 7273 2e67 6f6f  //developers.goo
+00004a50: 676c 652e 636f 6d2f 6170 7073 2d73 6372  gle.com/apps-scr
+00004a60: 6970 742f 6164 642d 6f6e 732f 636f 6e63  ipt/add-ons/conc
+00004a70: 6570 7473 2f77 6964 6765 7473 2374 6578  epts/widgets#tex
+00004a80: 745f 666f 726d 6174 7469 6e67 3e60 5f5f  t_formatting>`__
+00004a90: 2e0a 0a20 2020 2020 2020 2020 2020 2046  ...            F
+00004aa0: 6f72 2065 7861 6d70 6c65 2c20 7468 6520  or example, the 
+00004ab0: 666f 6c6c 6f77 696e 6720 4a53 4f4e 2063  following JSON c
+00004ac0: 7265 6174 6573 2061 2062 6f6c 6465 6420  reates a bolded 
+00004ad0: 7465 7874 3a0a 0a20 2020 2020 2020 2020  text:..         
+00004ae0: 2020 203a 3a0a 0a20 2020 2020 2020 2020     ::..         
+00004af0: 2020 2020 2020 2274 6578 7450 6172 6167        "textParag
+00004b00: 7261 7068 223a 207b 0a20 2020 2020 2020  raph": {.       
+00004b10: 2020 2020 2020 2020 2020 2274 6578 7422            "text"
+00004b20: 3a20 2220 203c 623e 626f 6c64 2074 6578  : "  <b>bold tex
+00004b30: 743c 2f62 3e22 0a20 2020 2020 2020 2020  t</b>".         
+00004b40: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
+00004b50: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
+00004b60: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
+00004b70: 6f6e 656f 6660 5f20 6060 6461 7461 6060  oneof`_ ``data``
+00004b80: 2e0a 2020 2020 2020 2020 696d 6167 6520  ..        image 
+00004b90: 2867 6f6f 676c 652e 6170 7073 2e63 6172  (google.apps.car
+00004ba0: 645f 7631 2e74 7970 6573 2e49 6d61 6765  d_v1.types.Image
+00004bb0: 293a 0a20 2020 2020 2020 2020 2020 2044  ):.            D
+00004bc0: 6973 706c 6179 7320 616e 2069 6d61 6765  isplays an image
+00004bd0: 2e0a 0a20 2020 2020 2020 2020 2020 2046  ...            F
+00004be0: 6f72 2065 7861 6d70 6c65 2c20 7468 6520  or example, the 
+00004bf0: 666f 6c6c 6f77 696e 6720 4a53 4f4e 2063  following JSON c
+00004c00: 7265 6174 6573 2061 6e20 696d 6167 6520  reates an image 
+00004c10: 7769 7468 0a20 2020 2020 2020 2020 2020  with.           
+00004c20: 2061 6c74 6572 6e61 7469 7665 2074 6578   alternative tex
+00004c30: 743a 0a0a 2020 2020 2020 2020 2020 2020  t:..            
+00004c40: 3a3a 0a0a 2020 2020 2020 2020 2020 2020  ::..            
+00004c50: 2020 2022 696d 6167 6522 3a20 7b0a 2020     "image": {.  
+00004c60: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00004c70: 696d 6167 6555 726c 223a 0a20 2020 2020  imageUrl":.     
+00004c80: 2020 2020 2020 2020 2020 2020 2268 7474              "htt
+00004c90: 7073 3a2f 2f64 6576 656c 6f70 6572 732e  ps://developers.
+00004ca0: 676f 6f67 6c65 2e63 6f6d 2f77 6f72 6b73  google.com/works
+00004cb0: 7061 6365 2f63 6861 742f 696d 6167 6573  pace/chat/images
+00004cc0: 2f71 7569 636b 7374 6172 742d 6170 702d  /quickstart-app-
+00004cd0: 6176 6174 6172 2e70 6e67 222c 0a20 2020  avatar.png",.   
+00004ce0: 2020 2020 2020 2020 2020 2020 2020 2261                "a
+00004cf0: 6c74 5465 7874 223a 2022 4368 6174 2061  ltText": "Chat a
+00004d00: 7070 2061 7661 7461 7222 0a20 2020 2020  pp avatar".     
+00004d10: 2020 2020 2020 2020 2020 7d0a 0a20 2020            }..   
+00004d20: 2020 2020 2020 2020 2054 6869 7320 6669           This fi
+00004d30: 656c 6420 6973 2061 206d 656d 6265 7220  eld is a member 
+00004d40: 6f66 2060 6f6e 656f 6660 5f20 6060 6461  of `oneof`_ ``da
+00004d50: 7461 6060 2e0a 2020 2020 2020 2020 6465  ta``..        de
+00004d60: 636f 7261 7465 645f 7465 7874 2028 676f  corated_text (go
+00004d70: 6f67 6c65 2e61 7070 732e 6361 7264 5f76  ogle.apps.card_v
+00004d80: 312e 7479 7065 732e 4465 636f 7261 7465  1.types.Decorate
+00004d90: 6454 6578 7429 3a0a 2020 2020 2020 2020  dText):.        
+00004da0: 2020 2020 4469 7370 6c61 7973 2061 2064      Displays a d
+00004db0: 6563 6f72 6174 6564 2074 6578 7420 6974  ecorated text it
+00004dc0: 656d 2e0a 0a20 2020 2020 2020 2020 2020  em...           
+00004dd0: 2046 6f72 2065 7861 6d70 6c65 2c20 7468   For example, th
+00004de0: 6520 666f 6c6c 6f77 696e 6720 4a53 4f4e  e following JSON
+00004df0: 2063 7265 6174 6573 2061 2064 6563 6f72   creates a decor
+00004e00: 6174 6564 2074 6578 740a 2020 2020 2020  ated text.      
+00004e10: 2020 2020 2020 7769 6467 6574 2073 686f        widget sho
+00004e20: 7769 6e67 2065 6d61 696c 2061 6464 7265  wing email addre
+00004e30: 7373 3a0a 0a20 2020 2020 2020 2020 2020  ss:..           
+00004e40: 203a 3a0a 0a20 2020 2020 2020 2020 2020   ::..           
+00004e50: 2020 2020 2264 6563 6f72 6174 6564 5465      "decoratedTe
+00004e60: 7874 223a 207b 0a20 2020 2020 2020 2020  xt": {.         
+00004e70: 2020 2020 2020 2020 2269 636f 6e22 3a20          "icon": 
+00004e80: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00004e90: 2020 2020 2022 6b6e 6f77 6e49 636f 6e22       "knownIcon"
+00004ea0: 3a20 2245 4d41 494c 220a 2020 2020 2020  : "EMAIL".      
+00004eb0: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
+00004ec0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00004ed0: 746f 704c 6162 656c 223a 2022 456d 6169  topLabel": "Emai
+00004ee0: 6c20 4164 6472 6573 7322 2c0a 2020 2020  l Address",.    
+00004ef0: 2020 2020 2020 2020 2020 2020 2022 7465               "te
+00004f00: 7874 223a 2022 7361 7368 6140 6578 616d  xt": "sasha@exam
+00004f10: 706c 652e 636f 6d22 2c0a 2020 2020 2020  ple.com",.      
+00004f20: 2020 2020 2020 2020 2020 2022 626f 7474             "bott
+00004f30: 6f6d 4c61 6265 6c22 3a20 2254 6869 7320  omLabel": "This 
+00004f40: 6973 2061 206e 6577 2045 6d61 696c 2061  is a new Email a
+00004f50: 6464 7265 7373 2122 2c0a 2020 2020 2020  ddress!",.      
+00004f60: 2020 2020 2020 2020 2020 2022 7377 6974             "swit
+00004f70: 6368 436f 6e74 726f 6c22 3a20 7b0a 2020  chControl": {.  
+00004f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f90: 2022 6e61 6d65 223a 2022 6861 735f 7365   "name": "has_se
+00004fa0: 6e64 5f77 656c 636f 6d65 5f65 6d61 696c  nd_welcome_email
+00004fb0: 5f74 6f5f 7361 7368 6122 2c0a 2020 2020  _to_sasha",.    
+00004fc0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00004fd0: 7365 6c65 6374 6564 223a 2066 616c 7365  selected": false
+00004fe0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00004ff0: 2020 2020 2022 636f 6e74 726f 6c54 7970       "controlTyp
+00005000: 6522 3a20 2243 4845 434b 424f 5822 0a20  e": "CHECKBOX". 
+00005010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005020: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00005030: 207d 0a0a 2020 2020 2020 2020 2020 2020   }..            
+00005040: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
+00005050: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
+00005060: 605f 2060 6064 6174 6160 602e 0a20 2020  `_ ``data``..   
+00005070: 2020 2020 2062 7574 746f 6e5f 6c69 7374       button_list
+00005080: 2028 676f 6f67 6c65 2e61 7070 732e 6361   (google.apps.ca
+00005090: 7264 5f76 312e 7479 7065 732e 4275 7474  rd_v1.types.Butt
+000050a0: 6f6e 4c69 7374 293a 0a20 2020 2020 2020  onList):.       
+000050b0: 2020 2020 2041 206c 6973 7420 6f66 2062       A list of b
+000050c0: 7574 746f 6e73 2e0a 0a20 2020 2020 2020  uttons...       
+000050d0: 2020 2020 2046 6f72 2065 7861 6d70 6c65       For example
+000050e0: 2c20 7468 6520 666f 6c6c 6f77 696e 6720  , the following 
+000050f0: 4a53 4f4e 2063 7265 6174 6573 2074 776f  JSON creates two
+00005100: 2062 7574 746f 6e73 2e20 5468 650a 2020   buttons. The.  
+00005110: 2020 2020 2020 2020 2020 6669 7273 7420            first 
+00005120: 6973 2061 2062 6c75 6520 7465 7874 2062  is a blue text b
+00005130: 7574 746f 6e20 616e 6420 7468 6520 7365  utton and the se
+00005140: 636f 6e64 2069 7320 616e 2069 6d61 6765  cond is an image
+00005150: 0a20 2020 2020 2020 2020 2020 2062 7574  .            but
+00005160: 746f 6e20 7468 6174 206f 7065 6e73 2061  ton that opens a
+00005170: 206c 696e 6b3a 0a0a 2020 2020 2020 2020   link:..        
+00005180: 2020 2020 3a3a 0a0a 2020 2020 2020 2020      ::..        
+00005190: 2020 2020 2020 2022 6275 7474 6f6e 4c69         "buttonLi
+000051a0: 7374 223a 207b 0a20 2020 2020 2020 2020  st": {.         
+000051b0: 2020 2020 2020 2020 2262 7574 746f 6e73          "buttons
+000051c0: 223a 205b 0a20 2020 2020 2020 2020 2020  ": [.           
+000051d0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+000051e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000051f0: 7465 7874 223a 2022 4564 6974 222c 0a20  text": "Edit",. 
+00005200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005210: 2020 2020 2263 6f6c 6f72 223a 207b 0a20      "color": {. 
 00005220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005230: 226b 6e6f 776e 4963 6f6e 223a 2022 494e  "knownIcon": "IN
-00005240: 5649 5445 222c 0a20 2020 2020 2020 2020  VITE",.         
-00005250: 2020 2020 2020 2020 2020 2020 2020 2261                "a
-00005260: 6c74 5465 7874 223a 2022 6368 6563 6b20  ltText": "check 
-00005270: 6361 6c65 6e64 6172 220a 2020 2020 2020  calendar".      
-00005280: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00005290: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000052a0: 2020 2020 2020 2022 6f6e 436c 6963 6b22         "onClick"
-000052b0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-000052c0: 2020 2020 2020 2020 2020 2022 6f70 656e             "open
-000052d0: 4c69 6e6b 223a 207b 0a20 2020 2020 2020  Link": {.       
-000052e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052f0: 2020 2275 726c 223a 2022 6874 7470 733a    "url": "https:
-00005300: 2f2f 6578 616d 706c 652e 636f 6d2f 6361  //example.com/ca
-00005310: 6c65 6e64 6172 220a 2020 2020 2020 2020  lendar".        
-00005320: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00005330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005340: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00005350: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-00005360: 2020 2020 2020 2020 2020 2020 2020 5d0a                ].
-00005370: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00005380: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
-00005390: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
-000053a0: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
-000053b0: 2060 6064 6174 6160 602e 0a20 2020 2020   ``data``..     
-000053c0: 2020 2074 6578 745f 696e 7075 7420 2867     text_input (g
-000053d0: 6f6f 676c 652e 6170 7073 2e63 6172 645f  oogle.apps.card_
-000053e0: 7631 2e74 7970 6573 2e54 6578 7449 6e70  v1.types.TextInp
-000053f0: 7574 293a 0a20 2020 2020 2020 2020 2020  ut):.           
-00005400: 2044 6973 706c 6179 7320 6120 7465 7874   Displays a text
-00005410: 2062 6f78 2074 6861 7420 7573 6572 7320   box that users 
-00005420: 6361 6e20 7479 7065 2069 6e74 6f2e 0a0a  can type into...
-00005430: 2020 2020 2020 2020 2020 2020 466f 7220              For 
-00005440: 6578 616d 706c 652c 2074 6865 2066 6f6c  example, the fol
-00005450: 6c6f 7769 6e67 204a 534f 4e20 6372 6561  lowing JSON crea
-00005460: 7465 7320 6120 7465 7874 2069 6e70 7574  tes a text input
-00005470: 2066 6f72 2061 6e0a 2020 2020 2020 2020   for an.        
-00005480: 2020 2020 656d 6169 6c20 6164 6472 6573      email addres
-00005490: 733a 0a0a 2020 2020 2020 2020 2020 2020  s:..            
-000054a0: 3a3a 0a0a 2020 2020 2020 2020 2020 2020  ::..            
-000054b0: 2020 2022 7465 7874 496e 7075 7422 3a20     "textInput": 
-000054c0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-000054d0: 2020 2022 6e61 6d65 223a 2022 6d61 696c     "name": "mail
-000054e0: 696e 675f 6164 6472 6573 7322 2c0a 2020  ing_address",.  
-000054f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00005500: 6c61 6265 6c22 3a20 224d 6169 6c69 6e67  label": "Mailing
-00005510: 2041 6464 7265 7373 220a 2020 2020 2020   Address".      
-00005520: 2020 2020 2020 2020 207d 0a0a 2020 2020           }..    
-00005530: 2020 2020 2020 2020 4173 2061 6e6f 7468          As anoth
-00005540: 6572 2065 7861 6d70 6c65 2c20 7468 6520  er example, the 
-00005550: 666f 6c6c 6f77 696e 6720 4a53 4f4e 2063  following JSON c
-00005560: 7265 6174 6573 2061 2074 6578 7420 696e  reates a text in
-00005570: 7075 740a 2020 2020 2020 2020 2020 2020  put.            
-00005580: 666f 7220 6120 7072 6f67 7261 6d6d 696e  for a programmin
-00005590: 6720 6c61 6e67 7561 6765 2077 6974 6820  g language with 
-000055a0: 7374 6174 6963 2073 7567 6765 7374 696f  static suggestio
-000055b0: 6e73 3a0a 0a20 2020 2020 2020 2020 2020  ns:..           
-000055c0: 203a 3a0a 0a20 2020 2020 2020 2020 2020   ::..           
-000055d0: 2020 2020 2274 6578 7449 6e70 7574 223a      "textInput":
-000055e0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-000055f0: 2020 2020 226e 616d 6522 3a20 2270 7265      "name": "pre
-00005600: 6665 7272 6564 5f70 726f 6772 616d 696e  ferred_programin
-00005610: 675f 6c61 6e67 7561 6765 222c 0a20 2020  g_language",.   
-00005620: 2020 2020 2020 2020 2020 2020 2020 226c                "l
-00005630: 6162 656c 223a 2022 5072 6566 6572 7265  abel": "Preferre
-00005640: 6420 4c61 6e67 7561 6765 222c 0a20 2020  d Language",.   
-00005650: 2020 2020 2020 2020 2020 2020 2020 2269                "i
-00005660: 6e69 7469 616c 5375 6767 6573 7469 6f6e  nitialSuggestion
-00005670: 7322 3a20 7b0a 2020 2020 2020 2020 2020  s": {.          
-00005680: 2020 2020 2020 2020 2022 6974 656d 7322           "items"
-00005690: 3a20 5b0a 2020 2020 2020 2020 2020 2020  : [.            
-000056a0: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
-000056b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056c0: 2020 2274 6578 7422 3a20 2243 2b2b 220a    "text": "C++".
-000056d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056e0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-000056f0: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
-00005700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005710: 2020 2020 2020 2274 6578 7422 3a20 224a        "text": "J
-00005720: 6176 6122 0a20 2020 2020 2020 2020 2020  ava".           
-00005730: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-00005740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005750: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
-00005760: 2020 2020 2020 2020 2020 2022 7465 7874             "text
-00005770: 223a 2022 4a61 7661 5363 7269 7074 220a  ": "JavaScript".
-00005780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005790: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-000057a0: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
+00005230: 2020 2020 2020 2272 6564 223a 2030 2c0a        "red": 0,.
+00005240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005250: 2020 2020 2020 2022 6772 6565 6e22 3a20         "green": 
+00005260: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
+00005270: 2020 2020 2020 2020 2020 2262 6c75 6522            "blue"
+00005280: 3a20 312c 0a20 2020 2020 2020 2020 2020  : 1,.           
+00005290: 2020 2020 2020 2020 2020 2020 2261 6c70              "alp
+000052a0: 6861 223a 2031 0a20 2020 2020 2020 2020  ha": 1.         
+000052b0: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+000052c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000052d0: 2020 2020 2264 6973 6162 6c65 6422 3a20      "disabled": 
+000052e0: 7472 7565 2c0a 2020 2020 2020 2020 2020  true,.          
+000052f0: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+00005300: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00005310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005320: 2020 2020 2020 2269 636f 6e22 3a20 7b0a        "icon": {.
+00005330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005340: 2020 2020 2020 2022 6b6e 6f77 6e49 636f         "knownIco
+00005350: 6e22 3a20 2249 4e56 4954 4522 2c0a 2020  n": "INVITE",.  
+00005360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005370: 2020 2020 2022 616c 7454 6578 7422 3a20       "altText": 
+00005380: 2263 6865 636b 2063 616c 656e 6461 7222  "check calendar"
+00005390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000053a0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+000053b0: 2020 2020 2020 2020 2020 2020 2020 226f                "o
+000053c0: 6e43 6c69 636b 223a 207b 0a20 2020 2020  nClick": {.     
+000053d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000053e0: 2020 226f 7065 6e4c 696e 6b22 3a20 7b0a    "openLink": {.
+000053f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005400: 2020 2020 2020 2020 2022 7572 6c22 3a20           "url": 
+00005410: 2268 7474 7073 3a2f 2f65 7861 6d70 6c65  "https://example
+00005420: 2e63 6f6d 2f63 616c 656e 6461 7222 0a20  .com/calendar". 
+00005430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005440: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00005450: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
+00005460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005470: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
+00005480: 2020 2020 205d 0a20 2020 2020 2020 2020       ].         
+00005490: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
+000054a0: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
+000054b0: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
+000054c0: 6f6e 656f 6660 5f20 6060 6461 7461 6060  oneof`_ ``data``
+000054d0: 2e0a 2020 2020 2020 2020 7465 7874 5f69  ..        text_i
+000054e0: 6e70 7574 2028 676f 6f67 6c65 2e61 7070  nput (google.app
+000054f0: 732e 6361 7264 5f76 312e 7479 7065 732e  s.card_v1.types.
+00005500: 5465 7874 496e 7075 7429 3a0a 2020 2020  TextInput):.    
+00005510: 2020 2020 2020 2020 4469 7370 6c61 7973          Displays
+00005520: 2061 2074 6578 7420 626f 7820 7468 6174   a text box that
+00005530: 2075 7365 7273 2063 616e 2074 7970 6520   users can type 
+00005540: 696e 746f 2e0a 0a20 2020 2020 2020 2020  into...         
+00005550: 2020 2046 6f72 2065 7861 6d70 6c65 2c20     For example, 
+00005560: 7468 6520 666f 6c6c 6f77 696e 6720 4a53  the following JS
+00005570: 4f4e 2063 7265 6174 6573 2061 2074 6578  ON creates a tex
+00005580: 7420 696e 7075 7420 666f 7220 616e 0a20  t input for an. 
+00005590: 2020 2020 2020 2020 2020 2065 6d61 696c             email
+000055a0: 2061 6464 7265 7373 3a0a 0a20 2020 2020   address:..     
+000055b0: 2020 2020 2020 203a 3a0a 0a20 2020 2020         ::..     
+000055c0: 2020 2020 2020 2020 2020 2274 6578 7449            "textI
+000055d0: 6e70 7574 223a 207b 0a20 2020 2020 2020  nput": {.       
+000055e0: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
+000055f0: 3a20 226d 6169 6c69 6e67 5f61 6464 7265  : "mailing_addre
+00005600: 7373 222c 0a20 2020 2020 2020 2020 2020  ss",.           
+00005610: 2020 2020 2020 226c 6162 656c 223a 2022        "label": "
+00005620: 4d61 696c 696e 6720 4164 6472 6573 7322  Mailing Address"
+00005630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005640: 7d0a 0a20 2020 2020 2020 2020 2020 2041  }..            A
+00005650: 7320 616e 6f74 6865 7220 6578 616d 706c  s another exampl
+00005660: 652c 2074 6865 2066 6f6c 6c6f 7769 6e67  e, the following
+00005670: 204a 534f 4e20 6372 6561 7465 7320 6120   JSON creates a 
+00005680: 7465 7874 2069 6e70 7574 0a20 2020 2020  text input.     
+00005690: 2020 2020 2020 2066 6f72 2061 2070 726f         for a pro
+000056a0: 6772 616d 6d69 6e67 206c 616e 6775 6167  gramming languag
+000056b0: 6520 7769 7468 2073 7461 7469 6320 7375  e with static su
+000056c0: 6767 6573 7469 6f6e 733a 0a0a 2020 2020  ggestions:..    
+000056d0: 2020 2020 2020 2020 3a3a 0a0a 2020 2020          ::..    
+000056e0: 2020 2020 2020 2020 2020 2022 7465 7874             "text
+000056f0: 496e 7075 7422 3a20 7b0a 2020 2020 2020  Input": {.      
+00005700: 2020 2020 2020 2020 2020 2022 6e61 6d65             "name
+00005710: 223a 2022 7072 6566 6572 7265 645f 7072  ": "preferred_pr
+00005720: 6f67 7261 6d69 6e67 5f6c 616e 6775 6167  ograming_languag
+00005730: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+00005740: 2020 2020 2022 6c61 6265 6c22 3a20 2250       "label": "P
+00005750: 7265 6665 7272 6564 204c 616e 6775 6167  referred Languag
+00005760: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+00005770: 2020 2020 2022 696e 6974 6961 6c53 7567       "initialSug
+00005780: 6765 7374 696f 6e73 223a 207b 0a20 2020  gestions": {.   
+00005790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000057a0: 2269 7465 6d73 223a 205b 0a20 2020 2020  "items": [.     
 000057b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057c0: 2020 2020 2020 2274 6578 7422 3a20 2250        "text": "P
-000057d0: 7974 686f 6e22 0a20 2020 2020 2020 2020  ython".         
-000057e0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-000057f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005800: 205d 0a20 2020 2020 2020 2020 2020 2020   ].             
-00005810: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
-00005820: 2020 2020 207d 0a0a 2020 2020 2020 2020       }..        
-00005830: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
-00005840: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
-00005850: 6e65 6f66 605f 2060 6064 6174 6160 602e  neof`_ ``data``.
-00005860: 0a20 2020 2020 2020 2073 656c 6563 7469  .        selecti
-00005870: 6f6e 5f69 6e70 7574 2028 676f 6f67 6c65  on_input (google
-00005880: 2e61 7070 732e 6361 7264 5f76 312e 7479  .apps.card_v1.ty
-00005890: 7065 732e 5365 6c65 6374 696f 6e49 6e70  pes.SelectionInp
-000058a0: 7574 293a 0a20 2020 2020 2020 2020 2020  ut):.           
-000058b0: 2044 6973 706c 6179 7320 6120 7365 6c65   Displays a sele
-000058c0: 6374 696f 6e20 636f 6e74 726f 6c20 7468  ction control th
-000058d0: 6174 206c 6574 7320 7573 6572 7320 7365  at lets users se
-000058e0: 6c65 6374 2069 7465 6d73 2e0a 2020 2020  lect items..    
-000058f0: 2020 2020 2020 2020 5365 6c65 6374 696f          Selectio
-00005900: 6e20 636f 6e74 726f 6c73 2063 616e 2062  n controls can b
-00005910: 6520 6368 6563 6b62 6f78 6573 2c20 7261  e checkboxes, ra
-00005920: 6469 6f20 6275 7474 6f6e 732c 0a20 2020  dio buttons,.   
-00005930: 2020 2020 2020 2020 2073 7769 7463 6865           switche
-00005940: 732c 206f 7220 6472 6f70 646f 776e 206d  s, or dropdown m
-00005950: 656e 7573 2e0a 0a20 2020 2020 2020 2020  enus...         
-00005960: 2020 2046 6f72 2065 7861 6d70 6c65 2c20     For example, 
-00005970: 7468 6520 666f 6c6c 6f77 696e 6720 4a53  the following JS
-00005980: 4f4e 2063 7265 6174 6573 2061 2064 726f  ON creates a dro
-00005990: 7064 6f77 6e20 6d65 6e75 2074 6861 740a  pdown menu that.
-000059a0: 2020 2020 2020 2020 2020 2020 6c65 7473              lets
-000059b0: 2075 7365 7273 2063 686f 6f73 6520 6120   users choose a 
-000059c0: 7369 7a65 3a0a 0a20 2020 2020 2020 2020  size:..         
-000059d0: 2020 203a 3a0a 0a20 2020 2020 2020 2020     ::..         
-000059e0: 2020 2020 2020 2273 656c 6563 7469 6f6e        "selection
-000059f0: 496e 7075 7422 3a20 7b0a 2020 2020 2020  Input": {.      
-00005a00: 2020 2020 2020 2020 2020 2022 6e61 6d65             "name
-00005a10: 223a 2022 7369 7a65 222c 0a20 2020 2020  ": "size",.     
-00005a20: 2020 2020 2020 2020 2020 2020 226c 6162              "lab
-00005a30: 656c 223a 2022 5369 7a65 220a 2020 2020  el": "Size".    
-00005a40: 2020 2020 2020 2020 2020 2020 2022 7479               "ty
-00005a50: 7065 223a 2022 4452 4f50 444f 574e 222c  pe": "DROPDOWN",
-00005a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005a70: 2020 2269 7465 6d73 223a 205b 0a20 2020    "items": [.   
-00005a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a90: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00005aa0: 2020 2020 2020 2022 7465 7874 223a 2022         "text": "
-00005ab0: 5322 2c0a 2020 2020 2020 2020 2020 2020  S",.            
-00005ac0: 2020 2020 2020 2020 2022 7661 6c75 6522           "value"
-00005ad0: 3a20 2273 6d61 6c6c 222c 0a20 2020 2020  : "small",.     
-00005ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005af0: 2273 656c 6563 7465 6422 3a20 6661 6c73  "selected": fals
-00005b00: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00005b10: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-00005b20: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
-00005b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b40: 2020 2274 6578 7422 3a20 224d 222c 0a20    "text": "M",. 
-00005b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b60: 2020 2020 2276 616c 7565 223a 2022 6d65      "value": "me
-00005b70: 6469 756d 222c 0a20 2020 2020 2020 2020  dium",.         
-00005b80: 2020 2020 2020 2020 2020 2020 2273 656c              "sel
-00005b90: 6563 7465 6422 3a20 7472 7565 0a20 2020  ected": true.   
-00005ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005bb0: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-00005bc0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-00005bd0: 2020 2020 2020 2020 2020 2020 2022 7465               "te
-00005be0: 7874 223a 2022 4c22 2c0a 2020 2020 2020  xt": "L",.      
-00005bf0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00005c00: 7661 6c75 6522 3a20 226c 6172 6765 222c  value": "large",
-00005c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005c20: 2020 2020 2020 2273 656c 6563 7465 6422        "selected"
-00005c30: 3a20 6661 6c73 650a 2020 2020 2020 2020  : false.        
-00005c40: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
-00005c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c60: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00005c70: 2020 2020 2020 2020 2274 6578 7422 3a20          "text": 
-00005c80: 2258 4c22 2c0a 2020 2020 2020 2020 2020  "XL",.          
-00005c90: 2020 2020 2020 2020 2020 2022 7661 6c75             "valu
-00005ca0: 6522 3a20 2265 7874 7261 5f6c 6172 6765  e": "extra_large
-00005cb0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00005cc0: 2020 2020 2020 2020 2273 656c 6563 7465          "selecte
-00005cd0: 6422 3a20 6661 6c73 650a 2020 2020 2020  d": false.      
-00005ce0: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
-00005cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d00: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00005d10: 207d 0a0a 2020 2020 2020 2020 2020 2020   }..            
-00005d20: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
-00005d30: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
-00005d40: 605f 2060 6064 6174 6160 602e 0a20 2020  `_ ``data``..   
-00005d50: 2020 2020 2064 6174 655f 7469 6d65 5f70       date_time_p
-00005d60: 6963 6b65 7220 2867 6f6f 676c 652e 6170  icker (google.ap
-00005d70: 7073 2e63 6172 645f 7631 2e74 7970 6573  ps.card_v1.types
-00005d80: 2e44 6174 6554 696d 6550 6963 6b65 7229  .DateTimePicker)
-00005d90: 3a0a 2020 2020 2020 2020 2020 2020 4469  :.            Di
-00005da0: 7370 6c61 7973 2061 2077 6964 6765 7420  splays a widget 
-00005db0: 7468 6174 206c 6574 7320 7573 6572 7320  that lets users 
-00005dc0: 696e 7075 7420 6120 6461 7465 2c20 7469  input a date, ti
-00005dd0: 6d65 2c20 6f72 0a20 2020 2020 2020 2020  me, or.         
-00005de0: 2020 2064 6174 6520 616e 6420 7469 6d65     date and time
-00005df0: 2e0a 0a20 2020 2020 2020 2020 2020 2046  ...            F
-00005e00: 6f72 2065 7861 6d70 6c65 2c20 7468 6520  or example, the 
-00005e10: 666f 6c6c 6f77 696e 6720 4a53 4f4e 2063  following JSON c
-00005e20: 7265 6174 6573 2061 2064 6174 6520 7469  reates a date ti
-00005e30: 6d65 2070 6963 6b65 720a 2020 2020 2020  me picker.      
-00005e40: 2020 2020 2020 746f 2073 6368 6564 756c        to schedul
-00005e50: 6520 616e 2061 7070 6f69 6e74 6d65 6e74  e an appointment
-00005e60: 3a0a 0a20 2020 2020 2020 2020 2020 203a  :..            :
-00005e70: 3a0a 0a20 2020 2020 2020 2020 2020 2020  :..             
-00005e80: 2020 2264 6174 6554 696d 6550 6963 6b65    "dateTimePicke
-00005e90: 7222 3a20 7b0a 2020 2020 2020 2020 2020  r": {.          
-00005ea0: 2020 2020 2020 2022 6e61 6d65 223a 2022         "name": "
-00005eb0: 6170 706f 696e 746d 656e 745f 7469 6d65  appointment_time
-00005ec0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00005ed0: 2020 2020 226c 6162 656c 223a 2022 426f      "label": "Bo
-00005ee0: 6f6b 2079 6f75 7220 6170 706f 696e 746d  ok your appointm
-00005ef0: 656e 7420 6174 3a22 2c0a 2020 2020 2020  ent at:",.      
-00005f00: 2020 2020 2020 2020 2020 2022 7479 7065             "type
-00005f10: 223a 2022 4441 5445 5f41 4e44 5f54 494d  ": "DATE_AND_TIM
-00005f20: 4522 2c0a 2020 2020 2020 2020 2020 2020  E",.            
-00005f30: 2020 2020 2022 7661 6c75 654d 7345 706f       "valueMsEpo
-00005f40: 6368 223a 2022 3739 3634 3335 3230 3030  ch": "7964352000
-00005f50: 3030 220a 2020 2020 2020 2020 2020 2020  00".            
-00005f60: 2020 207d 0a0a 2020 2020 2020 2020 2020     }..          
-00005f70: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
-00005f80: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
-00005f90: 6f66 605f 2060 6064 6174 6160 602e 0a20  of`_ ``data``.. 
-00005fa0: 2020 2020 2020 2064 6976 6964 6572 2028         divider (
-00005fb0: 676f 6f67 6c65 2e61 7070 732e 6361 7264  google.apps.card
-00005fc0: 5f76 312e 7479 7065 732e 4469 7669 6465  _v1.types.Divide
-00005fd0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-00005fe0: 4469 7370 6c61 7973 2061 2068 6f72 697a  Displays a horiz
-00005ff0: 6f6e 7461 6c20 6c69 6e65 2064 6976 6964  ontal line divid
-00006000: 6572 2062 6574 7765 656e 2077 6964 6765  er between widge
-00006010: 7473 2e0a 0a20 2020 2020 2020 2020 2020  ts...           
-00006020: 2046 6f72 2065 7861 6d70 6c65 2c20 7468   For example, th
-00006030: 6520 666f 6c6c 6f77 696e 6720 4a53 4f4e  e following JSON
-00006040: 2063 7265 6174 6573 2061 2064 6976 6964   creates a divid
-00006050: 6572 3a0a 0a20 2020 2020 2020 2020 2020  er:..           
-00006060: 203a 3a0a 0a20 2020 2020 2020 2020 2020   ::..           
-00006070: 2020 2020 2264 6976 6964 6572 223a 207b      "divider": {
-00006080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006090: 7d0a 0a20 2020 2020 2020 2020 2020 2054  }..            T
-000060a0: 6869 7320 6669 656c 6420 6973 2061 206d  his field is a m
-000060b0: 656d 6265 7220 6f66 2060 6f6e 656f 6660  ember of `oneof`
-000060c0: 5f20 6060 6461 7461 6060 2e0a 2020 2020  _ ``data``..    
-000060d0: 2020 2020 6772 6964 2028 676f 6f67 6c65      grid (google
-000060e0: 2e61 7070 732e 6361 7264 5f76 312e 7479  .apps.card_v1.ty
-000060f0: 7065 732e 4772 6964 293a 0a20 2020 2020  pes.Grid):.     
-00006100: 2020 2020 2020 2044 6973 706c 6179 7320         Displays 
-00006110: 6120 6772 6964 2077 6974 6820 6120 636f  a grid with a co
-00006120: 6c6c 6563 7469 6f6e 206f 6620 6974 656d  llection of item
-00006130: 732e 0a0a 2020 2020 2020 2020 2020 2020  s...            
-00006140: 4120 6772 6964 2073 7570 706f 7274 7320  A grid supports 
-00006150: 616e 7920 6e75 6d62 6572 206f 6620 636f  any number of co
-00006160: 6c75 6d6e 7320 616e 6420 6974 656d 732e  lumns and items.
-00006170: 2054 6865 206e 756d 6265 720a 2020 2020   The number.    
-00006180: 2020 2020 2020 2020 6f66 2072 6f77 7320          of rows 
-00006190: 6973 2064 6574 6572 6d69 6e65 6420 6279  is determined by
-000061a0: 2074 6865 2075 7070 6572 2062 6f75 6e64   the upper bound
-000061b0: 7320 6f66 2074 6865 206e 756d 6265 720a  s of the number.
-000061c0: 2020 2020 2020 2020 2020 2020 6974 656d              item
-000061d0: 7320 6469 7669 6465 6420 6279 2074 6865  s divided by the
-000061e0: 206e 756d 6265 7220 6f66 2063 6f6c 756d   number of colum
-000061f0: 6e73 2e20 4120 6772 6964 2077 6974 6820  ns. A grid with 
-00006200: 3130 2069 7465 6d73 0a20 2020 2020 2020  10 items.       
-00006210: 2020 2020 2061 6e64 2032 2063 6f6c 756d       and 2 colum
-00006220: 6e73 2068 6173 2035 2072 6f77 732e 2041  ns has 5 rows. A
-00006230: 2067 7269 6420 7769 7468 2031 3120 6974   grid with 11 it
-00006240: 656d 7320 616e 6420 3220 636f 6c75 6d6e  ems and 2 column
-00006250: 730a 2020 2020 2020 2020 2020 2020 6861  s.            ha
-00006260: 7320 3620 726f 7773 2e0a 0a20 2020 2020  s 6 rows...     
-00006270: 2020 2020 2020 2060 476f 6f67 6c65 2057         `Google W
-00006280: 6f72 6b73 7061 6365 2041 6464 2d6f 6e73  orkspace Add-ons
-00006290: 2061 6e64 2043 6861 740a 2020 2020 2020   and Chat.      
-000062a0: 2020 2020 2020 6170 7073 203c 6874 7470        apps <http
-000062b0: 733a 2f2f 6465 7665 6c6f 7065 7273 2e67  s://developers.g
-000062c0: 6f6f 676c 652e 636f 6d2f 776f 726b 7370  oogle.com/worksp
-000062d0: 6163 652f 6578 7465 6e64 3e60 5f5f 3a0a  ace/extend>`__:.
-000062e0: 0a20 2020 2020 2020 2020 2020 2046 6f72  .            For
-000062f0: 2065 7861 6d70 6c65 2c20 7468 6520 666f   example, the fo
-00006300: 6c6c 6f77 696e 6720 4a53 4f4e 2063 7265  llowing JSON cre
-00006310: 6174 6573 2061 2032 2063 6f6c 756d 6e20  ates a 2 column 
-00006320: 6772 6964 2077 6974 680a 2020 2020 2020  grid with.      
-00006330: 2020 2020 2020 6120 7369 6e67 6c65 2069        a single i
-00006340: 7465 6d3a 0a0a 2020 2020 2020 2020 2020  tem:..          
-00006350: 2020 3a3a 0a0a 2020 2020 2020 2020 2020    ::..          
-00006360: 2020 2020 2022 6772 6964 223a 207b 0a20       "grid": {. 
-00006370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006380: 2274 6974 6c65 223a 2022 4120 6669 6e65  "title": "A fine
-00006390: 2063 6f6c 6c65 6374 696f 6e20 6f66 2069   collection of i
-000063a0: 7465 6d73 222c 0a20 2020 2020 2020 2020  tems",.         
-000063b0: 2020 2020 2020 2020 2263 6f6c 756d 6e43          "columnC
-000063c0: 6f75 6e74 223a 2032 2c0a 2020 2020 2020  ount": 2,.      
-000063d0: 2020 2020 2020 2020 2020 2022 626f 7264             "bord
-000063e0: 6572 5374 796c 6522 3a20 7b0a 2020 2020  erStyle": {.    
-000063f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00006400: 7479 7065 223a 2022 5354 524f 4b45 222c  type": "STROKE",
-00006410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006420: 2020 2020 2263 6f72 6e65 7252 6164 6975      "cornerRadiu
-00006430: 7322 3a20 340a 2020 2020 2020 2020 2020  s": 4.          
-00006440: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00006450: 2020 2020 2020 2020 2020 2022 6974 656d             "item
-00006460: 7322 3a20 5b0a 2020 2020 2020 2020 2020  s": [.          
-00006470: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
-00006480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006490: 2269 6d61 6765 223a 207b 0a20 2020 2020  "image": {.     
-000064a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064b0: 2020 2269 6d61 6765 5572 6922 3a20 2268    "imageUri": "h
-000064c0: 7474 7073 3a2f 2f77 7777 2e65 7861 6d70  ttps://www.examp
-000064d0: 6c65 2e63 6f6d 2f69 6d61 6765 2e70 6e67  le.com/image.png
-000064e0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-000064f0: 2020 2020 2020 2020 2020 2263 726f 7053            "cropS
-00006500: 7479 6c65 223a 207b 0a20 2020 2020 2020  tyle": {.       
-00006510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006520: 2020 2274 7970 6522 3a20 2253 5155 4152    "type": "SQUAR
-00006530: 4522 0a20 2020 2020 2020 2020 2020 2020  E".             
-00006540: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-00006550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006560: 2020 2020 2262 6f72 6465 7253 7479 6c65      "borderStyle
-00006570: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-00006580: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-00006590: 7970 6522 3a20 2253 5452 4f4b 4522 0a20  ype": "STROKE". 
-000065a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065b0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-000065c0: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
-000065d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065e0: 2020 2020 2022 7469 746c 6522 3a20 2241       "title": "A
-000065f0: 6e20 6974 656d 222c 0a20 2020 2020 2020  n item",.       
-00006600: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-00006610: 6578 7441 6c69 676e 6d65 6e74 223a 2022  extAlignment": "
-00006620: 4345 4e54 4552 220a 2020 2020 2020 2020  CENTER".        
-00006630: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-00006640: 2020 2020 2020 2020 2020 2020 2020 5d2c                ],
-00006650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006660: 2020 226f 6e43 6c69 636b 223a 207b 0a20    "onClick": {. 
-00006670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006680: 2020 226f 7065 6e4c 696e 6b22 3a20 7b0a    "openLink": {.
+000057c0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+000057d0: 2020 2020 2020 2020 2022 7465 7874 223a           "text":
+000057e0: 2022 432b 2b22 0a20 2020 2020 2020 2020   "C++".         
+000057f0: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+00005800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005810: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+00005820: 2020 2020 2020 2020 2020 2020 2022 7465               "te
+00005830: 7874 223a 2022 4a61 7661 220a 2020 2020  xt": "Java".    
+00005840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005850: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
+00005860: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
+00005870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005880: 2020 2274 6578 7422 3a20 224a 6176 6153    "text": "JavaS
+00005890: 6372 6970 7422 0a20 2020 2020 2020 2020  cript".         
+000058a0: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+000058b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000058c0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+000058d0: 2020 2020 2020 2020 2020 2020 2022 7465               "te
+000058e0: 7874 223a 2022 5079 7468 6f6e 220a 2020  xt": "Python".  
+000058f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005900: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
+00005910: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
+00005920: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+00005930: 2020 2020 2020 2020 2020 2020 7d0a 0a20              }.. 
+00005940: 2020 2020 2020 2020 2020 2054 6869 7320             This 
+00005950: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
+00005960: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
+00005970: 6461 7461 6060 2e0a 2020 2020 2020 2020  data``..        
+00005980: 7365 6c65 6374 696f 6e5f 696e 7075 7420  selection_input 
+00005990: 2867 6f6f 676c 652e 6170 7073 2e63 6172  (google.apps.car
+000059a0: 645f 7631 2e74 7970 6573 2e53 656c 6563  d_v1.types.Selec
+000059b0: 7469 6f6e 496e 7075 7429 3a0a 2020 2020  tionInput):.    
+000059c0: 2020 2020 2020 2020 4469 7370 6c61 7973          Displays
+000059d0: 2061 2073 656c 6563 7469 6f6e 2063 6f6e   a selection con
+000059e0: 7472 6f6c 2074 6861 7420 6c65 7473 2075  trol that lets u
+000059f0: 7365 7273 2073 656c 6563 7420 6974 656d  sers select item
+00005a00: 732e 0a20 2020 2020 2020 2020 2020 2053  s..            S
+00005a10: 656c 6563 7469 6f6e 2063 6f6e 7472 6f6c  election control
+00005a20: 7320 6361 6e20 6265 2063 6865 636b 626f  s can be checkbo
+00005a30: 7865 732c 2072 6164 696f 2062 7574 746f  xes, radio butto
+00005a40: 6e73 2c0a 2020 2020 2020 2020 2020 2020  ns,.            
+00005a50: 7377 6974 6368 6573 2c20 6f72 2064 726f  switches, or dro
+00005a60: 7064 6f77 6e20 6d65 6e75 732e 0a0a 2020  pdown menus...  
+00005a70: 2020 2020 2020 2020 2020 466f 7220 6578            For ex
+00005a80: 616d 706c 652c 2074 6865 2066 6f6c 6c6f  ample, the follo
+00005a90: 7769 6e67 204a 534f 4e20 6372 6561 7465  wing JSON create
+00005aa0: 7320 6120 6472 6f70 646f 776e 206d 656e  s a dropdown men
+00005ab0: 7520 7468 6174 0a20 2020 2020 2020 2020  u that.         
+00005ac0: 2020 206c 6574 7320 7573 6572 7320 6368     lets users ch
+00005ad0: 6f6f 7365 2061 2073 697a 653a 0a0a 2020  oose a size:..  
+00005ae0: 2020 2020 2020 2020 2020 3a3a 0a0a 2020            ::..  
+00005af0: 2020 2020 2020 2020 2020 2020 2022 7365               "se
+00005b00: 6c65 6374 696f 6e49 6e70 7574 223a 207b  lectionInput": {
+00005b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005b20: 2020 226e 616d 6522 3a20 2273 697a 6522    "name": "size"
+00005b30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00005b40: 2020 2022 6c61 6265 6c22 3a20 2253 697a     "label": "Siz
+00005b50: 6522 0a20 2020 2020 2020 2020 2020 2020  e".             
+00005b60: 2020 2020 2274 7970 6522 3a20 2244 524f      "type": "DRO
+00005b70: 5044 4f57 4e22 2c0a 2020 2020 2020 2020  PDOWN",.        
+00005b80: 2020 2020 2020 2020 2022 6974 656d 7322           "items"
+00005b90: 3a20 5b0a 2020 2020 2020 2020 2020 2020  : [.            
+00005ba0: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00005bb0: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+00005bc0: 6578 7422 3a20 2253 222c 0a20 2020 2020  ext": "S",.     
+00005bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005be0: 2276 616c 7565 223a 2022 736d 616c 6c22  "value": "small"
+00005bf0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00005c00: 2020 2020 2020 2022 7365 6c65 6374 6564         "selected
+00005c10: 223a 2066 616c 7365 0a20 2020 2020 2020  ": false.       
+00005c20: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+00005c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c40: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
+00005c50: 2020 2020 2020 2020 2022 7465 7874 223a           "text":
+00005c60: 2022 4d22 2c0a 2020 2020 2020 2020 2020   "M",.          
+00005c70: 2020 2020 2020 2020 2020 2022 7661 6c75             "valu
+00005c80: 6522 3a20 226d 6564 6975 6d22 2c0a 2020  e": "medium",.  
+00005c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ca0: 2020 2022 7365 6c65 6374 6564 223a 2074     "selected": t
+00005cb0: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
+00005cc0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00005cd0: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
+00005ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005cf0: 2020 2020 2274 6578 7422 3a20 224c 222c      "text": "L",
+00005d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005d10: 2020 2020 2020 2276 616c 7565 223a 2022        "value": "
+00005d20: 6c61 7267 6522 2c0a 2020 2020 2020 2020  large",.        
+00005d30: 2020 2020 2020 2020 2020 2020 2022 7365               "se
+00005d40: 6c65 6374 6564 223a 2066 616c 7365 0a20  lected": false. 
+00005d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d60: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
+00005d70: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+00005d80: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00005d90: 7465 7874 223a 2022 584c 222c 0a20 2020  text": "XL",.   
+00005da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005db0: 2020 2276 616c 7565 223a 2022 6578 7472    "value": "extr
+00005dc0: 615f 6c61 7267 6522 2c0a 2020 2020 2020  a_large",.      
+00005dd0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00005de0: 7365 6c65 6374 6564 223a 2066 616c 7365  selected": false
+00005df0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005e00: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
+00005e10: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
+00005e20: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
+00005e30: 2020 2020 2020 2054 6869 7320 6669 656c         This fiel
+00005e40: 6420 6973 2061 206d 656d 6265 7220 6f66  d is a member of
+00005e50: 2060 6f6e 656f 6660 5f20 6060 6461 7461   `oneof`_ ``data
+00005e60: 6060 2e0a 2020 2020 2020 2020 6461 7465  ``..        date
+00005e70: 5f74 696d 655f 7069 636b 6572 2028 676f  _time_picker (go
+00005e80: 6f67 6c65 2e61 7070 732e 6361 7264 5f76  ogle.apps.card_v
+00005e90: 312e 7479 7065 732e 4461 7465 5469 6d65  1.types.DateTime
+00005ea0: 5069 636b 6572 293a 0a20 2020 2020 2020  Picker):.       
+00005eb0: 2020 2020 2044 6973 706c 6179 7320 6120       Displays a 
+00005ec0: 7769 6467 6574 2074 6861 7420 6c65 7473  widget that lets
+00005ed0: 2075 7365 7273 2069 6e70 7574 2061 2064   users input a d
+00005ee0: 6174 652c 2074 696d 652c 206f 720a 2020  ate, time, or.  
+00005ef0: 2020 2020 2020 2020 2020 6461 7465 2061            date a
+00005f00: 6e64 2074 696d 652e 0a0a 2020 2020 2020  nd time...      
+00005f10: 2020 2020 2020 466f 7220 6578 616d 706c        For exampl
+00005f20: 652c 2074 6865 2066 6f6c 6c6f 7769 6e67  e, the following
+00005f30: 204a 534f 4e20 6372 6561 7465 7320 6120   JSON creates a 
+00005f40: 6461 7465 2074 696d 6520 7069 636b 6572  date time picker
+00005f50: 0a20 2020 2020 2020 2020 2020 2074 6f20  .            to 
+00005f60: 7363 6865 6475 6c65 2061 6e20 6170 706f  schedule an appo
+00005f70: 696e 746d 656e 743a 0a0a 2020 2020 2020  intment:..      
+00005f80: 2020 2020 2020 3a3a 0a0a 2020 2020 2020        ::..      
+00005f90: 2020 2020 2020 2020 2022 6461 7465 5469           "dateTi
+00005fa0: 6d65 5069 636b 6572 223a 207b 0a20 2020  mePicker": {.   
+00005fb0: 2020 2020 2020 2020 2020 2020 2020 226e                "n
+00005fc0: 616d 6522 3a20 2261 7070 6f69 6e74 6d65  ame": "appointme
+00005fd0: 6e74 5f74 696d 6522 2c0a 2020 2020 2020  nt_time",.      
+00005fe0: 2020 2020 2020 2020 2020 2022 6c61 6265             "labe
+00005ff0: 6c22 3a20 2242 6f6f 6b20 796f 7572 2061  l": "Book your a
+00006000: 7070 6f69 6e74 6d65 6e74 2061 743a 222c  ppointment at:",
+00006010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006020: 2020 2274 7970 6522 3a20 2244 4154 455f    "type": "DATE_
+00006030: 414e 445f 5449 4d45 222c 0a20 2020 2020  AND_TIME",.     
+00006040: 2020 2020 2020 2020 2020 2020 2276 616c              "val
+00006050: 7565 4d73 4570 6f63 6822 3a20 2237 3936  ueMsEpoch": "796
+00006060: 3433 3532 3030 3030 3022 0a20 2020 2020  435200000".     
+00006070: 2020 2020 2020 2020 2020 7d0a 0a20 2020            }..   
+00006080: 2020 2020 2020 2020 2054 6869 7320 6669           This fi
+00006090: 656c 6420 6973 2061 206d 656d 6265 7220  eld is a member 
+000060a0: 6f66 2060 6f6e 656f 6660 5f20 6060 6461  of `oneof`_ ``da
+000060b0: 7461 6060 2e0a 2020 2020 2020 2020 6469  ta``..        di
+000060c0: 7669 6465 7220 2867 6f6f 676c 652e 6170  vider (google.ap
+000060d0: 7073 2e63 6172 645f 7631 2e74 7970 6573  ps.card_v1.types
+000060e0: 2e44 6976 6964 6572 293a 0a20 2020 2020  .Divider):.     
+000060f0: 2020 2020 2020 2044 6973 706c 6179 7320         Displays 
+00006100: 6120 686f 7269 7a6f 6e74 616c 206c 696e  a horizontal lin
+00006110: 6520 6469 7669 6465 7220 6265 7477 6565  e divider betwee
+00006120: 6e20 7769 6467 6574 732e 0a0a 2020 2020  n widgets...    
+00006130: 2020 2020 2020 2020 466f 7220 6578 616d          For exam
+00006140: 706c 652c 2074 6865 2066 6f6c 6c6f 7769  ple, the followi
+00006150: 6e67 204a 534f 4e20 6372 6561 7465 7320  ng JSON creates 
+00006160: 6120 6469 7669 6465 723a 0a0a 2020 2020  a divider:..    
+00006170: 2020 2020 2020 2020 3a3a 0a0a 2020 2020          ::..    
+00006180: 2020 2020 2020 2020 2020 2022 6469 7669             "divi
+00006190: 6465 7222 3a20 7b0a 2020 2020 2020 2020  der": {.        
+000061a0: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
+000061b0: 2020 2020 2020 5468 6973 2066 6965 6c64        This field
+000061c0: 2069 7320 6120 6d65 6d62 6572 206f 6620   is a member of 
+000061d0: 606f 6e65 6f66 605f 2060 6064 6174 6160  `oneof`_ ``data`
+000061e0: 602e 0a20 2020 2020 2020 2067 7269 6420  `..        grid 
+000061f0: 2867 6f6f 676c 652e 6170 7073 2e63 6172  (google.apps.car
+00006200: 645f 7631 2e74 7970 6573 2e47 7269 6429  d_v1.types.Grid)
+00006210: 3a0a 2020 2020 2020 2020 2020 2020 4469  :.            Di
+00006220: 7370 6c61 7973 2061 2067 7269 6420 7769  splays a grid wi
+00006230: 7468 2061 2063 6f6c 6c65 6374 696f 6e20  th a collection 
+00006240: 6f66 2069 7465 6d73 2e0a 0a20 2020 2020  of items...     
+00006250: 2020 2020 2020 2041 2067 7269 6420 7375         A grid su
+00006260: 7070 6f72 7473 2061 6e79 206e 756d 6265  pports any numbe
+00006270: 7220 6f66 2063 6f6c 756d 6e73 2061 6e64  r of columns and
+00006280: 2069 7465 6d73 2e20 5468 6520 6e75 6d62   items. The numb
+00006290: 6572 0a20 2020 2020 2020 2020 2020 206f  er.            o
+000062a0: 6620 726f 7773 2069 7320 6465 7465 726d  f rows is determ
+000062b0: 696e 6564 2062 7920 7468 6520 7570 7065  ined by the uppe
+000062c0: 7220 626f 756e 6473 206f 6620 7468 6520  r bounds of the 
+000062d0: 6e75 6d62 6572 0a20 2020 2020 2020 2020  number.         
+000062e0: 2020 2069 7465 6d73 2064 6976 6964 6564     items divided
+000062f0: 2062 7920 7468 6520 6e75 6d62 6572 206f   by the number o
+00006300: 6620 636f 6c75 6d6e 732e 2041 2067 7269  f columns. A gri
+00006310: 6420 7769 7468 2031 3020 6974 656d 730a  d with 10 items.
+00006320: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+00006330: 3220 636f 6c75 6d6e 7320 6861 7320 3520  2 columns has 5 
+00006340: 726f 7773 2e20 4120 6772 6964 2077 6974  rows. A grid wit
+00006350: 6820 3131 2069 7465 6d73 2061 6e64 2032  h 11 items and 2
+00006360: 2063 6f6c 756d 6e73 0a20 2020 2020 2020   columns.       
+00006370: 2020 2020 2068 6173 2036 2072 6f77 732e       has 6 rows.
+00006380: 0a0a 2020 2020 2020 2020 2020 2020 6047  ..            `G
+00006390: 6f6f 676c 6520 576f 726b 7370 6163 6520  oogle Workspace 
+000063a0: 4164 642d 6f6e 7320 616e 6420 4368 6174  Add-ons and Chat
+000063b0: 0a20 2020 2020 2020 2020 2020 2061 7070  .            app
+000063c0: 7320 3c68 7474 7073 3a2f 2f64 6576 656c  s <https://devel
+000063d0: 6f70 6572 732e 676f 6f67 6c65 2e63 6f6d  opers.google.com
+000063e0: 2f77 6f72 6b73 7061 6365 2f65 7874 656e  /workspace/exten
+000063f0: 643e 605f 5f3a 0a0a 2020 2020 2020 2020  d>`__:..        
+00006400: 2020 2020 466f 7220 6578 616d 706c 652c      For example,
+00006410: 2074 6865 2066 6f6c 6c6f 7769 6e67 204a   the following J
+00006420: 534f 4e20 6372 6561 7465 7320 6120 3220  SON creates a 2 
+00006430: 636f 6c75 6d6e 2067 7269 6420 7769 7468  column grid with
+00006440: 0a20 2020 2020 2020 2020 2020 2061 2073  .            a s
+00006450: 696e 676c 6520 6974 656d 3a0a 0a20 2020  ingle item:..   
+00006460: 2020 2020 2020 2020 203a 3a0a 0a20 2020           ::..   
+00006470: 2020 2020 2020 2020 2020 2020 2267 7269              "gri
+00006480: 6422 3a20 7b0a 2020 2020 2020 2020 2020  d": {.          
+00006490: 2020 2020 2020 2022 7469 746c 6522 3a20         "title": 
+000064a0: 2241 2066 696e 6520 636f 6c6c 6563 7469  "A fine collecti
+000064b0: 6f6e 206f 6620 6974 656d 7322 2c0a 2020  on of items",.  
+000064c0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000064d0: 636f 6c75 6d6e 436f 756e 7422 3a20 322c  columnCount": 2,
+000064e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000064f0: 2020 2262 6f72 6465 7253 7479 6c65 223a    "borderStyle":
+00006500: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00006510: 2020 2020 2020 2274 7970 6522 3a20 2253        "type": "S
+00006520: 5452 4f4b 4522 2c0a 2020 2020 2020 2020  TROKE",.        
+00006530: 2020 2020 2020 2020 2020 2022 636f 726e             "corn
+00006540: 6572 5261 6469 7573 223a 2034 0a20 2020  erRadius": 4.   
+00006550: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
+00006560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006570: 2020 2269 7465 6d73 223a 205b 0a20 2020    "items": [.   
+00006580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006590: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+000065a0: 2020 2020 2020 2022 696d 6167 6522 3a20         "image": 
+000065b0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+000065c0: 2020 2020 2020 2020 2022 696d 6167 6555           "imageU
+000065d0: 7269 223a 2022 6874 7470 733a 2f2f 7777  ri": "https://ww
+000065e0: 772e 6578 616d 706c 652e 636f 6d2f 696d  w.example.com/im
+000065f0: 6167 652e 706e 6722 2c0a 2020 2020 2020  age.png",.      
+00006600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006610: 2022 6372 6f70 5374 796c 6522 3a20 7b0a   "cropStyle": {.
+00006620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006630: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
+00006640: 2022 5351 5541 5245 220a 2020 2020 2020   "SQUARE".      
+00006650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006660: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
+00006670: 2020 2020 2020 2020 2020 2022 626f 7264             "bord
+00006680: 6572 5374 796c 6522 3a20 7b0a 2020 2020  erStyle": {.    
 00006690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066a0: 2020 2020 2022 7572 6c22 3a20 2268 7474       "url": "htt
-000066b0: 7073 3a2f 2f77 7777 2e65 7861 6d70 6c65  ps://www.example
-000066c0: 2e63 6f6d 220a 2020 2020 2020 2020 2020  .com".          
-000066d0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-000066e0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-000066f0: 2020 2020 2020 2020 2020 2020 207d 0a0a               }..
-00006700: 2020 2020 2020 2020 2020 2020 5468 6973              This
-00006710: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
-00006720: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
-00006730: 6064 6174 6160 602e 0a20 2020 2020 2020  `data``..       
-00006740: 2063 6f6c 756d 6e73 2028 676f 6f67 6c65   columns (google
-00006750: 2e61 7070 732e 6361 7264 5f76 312e 7479  .apps.card_v1.ty
-00006760: 7065 732e 436f 6c75 6d6e 7329 3a0a 2020  pes.Columns):.  
-00006770: 2020 2020 2020 2020 2020 4469 7370 6c61            Displa
-00006780: 7973 2075 7020 746f 2032 2063 6f6c 756d  ys up to 2 colum
-00006790: 6e73 2e0a 0a20 2020 2020 2020 2020 2020  ns...           
-000067a0: 2054 6f20 696e 636c 7564 6520 6d6f 7265   To include more
-000067b0: 2074 6861 6e20 3220 636f 6c75 6d6e 732c   than 2 columns,
-000067c0: 206f 7220 746f 2075 7365 2072 6f77 732c   or to use rows,
-000067d0: 2075 7365 2074 6865 0a20 2020 2020 2020   use the.       
-000067e0: 2020 2020 2060 6047 7269 6460 6020 7769       ``Grid`` wi
-000067f0: 6467 6574 2e0a 0a20 2020 2020 2020 2020  dget...         
-00006800: 2020 2046 6f72 2065 7861 6d70 6c65 2c20     For example, 
-00006810: 7468 6520 666f 6c6c 6f77 696e 6720 4a53  the following JS
-00006820: 4f4e 2063 7265 6174 6573 2032 2063 6f6c  ON creates 2 col
-00006830: 756d 6e73 2074 6861 7420 6561 6368 0a20  umns that each. 
-00006840: 2020 2020 2020 2020 2020 2063 6f6e 7461             conta
-00006850: 696e 2074 6578 7420 7061 7261 6772 6170  in text paragrap
-00006860: 6873 3a0a 0a20 2020 2020 2020 2020 2020  hs:..           
-00006870: 203a 3a0a 0a20 2020 2020 2020 2020 2020   ::..           
-00006880: 2020 2020 2263 6f6c 756d 6e73 223a 207b      "columns": {
-00006890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000068a0: 2020 2263 6f6c 756d 6e49 7465 6d73 223a    "columnItems":
-000068b0: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
-000068c0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-000068d0: 2020 2020 2020 2020 2020 2020 2022 686f               "ho
-000068e0: 7269 7a6f 6e74 616c 5369 7a65 5374 796c  rizontalSizeStyl
-000068f0: 6522 3a20 2246 494c 4c5f 4156 4149 4c41  e": "FILL_AVAILA
-00006900: 424c 455f 5350 4143 4522 2c0a 2020 2020  BLE_SPACE",.    
-00006910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006920: 2022 686f 7269 7a6f 6e74 616c 416c 6967   "horizontalAlig
-00006930: 6e6d 656e 7422 3a20 2243 454e 5445 5222  nment": "CENTER"
-00006940: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00006950: 2020 2020 2020 2022 7665 7274 6963 616c         "vertical
-00006960: 416c 6967 6e6d 656e 7422 3a20 2243 454e  Alignment": "CEN
-00006970: 5445 5222 2c0a 2020 2020 2020 2020 2020  TER",.          
-00006980: 2020 2020 2020 2020 2020 2022 7769 6467             "widg
-00006990: 6574 7322 3a20 5b0a 2020 2020 2020 2020  ets": [.        
-000069a0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-000069b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000069c0: 2020 2020 2020 2020 2020 2274 6578 7450            "textP
-000069d0: 6172 6167 7261 7068 223a 207b 0a20 2020  aragraph": {.   
+000066a0: 2020 2020 2022 7479 7065 223a 2022 5354       "type": "ST
+000066b0: 524f 4b45 220a 2020 2020 2020 2020 2020  ROKE".          
+000066c0: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
+000066d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000066e0: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
+000066f0: 2020 2020 2020 2020 2020 2020 2274 6974              "tit
+00006700: 6c65 223a 2022 416e 2069 7465 6d22 2c0a  le": "An item",.
+00006710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006720: 2020 2020 2022 7465 7874 416c 6967 6e6d       "textAlignm
+00006730: 656e 7422 3a20 2243 454e 5445 5222 0a20  ent": "CENTER". 
+00006740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006750: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
+00006760: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
+00006770: 2020 2020 2020 2020 2022 6f6e 436c 6963           "onClic
+00006780: 6b22 3a20 7b0a 2020 2020 2020 2020 2020  k": {.          
+00006790: 2020 2020 2020 2020 2022 6f70 656e 4c69           "openLi
+000067a0: 6e6b 223a 207b 0a20 2020 2020 2020 2020  nk": {.         
+000067b0: 2020 2020 2020 2020 2020 2020 2275 726c              "url
+000067c0: 223a 2022 6874 7470 733a 2f2f 7777 772e  ": "https://www.
+000067d0: 6578 616d 706c 652e 636f 6d22 0a20 2020  example.com".   
+000067e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000067f0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00006800: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
+00006810: 2020 2020 7d0a 0a20 2020 2020 2020 2020      }..         
+00006820: 2020 2054 6869 7320 6669 656c 6420 6973     This field is
+00006830: 2061 206d 656d 6265 7220 6f66 2060 6f6e   a member of `on
+00006840: 656f 6660 5f20 6060 6461 7461 6060 2e0a  eof`_ ``data``..
+00006850: 2020 2020 2020 2020 636f 6c75 6d6e 7320          columns 
+00006860: 2867 6f6f 676c 652e 6170 7073 2e63 6172  (google.apps.car
+00006870: 645f 7631 2e74 7970 6573 2e43 6f6c 756d  d_v1.types.Colum
+00006880: 6e73 293a 0a20 2020 2020 2020 2020 2020  ns):.           
+00006890: 2044 6973 706c 6179 7320 7570 2074 6f20   Displays up to 
+000068a0: 3220 636f 6c75 6d6e 732e 0a0a 2020 2020  2 columns...    
+000068b0: 2020 2020 2020 2020 546f 2069 6e63 6c75          To inclu
+000068c0: 6465 206d 6f72 6520 7468 616e 2032 2063  de more than 2 c
+000068d0: 6f6c 756d 6e73 2c20 6f72 2074 6f20 7573  olumns, or to us
+000068e0: 6520 726f 7773 2c20 7573 6520 7468 650a  e rows, use the.
+000068f0: 2020 2020 2020 2020 2020 2020 6060 4772              ``Gr
+00006900: 6964 6060 2077 6964 6765 742e 0a0a 2020  id`` widget...  
+00006910: 2020 2020 2020 2020 2020 466f 7220 6578            For ex
+00006920: 616d 706c 652c 2074 6865 2066 6f6c 6c6f  ample, the follo
+00006930: 7769 6e67 204a 534f 4e20 6372 6561 7465  wing JSON create
+00006940: 7320 3220 636f 6c75 6d6e 7320 7468 6174  s 2 columns that
+00006950: 2065 6163 680a 2020 2020 2020 2020 2020   each.          
+00006960: 2020 636f 6e74 6169 6e20 7465 7874 2070    contain text p
+00006970: 6172 6167 7261 7068 733a 0a0a 2020 2020  aragraphs:..    
+00006980: 2020 2020 2020 2020 3a3a 0a0a 2020 2020          ::..    
+00006990: 2020 2020 2020 2020 2020 2022 636f 6c75             "colu
+000069a0: 6d6e 7322 3a20 7b0a 2020 2020 2020 2020  mns": {.        
+000069b0: 2020 2020 2020 2020 2022 636f 6c75 6d6e           "column
+000069c0: 4974 656d 7322 3a20 5b0a 2020 2020 2020  Items": [.      
+000069d0: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
 000069e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069f0: 2020 2020 2020 2020 2274 6578 7422 3a20          "text": 
-00006a00: 2246 6972 7374 2063 6f6c 756d 6e20 7465  "First column te
-00006a10: 7874 2070 6172 6167 7261 7068 220a 2020  xt paragraph".  
-00006a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a30: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-00006a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a50: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00006a60: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
-00006a70: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-00006a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a90: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
-00006aa0: 2020 2020 2020 2020 2022 686f 7269 7a6f           "horizo
-00006ab0: 6e74 616c 5369 7a65 5374 796c 6522 3a20  ntalSizeStyle": 
-00006ac0: 2246 494c 4c5f 4156 4149 4c41 424c 455f  "FILL_AVAILABLE_
-00006ad0: 5350 4143 4522 2c0a 2020 2020 2020 2020  SPACE",.        
-00006ae0: 2020 2020 2020 2020 2020 2020 2022 686f               "ho
-00006af0: 7269 7a6f 6e74 616c 416c 6967 6e6d 656e  rizontalAlignmen
-00006b00: 7422 3a20 2243 454e 5445 5222 2c0a 2020  t": "CENTER",.  
-00006b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b20: 2020 2022 7665 7274 6963 616c 416c 6967     "verticalAlig
-00006b30: 6e6d 656e 7422 3a20 2243 454e 5445 5222  nment": "CENTER"
-00006b40: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00006b50: 2020 2020 2020 2022 7769 6467 6574 7322         "widgets"
-00006b60: 3a20 5b0a 2020 2020 2020 2020 2020 2020  : [.            
-00006b70: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
+000069f0: 2020 2020 2268 6f72 697a 6f6e 7461 6c53      "horizontalS
+00006a00: 697a 6553 7479 6c65 223a 2022 4649 4c4c  izeStyle": "FILL
+00006a10: 5f41 5641 494c 4142 4c45 5f53 5041 4345  _AVAILABLE_SPACE
+00006a20: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00006a30: 2020 2020 2020 2020 2268 6f72 697a 6f6e          "horizon
+00006a40: 7461 6c41 6c69 676e 6d65 6e74 223a 2022  talAlignment": "
+00006a50: 4345 4e54 4552 222c 0a20 2020 2020 2020  CENTER",.       
+00006a60: 2020 2020 2020 2020 2020 2020 2020 2276                "v
+00006a70: 6572 7469 6361 6c41 6c69 676e 6d65 6e74  erticalAlignment
+00006a80: 223a 2022 4345 4e54 4552 222c 0a20 2020  ": "CENTER",.   
+00006a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006aa0: 2020 2277 6964 6765 7473 223a 205b 0a20    "widgets": [. 
+00006ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ac0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00006ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ae0: 2022 7465 7874 5061 7261 6772 6170 6822   "textParagraph"
+00006af0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00006b00: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00006b10: 7465 7874 223a 2022 4669 7273 7420 636f  text": "First co
+00006b20: 6c75 6d6e 2074 6578 7420 7061 7261 6772  lumn text paragr
+00006b30: 6170 6822 0a20 2020 2020 2020 2020 2020  aph".           
+00006b40: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
+00006b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b60: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00006b70: 2020 2020 2020 2020 2020 2020 2020 5d0a                ].
 00006b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b90: 2020 2020 2020 2274 6578 7450 6172 6167        "textParag
-00006ba0: 7261 7068 223a 207b 0a20 2020 2020 2020  raph": {.       
+00006b90: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
+00006ba0: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
 00006bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006bc0: 2020 2020 2274 6578 7422 3a20 2253 6563      "text": "Sec
-00006bd0: 6f6e 6420 636f 6c75 6d6e 2074 6578 7420  ond column text 
-00006be0: 7061 7261 6772 6170 6822 0a20 2020 2020  paragraph".     
+00006bc0: 2268 6f72 697a 6f6e 7461 6c53 697a 6553  "horizontalSizeS
+00006bd0: 7479 6c65 223a 2022 4649 4c4c 5f41 5641  tyle": "FILL_AVA
+00006be0: 494c 4142 4c45 5f53 5041 4345 222c 0a20  ILABLE_SPACE",. 
 00006bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c00: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
-00006c10: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
-00006c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c30: 2020 2020 5d0a 2020 2020 2020 2020 2020      ].          
-00006c40: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00006c50: 2020 2020 2020 2020 2020 2020 5d0a 2020              ].  
-00006c60: 2020 2020 2020 2020 2020 2020 207d 0a0a               }..
-00006c70: 2020 2020 2020 2020 2020 2020 5468 6973              This
-00006c80: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
-00006c90: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
-00006ca0: 6064 6174 6160 602e 0a20 2020 2020 2020  `data``..       
-00006cb0: 2068 6f72 697a 6f6e 7461 6c5f 616c 6967   horizontal_alig
-00006cc0: 6e6d 656e 7420 2867 6f6f 676c 652e 6170  nment (google.ap
-00006cd0: 7073 2e63 6172 645f 7631 2e74 7970 6573  ps.card_v1.types
-00006ce0: 2e57 6964 6765 742e 486f 7269 7a6f 6e74  .Widget.Horizont
-00006cf0: 616c 416c 6967 6e6d 656e 7429 3a0a 2020  alAlignment):.  
-00006d00: 2020 2020 2020 2020 2020 5370 6563 6966            Specif
-00006d10: 6965 7320 7768 6574 6865 7220 7769 6467  ies whether widg
-00006d20: 6574 7320 616c 6967 6e20 746f 2074 6865  ets align to the
-00006d30: 206c 6566 742c 0a20 2020 2020 2020 2020   left,.         
-00006d40: 2020 2072 6967 6874 2c20 6f72 2063 656e     right, or cen
-00006d50: 7465 7220 6f66 2061 2063 6f6c 756d 6e2e  ter of a column.
-00006d60: 0a20 2020 2022 2222 0a0a 2020 2020 636c  .    """..    cl
-00006d70: 6173 7320 496d 6167 6554 7970 6528 7072  ass ImageType(pr
-00006d80: 6f74 6f2e 456e 756d 293a 0a20 2020 2020  oto.Enum):.     
-00006d90: 2020 2072 2222 2254 6865 2073 6861 7065     r"""The shape
-00006da0: 2075 7365 6420 746f 2063 726f 7020 7468   used to crop th
-00006db0: 6520 696d 6167 652e 0a0a 2020 2020 2020  e image...      
-00006dc0: 2020 6047 6f6f 676c 6520 576f 726b 7370    `Google Worksp
-00006dd0: 6163 6520 4164 642d 6f6e 7320 616e 6420  ace Add-ons and 
-00006de0: 4368 6174 0a20 2020 2020 2020 2061 7070  Chat.        app
-00006df0: 7320 3c68 7474 7073 3a2f 2f64 6576 656c  s <https://devel
-00006e00: 6f70 6572 732e 676f 6f67 6c65 2e63 6f6d  opers.google.com
-00006e10: 2f77 6f72 6b73 7061 6365 2f65 7874 656e  /workspace/exten
-00006e20: 643e 605f 5f3a 0a0a 2020 2020 2020 2020  d>`__:..        
-00006e30: 5661 6c75 6573 3a0a 2020 2020 2020 2020  Values:.        
-00006e40: 2020 2020 5351 5541 5245 2028 3029 3a0a      SQUARE (0):.
-00006e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e60: 4465 6661 756c 7420 7661 6c75 652e 2041  Default value. A
-00006e70: 7070 6c69 6573 2061 2073 7175 6172 6520  pplies a square 
-00006e80: 6d61 736b 2074 6f20 7468 650a 2020 2020  mask to the.    
-00006e90: 2020 2020 2020 2020 2020 2020 696d 6167              imag
-00006ea0: 652e 2046 6f72 2065 7861 6d70 6c65 2c20  e. For example, 
-00006eb0: 6120 3478 3320 696d 6167 6520 6265 636f  a 4x3 image beco
-00006ec0: 6d65 7320 3378 332e 0a20 2020 2020 2020  mes 3x3..       
-00006ed0: 2020 2020 2043 4952 434c 4520 2831 293a       CIRCLE (1):
-00006ee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006ef0: 2041 7070 6c69 6573 2061 2063 6972 6375   Applies a circu
-00006f00: 6c61 7220 6d61 736b 2074 6f20 7468 6520  lar mask to the 
-00006f10: 696d 6167 652e 2046 6f72 0a20 2020 2020  image. For.     
-00006f20: 2020 2020 2020 2020 2020 2065 7861 6d70             examp
-00006f30: 6c65 2c20 6120 3478 3320 696d 6167 6520  le, a 4x3 image 
-00006f40: 6265 636f 6d65 7320 6120 6369 7263 6c65  becomes a circle
-00006f50: 2077 6974 6820 610a 2020 2020 2020 2020   with a.        
-00006f60: 2020 2020 2020 2020 6469 616d 6574 6572          diameter
-00006f70: 206f 6620 332e 0a20 2020 2020 2020 2022   of 3..        "
-00006f80: 2222 0a20 2020 2020 2020 2053 5155 4152  "".        SQUAR
-00006f90: 4520 3d20 300a 2020 2020 2020 2020 4349  E = 0.        CI
-00006fa0: 5243 4c45 203d 2031 0a0a 2020 2020 636c  RCLE = 1..    cl
-00006fb0: 6173 7320 486f 7269 7a6f 6e74 616c 416c  ass HorizontalAl
-00006fc0: 6967 6e6d 656e 7428 7072 6f74 6f2e 456e  ignment(proto.En
-00006fd0: 756d 293a 0a20 2020 2020 2020 2072 2222  um):.        r""
-00006fe0: 2253 7065 6369 6669 6573 2077 6865 7468  "Specifies wheth
-00006ff0: 6572 2077 6964 6765 7473 2061 6c69 676e  er widgets align
-00007000: 2074 6f20 7468 6520 6c65 6674 2c20 7269   to the left, ri
-00007010: 6768 742c 206f 7220 6365 6e74 6572 206f  ght, or center o
-00007020: 6620 610a 2020 2020 2020 2020 636f 6c75  f a.        colu
-00007030: 6d6e 2e0a 0a20 2020 2020 2020 2060 476f  mn...        `Go
-00007040: 6f67 6c65 2043 6861 7420 6170 7073 203c  ogle Chat apps <
-00007050: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
-00007060: 7273 2e67 6f6f 676c 652e 636f 6d2f 6368  rs.google.com/ch
-00007070: 6174 3e60 5f5f 3a0a 0a20 2020 2020 2020  at>`__:..       
-00007080: 2056 616c 7565 733a 0a20 2020 2020 2020   Values:.       
-00007090: 2020 2020 2048 4f52 495a 4f4e 5441 4c5f       HORIZONTAL_
-000070a0: 414c 4947 4e4d 454e 545f 554e 5350 4543  ALIGNMENT_UNSPEC
-000070b0: 4946 4945 4420 2830 293a 0a20 2020 2020  IFIED (0):.     
-000070c0: 2020 2020 2020 2020 2020 2044 6f6e 2774             Don't
-000070d0: 2075 7365 2e20 556e 7370 6563 6966 6965   use. Unspecifie
-000070e0: 642e 0a20 2020 2020 2020 2020 2020 2053  d..            S
-000070f0: 5441 5254 2028 3129 3a0a 2020 2020 2020  TART (1):.      
-00007100: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
-00007110: 7420 7661 6c75 652e 2041 6c69 676e 7320  t value. Aligns 
-00007120: 7769 6467 6574 7320 746f 2074 6865 2073  widgets to the s
-00007130: 7461 7274 0a20 2020 2020 2020 2020 2020  tart.           
-00007140: 2020 2020 2070 6f73 6974 696f 6e20 6f66       position of
-00007150: 2074 6865 2063 6f6c 756d 6e2e 2046 6f72   the column. For
-00007160: 206c 6566 742d 746f 2d72 6967 6874 0a20   left-to-right. 
-00007170: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00007180: 6179 6f75 7473 2c20 616c 6967 6e73 2074  ayouts, aligns t
-00007190: 6f20 7468 6520 6c65 6674 2e20 466f 7220  o the left. For 
-000071a0: 7269 6768 742d 746f 2d6c 6566 740a 2020  right-to-left.  
-000071b0: 2020 2020 2020 2020 2020 2020 2020 6c61                la
-000071c0: 796f 7574 732c 2061 6c69 676e 7320 746f  youts, aligns to
-000071d0: 2074 6865 2072 6967 6874 2e0a 2020 2020   the right..    
-000071e0: 2020 2020 2020 2020 4345 4e54 4552 2028          CENTER (
-000071f0: 3229 3a0a 2020 2020 2020 2020 2020 2020  2):.            
-00007200: 2020 2020 416c 6967 6e73 2077 6964 6765      Aligns widge
-00007210: 7473 2074 6f20 7468 6520 6365 6e74 6572  ts to the center
-00007220: 206f 6620 7468 6520 636f 6c75 6d6e 2e0a   of the column..
-00007230: 2020 2020 2020 2020 2020 2020 454e 4420              END 
-00007240: 2833 293a 0a20 2020 2020 2020 2020 2020  (3):.           
-00007250: 2020 2020 2041 6c69 676e 7320 7769 6467       Aligns widg
-00007260: 6574 7320 746f 2074 6865 2065 6e64 2070  ets to the end p
-00007270: 6f73 6974 696f 6e20 6f66 2074 6865 0a20  osition of the. 
-00007280: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00007290: 6f6c 756d 6e2e 2046 6f72 206c 6566 742d  olumn. For left-
-000072a0: 746f 2d72 6967 6874 206c 6179 6f75 7473  to-right layouts
-000072b0: 2c20 616c 6967 6e73 0a20 2020 2020 2020  , aligns.       
-000072c0: 2020 2020 2020 2020 2077 6964 6765 7473           widgets
-000072d0: 2074 6f20 7468 6520 7269 6768 742e 2046   to the right. F
-000072e0: 6f72 2072 6967 6874 2d74 6f2d 6c65 6674  or right-to-left
-000072f0: 206c 6179 6f75 7473 2c0a 2020 2020 2020   layouts,.      
-00007300: 2020 2020 2020 2020 2020 616c 6967 6e73            aligns
-00007310: 2077 6964 6765 7473 2074 6f20 7468 6520   widgets to the 
-00007320: 6c65 6674 2e0a 2020 2020 2020 2020 2222  left..        ""
-00007330: 220a 2020 2020 2020 2020 484f 5249 5a4f  ".        HORIZO
-00007340: 4e54 414c 5f41 4c49 474e 4d45 4e54 5f55  NTAL_ALIGNMENT_U
-00007350: 4e53 5045 4349 4649 4544 203d 2030 0a20  NSPECIFIED = 0. 
-00007360: 2020 2020 2020 2053 5441 5254 203d 2031         START = 1
-00007370: 0a20 2020 2020 2020 2043 454e 5445 5220  .        CENTER 
-00007380: 3d20 320a 2020 2020 2020 2020 454e 4420  = 2.        END 
-00007390: 3d20 330a 0a20 2020 2074 6578 745f 7061  = 3..    text_pa
-000073a0: 7261 6772 6170 683a 2022 5465 7874 5061  ragraph: "TextPa
-000073b0: 7261 6772 6170 6822 203d 2070 726f 746f  ragraph" = proto
-000073c0: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
-000073d0: 7072 6f74 6f2e 4d45 5353 4147 452c 0a20  proto.MESSAGE,. 
-000073e0: 2020 2020 2020 206e 756d 6265 723d 312c         number=1,
-000073f0: 0a20 2020 2020 2020 206f 6e65 6f66 3d22  .        oneof="
-00007400: 6461 7461 222c 0a20 2020 2020 2020 206d  data",.        m
-00007410: 6573 7361 6765 3d22 5465 7874 5061 7261  essage="TextPara
-00007420: 6772 6170 6822 2c0a 2020 2020 290a 2020  graph",.    ).  
-00007430: 2020 696d 6167 653a 2022 496d 6167 6522    image: "Image"
-00007440: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
-00007450: 2020 2020 2020 2020 7072 6f74 6f2e 4d45          proto.ME
-00007460: 5353 4147 452c 0a20 2020 2020 2020 206e  SSAGE,.        n
-00007470: 756d 6265 723d 322c 0a20 2020 2020 2020  umber=2,.       
-00007480: 206f 6e65 6f66 3d22 6461 7461 222c 0a20   oneof="data",. 
-00007490: 2020 2020 2020 206d 6573 7361 6765 3d22         message="
-000074a0: 496d 6167 6522 2c0a 2020 2020 290a 2020  Image",.    ).  
-000074b0: 2020 6465 636f 7261 7465 645f 7465 7874    decorated_text
-000074c0: 3a20 2244 6563 6f72 6174 6564 5465 7874  : "DecoratedText
-000074d0: 2220 3d20 7072 6f74 6f2e 4669 656c 6428  " = proto.Field(
-000074e0: 0a20 2020 2020 2020 2070 726f 746f 2e4d  .        proto.M
-000074f0: 4553 5341 4745 2c0a 2020 2020 2020 2020  ESSAGE,.        
-00007500: 6e75 6d62 6572 3d33 2c0a 2020 2020 2020  number=3,.      
-00007510: 2020 6f6e 656f 663d 2264 6174 6122 2c0a    oneof="data",.
-00007520: 2020 2020 2020 2020 6d65 7373 6167 653d          message=
-00007530: 2244 6563 6f72 6174 6564 5465 7874 222c  "DecoratedText",
-00007540: 0a20 2020 2029 0a20 2020 2062 7574 746f  .    ).    butto
-00007550: 6e5f 6c69 7374 3a20 2242 7574 746f 6e4c  n_list: "ButtonL
-00007560: 6973 7422 203d 2070 726f 746f 2e46 6965  ist" = proto.Fie
-00007570: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
-00007580: 6f2e 4d45 5353 4147 452c 0a20 2020 2020  o.MESSAGE,.     
-00007590: 2020 206e 756d 6265 723d 342c 0a20 2020     number=4,.   
-000075a0: 2020 2020 206f 6e65 6f66 3d22 6461 7461       oneof="data
-000075b0: 222c 0a20 2020 2020 2020 206d 6573 7361  ",.        messa
-000075c0: 6765 3d22 4275 7474 6f6e 4c69 7374 222c  ge="ButtonList",
-000075d0: 0a20 2020 2029 0a20 2020 2074 6578 745f  .    ).    text_
-000075e0: 696e 7075 743a 2022 5465 7874 496e 7075  input: "TextInpu
+00006c00: 2020 2020 2268 6f72 697a 6f6e 7461 6c41      "horizontalA
+00006c10: 6c69 676e 6d65 6e74 223a 2022 4345 4e54  lignment": "CENT
+00006c20: 4552 222c 0a20 2020 2020 2020 2020 2020  ER",.           
+00006c30: 2020 2020 2020 2020 2020 2276 6572 7469            "verti
+00006c40: 6361 6c41 6c69 676e 6d65 6e74 223a 2022  calAlignment": "
+00006c50: 4345 4e54 4552 222c 0a20 2020 2020 2020  CENTER",.       
+00006c60: 2020 2020 2020 2020 2020 2020 2020 2277                "w
+00006c70: 6964 6765 7473 223a 205b 0a20 2020 2020  idgets": [.     
+00006c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c90: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
+00006ca0: 2020 2020 2020 2020 2020 2020 2022 7465               "te
+00006cb0: 7874 5061 7261 6772 6170 6822 3a20 7b0a  xtParagraph": {.
+00006cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006cd0: 2020 2020 2020 2020 2020 2022 7465 7874             "text
+00006ce0: 223a 2022 5365 636f 6e64 2063 6f6c 756d  ": "Second colum
+00006cf0: 6e20 7465 7874 2070 6172 6167 7261 7068  n text paragraph
+00006d00: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00006d10: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+00006d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d30: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
+00006d40: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
+00006d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d60: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00006d70: 2020 205d 0a20 2020 2020 2020 2020 2020     ].           
+00006d80: 2020 2020 7d0a 0a20 2020 2020 2020 2020      }..         
+00006d90: 2020 2054 6869 7320 6669 656c 6420 6973     This field is
+00006da0: 2061 206d 656d 6265 7220 6f66 2060 6f6e   a member of `on
+00006db0: 656f 6660 5f20 6060 6461 7461 6060 2e0a  eof`_ ``data``..
+00006dc0: 2020 2020 2020 2020 686f 7269 7a6f 6e74          horizont
+00006dd0: 616c 5f61 6c69 676e 6d65 6e74 2028 676f  al_alignment (go
+00006de0: 6f67 6c65 2e61 7070 732e 6361 7264 5f76  ogle.apps.card_v
+00006df0: 312e 7479 7065 732e 5769 6467 6574 2e48  1.types.Widget.H
+00006e00: 6f72 697a 6f6e 7461 6c41 6c69 676e 6d65  orizontalAlignme
+00006e10: 6e74 293a 0a20 2020 2020 2020 2020 2020  nt):.           
+00006e20: 2053 7065 6369 6669 6573 2077 6865 7468   Specifies wheth
+00006e30: 6572 2077 6964 6765 7473 2061 6c69 676e  er widgets align
+00006e40: 2074 6f20 7468 6520 6c65 6674 2c0a 2020   to the left,.  
+00006e50: 2020 2020 2020 2020 2020 7269 6768 742c            right,
+00006e60: 206f 7220 6365 6e74 6572 206f 6620 6120   or center of a 
+00006e70: 636f 6c75 6d6e 2e0a 2020 2020 2222 220a  column..    """.
+00006e80: 0a20 2020 2063 6c61 7373 2049 6d61 6765  .    class Image
+00006e90: 5479 7065 2870 726f 746f 2e45 6e75 6d29  Type(proto.Enum)
+00006ea0: 3a0a 2020 2020 2020 2020 7222 2222 5468  :.        r"""Th
+00006eb0: 6520 7368 6170 6520 7573 6564 2074 6f20  e shape used to 
+00006ec0: 6372 6f70 2074 6865 2069 6d61 6765 2e0a  crop the image..
+00006ed0: 0a20 2020 2020 2020 2060 476f 6f67 6c65  .        `Google
+00006ee0: 2057 6f72 6b73 7061 6365 2041 6464 2d6f   Workspace Add-o
+00006ef0: 6e73 2061 6e64 2043 6861 740a 2020 2020  ns and Chat.    
+00006f00: 2020 2020 6170 7073 203c 6874 7470 733a      apps <https:
+00006f10: 2f2f 6465 7665 6c6f 7065 7273 2e67 6f6f  //developers.goo
+00006f20: 676c 652e 636f 6d2f 776f 726b 7370 6163  gle.com/workspac
+00006f30: 652f 6578 7465 6e64 3e60 5f5f 3a0a 0a20  e/extend>`__:.. 
+00006f40: 2020 2020 2020 2056 616c 7565 733a 0a20         Values:. 
+00006f50: 2020 2020 2020 2020 2020 2053 5155 4152             SQUAR
+00006f60: 4520 2830 293a 0a20 2020 2020 2020 2020  E (0):.         
+00006f70: 2020 2020 2020 2044 6566 6175 6c74 2076         Default v
+00006f80: 616c 7565 2e20 4170 706c 6965 7320 6120  alue. Applies a 
+00006f90: 7371 7561 7265 206d 6173 6b20 746f 2074  square mask to t
+00006fa0: 6865 0a20 2020 2020 2020 2020 2020 2020  he.             
+00006fb0: 2020 2069 6d61 6765 2e20 466f 7220 6578     image. For ex
+00006fc0: 616d 706c 652c 2061 2034 7833 2069 6d61  ample, a 4x3 ima
+00006fd0: 6765 2062 6563 6f6d 6573 2033 7833 2e0a  ge becomes 3x3..
+00006fe0: 2020 2020 2020 2020 2020 2020 4349 5243              CIRC
+00006ff0: 4c45 2028 3129 3a0a 2020 2020 2020 2020  LE (1):.        
+00007000: 2020 2020 2020 2020 4170 706c 6965 7320          Applies 
+00007010: 6120 6369 7263 756c 6172 206d 6173 6b20  a circular mask 
+00007020: 746f 2074 6865 2069 6d61 6765 2e20 466f  to the image. Fo
+00007030: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
+00007040: 2020 6578 616d 706c 652c 2061 2034 7833    example, a 4x3
+00007050: 2069 6d61 6765 2062 6563 6f6d 6573 2061   image becomes a
+00007060: 2063 6972 636c 6520 7769 7468 2061 0a20   circle with a. 
+00007070: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00007080: 6961 6d65 7465 7220 6f66 2033 2e0a 2020  iameter of 3..  
+00007090: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000070a0: 2020 5351 5541 5245 203d 2030 0a20 2020    SQUARE = 0.   
+000070b0: 2020 2020 2043 4952 434c 4520 3d20 310a       CIRCLE = 1.
+000070c0: 0a20 2020 2063 6c61 7373 2048 6f72 697a  .    class Horiz
+000070d0: 6f6e 7461 6c41 6c69 676e 6d65 6e74 2870  ontalAlignment(p
+000070e0: 726f 746f 2e45 6e75 6d29 3a0a 2020 2020  roto.Enum):.    
+000070f0: 2020 2020 7222 2222 5370 6563 6966 6965      r"""Specifie
+00007100: 7320 7768 6574 6865 7220 7769 6467 6574  s whether widget
+00007110: 7320 616c 6967 6e20 746f 2074 6865 206c  s align to the l
+00007120: 6566 742c 2072 6967 6874 2c20 6f72 2063  eft, right, or c
+00007130: 656e 7465 7220 6f66 2061 0a20 2020 2020  enter of a.     
+00007140: 2020 2063 6f6c 756d 6e2e 0a0a 2020 2020     column...    
+00007150: 2020 2020 6047 6f6f 676c 6520 4368 6174      `Google Chat
+00007160: 2061 7070 7320 3c68 7474 7073 3a2f 2f64   apps <https://d
+00007170: 6576 656c 6f70 6572 732e 676f 6f67 6c65  evelopers.google
+00007180: 2e63 6f6d 2f77 6f72 6b73 7061 6365 2f63  .com/workspace/c
+00007190: 6861 743e 605f 5f3a 0a0a 2020 2020 2020  hat>`__:..      
+000071a0: 2020 5661 6c75 6573 3a0a 2020 2020 2020    Values:.      
+000071b0: 2020 2020 2020 484f 5249 5a4f 4e54 414c        HORIZONTAL
+000071c0: 5f41 4c49 474e 4d45 4e54 5f55 4e53 5045  _ALIGNMENT_UNSPE
+000071d0: 4349 4649 4544 2028 3029 3a0a 2020 2020  CIFIED (0):.    
+000071e0: 2020 2020 2020 2020 2020 2020 446f 6e27              Don'
+000071f0: 7420 7573 652e 2055 6e73 7065 6369 6669  t use. Unspecifi
+00007200: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
+00007210: 5354 4152 5420 2831 293a 0a20 2020 2020  START (1):.     
+00007220: 2020 2020 2020 2020 2020 2044 6566 6175             Defau
+00007230: 6c74 2076 616c 7565 2e20 416c 6967 6e73  lt value. Aligns
+00007240: 2077 6964 6765 7473 2074 6f20 7468 6520   widgets to the 
+00007250: 7374 6172 740a 2020 2020 2020 2020 2020  start.          
+00007260: 2020 2020 2020 706f 7369 7469 6f6e 206f        position o
+00007270: 6620 7468 6520 636f 6c75 6d6e 2e20 466f  f the column. Fo
+00007280: 7220 6c65 6674 2d74 6f2d 7269 6768 740a  r left-to-right.
+00007290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072a0: 6c61 796f 7574 732c 2061 6c69 676e 7320  layouts, aligns 
+000072b0: 746f 2074 6865 206c 6566 742e 2046 6f72  to the left. For
+000072c0: 2072 6967 6874 2d74 6f2d 6c65 6674 0a20   right-to-left. 
+000072d0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+000072e0: 6179 6f75 7473 2c20 616c 6967 6e73 2074  ayouts, aligns t
+000072f0: 6f20 7468 6520 7269 6768 742e 0a20 2020  o the right..   
+00007300: 2020 2020 2020 2020 2043 454e 5445 5220           CENTER 
+00007310: 2832 293a 0a20 2020 2020 2020 2020 2020  (2):.           
+00007320: 2020 2020 2041 6c69 676e 7320 7769 6467       Aligns widg
+00007330: 6574 7320 746f 2074 6865 2063 656e 7465  ets to the cente
+00007340: 7220 6f66 2074 6865 2063 6f6c 756d 6e2e  r of the column.
+00007350: 0a20 2020 2020 2020 2020 2020 2045 4e44  .            END
+00007360: 2028 3329 3a0a 2020 2020 2020 2020 2020   (3):.          
+00007370: 2020 2020 2020 416c 6967 6e73 2077 6964        Aligns wid
+00007380: 6765 7473 2074 6f20 7468 6520 656e 6420  gets to the end 
+00007390: 706f 7369 7469 6f6e 206f 6620 7468 650a  position of the.
+000073a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000073b0: 636f 6c75 6d6e 2e20 466f 7220 6c65 6674  column. For left
+000073c0: 2d74 6f2d 7269 6768 7420 6c61 796f 7574  -to-right layout
+000073d0: 732c 2061 6c69 676e 730a 2020 2020 2020  s, aligns.      
+000073e0: 2020 2020 2020 2020 2020 7769 6467 6574            widget
+000073f0: 7320 746f 2074 6865 2072 6967 6874 2e20  s to the right. 
+00007400: 466f 7220 7269 6768 742d 746f 2d6c 6566  For right-to-lef
+00007410: 7420 6c61 796f 7574 732c 0a20 2020 2020  t layouts,.     
+00007420: 2020 2020 2020 2020 2020 2061 6c69 676e             align
+00007430: 7320 7769 6467 6574 7320 746f 2074 6865  s widgets to the
+00007440: 206c 6566 742e 0a20 2020 2020 2020 2022   left..        "
+00007450: 2222 0a20 2020 2020 2020 2048 4f52 495a  "".        HORIZ
+00007460: 4f4e 5441 4c5f 414c 4947 4e4d 454e 545f  ONTAL_ALIGNMENT_
+00007470: 554e 5350 4543 4946 4945 4420 3d20 300a  UNSPECIFIED = 0.
+00007480: 2020 2020 2020 2020 5354 4152 5420 3d20          START = 
+00007490: 310a 2020 2020 2020 2020 4345 4e54 4552  1.        CENTER
+000074a0: 203d 2032 0a20 2020 2020 2020 2045 4e44   = 2.        END
+000074b0: 203d 2033 0a0a 2020 2020 7465 7874 5f70   = 3..    text_p
+000074c0: 6172 6167 7261 7068 3a20 2254 6578 7450  aragraph: "TextP
+000074d0: 6172 6167 7261 7068 2220 3d20 7072 6f74  aragraph" = prot
+000074e0: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+000074f0: 2070 726f 746f 2e4d 4553 5341 4745 2c0a   proto.MESSAGE,.
+00007500: 2020 2020 2020 2020 6e75 6d62 6572 3d31          number=1
+00007510: 2c0a 2020 2020 2020 2020 6f6e 656f 663d  ,.        oneof=
+00007520: 2264 6174 6122 2c0a 2020 2020 2020 2020  "data",.        
+00007530: 6d65 7373 6167 653d 2254 6578 7450 6172  message="TextPar
+00007540: 6167 7261 7068 222c 0a20 2020 2029 0a20  agraph",.    ). 
+00007550: 2020 2069 6d61 6765 3a20 2249 6d61 6765     image: "Image
+00007560: 2220 3d20 7072 6f74 6f2e 4669 656c 6428  " = proto.Field(
+00007570: 0a20 2020 2020 2020 2070 726f 746f 2e4d  .        proto.M
+00007580: 4553 5341 4745 2c0a 2020 2020 2020 2020  ESSAGE,.        
+00007590: 6e75 6d62 6572 3d32 2c0a 2020 2020 2020  number=2,.      
+000075a0: 2020 6f6e 656f 663d 2264 6174 6122 2c0a    oneof="data",.
+000075b0: 2020 2020 2020 2020 6d65 7373 6167 653d          message=
+000075c0: 2249 6d61 6765 222c 0a20 2020 2029 0a20  "Image",.    ). 
+000075d0: 2020 2064 6563 6f72 6174 6564 5f74 6578     decorated_tex
+000075e0: 743a 2022 4465 636f 7261 7465 6454 6578  t: "DecoratedTex
 000075f0: 7422 203d 2070 726f 746f 2e46 6965 6c64  t" = proto.Field
 00007600: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
 00007610: 4d45 5353 4147 452c 0a20 2020 2020 2020  MESSAGE,.       
-00007620: 206e 756d 6265 723d 352c 0a20 2020 2020   number=5,.     
+00007620: 206e 756d 6265 723d 332c 0a20 2020 2020   number=3,.     
 00007630: 2020 206f 6e65 6f66 3d22 6461 7461 222c     oneof="data",
 00007640: 0a20 2020 2020 2020 206d 6573 7361 6765  .        message
-00007650: 3d22 5465 7874 496e 7075 7422 2c0a 2020  ="TextInput",.  
-00007660: 2020 290a 2020 2020 7365 6c65 6374 696f    ).    selectio
-00007670: 6e5f 696e 7075 743a 2022 5365 6c65 6374  n_input: "Select
-00007680: 696f 6e49 6e70 7574 2220 3d20 7072 6f74  ionInput" = prot
-00007690: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-000076a0: 2070 726f 746f 2e4d 4553 5341 4745 2c0a   proto.MESSAGE,.
-000076b0: 2020 2020 2020 2020 6e75 6d62 6572 3d36          number=6
-000076c0: 2c0a 2020 2020 2020 2020 6f6e 656f 663d  ,.        oneof=
-000076d0: 2264 6174 6122 2c0a 2020 2020 2020 2020  "data",.        
-000076e0: 6d65 7373 6167 653d 2253 656c 6563 7469  message="Selecti
-000076f0: 6f6e 496e 7075 7422 2c0a 2020 2020 290a  onInput",.    ).
-00007700: 2020 2020 6461 7465 5f74 696d 655f 7069      date_time_pi
-00007710: 636b 6572 3a20 2244 6174 6554 696d 6550  cker: "DateTimeP
-00007720: 6963 6b65 7222 203d 2070 726f 746f 2e46  icker" = proto.F
-00007730: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
-00007740: 6f74 6f2e 4d45 5353 4147 452c 0a20 2020  oto.MESSAGE,.   
-00007750: 2020 2020 206e 756d 6265 723d 372c 0a20       number=7,. 
-00007760: 2020 2020 2020 206f 6e65 6f66 3d22 6461         oneof="da
-00007770: 7461 222c 0a20 2020 2020 2020 206d 6573  ta",.        mes
-00007780: 7361 6765 3d22 4461 7465 5469 6d65 5069  sage="DateTimePi
-00007790: 636b 6572 222c 0a20 2020 2029 0a20 2020  cker",.    ).   
-000077a0: 2064 6976 6964 6572 3a20 2244 6976 6964   divider: "Divid
-000077b0: 6572 2220 3d20 7072 6f74 6f2e 4669 656c  er" = proto.Fiel
-000077c0: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
-000077d0: 2e4d 4553 5341 4745 2c0a 2020 2020 2020  .MESSAGE,.      
-000077e0: 2020 6e75 6d62 6572 3d39 2c0a 2020 2020    number=9,.    
-000077f0: 2020 2020 6f6e 656f 663d 2264 6174 6122      oneof="data"
-00007800: 2c0a 2020 2020 2020 2020 6d65 7373 6167  ,.        messag
-00007810: 653d 2244 6976 6964 6572 222c 0a20 2020  e="Divider",.   
-00007820: 2029 0a20 2020 2067 7269 643a 2022 4772   ).    grid: "Gr
-00007830: 6964 2220 3d20 7072 6f74 6f2e 4669 656c  id" = proto.Fiel
-00007840: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
-00007850: 2e4d 4553 5341 4745 2c0a 2020 2020 2020  .MESSAGE,.      
-00007860: 2020 6e75 6d62 6572 3d31 302c 0a20 2020    number=10,.   
-00007870: 2020 2020 206f 6e65 6f66 3d22 6461 7461       oneof="data
-00007880: 222c 0a20 2020 2020 2020 206d 6573 7361  ",.        messa
-00007890: 6765 3d22 4772 6964 222c 0a20 2020 2029  ge="Grid",.    )
-000078a0: 0a20 2020 2063 6f6c 756d 6e73 3a20 2243  .    columns: "C
-000078b0: 6f6c 756d 6e73 2220 3d20 7072 6f74 6f2e  olumns" = proto.
-000078c0: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
-000078d0: 726f 746f 2e4d 4553 5341 4745 2c0a 2020  roto.MESSAGE,.  
-000078e0: 2020 2020 2020 6e75 6d62 6572 3d31 312c        number=11,
-000078f0: 0a20 2020 2020 2020 206f 6e65 6f66 3d22  .        oneof="
-00007900: 6461 7461 222c 0a20 2020 2020 2020 206d  data",.        m
-00007910: 6573 7361 6765 3d22 436f 6c75 6d6e 7322  essage="Columns"
-00007920: 2c0a 2020 2020 290a 2020 2020 686f 7269  ,.    ).    hori
-00007930: 7a6f 6e74 616c 5f61 6c69 676e 6d65 6e74  zontal_alignment
-00007940: 3a20 486f 7269 7a6f 6e74 616c 416c 6967  : HorizontalAlig
-00007950: 6e6d 656e 7420 3d20 7072 6f74 6f2e 4669  nment = proto.Fi
-00007960: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
-00007970: 746f 2e45 4e55 4d2c 0a20 2020 2020 2020  to.ENUM,.       
-00007980: 206e 756d 6265 723d 382c 0a20 2020 2020   number=8,.     
-00007990: 2020 2065 6e75 6d3d 486f 7269 7a6f 6e74     enum=Horizont
-000079a0: 616c 416c 6967 6e6d 656e 742c 0a20 2020  alAlignment,.   
-000079b0: 2029 0a0a 0a63 6c61 7373 2054 6578 7450   )...class TextP
-000079c0: 6172 6167 7261 7068 2870 726f 746f 2e4d  aragraph(proto.M
-000079d0: 6573 7361 6765 293a 0a20 2020 2072 2222  essage):.    r""
-000079e0: 2241 2070 6172 6167 7261 7068 206f 6620  "A paragraph of 
-000079f0: 7465 7874 2074 6861 7420 7375 7070 6f72  text that suppor
-00007a00: 7473 2066 6f72 6d61 7474 696e 672e 2046  ts formatting. F
-00007a10: 6f72 2061 6e20 6578 616d 706c 6520 696e  or an example in
-00007a20: 0a20 2020 2047 6f6f 676c 6520 4368 6174  .    Google Chat
-00007a30: 2061 7070 732c 2073 6565 2060 5465 7874   apps, see `Text
-00007a40: 0a20 2020 2070 6172 6167 7261 7068 203c  .    paragraph <
-00007a50: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
-00007a60: 7273 2e67 6f6f 676c 652e 636f 6d2f 6368  rs.google.com/ch
-00007a70: 6174 2f75 692f 7769 6467 6574 732f 7465  at/ui/widgets/te
-00007a80: 7874 2d70 6172 6167 7261 7068 3e60 5f5f  xt-paragraph>`__
-00007a90: 2e0a 2020 2020 466f 7220 6d6f 7265 2069  ..    For more i
-00007aa0: 6e66 6f72 6d61 7469 6f6e 2061 626f 7574  nformation about
-00007ab0: 2066 6f72 6d61 7474 696e 6720 7465 7874   formatting text
-00007ac0: 2c20 7365 6520 6046 6f72 6d61 7474 696e  , see `Formattin
-00007ad0: 6720 7465 7874 2069 6e0a 2020 2020 476f  g text in.    Go
-00007ae0: 6f67 6c65 2043 6861 740a 2020 2020 6170  ogle Chat.    ap
-00007af0: 7073 203c 6874 7470 733a 2f2f 6465 7665  ps <https://deve
-00007b00: 6c6f 7065 7273 2e67 6f6f 676c 652e 636f  lopers.google.co
-00007b10: 6d2f 6368 6174 2f66 6f72 6d61 742d 6d65  m/chat/format-me
-00007b20: 7373 6167 6573 2363 6172 642d 666f 726d  ssages#card-form
-00007b30: 6174 7469 6e67 3e60 5f5f 0a20 2020 2061  atting>`__.    a
-00007b40: 6e64 2060 466f 726d 6174 7469 6e67 2074  nd `Formatting t
-00007b50: 6578 7420 696e 2047 6f6f 676c 6520 576f  ext in Google Wo
-00007b60: 726b 7370 6163 650a 2020 2020 4164 642d  rkspace.    Add-
-00007b70: 6f6e 7320 3c68 7474 7073 3a2f 2f64 6576  ons <https://dev
-00007b80: 656c 6f70 6572 732e 676f 6f67 6c65 2e63  elopers.google.c
-00007b90: 6f6d 2f61 7070 732d 7363 7269 7074 2f61  om/apps-script/a
-00007ba0: 6464 2d6f 6e73 2f63 6f6e 6365 7074 732f  dd-ons/concepts/
-00007bb0: 7769 6467 6574 7323 7465 7874 5f66 6f72  widgets#text_for
-00007bc0: 6d61 7474 696e 673e 605f 5f2e 0a0a 2020  matting>`__...  
-00007bd0: 2020 6047 6f6f 676c 6520 576f 726b 7370    `Google Worksp
-00007be0: 6163 6520 4164 642d 6f6e 7320 616e 6420  ace Add-ons and 
-00007bf0: 4368 6174 0a20 2020 2061 7070 7320 3c68  Chat.    apps <h
-00007c00: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
-00007c10: 732e 676f 6f67 6c65 2e63 6f6d 2f77 6f72  s.google.com/wor
-00007c20: 6b73 7061 6365 2f65 7874 656e 643e 605f  kspace/extend>`_
-00007c30: 5f3a 0a0a 2020 2020 4174 7472 6962 7574  _:..    Attribut
-00007c40: 6573 3a0a 2020 2020 2020 2020 7465 7874  es:.        text
-00007c50: 2028 7374 7229 3a0a 2020 2020 2020 2020   (str):.        
-00007c60: 2020 2020 5468 6520 7465 7874 2074 6861      The text tha
-00007c70: 7427 7320 7368 6f77 6e20 696e 2074 6865  t's shown in the
-00007c80: 2077 6964 6765 742e 0a20 2020 2022 2222   widget..    """
-00007c90: 0a0a 2020 2020 7465 7874 3a20 7374 7220  ..    text: str 
-00007ca0: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
-00007cb0: 2020 2020 2020 2070 726f 746f 2e53 5452         proto.STR
-00007cc0: 494e 472c 0a20 2020 2020 2020 206e 756d  ING,.        num
-00007cd0: 6265 723d 312c 0a20 2020 2029 0a0a 0a63  ber=1,.    )...c
-00007ce0: 6c61 7373 2049 6d61 6765 2870 726f 746f  lass Image(proto
-00007cf0: 2e4d 6573 7361 6765 293a 0a20 2020 2072  .Message):.    r
-00007d00: 2222 2241 6e20 696d 6167 6520 7468 6174  """An image that
-00007d10: 2069 7320 7370 6563 6966 6965 6420 6279   is specified by
-00007d20: 2061 2055 524c 2061 6e64 2063 616e 2068   a URL and can h
-00007d30: 6176 6520 616e 2060 606f 6e43 6c69 636b  ave an ``onClick
-00007d40: 6060 0a20 2020 2061 6374 696f 6e2e 2046  ``.    action. F
-00007d50: 6f72 2061 6e20 6578 616d 706c 652c 2073  or an example, s
-00007d60: 6565 0a20 2020 2060 496d 6167 6520 3c68  ee.    `Image <h
-00007d70: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
-00007d80: 732e 676f 6f67 6c65 2e63 6f6d 2f63 6861  s.google.com/cha
-00007d90: 742f 7569 2f77 6964 6765 7473 2f69 6d61  t/ui/widgets/ima
-00007da0: 6765 3e60 5f5f 2e0a 0a20 2020 2060 476f  ge>`__...    `Go
-00007db0: 6f67 6c65 2057 6f72 6b73 7061 6365 2041  ogle Workspace A
-00007dc0: 6464 2d6f 6e73 2061 6e64 2043 6861 740a  dd-ons and Chat.
-00007dd0: 2020 2020 6170 7073 203c 6874 7470 733a      apps <https:
-00007de0: 2f2f 6465 7665 6c6f 7065 7273 2e67 6f6f  //developers.goo
-00007df0: 676c 652e 636f 6d2f 776f 726b 7370 6163  gle.com/workspac
-00007e00: 652f 6578 7465 6e64 3e60 5f5f 3a0a 0a20  e/extend>`__:.. 
-00007e10: 2020 2041 7474 7269 6275 7465 733a 0a20     Attributes:. 
-00007e20: 2020 2020 2020 2069 6d61 6765 5f75 726c         image_url
-00007e30: 2028 7374 7229 3a0a 2020 2020 2020 2020   (str):.        
-00007e40: 2020 2020 5468 6520 4854 5450 5320 5552      The HTTPS UR
-00007e50: 4c20 7468 6174 2068 6f73 7473 2074 6865  L that hosts the
-00007e60: 2069 6d61 6765 2e0a 0a20 2020 2020 2020   image...       
-00007e70: 2020 2020 2046 6f72 2065 7861 6d70 6c65       For example
-00007e80: 3a0a 0a20 2020 2020 2020 2020 2020 203a  :..            :
-00007e90: 3a0a 0a20 2020 2020 2020 2020 2020 2020  :..             
-00007ea0: 2020 6874 7470 733a 2f2f 6465 7665 6c6f    https://develo
-00007eb0: 7065 7273 2e67 6f6f 676c 652e 636f 6d2f  pers.google.com/
-00007ec0: 6368 6174 2f69 6d61 6765 732f 7175 6963  chat/images/quic
-00007ed0: 6b73 7461 7274 2d61 7070 2d61 7661 7461  kstart-app-avata
-00007ee0: 722e 706e 670a 2020 2020 2020 2020 6f6e  r.png.        on
-00007ef0: 5f63 6c69 636b 2028 676f 6f67 6c65 2e61  _click (google.a
-00007f00: 7070 732e 6361 7264 5f76 312e 7479 7065  pps.card_v1.type
-00007f10: 732e 4f6e 436c 6963 6b29 3a0a 2020 2020  s.OnClick):.    
-00007f20: 2020 2020 2020 2020 5768 656e 2061 2075          When a u
-00007f30: 7365 7220 636c 6963 6b73 2074 6865 2069  ser clicks the i
-00007f40: 6d61 6765 2c20 7468 6520 636c 6963 6b0a  mage, the click.
-00007f50: 2020 2020 2020 2020 2020 2020 7472 6967              trig
-00007f60: 6765 7273 2074 6869 7320 6163 7469 6f6e  gers this action
-00007f70: 2e0a 2020 2020 2020 2020 616c 745f 7465  ..        alt_te
-00007f80: 7874 2028 7374 7229 3a0a 2020 2020 2020  xt (str):.      
-00007f90: 2020 2020 2020 5468 6520 616c 7465 726e        The altern
-00007fa0: 6174 6976 6520 7465 7874 206f 6620 7468  ative text of th
-00007fb0: 6973 2069 6d61 6765 2074 6861 7427 730a  is image that's.
-00007fc0: 2020 2020 2020 2020 2020 2020 7573 6564              used
-00007fd0: 2066 6f72 2061 6363 6573 7369 6269 6c69   for accessibili
-00007fe0: 7479 2e0a 2020 2020 2222 220a 0a20 2020  ty..    """..   
-00007ff0: 2069 6d61 6765 5f75 726c 3a20 7374 7220   image_url: str 
-00008000: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
-00008010: 2020 2020 2020 2070 726f 746f 2e53 5452         proto.STR
-00008020: 494e 472c 0a20 2020 2020 2020 206e 756d  ING,.        num
-00008030: 6265 723d 312c 0a20 2020 2029 0a20 2020  ber=1,.    ).   
-00008040: 206f 6e5f 636c 6963 6b3a 2022 4f6e 436c   on_click: "OnCl
-00008050: 6963 6b22 203d 2070 726f 746f 2e46 6965  ick" = proto.Fie
-00008060: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
-00008070: 6f2e 4d45 5353 4147 452c 0a20 2020 2020  o.MESSAGE,.     
-00008080: 2020 206e 756d 6265 723d 322c 0a20 2020     number=2,.   
-00008090: 2020 2020 206d 6573 7361 6765 3d22 4f6e       message="On
-000080a0: 436c 6963 6b22 2c0a 2020 2020 290a 2020  Click",.    ).  
-000080b0: 2020 616c 745f 7465 7874 3a20 7374 7220    alt_text: str 
-000080c0: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
-000080d0: 2020 2020 2020 2070 726f 746f 2e53 5452         proto.STR
-000080e0: 494e 472c 0a20 2020 2020 2020 206e 756d  ING,.        num
-000080f0: 6265 723d 332c 0a20 2020 2029 0a0a 0a63  ber=3,.    )...c
-00008100: 6c61 7373 2044 6976 6964 6572 2870 726f  lass Divider(pro
-00008110: 746f 2e4d 6573 7361 6765 293a 0a20 2020  to.Message):.   
-00008120: 2072 2222 2244 6973 706c 6179 7320 6120   r"""Displays a 
-00008130: 6469 7669 6465 7220 6265 7477 6565 6e20  divider between 
-00008140: 7769 6467 6574 7320 6173 2061 2068 6f72  widgets as a hor
-00008150: 697a 6f6e 7461 6c20 6c69 6e65 2e20 466f  izontal line. Fo
-00008160: 7220 616e 0a20 2020 2065 7861 6d70 6c65  r an.    example
-00008170: 2069 6e20 476f 6f67 6c65 2043 6861 7420   in Google Chat 
-00008180: 6170 7073 2c20 7365 650a 2020 2020 6044  apps, see.    `D
-00008190: 6976 6964 6572 203c 6874 7470 733a 2f2f  ivider <https://
-000081a0: 6465 7665 6c6f 7065 7273 2e67 6f6f 676c  developers.googl
-000081b0: 652e 636f 6d2f 6368 6174 2f75 692f 7769  e.com/chat/ui/wi
-000081c0: 6467 6574 732f 6469 7669 6465 723e 605f  dgets/divider>`_
-000081d0: 5f2e 0a0a 2020 2020 6047 6f6f 676c 6520  _...    `Google 
-000081e0: 576f 726b 7370 6163 6520 4164 642d 6f6e  Workspace Add-on
-000081f0: 7320 616e 6420 4368 6174 0a20 2020 2061  s and Chat.    a
-00008200: 7070 7320 3c68 7474 7073 3a2f 2f64 6576  pps <https://dev
-00008210: 656c 6f70 6572 732e 676f 6f67 6c65 2e63  elopers.google.c
-00008220: 6f6d 2f77 6f72 6b73 7061 6365 2f65 7874  om/workspace/ext
-00008230: 656e 643e 605f 5f3a 0a0a 2020 2020 466f  end>`__:..    Fo
-00008240: 7220 6578 616d 706c 652c 2074 6865 2066  r example, the f
-00008250: 6f6c 6c6f 7769 6e67 204a 534f 4e20 6372  ollowing JSON cr
-00008260: 6561 7465 7320 6120 6469 7669 6465 723a  eates a divider:
-00008270: 0a0a 2020 2020 3a3a 0a0a 2020 2020 2020  ..    ::..      
-00008280: 2022 6469 7669 6465 7222 3a20 7b7d 0a0a   "divider": {}..
-00008290: 2020 2020 2222 220a 0a0a 636c 6173 7320      """...class 
-000082a0: 4465 636f 7261 7465 6454 6578 7428 7072  DecoratedText(pr
-000082b0: 6f74 6f2e 4d65 7373 6167 6529 3a0a 2020  oto.Message):.  
-000082c0: 2020 7222 2222 4120 7769 6467 6574 2074    r"""A widget t
-000082d0: 6861 7420 6469 7370 6c61 7973 2074 6578  hat displays tex
-000082e0: 7420 7769 7468 206f 7074 696f 6e61 6c20  t with optional 
-000082f0: 6465 636f 7261 7469 6f6e 7320 7375 6368  decorations such
-00008300: 2061 7320 610a 2020 2020 6c61 6265 6c20   as a.    label 
-00008310: 6162 6f76 6520 6f72 2062 656c 6f77 2074  above or below t
-00008320: 6865 2074 6578 742c 2061 6e20 6963 6f6e  he text, an icon
-00008330: 2069 6e20 6672 6f6e 7420 6f66 2074 6865   in front of the
-00008340: 2074 6578 742c 2061 0a20 2020 2073 656c   text, a.    sel
-00008350: 6563 7469 6f6e 2077 6964 6765 742c 206f  ection widget, o
-00008360: 7220 6120 6275 7474 6f6e 2061 6674 6572  r a button after
-00008370: 2074 6865 2074 6578 742e 2046 6f72 2061   the text. For a
-00008380: 6e20 6578 616d 706c 6520 696e 0a20 2020  n example in.   
-00008390: 2047 6f6f 676c 6520 4368 6174 2061 7070   Google Chat app
-000083a0: 732c 2073 6565 2060 4465 636f 7261 7465  s, see `Decorate
-000083b0: 640a 2020 2020 7465 7874 203c 6874 7470  d.    text <http
-000083c0: 733a 2f2f 6465 7665 6c6f 7065 7273 2e67  s://developers.g
-000083d0: 6f6f 676c 652e 636f 6d2f 6368 6174 2f75  oogle.com/chat/u
-000083e0: 692f 7769 6467 6574 732f 6465 636f 7261  i/widgets/decora
-000083f0: 7465 642d 7465 7874 3e60 5f5f 2e0a 0a20  ted-text>`__... 
-00008400: 2020 2060 476f 6f67 6c65 2057 6f72 6b73     `Google Works
-00008410: 7061 6365 2041 6464 2d6f 6e73 2061 6e64  pace Add-ons and
-00008420: 2043 6861 740a 2020 2020 6170 7073 203c   Chat.    apps <
-00008430: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
-00008440: 7273 2e67 6f6f 676c 652e 636f 6d2f 776f  rs.google.com/wo
-00008450: 726b 7370 6163 652f 6578 7465 6e64 3e60  rkspace/extend>`
-00008460: 5f5f 3a0a 0a20 2020 2054 6869 7320 6d65  __:..    This me
-00008470: 7373 6167 6520 6861 7320 606f 6e65 6f66  ssage has `oneof
-00008480: 605f 2066 6965 6c64 7320 286d 7574 7561  `_ fields (mutua
-00008490: 6c6c 7920 6578 636c 7573 6976 6520 6669  lly exclusive fi
-000084a0: 656c 6473 292e 0a20 2020 2046 6f72 2065  elds)..    For e
-000084b0: 6163 6820 6f6e 656f 662c 2061 7420 6d6f  ach oneof, at mo
-000084c0: 7374 206f 6e65 206d 656d 6265 7220 6669  st one member fi
-000084d0: 656c 6420 6361 6e20 6265 2073 6574 2061  eld can be set a
-000084e0: 7420 7468 6520 7361 6d65 2074 696d 652e  t the same time.
-000084f0: 0a20 2020 2053 6574 7469 6e67 2061 6e79  .    Setting any
-00008500: 206d 656d 6265 7220 6f66 2074 6865 206f   member of the o
-00008510: 6e65 6f66 2061 7574 6f6d 6174 6963 616c  neof automatical
-00008520: 6c79 2063 6c65 6172 7320 616c 6c20 6f74  ly clears all ot
-00008530: 6865 720a 2020 2020 6d65 6d62 6572 732e  her.    members.
-00008540: 0a0a 2020 2020 2e2e 205f 6f6e 656f 663a  ..    .. _oneof:
-00008550: 2068 7474 7073 3a2f 2f70 726f 746f 2d70   https://proto-p
-00008560: 6c75 732d 7079 7468 6f6e 2e72 6561 6474  lus-python.readt
-00008570: 6865 646f 6373 2e69 6f2f 656e 2f73 7461  hedocs.io/en/sta
-00008580: 626c 652f 6669 656c 6473 2e68 746d 6c23  ble/fields.html#
-00008590: 6f6e 656f 6673 2d6d 7574 7561 6c6c 792d  oneofs-mutually-
-000085a0: 6578 636c 7573 6976 652d 6669 656c 6473  exclusive-fields
-000085b0: 0a0a 2020 2020 4174 7472 6962 7574 6573  ..    Attributes
-000085c0: 3a0a 2020 2020 2020 2020 6963 6f6e 2028  :.        icon (
-000085d0: 676f 6f67 6c65 2e61 7070 732e 6361 7264  google.apps.card
-000085e0: 5f76 312e 7479 7065 732e 4963 6f6e 293a  _v1.types.Icon):
-000085f0: 0a20 2020 2020 2020 2020 2020 2044 6570  .            Dep
-00008600: 7265 6361 7465 6420 696e 2066 6176 6f72  recated in favor
-00008610: 206f 6620 6060 7374 6172 7449 636f 6e60   of ``startIcon`
-00008620: 602e 0a20 2020 2020 2020 2073 7461 7274  `..        start
-00008630: 5f69 636f 6e20 2867 6f6f 676c 652e 6170  _icon (google.ap
-00008640: 7073 2e63 6172 645f 7631 2e74 7970 6573  ps.card_v1.types
-00008650: 2e49 636f 6e29 3a0a 2020 2020 2020 2020  .Icon):.        
-00008660: 2020 2020 5468 6520 6963 6f6e 2064 6973      The icon dis
-00008670: 706c 6179 6564 2069 6e20 6672 6f6e 7420  played in front 
-00008680: 6f66 2074 6865 2074 6578 742e 0a20 2020  of the text..   
-00008690: 2020 2020 2074 6f70 5f6c 6162 656c 2028       top_label (
-000086a0: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
-000086b0: 2020 5468 6520 7465 7874 2074 6861 7420    The text that 
-000086c0: 6170 7065 6172 7320 6162 6f76 6520 6060  appears above ``
-000086d0: 7465 7874 6060 2e20 416c 7761 7973 2074  text``. Always t
-000086e0: 7275 6e63 6174 6573 2e0a 2020 2020 2020  runcates..      
-000086f0: 2020 7465 7874 2028 7374 7229 3a0a 2020    text (str):.  
-00008700: 2020 2020 2020 2020 2020 5265 7175 6972            Requir
-00008710: 6564 2e20 5468 6520 7072 696d 6172 7920  ed. The primary 
-00008720: 7465 7874 2e0a 0a20 2020 2020 2020 2020  text...         
-00008730: 2020 2053 7570 706f 7274 7320 7369 6d70     Supports simp
-00008740: 6c65 2066 6f72 6d61 7474 696e 672e 2046  le formatting. F
-00008750: 6f72 206d 6f72 6520 696e 666f 726d 6174  or more informat
-00008760: 696f 6e20 6162 6f75 740a 2020 2020 2020  ion about.      
-00008770: 2020 2020 2020 666f 726d 6174 7469 6e67        formatting
-00008780: 2074 6578 742c 2073 6565 2060 466f 726d   text, see `Form
-00008790: 6174 7469 6e67 2074 6578 7420 696e 2047  atting text in G
-000087a0: 6f6f 676c 6520 4368 6174 0a20 2020 2020  oogle Chat.     
-000087b0: 2020 2020 2020 2061 7070 7320 3c68 7474         apps <htt
-000087c0: 7073 3a2f 2f64 6576 656c 6f70 6572 732e  ps://developers.
-000087d0: 676f 6f67 6c65 2e63 6f6d 2f63 6861 742f  google.com/chat/
-000087e0: 666f 726d 6174 2d6d 6573 7361 6765 7323  format-messages#
-000087f0: 6361 7264 2d66 6f72 6d61 7474 696e 673e  card-formatting>
-00008800: 605f 5f0a 2020 2020 2020 2020 2020 2020  `__.            
-00008810: 616e 6420 6046 6f72 6d61 7474 696e 6720  and `Formatting 
-00008820: 7465 7874 2069 6e20 476f 6f67 6c65 2057  text in Google W
-00008830: 6f72 6b73 7061 6365 0a20 2020 2020 2020  orkspace.       
-00008840: 2020 2020 2041 6464 2d6f 6e73 203c 6874       Add-ons <ht
-00008850: 7470 733a 2f2f 6465 7665 6c6f 7065 7273  tps://developers
-00008860: 2e67 6f6f 676c 652e 636f 6d2f 6170 7073  .google.com/apps
-00008870: 2d73 6372 6970 742f 6164 642d 6f6e 732f  -script/add-ons/
-00008880: 636f 6e63 6570 7473 2f77 6964 6765 7473  concepts/widgets
-00008890: 2374 6578 745f 666f 726d 6174 7469 6e67  #text_formatting
-000088a0: 3e60 5f5f 2e0a 2020 2020 2020 2020 7772  >`__..        wr
-000088b0: 6170 5f74 6578 7420 2862 6f6f 6c29 3a0a  ap_text (bool):.
-000088c0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-000088d0: 7772 6170 2074 6578 7420 7365 7474 696e  wrap text settin
-000088e0: 672e 2049 6620 6060 7472 7565 6060 2c20  g. If ``true``, 
-000088f0: 7468 6520 7465 7874 2077 7261 7073 2061  the text wraps a
-00008900: 6e64 0a20 2020 2020 2020 2020 2020 2064  nd.            d
-00008910: 6973 706c 6179 7320 6f6e 206d 756c 7469  isplays on multi
-00008920: 706c 6520 6c69 6e65 732e 204f 7468 6572  ple lines. Other
-00008930: 7769 7365 2c20 7468 6520 7465 7874 2069  wise, the text i
-00008940: 730a 2020 2020 2020 2020 2020 2020 7472  s.            tr
-00008950: 756e 6361 7465 642e 0a0a 2020 2020 2020  uncated...      
-00008960: 2020 2020 2020 4f6e 6c79 2061 7070 6c69        Only appli
-00008970: 6573 2074 6f20 6060 7465 7874 6060 2c20  es to ``text``, 
-00008980: 6e6f 7420 6060 746f 704c 6162 656c 6060  not ``topLabel``
-00008990: 2061 6e64 0a20 2020 2020 2020 2020 2020   and.           
-000089a0: 2060 6062 6f74 746f 6d4c 6162 656c 6060   ``bottomLabel``
-000089b0: 2e0a 2020 2020 2020 2020 626f 7474 6f6d  ..        bottom
-000089c0: 5f6c 6162 656c 2028 7374 7229 3a0a 2020  _label (str):.  
-000089d0: 2020 2020 2020 2020 2020 5468 6520 7465            The te
-000089e0: 7874 2074 6861 7420 6170 7065 6172 7320  xt that appears 
-000089f0: 6265 6c6f 7720 6060 7465 7874 6060 2e20  below ``text``. 
-00008a00: 416c 7761 7973 2077 7261 7073 2e0a 2020  Always wraps..  
-00008a10: 2020 2020 2020 6f6e 5f63 6c69 636b 2028        on_click (
-00008a20: 676f 6f67 6c65 2e61 7070 732e 6361 7264  google.apps.card
-00008a30: 5f76 312e 7479 7065 732e 4f6e 436c 6963  _v1.types.OnClic
-00008a40: 6b29 3a0a 2020 2020 2020 2020 2020 2020  k):.            
-00008a50: 5468 6973 2061 6374 696f 6e20 6973 2074  This action is t
-00008a60: 7269 6767 6572 6564 2077 6865 6e20 7573  riggered when us
-00008a70: 6572 7320 636c 6963 6b20 6060 746f 704c  ers click ``topL
-00008a80: 6162 656c 6060 206f 720a 2020 2020 2020  abel`` or.      
-00008a90: 2020 2020 2020 6060 626f 7474 6f6d 4c61        ``bottomLa
-00008aa0: 6265 6c60 602e 0a20 2020 2020 2020 2062  bel``..        b
-00008ab0: 7574 746f 6e20 2867 6f6f 676c 652e 6170  utton (google.ap
-00008ac0: 7073 2e63 6172 645f 7631 2e74 7970 6573  ps.card_v1.types
-00008ad0: 2e42 7574 746f 6e29 3a0a 2020 2020 2020  .Button):.      
-00008ae0: 2020 2020 2020 4120 6275 7474 6f6e 2074        A button t
-00008af0: 6861 7420 6120 7573 6572 2063 616e 2063  hat a user can c
-00008b00: 6c69 636b 2074 6f20 7472 6967 6765 7220  lick to trigger 
-00008b10: 616e 0a20 2020 2020 2020 2020 2020 2061  an.            a
-00008b20: 6374 696f 6e2e 0a0a 2020 2020 2020 2020  ction...        
-00008b30: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
-00008b40: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
-00008b50: 6e65 6f66 605f 2060 6063 6f6e 7472 6f6c  neof`_ ``control
-00008b60: 6060 2e0a 2020 2020 2020 2020 7377 6974  ``..        swit
-00008b70: 6368 5f63 6f6e 7472 6f6c 2028 676f 6f67  ch_control (goog
-00008b80: 6c65 2e61 7070 732e 6361 7264 5f76 312e  le.apps.card_v1.
-00008b90: 7479 7065 732e 4465 636f 7261 7465 6454  types.DecoratedT
-00008ba0: 6578 742e 5377 6974 6368 436f 6e74 726f  ext.SwitchContro
-00008bb0: 6c29 3a0a 2020 2020 2020 2020 2020 2020  l):.            
-00008bc0: 4120 7377 6974 6368 2077 6964 6765 7420  A switch widget 
-00008bd0: 7468 6174 2061 2075 7365 7220 6361 6e20  that a user can 
-00008be0: 636c 6963 6b20 746f 0a20 2020 2020 2020  click to.       
-00008bf0: 2020 2020 2063 6861 6e67 6520 6974 7320       change its 
-00008c00: 7374 6174 6520 616e 6420 7472 6967 6765  state and trigge
-00008c10: 7220 616e 2061 6374 696f 6e2e 0a0a 2020  r an action...  
-00008c20: 2020 2020 2020 2020 2020 5468 6973 2066            This f
-00008c30: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
-00008c40: 206f 6620 606f 6e65 6f66 605f 2060 6063   of `oneof`_ ``c
-00008c50: 6f6e 7472 6f6c 6060 2e0a 2020 2020 2020  ontrol``..      
-00008c60: 2020 656e 645f 6963 6f6e 2028 676f 6f67    end_icon (goog
-00008c70: 6c65 2e61 7070 732e 6361 7264 5f76 312e  le.apps.card_v1.
-00008c80: 7479 7065 732e 4963 6f6e 293a 0a20 2020  types.Icon):.   
-00008c90: 2020 2020 2020 2020 2041 6e20 6963 6f6e           An icon
-00008ca0: 2064 6973 706c 6179 6564 2061 6674 6572   displayed after
-00008cb0: 2074 6865 2074 6578 742e 0a0a 2020 2020   the text...    
-00008cc0: 2020 2020 2020 2020 5375 7070 6f72 7473          Supports
-00008cd0: 0a20 2020 2020 2020 2020 2020 2060 6275  .            `bu
-00008ce0: 696c 742d 696e 203c 6874 7470 733a 2f2f  ilt-in <https://
-00008cf0: 6465 7665 6c6f 7065 7273 2e67 6f6f 676c  developers.googl
-00008d00: 652e 636f 6d2f 6368 6174 2f66 6f72 6d61  e.com/chat/forma
-00008d10: 742d 6d65 7373 6167 6573 2362 7569 6c74  t-messages#built
-00008d20: 696e 6963 6f6e 733e 605f 5f0a 2020 2020  inicons>`__.    
-00008d30: 2020 2020 2020 2020 616e 640a 2020 2020          and.    
-00008d40: 2020 2020 2020 2020 6063 7573 746f 6d20          `custom 
-00008d50: 3c68 7474 7073 3a2f 2f64 6576 656c 6f70  <https://develop
-00008d60: 6572 732e 676f 6f67 6c65 2e63 6f6d 2f63  ers.google.com/c
-00008d70: 6861 742f 666f 726d 6174 2d6d 6573 7361  hat/format-messa
-00008d80: 6765 7323 6375 7374 6f6d 6963 6f6e 733e  ges#customicons>
-00008d90: 605f 5f0a 2020 2020 2020 2020 2020 2020  `__.            
-00008da0: 6963 6f6e 732e 0a0a 2020 2020 2020 2020  icons...        
-00008db0: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
-00008dc0: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
-00008dd0: 6e65 6f66 605f 2060 6063 6f6e 7472 6f6c  neof`_ ``control
-00008de0: 6060 2e0a 2020 2020 2222 220a 0a20 2020  ``..    """..   
-00008df0: 2063 6c61 7373 2053 7769 7463 6843 6f6e   class SwitchCon
-00008e00: 7472 6f6c 2870 726f 746f 2e4d 6573 7361  trol(proto.Messa
-00008e10: 6765 293a 0a20 2020 2020 2020 2072 2222  ge):.        r""
-00008e20: 2245 6974 6865 7220 6120 746f 6767 6c65  "Either a toggle
-00008e30: 2d73 7479 6c65 2073 7769 7463 6820 6f72  -style switch or
-00008e40: 2061 2063 6865 636b 626f 7820 696e 7369   a checkbox insi
-00008e50: 6465 2061 0a20 2020 2020 2020 2060 6064  de a.        ``d
-00008e60: 6563 6f72 6174 6564 5465 7874 6060 2077  ecoratedText`` w
-00008e70: 6964 6765 742e 0a0a 2020 2020 2020 2020  idget...        
-00008e80: 6047 6f6f 676c 6520 576f 726b 7370 6163  `Google Workspac
-00008e90: 6520 4164 642d 6f6e 7320 616e 6420 4368  e Add-ons and Ch
-00008ea0: 6174 0a20 2020 2020 2020 2061 7070 7320  at.        apps 
-00008eb0: 3c68 7474 7073 3a2f 2f64 6576 656c 6f70  <https://develop
-00008ec0: 6572 732e 676f 6f67 6c65 2e63 6f6d 2f77  ers.google.com/w
-00008ed0: 6f72 6b73 7061 6365 2f65 7874 656e 643e  orkspace/extend>
-00008ee0: 605f 5f3a 0a0a 2020 2020 2020 2020 4f6e  `__:..        On
-00008ef0: 6c79 2073 7570 706f 7274 6564 2069 6e20  ly supported in 
-00008f00: 7468 6520 6060 6465 636f 7261 7465 6454  the ``decoratedT
-00008f10: 6578 7460 6020 7769 6467 6574 2e0a 0a20  ext`` widget... 
-00008f20: 2020 2020 2020 2041 7474 7269 6275 7465         Attribute
-00008f30: 733a 0a20 2020 2020 2020 2020 2020 206e  s:.            n
-00008f40: 616d 6520 2873 7472 293a 0a20 2020 2020  ame (str):.     
-00008f50: 2020 2020 2020 2020 2020 2054 6865 206e             The n
-00008f60: 616d 6520 6279 2077 6869 6368 2074 6865  ame by which the
-00008f70: 2073 7769 7463 6820 7769 6467 6574 2069   switch widget i
-00008f80: 7320 6964 656e 7469 6669 6564 2069 6e20  s identified in 
-00008f90: 6120 666f 726d 0a20 2020 2020 2020 2020  a form.         
-00008fa0: 2020 2020 2020 2069 6e70 7574 2065 7665         input eve
-00008fb0: 6e74 2e0a 0a20 2020 2020 2020 2020 2020  nt...           
-00008fc0: 2020 2020 2046 6f72 2064 6574 6169 6c73       For details
-00008fd0: 2061 626f 7574 2077 6f72 6b69 6e67 2077   about working w
-00008fe0: 6974 6820 666f 726d 2069 6e70 7574 732c  ith form inputs,
-00008ff0: 2073 6565 2060 5265 6365 6976 650a 2020   see `Receive.  
-00009000: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00009010: 726d 0a20 2020 2020 2020 2020 2020 2020  rm.             
-00009020: 2020 2064 6174 6120 3c68 7474 7073 3a2f     data <https:/
-00009030: 2f64 6576 656c 6f70 6572 732e 676f 6f67  /developers.goog
-00009040: 6c65 2e63 6f6d 2f63 6861 742f 7569 2f72  le.com/chat/ui/r
-00009050: 6561 642d 666f 726d 2d64 6174 613e 605f  ead-form-data>`_
-00009060: 5f2e 0a20 2020 2020 2020 2020 2020 2076  _..            v
-00009070: 616c 7565 2028 7374 7229 3a0a 2020 2020  alue (str):.    
-00009080: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00009090: 7661 6c75 6520 656e 7465 7265 6420 6279  value entered by
-000090a0: 2061 2075 7365 722c 2072 6574 7572 6e65   a user, returne
-000090b0: 6420 6173 2070 6172 7420 6f66 2061 2066  d as part of a f
-000090c0: 6f72 6d0a 2020 2020 2020 2020 2020 2020  orm.            
-000090d0: 2020 2020 696e 7075 7420 6576 656e 742e      input event.
-000090e0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000090f0: 2020 466f 7220 6465 7461 696c 7320 6162    For details ab
-00009100: 6f75 7420 776f 726b 696e 6720 7769 7468  out working with
-00009110: 2066 6f72 6d20 696e 7075 7473 2c20 7365   form inputs, se
-00009120: 6520 6052 6563 6569 7665 0a20 2020 2020  e `Receive.     
-00009130: 2020 2020 2020 2020 2020 2066 6f72 6d0a             form.
-00009140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009150: 6461 7461 203c 6874 7470 733a 2f2f 6465  data <https://de
-00009160: 7665 6c6f 7065 7273 2e67 6f6f 676c 652e  velopers.google.
-00009170: 636f 6d2f 6368 6174 2f75 692f 7265 6164  com/chat/ui/read
-00009180: 2d66 6f72 6d2d 6461 7461 3e60 5f5f 2e0a  -form-data>`__..
-00009190: 2020 2020 2020 2020 2020 2020 7365 6c65              sele
-000091a0: 6374 6564 2028 626f 6f6c 293a 0a20 2020  cted (bool):.   
-000091b0: 2020 2020 2020 2020 2020 2020 2057 6865               Whe
-000091c0: 6e20 6060 7472 7565 6060 2c20 7468 6520  n ``true``, the 
-000091d0: 7377 6974 6368 2069 7320 7365 6c65 6374  switch is select
-000091e0: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
-000091f0: 6f6e 5f63 6861 6e67 655f 6163 7469 6f6e  on_change_action
-00009200: 2028 676f 6f67 6c65 2e61 7070 732e 6361   (google.apps.ca
-00009210: 7264 5f76 312e 7479 7065 732e 4163 7469  rd_v1.types.Acti
-00009220: 6f6e 293a 0a20 2020 2020 2020 2020 2020  on):.           
-00009230: 2020 2020 2054 6865 2061 6374 696f 6e20       The action 
-00009240: 746f 2070 6572 666f 726d 2077 6865 6e20  to perform when 
-00009250: 7468 6520 7377 6974 6368 2073 7461 7465  the switch state
-00009260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009270: 2069 7320 6368 616e 6765 642c 2073 7563   is changed, suc
-00009280: 6820 6173 2077 6861 7420 2066 756e 6374  h as what  funct
-00009290: 696f 6e20 746f 2072 756e 2e0a 2020 2020  ion to run..    
-000092a0: 2020 2020 2020 2020 636f 6e74 726f 6c5f          control_
-000092b0: 7479 7065 2028 676f 6f67 6c65 2e61 7070  type (google.app
-000092c0: 732e 6361 7264 5f76 312e 7479 7065 732e  s.card_v1.types.
-000092d0: 4465 636f 7261 7465 6454 6578 742e 5377  DecoratedText.Sw
-000092e0: 6974 6368 436f 6e74 726f 6c2e 436f 6e74  itchControl.Cont
-000092f0: 726f 6c54 7970 6529 3a0a 2020 2020 2020  rolType):.      
-00009300: 2020 2020 2020 2020 2020 486f 7720 7468            How th
-00009310: 6520 7377 6974 6368 2061 7070 6561 7273  e switch appears
-00009320: 2069 6e20 7468 6520 7573 6572 2069 6e74   in the user int
-00009330: 6572 6661 6365 2e0a 0a20 2020 2020 2020  erface...       
-00009340: 2020 2020 2020 2020 2060 476f 6f67 6c65           `Google
-00009350: 2057 6f72 6b73 7061 6365 2041 6464 2d6f   Workspace Add-o
-00009360: 6e73 2061 6e64 2043 6861 740a 2020 2020  ns and Chat.    
-00009370: 2020 2020 2020 2020 2020 2020 6170 7073              apps
-00009380: 203c 6874 7470 733a 2f2f 6465 7665 6c6f   <https://develo
-00009390: 7065 7273 2e67 6f6f 676c 652e 636f 6d2f  pers.google.com/
-000093a0: 776f 726b 7370 6163 652f 6578 7465 6e64  workspace/extend
-000093b0: 3e60 5f5f 3a0a 2020 2020 2020 2020 2222  >`__:.        ""
-000093c0: 220a 0a20 2020 2020 2020 2063 6c61 7373  "..        class
-000093d0: 2043 6f6e 7472 6f6c 5479 7065 2870 726f   ControlType(pro
-000093e0: 746f 2e45 6e75 6d29 3a0a 2020 2020 2020  to.Enum):.      
-000093f0: 2020 2020 2020 7222 2222 486f 7720 7468        r"""How th
-00009400: 6520 7377 6974 6368 2061 7070 6561 7273  e switch appears
-00009410: 2069 6e20 7468 6520 7573 6572 2069 6e74   in the user int
-00009420: 6572 6661 6365 2e0a 0a20 2020 2020 2020  erface...       
-00009430: 2020 2020 2060 476f 6f67 6c65 2057 6f72       `Google Wor
-00009440: 6b73 7061 6365 2041 6464 2d6f 6e73 2061  kspace Add-ons a
-00009450: 6e64 2043 6861 740a 2020 2020 2020 2020  nd Chat.        
-00009460: 2020 2020 6170 7073 203c 6874 7470 733a      apps <https:
-00009470: 2f2f 6465 7665 6c6f 7065 7273 2e67 6f6f  //developers.goo
-00009480: 676c 652e 636f 6d2f 776f 726b 7370 6163  gle.com/workspac
-00009490: 652f 6578 7465 6e64 3e60 5f5f 3a0a 0a20  e/extend>`__:.. 
-000094a0: 2020 2020 2020 2020 2020 2056 616c 7565             Value
-000094b0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-000094c0: 2020 2053 5749 5443 4820 2830 293a 0a20     SWITCH (0):. 
-000094d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094e0: 2020 2041 2074 6f67 676c 652d 7374 796c     A toggle-styl
-000094f0: 6520 7377 6974 6368 2e0a 2020 2020 2020  e switch..      
-00009500: 2020 2020 2020 2020 2020 4348 4543 4b42            CHECKB
-00009510: 4f58 2028 3129 3a0a 2020 2020 2020 2020  OX (1):.        
-00009520: 2020 2020 2020 2020 2020 2020 4465 7072              Depr
-00009530: 6563 6174 6564 2069 6e20 6661 766f 7220  ecated in favor 
-00009540: 6f66 2060 6043 4845 434b 5f42 4f58 6060  of ``CHECK_BOX``
-00009550: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009560: 2020 4348 4543 4b5f 424f 5820 2832 293a    CHECK_BOX (2):
-00009570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009580: 2020 2020 2041 2063 6865 636b 626f 782e       A checkbox.
-00009590: 0a20 2020 2020 2020 2020 2020 2022 2222  .            """
-000095a0: 0a20 2020 2020 2020 2020 2020 2053 5749  .            SWI
-000095b0: 5443 4820 3d20 300a 2020 2020 2020 2020  TCH = 0.        
-000095c0: 2020 2020 4348 4543 4b42 4f58 203d 2031      CHECKBOX = 1
-000095d0: 0a20 2020 2020 2020 2020 2020 2043 4845  .            CHE
-000095e0: 434b 5f42 4f58 203d 2032 0a0a 2020 2020  CK_BOX = 2..    
-000095f0: 2020 2020 6e61 6d65 3a20 7374 7220 3d20      name: str = 
-00009600: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
-00009610: 2020 2020 2020 2020 2070 726f 746f 2e53           proto.S
-00009620: 5452 494e 472c 0a20 2020 2020 2020 2020  TRING,.         
-00009630: 2020 206e 756d 6265 723d 312c 0a20 2020     number=1,.   
-00009640: 2020 2020 2029 0a20 2020 2020 2020 2076       ).        v
-00009650: 616c 7565 3a20 7374 7220 3d20 7072 6f74  alue: str = prot
-00009660: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-00009670: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
-00009680: 472c 0a20 2020 2020 2020 2020 2020 206e  G,.            n
-00009690: 756d 6265 723d 322c 0a20 2020 2020 2020  umber=2,.       
-000096a0: 2029 0a20 2020 2020 2020 2073 656c 6563   ).        selec
-000096b0: 7465 643a 2062 6f6f 6c20 3d20 7072 6f74  ted: bool = prot
-000096c0: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-000096d0: 2020 2020 2070 726f 746f 2e42 4f4f 4c2c       proto.BOOL,
-000096e0: 0a20 2020 2020 2020 2020 2020 206e 756d  .            num
-000096f0: 6265 723d 332c 0a20 2020 2020 2020 2029  ber=3,.        )
-00009700: 0a20 2020 2020 2020 206f 6e5f 6368 616e  .        on_chan
-00009710: 6765 5f61 6374 696f 6e3a 2022 4163 7469  ge_action: "Acti
-00009720: 6f6e 2220 3d20 7072 6f74 6f2e 4669 656c  on" = proto.Fiel
-00009730: 6428 0a20 2020 2020 2020 2020 2020 2070  d(.            p
-00009740: 726f 746f 2e4d 4553 5341 4745 2c0a 2020  roto.MESSAGE,.  
-00009750: 2020 2020 2020 2020 2020 6e75 6d62 6572            number
-00009760: 3d34 2c0a 2020 2020 2020 2020 2020 2020  =4,.            
-00009770: 6d65 7373 6167 653d 2241 6374 696f 6e22  message="Action"
-00009780: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-00009790: 2020 2020 636f 6e74 726f 6c5f 7479 7065      control_type
-000097a0: 3a20 2244 6563 6f72 6174 6564 5465 7874  : "DecoratedText
-000097b0: 2e53 7769 7463 6843 6f6e 7472 6f6c 2e43  .SwitchControl.C
-000097c0: 6f6e 7472 6f6c 5479 7065 2220 3d20 7072  ontrolType" = pr
-000097d0: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
-000097e0: 2020 2020 2020 2070 726f 746f 2e45 4e55         proto.ENU
-000097f0: 4d2c 0a20 2020 2020 2020 2020 2020 206e  M,.            n
-00009800: 756d 6265 723d 352c 0a20 2020 2020 2020  umber=5,.       
-00009810: 2020 2020 2065 6e75 6d3d 2244 6563 6f72       enum="Decor
-00009820: 6174 6564 5465 7874 2e53 7769 7463 6843  atedText.SwitchC
-00009830: 6f6e 7472 6f6c 2e43 6f6e 7472 6f6c 5479  ontrol.ControlTy
-00009840: 7065 222c 0a20 2020 2020 2020 2029 0a0a  pe",.        )..
-00009850: 2020 2020 6963 6f6e 3a20 2249 636f 6e22      icon: "Icon"
-00009860: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
-00009870: 2020 2020 2020 2020 7072 6f74 6f2e 4d45          proto.ME
-00009880: 5353 4147 452c 0a20 2020 2020 2020 206e  SSAGE,.        n
-00009890: 756d 6265 723d 312c 0a20 2020 2020 2020  umber=1,.       
-000098a0: 206d 6573 7361 6765 3d22 4963 6f6e 222c   message="Icon",
-000098b0: 0a20 2020 2029 0a20 2020 2073 7461 7274  .    ).    start
-000098c0: 5f69 636f 6e3a 2022 4963 6f6e 2220 3d20  _icon: "Icon" = 
-000098d0: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
-000098e0: 2020 2020 2070 726f 746f 2e4d 4553 5341       proto.MESSA
-000098f0: 4745 2c0a 2020 2020 2020 2020 6e75 6d62  GE,.        numb
-00009900: 6572 3d31 322c 0a20 2020 2020 2020 206d  er=12,.        m
-00009910: 6573 7361 6765 3d22 4963 6f6e 222c 0a20  essage="Icon",. 
-00009920: 2020 2029 0a20 2020 2074 6f70 5f6c 6162     ).    top_lab
-00009930: 656c 3a20 7374 7220 3d20 7072 6f74 6f2e  el: str = proto.
-00009940: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
-00009950: 726f 746f 2e53 5452 494e 472c 0a20 2020  roto.STRING,.   
-00009960: 2020 2020 206e 756d 6265 723d 332c 0a20       number=3,. 
-00009970: 2020 2029 0a20 2020 2074 6578 743a 2073     ).    text: s
-00009980: 7472 203d 2070 726f 746f 2e46 6965 6c64  tr = proto.Field
-00009990: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
-000099a0: 5354 5249 4e47 2c0a 2020 2020 2020 2020  STRING,.        
-000099b0: 6e75 6d62 6572 3d34 2c0a 2020 2020 290a  number=4,.    ).
-000099c0: 2020 2020 7772 6170 5f74 6578 743a 2062      wrap_text: b
-000099d0: 6f6f 6c20 3d20 7072 6f74 6f2e 4669 656c  ool = proto.Fiel
-000099e0: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
-000099f0: 2e42 4f4f 4c2c 0a20 2020 2020 2020 206e  .BOOL,.        n
-00009a00: 756d 6265 723d 352c 0a20 2020 2029 0a20  umber=5,.    ). 
-00009a10: 2020 2062 6f74 746f 6d5f 6c61 6265 6c3a     bottom_label:
-00009a20: 2073 7472 203d 2070 726f 746f 2e46 6965   str = proto.Fie
-00009a30: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
-00009a40: 6f2e 5354 5249 4e47 2c0a 2020 2020 2020  o.STRING,.      
-00009a50: 2020 6e75 6d62 6572 3d36 2c0a 2020 2020    number=6,.    
-00009a60: 290a 2020 2020 6f6e 5f63 6c69 636b 3a20  ).    on_click: 
-00009a70: 224f 6e43 6c69 636b 2220 3d20 7072 6f74  "OnClick" = prot
-00009a80: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-00009a90: 2070 726f 746f 2e4d 4553 5341 4745 2c0a   proto.MESSAGE,.
-00009aa0: 2020 2020 2020 2020 6e75 6d62 6572 3d37          number=7
-00009ab0: 2c0a 2020 2020 2020 2020 6d65 7373 6167  ,.        messag
-00009ac0: 653d 224f 6e43 6c69 636b 222c 0a20 2020  e="OnClick",.   
-00009ad0: 2029 0a20 2020 2062 7574 746f 6e3a 2022   ).    button: "
-00009ae0: 4275 7474 6f6e 2220 3d20 7072 6f74 6f2e  Button" = proto.
-00009af0: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
-00009b00: 726f 746f 2e4d 4553 5341 4745 2c0a 2020  roto.MESSAGE,.  
-00009b10: 2020 2020 2020 6e75 6d62 6572 3d38 2c0a        number=8,.
-00009b20: 2020 2020 2020 2020 6f6e 656f 663d 2263          oneof="c
-00009b30: 6f6e 7472 6f6c 222c 0a20 2020 2020 2020  ontrol",.       
-00009b40: 206d 6573 7361 6765 3d22 4275 7474 6f6e   message="Button
-00009b50: 222c 0a20 2020 2029 0a20 2020 2073 7769  ",.    ).    swi
-00009b60: 7463 685f 636f 6e74 726f 6c3a 2053 7769  tch_control: Swi
-00009b70: 7463 6843 6f6e 7472 6f6c 203d 2070 726f  tchControl = pro
-00009b80: 746f 2e46 6965 6c64 280a 2020 2020 2020  to.Field(.      
-00009b90: 2020 7072 6f74 6f2e 4d45 5353 4147 452c    proto.MESSAGE,
-00009ba0: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
-00009bb0: 392c 0a20 2020 2020 2020 206f 6e65 6f66  9,.        oneof
-00009bc0: 3d22 636f 6e74 726f 6c22 2c0a 2020 2020  ="control",.    
-00009bd0: 2020 2020 6d65 7373 6167 653d 5377 6974      message=Swit
-00009be0: 6368 436f 6e74 726f 6c2c 0a20 2020 2029  chControl,.    )
-00009bf0: 0a20 2020 2065 6e64 5f69 636f 6e3a 2022  .    end_icon: "
-00009c00: 4963 6f6e 2220 3d20 7072 6f74 6f2e 4669  Icon" = proto.Fi
-00009c10: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
-00009c20: 746f 2e4d 4553 5341 4745 2c0a 2020 2020  to.MESSAGE,.    
-00009c30: 2020 2020 6e75 6d62 6572 3d31 312c 0a20      number=11,. 
-00009c40: 2020 2020 2020 206f 6e65 6f66 3d22 636f         oneof="co
-00009c50: 6e74 726f 6c22 2c0a 2020 2020 2020 2020  ntrol",.        
-00009c60: 6d65 7373 6167 653d 2249 636f 6e22 2c0a  message="Icon",.
-00009c70: 2020 2020 290a 0a0a 636c 6173 7320 5465      )...class Te
-00009c80: 7874 496e 7075 7428 7072 6f74 6f2e 4d65  xtInput(proto.Me
-00009c90: 7373 6167 6529 3a0a 2020 2020 7222 2222  ssage):.    r"""
-00009ca0: 4120 6669 656c 6420 696e 2077 6869 6368  A field in which
-00009cb0: 2075 7365 7273 2063 616e 2065 6e74 6572   users can enter
-00009cc0: 2074 6578 742e 2053 7570 706f 7274 7320   text. Supports 
-00009cd0: 7375 6767 6573 7469 6f6e 7320 616e 640a  suggestions and.
-00009ce0: 2020 2020 6f6e 2d63 6861 6e67 6520 6163      on-change ac
-00009cf0: 7469 6f6e 732e 2046 6f72 2061 6e20 6578  tions. For an ex
-00009d00: 616d 706c 6520 696e 2047 6f6f 676c 6520  ample in Google 
-00009d10: 4368 6174 2061 7070 732c 2073 6565 2060  Chat apps, see `
-00009d20: 5465 7874 0a20 2020 2069 6e70 7574 203c  Text.    input <
-00009d30: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
-00009d40: 7273 2e67 6f6f 676c 652e 636f 6d2f 6368  rs.google.com/ch
-00009d50: 6174 2f75 692f 7769 6467 6574 732f 7465  at/ui/widgets/te
-00009d60: 7874 2d69 6e70 7574 3e60 5f5f 2e0a 0a20  xt-input>`__... 
-00009d70: 2020 2043 6861 7420 6170 7073 2072 6563     Chat apps rec
-00009d80: 6569 7665 2061 6e64 2063 616e 2070 726f  eive and can pro
-00009d90: 6365 7373 2074 6865 2076 616c 7565 206f  cess the value o
-00009da0: 6620 656e 7465 7265 6420 7465 7874 2064  f entered text d
-00009db0: 7572 696e 670a 2020 2020 666f 726d 2069  uring.    form i
-00009dc0: 6e70 7574 2065 7665 6e74 732e 2046 6f72  nput events. For
-00009dd0: 2064 6574 6169 6c73 2061 626f 7574 2077   details about w
-00009de0: 6f72 6b69 6e67 2077 6974 6820 666f 726d  orking with form
-00009df0: 2069 6e70 7574 732c 2073 6565 0a20 2020   inputs, see.   
-00009e00: 2060 5265 6365 6976 6520 666f 726d 0a20   `Receive form. 
-00009e10: 2020 2064 6174 6120 3c68 7474 7073 3a2f     data <https:/
-00009e20: 2f64 6576 656c 6f70 6572 732e 676f 6f67  /developers.goog
-00009e30: 6c65 2e63 6f6d 2f63 6861 742f 7569 2f72  le.com/chat/ui/r
-00009e40: 6561 642d 666f 726d 2d64 6174 613e 605f  ead-form-data>`_
-00009e50: 5f2e 0a0a 2020 2020 5768 656e 2079 6f75  _...    When you
-00009e60: 206e 6565 6420 746f 2063 6f6c 6c65 6374   need to collect
-00009e70: 2075 6e64 6566 696e 6564 206f 7220 6162   undefined or ab
-00009e80: 7374 7261 6374 2064 6174 6120 6672 6f6d  stract data from
-00009e90: 2075 7365 7273 2c20 7573 650a 2020 2020   users, use.    
-00009ea0: 6120 7465 7874 2069 6e70 7574 2e20 546f  a text input. To
-00009eb0: 2063 6f6c 6c65 6374 2064 6566 696e 6564   collect defined
-00009ec0: 206f 7220 656e 756d 6572 6174 6564 2064   or enumerated d
-00009ed0: 6174 6120 6672 6f6d 2075 7365 7273 2c20  ata from users, 
-00009ee0: 7573 650a 2020 2020 7468 6520 5b53 656c  use.    the [Sel
-00009ef0: 6563 7469 6f6e 496e 7075 745d 5b67 6f6f  ectionInput][goo
-00009f00: 676c 652e 6170 7073 2e63 6172 642e 7631  gle.apps.card.v1
-00009f10: 2e53 656c 6563 7469 6f6e 496e 7075 745d  .SelectionInput]
-00009f20: 2077 6964 6765 742e 0a0a 2020 2020 6047   widget...    `G
-00009f30: 6f6f 676c 6520 576f 726b 7370 6163 6520  oogle Workspace 
-00009f40: 4164 642d 6f6e 7320 616e 6420 4368 6174  Add-ons and Chat
-00009f50: 0a20 2020 2061 7070 7320 3c68 7474 7073  .    apps <https
-00009f60: 3a2f 2f64 6576 656c 6f70 6572 732e 676f  ://developers.go
-00009f70: 6f67 6c65 2e63 6f6d 2f77 6f72 6b73 7061  ogle.com/workspa
-00009f80: 6365 2f65 7874 656e 643e 605f 5f3a 0a0a  ce/extend>`__:..
-00009f90: 2020 2020 4174 7472 6962 7574 6573 3a0a      Attributes:.
-00009fa0: 2020 2020 2020 2020 6e61 6d65 2028 7374          name (st
-00009fb0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-00009fc0: 5468 6520 6e61 6d65 2062 7920 7768 6963  The name by whic
-00009fd0: 6820 7468 6520 7465 7874 2069 6e70 7574  h the text input
-00009fe0: 2069 7320 6964 656e 7469 6669 6564 2069   is identified i
-00009ff0: 6e20 6120 666f 726d 0a20 2020 2020 2020  n a form.       
-0000a000: 2020 2020 2069 6e70 7574 2065 7665 6e74       input event
-0000a010: 2e0a 0a20 2020 2020 2020 2020 2020 2046  ...            F
-0000a020: 6f72 2064 6574 6169 6c73 2061 626f 7574  or details about
-0000a030: 2077 6f72 6b69 6e67 2077 6974 6820 666f   working with fo
-0000a040: 726d 2069 6e70 7574 732c 2073 6565 2060  rm inputs, see `
-0000a050: 5265 6365 6976 650a 2020 2020 2020 2020  Receive.        
-0000a060: 2020 2020 666f 726d 0a20 2020 2020 2020      form.       
-0000a070: 2020 2020 2064 6174 6120 3c68 7474 7073       data <https
-0000a080: 3a2f 2f64 6576 656c 6f70 6572 732e 676f  ://developers.go
-0000a090: 6f67 6c65 2e63 6f6d 2f63 6861 742f 7569  ogle.com/chat/ui
-0000a0a0: 2f72 6561 642d 666f 726d 2d64 6174 613e  /read-form-data>
-0000a0b0: 605f 5f2e 0a20 2020 2020 2020 206c 6162  `__..        lab
-0000a0c0: 656c 2028 7374 7229 3a0a 2020 2020 2020  el (str):.      
-0000a0d0: 2020 2020 2020 5468 6520 7465 7874 2074        The text t
-0000a0e0: 6861 7420 6170 7065 6172 7320 6162 6f76  hat appears abov
-0000a0f0: 6520 7468 6520 7465 7874 2069 6e70 7574  e the text input
-0000a100: 2066 6965 6c64 2069 6e20 7468 6520 7573   field in the us
-0000a110: 6572 0a20 2020 2020 2020 2020 2020 2069  er.            i
-0000a120: 6e74 6572 6661 6365 2e0a 0a20 2020 2020  nterface...     
-0000a130: 2020 2020 2020 2053 7065 6369 6679 2074         Specify t
-0000a140: 6578 7420 7468 6174 2068 656c 7073 2074  ext that helps t
-0000a150: 6865 2075 7365 7220 656e 7465 7220 7468  he user enter th
-0000a160: 6520 696e 666f 726d 6174 696f 6e20 796f  e information yo
-0000a170: 7572 0a20 2020 2020 2020 2020 2020 2061  ur.            a
-0000a180: 7070 206e 6565 6473 2e20 466f 7220 6578  pp needs. For ex
-0000a190: 616d 706c 652c 2069 6620 796f 7520 6172  ample, if you ar
-0000a1a0: 6520 6173 6b69 6e67 2073 6f6d 656f 6e65  e asking someone
-0000a1b0: 2773 206e 616d 652c 0a20 2020 2020 2020  's name,.       
-0000a1c0: 2020 2020 2062 7574 2073 7065 6369 6669       but specifi
-0000a1d0: 6361 6c6c 7920 6e65 6564 2074 6865 6972  cally need their
-0000a1e0: 2073 7572 6e61 6d65 2c20 7772 6974 6520   surname, write 
-0000a1f0: 6060 7375 726e 616d 6560 600a 2020 2020  ``surname``.    
-0000a200: 2020 2020 2020 2020 696e 7374 6561 6420          instead 
-0000a210: 6f66 2060 606e 616d 6560 602e 0a0a 2020  of ``name``...  
-0000a220: 2020 2020 2020 2020 2020 5265 7175 6972            Requir
-0000a230: 6564 2069 6620 6060 6869 6e74 5465 7874  ed if ``hintText
-0000a240: 6060 2069 7320 756e 7370 6563 6966 6965  `` is unspecifie
-0000a250: 642e 204f 7468 6572 7769 7365 2c0a 2020  d. Otherwise,.  
-0000a260: 2020 2020 2020 2020 2020 6f70 7469 6f6e            option
-0000a270: 616c 2e0a 2020 2020 2020 2020 6869 6e74  al..        hint
-0000a280: 5f74 6578 7420 2873 7472 293a 0a20 2020  _text (str):.   
-0000a290: 2020 2020 2020 2020 2054 6578 7420 7468           Text th
-0000a2a0: 6174 2061 7070 6561 7273 2062 656c 6f77  at appears below
-0000a2b0: 2074 6865 2074 6578 7420 696e 7075 7420   the text input 
-0000a2c0: 6669 656c 6420 6d65 616e 7420 746f 2061  field meant to a
-0000a2d0: 7373 6973 740a 2020 2020 2020 2020 2020  ssist.          
-0000a2e0: 2020 7573 6572 7320 6279 2070 726f 6d70    users by promp
-0000a2f0: 7469 6e67 2074 6865 6d20 746f 2065 6e74  ting them to ent
-0000a300: 6572 2061 2063 6572 7461 696e 2076 616c  er a certain val
-0000a310: 7565 2e20 5468 6973 2074 6578 740a 2020  ue. This text.  
-0000a320: 2020 2020 2020 2020 2020 6973 2061 6c77            is alw
-0000a330: 6179 7320 7669 7369 626c 652e 0a0a 2020  ays visible...  
-0000a340: 2020 2020 2020 2020 2020 5265 7175 6972            Requir
-0000a350: 6564 2069 6620 6060 6c61 6265 6c60 6020  ed if ``label`` 
-0000a360: 6973 2075 6e73 7065 6369 6669 6564 2e20  is unspecified. 
-0000a370: 4f74 6865 7277 6973 652c 206f 7074 696f  Otherwise, optio
-0000a380: 6e61 6c2e 0a20 2020 2020 2020 2076 616c  nal..        val
-0000a390: 7565 2028 7374 7229 3a0a 2020 2020 2020  ue (str):.      
-0000a3a0: 2020 2020 2020 5468 6520 7661 6c75 6520        The value 
-0000a3b0: 656e 7465 7265 6420 6279 2061 2075 7365  entered by a use
-0000a3c0: 722c 2072 6574 7572 6e65 6420 6173 2070  r, returned as p
-0000a3d0: 6172 7420 6f66 2061 2066 6f72 6d0a 2020  art of a form.  
-0000a3e0: 2020 2020 2020 2020 2020 696e 7075 7420            input 
-0000a3f0: 6576 656e 742e 0a0a 2020 2020 2020 2020  event...        
-0000a400: 2020 2020 466f 7220 6465 7461 696c 7320      For details 
-0000a410: 6162 6f75 7420 776f 726b 696e 6720 7769  about working wi
-0000a420: 7468 2066 6f72 6d20 696e 7075 7473 2c20  th form inputs, 
-0000a430: 7365 6520 6052 6563 6569 7665 0a20 2020  see `Receive.   
-0000a440: 2020 2020 2020 2020 2066 6f72 6d0a 2020           form.  
-0000a450: 2020 2020 2020 2020 2020 6461 7461 203c            data <
-0000a460: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
-0000a470: 7273 2e67 6f6f 676c 652e 636f 6d2f 6368  rs.google.com/ch
-0000a480: 6174 2f75 692f 7265 6164 2d66 6f72 6d2d  at/ui/read-form-
-0000a490: 6461 7461 3e60 5f5f 2e0a 2020 2020 2020  data>`__..      
-0000a4a0: 2020 7479 7065 5f20 2867 6f6f 676c 652e    type_ (google.
-0000a4b0: 6170 7073 2e63 6172 645f 7631 2e74 7970  apps.card_v1.typ
-0000a4c0: 6573 2e54 6578 7449 6e70 7574 2e54 7970  es.TextInput.Typ
-0000a4d0: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-0000a4e0: 486f 7720 6120 7465 7874 2069 6e70 7574  How a text input
-0000a4f0: 2066 6965 6c64 2061 7070 6561 7273 2069   field appears i
-0000a500: 6e20 7468 6520 7573 6572 0a20 2020 2020  n the user.     
-0000a510: 2020 2020 2020 2069 6e74 6572 6661 6365         interface
-0000a520: 2e20 466f 7220 6578 616d 706c 652c 2077  . For example, w
-0000a530: 6865 7468 6572 2074 6865 2066 6965 6c64  hether the field
-0000a540: 2069 730a 2020 2020 2020 2020 2020 2020   is.            
-0000a550: 7369 6e67 6c65 206f 7220 6d75 6c74 692d  single or multi-
-0000a560: 6c69 6e65 2e0a 2020 2020 2020 2020 6f6e  line..        on
-0000a570: 5f63 6861 6e67 655f 6163 7469 6f6e 2028  _change_action (
-0000a580: 676f 6f67 6c65 2e61 7070 732e 6361 7264  google.apps.card
-0000a590: 5f76 312e 7479 7065 732e 4163 7469 6f6e  _v1.types.Action
-0000a5a0: 293a 0a20 2020 2020 2020 2020 2020 2057  ):.            W
-0000a5b0: 6861 7420 746f 2064 6f20 7768 656e 2061  hat to do when a
-0000a5c0: 2063 6861 6e67 6520 6f63 6375 7273 2069   change occurs i
-0000a5d0: 6e20 7468 6520 7465 7874 2069 6e70 7574  n the text input
-0000a5e0: 2066 6965 6c64 2e20 466f 720a 2020 2020   field. For.    
-0000a5f0: 2020 2020 2020 2020 6578 616d 706c 652c          example,
-0000a600: 2061 2075 7365 7220 6164 6469 6e67 2074   a user adding t
-0000a610: 6f20 7468 6520 6669 656c 6420 6f72 2064  o the field or d
-0000a620: 656c 6574 696e 6720 7465 7874 2e0a 0a20  eleting text... 
-0000a630: 2020 2020 2020 2020 2020 2045 7861 6d70             Examp
-0000a640: 6c65 7320 6f66 2061 6374 696f 6e73 2074  les of actions t
-0000a650: 6f20 7461 6b65 2069 6e63 6c75 6465 2072  o take include r
-0000a660: 756e 6e69 6e67 2061 2063 7573 746f 6d0a  unning a custom.
-0000a670: 2020 2020 2020 2020 2020 2020 6675 6e63              func
-0000a680: 7469 6f6e 206f 7220 6f70 656e 696e 6720  tion or opening 
-0000a690: 610a 2020 2020 2020 2020 2020 2020 6064  a.            `d
-0000a6a0: 6961 6c6f 6720 3c68 7474 7073 3a2f 2f64  ialog <https://d
-0000a6b0: 6576 656c 6f70 6572 732e 676f 6f67 6c65  evelopers.google
-0000a6c0: 2e63 6f6d 2f63 6861 742f 686f 772d 746f  .com/chat/how-to
-0000a6d0: 732f 6469 616c 6f67 733e 605f 5f0a 2020  s/dialogs>`__.  
-0000a6e0: 2020 2020 2020 2020 2020 696e 2047 6f6f            in Goo
-0000a6f0: 676c 6520 4368 6174 2e0a 2020 2020 2020  gle Chat..      
-0000a700: 2020 696e 6974 6961 6c5f 7375 6767 6573    initial_sugges
-0000a710: 7469 6f6e 7320 2867 6f6f 676c 652e 6170  tions (google.ap
-0000a720: 7073 2e63 6172 645f 7631 2e74 7970 6573  ps.card_v1.types
-0000a730: 2e53 7567 6765 7374 696f 6e73 293a 0a20  .Suggestions):. 
-0000a740: 2020 2020 2020 2020 2020 2053 7567 6765             Sugge
-0000a750: 7374 6564 2076 616c 7565 7320 7468 6174  sted values that
-0000a760: 2075 7365 7273 2063 616e 2065 6e74 6572   users can enter
-0000a770: 2e20 5468 6573 6520 7661 6c75 6573 2061  . These values a
-0000a780: 7070 6561 720a 2020 2020 2020 2020 2020  ppear.          
-0000a790: 2020 7768 656e 2075 7365 7273 2063 6c69    when users cli
-0000a7a0: 636b 2069 6e73 6964 6520 7468 6520 7465  ck inside the te
-0000a7b0: 7874 2069 6e70 7574 2066 6965 6c64 2e20  xt input field. 
-0000a7c0: 4173 2075 7365 7273 2074 7970 652c 0a20  As users type,. 
-0000a7d0: 2020 2020 2020 2020 2020 2074 6865 2073             the s
-0000a7e0: 7567 6765 7374 6564 2076 616c 7565 7320  uggested values 
-0000a7f0: 6479 6e61 6d69 6361 6c6c 7920 6669 6c74  dynamically filt
-0000a800: 6572 2074 6f20 6d61 7463 6820 7768 6174  er to match what
-0000a810: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
-0000a820: 2075 7365 7273 2068 6176 6520 7479 7065   users have type
-0000a830: 642e 0a0a 2020 2020 2020 2020 2020 2020  d...            
-0000a840: 466f 7220 6578 616d 706c 652c 2061 2074  For example, a t
-0000a850: 6578 7420 696e 7075 7420 6669 656c 6420  ext input field 
-0000a860: 666f 7220 7072 6f67 7261 6d6d 696e 6720  for programming 
-0000a870: 6c61 6e67 7561 6765 0a20 2020 2020 2020  language.       
-0000a880: 2020 2020 206d 6967 6874 2073 7567 6765       might sugge
-0000a890: 7374 204a 6176 612c 204a 6176 6153 6372  st Java, JavaScr
-0000a8a0: 6970 742c 2050 7974 686f 6e2c 2061 6e64  ipt, Python, and
-0000a8b0: 2043 2b2b 2e20 5768 656e 2075 7365 7273   C++. When users
-0000a8c0: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
-0000a8d0: 7274 2074 7970 696e 6720 6060 4a61 7660  rt typing ``Jav`
-0000a8e0: 602c 2074 6865 206c 6973 7420 6f66 2073  `, the list of s
-0000a8f0: 7567 6765 7374 696f 6e73 2066 696c 7465  uggestions filte
-0000a900: 7273 2074 6f0a 2020 2020 2020 2020 2020  rs to.          
-0000a910: 2020 7368 6f77 206a 7573 7420 6060 4a61    show just ``Ja
-0000a920: 7661 6060 2061 6e64 2060 604a 6176 6153  va`` and ``JavaS
-0000a930: 6372 6970 7460 602e 0a0a 2020 2020 2020  cript``...      
-0000a940: 2020 2020 2020 5375 6767 6573 7465 6420        Suggested 
-0000a950: 7661 6c75 6573 2068 656c 7020 6775 6964  values help guid
-0000a960: 6520 7573 6572 7320 746f 2065 6e74 6572  e users to enter
-0000a970: 2076 616c 7565 7320 7468 6174 2079 6f75   values that you
-0000a980: 720a 2020 2020 2020 2020 2020 2020 6170  r.            ap
-0000a990: 7020 6361 6e20 6d61 6b65 2073 656e 7365  p can make sense
-0000a9a0: 206f 662e 2057 6865 6e20 7265 6665 7272   of. When referr
-0000a9b0: 696e 6720 746f 204a 6176 6153 6372 6970  ing to JavaScrip
-0000a9c0: 742c 2073 6f6d 650a 2020 2020 2020 2020  t, some.        
-0000a9d0: 2020 2020 7573 6572 7320 6d69 6768 7420      users might 
-0000a9e0: 656e 7465 7220 6060 6a61 7661 7363 7269  enter ``javascri
-0000a9f0: 7074 6060 2061 6e64 206f 7468 6572 7320  pt`` and others 
-0000aa00: 6060 6a61 7661 2073 6372 6970 7460 602e  ``java script``.
-0000aa10: 0a20 2020 2020 2020 2020 2020 2053 7567  .            Sug
-0000aa20: 6765 7374 696e 6720 6060 4a61 7661 5363  gesting ``JavaSc
-0000aa30: 7269 7074 6060 2063 616e 2073 7461 6e64  ript`` can stand
-0000aa40: 6172 6469 7a65 2068 6f77 2075 7365 7273  ardize how users
-0000aa50: 2069 6e74 6572 6163 740a 2020 2020 2020   interact.      
-0000aa60: 2020 2020 2020 7769 7468 2079 6f75 7220        with your 
-0000aa70: 6170 702e 0a0a 2020 2020 2020 2020 2020  app...          
-0000aa80: 2020 5768 656e 2073 7065 6369 6669 6564    When specified
-0000aa90: 2c20 6060 5465 7874 496e 7075 742e 7479  , ``TextInput.ty
-0000aaa0: 7065 6060 2069 7320 616c 7761 7973 0a20  pe`` is always. 
-0000aab0: 2020 2020 2020 2020 2020 2060 6053 494e             ``SIN
-0000aac0: 474c 455f 4c49 4e45 6060 2c20 6576 656e  GLE_LINE``, even
-0000aad0: 2069 6620 6974 2773 2073 6574 2074 6f20   if it's set to 
-0000aae0: 6060 4d55 4c54 4950 4c45 5f4c 494e 4560  ``MULTIPLE_LINE`
-0000aaf0: 602e 0a0a 2020 2020 2020 2020 2020 2020  `...            
-0000ab00: 6047 6f6f 676c 6520 576f 726b 7370 6163  `Google Workspac
-0000ab10: 6520 4164 642d 6f6e 7320 616e 6420 4368  e Add-ons and Ch
-0000ab20: 6174 0a20 2020 2020 2020 2020 2020 2061  at.            a
-0000ab30: 7070 7320 3c68 7474 7073 3a2f 2f64 6576  pps <https://dev
-0000ab40: 656c 6f70 6572 732e 676f 6f67 6c65 2e63  elopers.google.c
-0000ab50: 6f6d 2f77 6f72 6b73 7061 6365 2f65 7874  om/workspace/ext
-0000ab60: 656e 643e 605f 5f3a 0a20 2020 2020 2020  end>`__:.       
-0000ab70: 2061 7574 6f5f 636f 6d70 6c65 7465 5f61   auto_complete_a
-0000ab80: 6374 696f 6e20 2867 6f6f 676c 652e 6170  ction (google.ap
-0000ab90: 7073 2e63 6172 645f 7631 2e74 7970 6573  ps.card_v1.types
-0000aba0: 2e41 6374 696f 6e29 3a0a 2020 2020 2020  .Action):.      
-0000abb0: 2020 2020 2020 4f70 7469 6f6e 616c 2e20        Optional. 
-0000abc0: 5370 6563 6966 7920 7768 6174 2061 6374  Specify what act
-0000abd0: 696f 6e20 746f 2074 616b 6520 7768 656e  ion to take when
-0000abe0: 2074 6865 2074 6578 7420 696e 7075 740a   the text input.
-0000abf0: 2020 2020 2020 2020 2020 2020 6669 656c              fiel
-0000ac00: 6420 7072 6f76 6964 6573 2073 7567 6765  d provides sugge
-0000ac10: 7374 696f 6e73 2074 6f20 7573 6572 7320  stions to users 
-0000ac20: 7768 6f20 696e 7465 7261 6374 2077 6974  who interact wit
-0000ac30: 6820 6974 2e0a 0a20 2020 2020 2020 2020  h it...         
-0000ac40: 2020 2049 6620 756e 7370 6563 6966 6965     If unspecifie
-0000ac50: 642c 2074 6865 2073 7567 6765 7374 696f  d, the suggestio
-0000ac60: 6e73 2061 7265 2073 6574 2062 790a 2020  ns are set by.  
-0000ac70: 2020 2020 2020 2020 2020 6060 696e 6974            ``init
-0000ac80: 6961 6c53 7567 6765 7374 696f 6e73 6060  ialSuggestions``
-0000ac90: 2061 6e64 2061 7265 2070 726f 6365 7373   and are process
-0000aca0: 6564 2062 7920 7468 6520 636c 6965 6e74  ed by the client
-0000acb0: 2e0a 0a20 2020 2020 2020 2020 2020 2049  ...            I
-0000acc0: 6620 7370 6563 6966 6965 642c 2074 6865  f specified, the
-0000acd0: 2061 7070 2074 616b 6573 2074 6865 2061   app takes the a
-0000ace0: 6374 696f 6e20 7370 6563 6966 6965 6420  ction specified 
-0000acf0: 6865 7265 2c20 7375 6368 0a20 2020 2020  here, such.     
-0000ad00: 2020 2020 2020 2061 7320 7275 6e6e 696e         as runnin
-0000ad10: 6720 6120 6375 7374 6f6d 2066 756e 6374  g a custom funct
-0000ad20: 696f 6e2e 0a0a 2020 2020 2020 2020 2020  ion...          
-0000ad30: 2020 6047 6f6f 676c 6520 576f 726b 7370    `Google Worksp
-0000ad40: 6163 650a 2020 2020 2020 2020 2020 2020  ace.            
-0000ad50: 4164 642d 6f6e 7320 3c68 7474 7073 3a2f  Add-ons <https:/
-0000ad60: 2f64 6576 656c 6f70 6572 732e 676f 6f67  /developers.goog
-0000ad70: 6c65 2e63 6f6d 2f77 6f72 6b73 7061 6365  le.com/workspace
-0000ad80: 2f61 6464 2d6f 6e73 3e60 5f5f 3a0a 2020  /add-ons>`__:.  
-0000ad90: 2020 2020 2020 706c 6163 6568 6f6c 6465        placeholde
-0000ada0: 725f 7465 7874 2028 7374 7229 3a0a 2020  r_text (str):.  
-0000adb0: 2020 2020 2020 2020 2020 5465 7874 2074            Text t
-0000adc0: 6861 7420 6170 7065 6172 7320 696e 2074  hat appears in t
-0000add0: 6865 2074 6578 7420 696e 7075 7420 6669  he text input fi
-0000ade0: 656c 6420 7768 656e 2074 6865 2066 6965  eld when the fie
-0000adf0: 6c64 2069 730a 2020 2020 2020 2020 2020  ld is.          
-0000ae00: 2020 656d 7074 792e 2055 7365 2074 6869    empty. Use thi
-0000ae10: 7320 7465 7874 2074 6f20 7072 6f6d 7074  s text to prompt
-0000ae20: 2075 7365 7273 2074 6f20 656e 7465 7220   users to enter 
-0000ae30: 6120 7661 6c75 652e 2046 6f72 0a20 2020  a value. For.   
-0000ae40: 2020 2020 2020 2020 2065 7861 6d70 6c65           example
-0000ae50: 2c20 6060 456e 7465 7220 6120 6e75 6d62  , ``Enter a numb
-0000ae60: 6572 2066 726f 6d20 3020 746f 2031 3030  er from 0 to 100
-0000ae70: 6060 2e0a 0a20 2020 2020 2020 2020 2020  ``...           
-0000ae80: 2060 476f 6f67 6c65 2043 6861 7420 6170   `Google Chat ap
-0000ae90: 7073 203c 6874 7470 733a 2f2f 6465 7665  ps <https://deve
-0000aea0: 6c6f 7065 7273 2e67 6f6f 676c 652e 636f  lopers.google.co
-0000aeb0: 6d2f 6368 6174 3e60 5f5f 3a0a 2020 2020  m/chat>`__:.    
-0000aec0: 2222 220a 0a20 2020 2063 6c61 7373 2054  """..    class T
-0000aed0: 7970 6528 7072 6f74 6f2e 456e 756d 293a  ype(proto.Enum):
-0000aee0: 0a20 2020 2020 2020 2072 2222 2248 6f77  .        r"""How
-0000aef0: 2061 2074 6578 7420 696e 7075 7420 6669   a text input fi
-0000af00: 656c 6420 6170 7065 6172 7320 696e 2074  eld appears in t
-0000af10: 6865 2075 7365 7220 696e 7465 7266 6163  he user interfac
-0000af20: 652e 2046 6f72 2065 7861 6d70 6c65 2c0a  e. For example,.
-0000af30: 2020 2020 2020 2020 7768 6574 6865 7220          whether 
-0000af40: 6974 2773 2061 2073 696e 676c 6520 6c69  it's a single li
-0000af50: 6e65 2069 6e70 7574 2066 6965 6c64 2c20  ne input field, 
-0000af60: 6f72 2061 206d 756c 7469 2d6c 696e 6520  or a multi-line 
-0000af70: 696e 7075 742e 2049 660a 2020 2020 2020  input. If.      
-0000af80: 2020 6060 696e 6974 6961 6c53 7567 6765    ``initialSugge
-0000af90: 7374 696f 6e73 6060 2069 7320 7370 6563  stions`` is spec
-0000afa0: 6966 6965 642c 2060 6074 7970 6560 6020  ified, ``type`` 
-0000afb0: 6973 2061 6c77 6179 730a 2020 2020 2020  is always.      
-0000afc0: 2020 6060 5349 4e47 4c45 5f4c 494e 4560    ``SINGLE_LINE`
-0000afd0: 602c 2065 7665 6e20 6966 2069 7427 7320  `, even if it's 
-0000afe0: 7365 7420 746f 2060 604d 554c 5449 504c  set to ``MULTIPL
-0000aff0: 455f 4c49 4e45 6060 2e0a 0a20 2020 2020  E_LINE``...     
-0000b000: 2020 2060 476f 6f67 6c65 2057 6f72 6b73     `Google Works
-0000b010: 7061 6365 2041 6464 2d6f 6e73 2061 6e64  pace Add-ons and
-0000b020: 2043 6861 740a 2020 2020 2020 2020 6170   Chat.        ap
-0000b030: 7073 203c 6874 7470 733a 2f2f 6465 7665  ps <https://deve
-0000b040: 6c6f 7065 7273 2e67 6f6f 676c 652e 636f  lopers.google.co
-0000b050: 6d2f 776f 726b 7370 6163 652f 6578 7465  m/workspace/exte
-0000b060: 6e64 3e60 5f5f 3a0a 0a20 2020 2020 2020  nd>`__:..       
-0000b070: 2056 616c 7565 733a 0a20 2020 2020 2020   Values:.       
-0000b080: 2020 2020 2053 494e 474c 455f 4c49 4e45       SINGLE_LINE
-0000b090: 2028 3029 3a0a 2020 2020 2020 2020 2020   (0):.          
-0000b0a0: 2020 2020 2020 5468 6520 7465 7874 2069        The text i
-0000b0b0: 6e70 7574 2066 6965 6c64 2068 6173 2061  nput field has a
-0000b0c0: 2066 6978 6564 2068 6569 6768 7420 6f66   fixed height of
-0000b0d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b0e0: 206f 6e65 206c 696e 652e 0a20 2020 2020   one line..     
-0000b0f0: 2020 2020 2020 204d 554c 5449 504c 455f         MULTIPLE_
-0000b100: 4c49 4e45 2028 3129 3a0a 2020 2020 2020  LINE (1):.      
-0000b110: 2020 2020 2020 2020 2020 5468 6520 7465            The te
-0000b120: 7874 2069 6e70 7574 2066 6965 6c64 2068  xt input field h
-0000b130: 6173 2061 2066 6978 6564 2068 6569 6768  as a fixed heigh
-0000b140: 7420 6f66 0a20 2020 2020 2020 2020 2020  t of.           
-0000b150: 2020 2020 206d 756c 7469 706c 6520 6c69       multiple li
-0000b160: 6e65 732e 0a20 2020 2020 2020 2022 2222  nes..        """
-0000b170: 0a20 2020 2020 2020 2053 494e 474c 455f  .        SINGLE_
-0000b180: 4c49 4e45 203d 2030 0a20 2020 2020 2020  LINE = 0.       
-0000b190: 204d 554c 5449 504c 455f 4c49 4e45 203d   MULTIPLE_LINE =
-0000b1a0: 2031 0a0a 2020 2020 6e61 6d65 3a20 7374   1..    name: st
-0000b1b0: 7220 3d20 7072 6f74 6f2e 4669 656c 6428  r = proto.Field(
-0000b1c0: 0a20 2020 2020 2020 2070 726f 746f 2e53  .        proto.S
-0000b1d0: 5452 494e 472c 0a20 2020 2020 2020 206e  TRING,.        n
-0000b1e0: 756d 6265 723d 312c 0a20 2020 2029 0a20  umber=1,.    ). 
-0000b1f0: 2020 206c 6162 656c 3a20 7374 7220 3d20     label: str = 
-0000b200: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
-0000b210: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
-0000b220: 472c 0a20 2020 2020 2020 206e 756d 6265  G,.        numbe
-0000b230: 723d 322c 0a20 2020 2029 0a20 2020 2068  r=2,.    ).    h
-0000b240: 696e 745f 7465 7874 3a20 7374 7220 3d20  int_text: str = 
-0000b250: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
-0000b260: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
-0000b270: 472c 0a20 2020 2020 2020 206e 756d 6265  G,.        numbe
-0000b280: 723d 332c 0a20 2020 2029 0a20 2020 2076  r=3,.    ).    v
-0000b290: 616c 7565 3a20 7374 7220 3d20 7072 6f74  alue: str = prot
-0000b2a0: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-0000b2b0: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
-0000b2c0: 2020 2020 2020 206e 756d 6265 723d 342c         number=4,
-0000b2d0: 0a20 2020 2029 0a20 2020 2074 7970 655f  .    ).    type_
-0000b2e0: 3a20 5479 7065 203d 2070 726f 746f 2e46  : Type = proto.F
-0000b2f0: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
-0000b300: 6f74 6f2e 454e 554d 2c0a 2020 2020 2020  oto.ENUM,.      
-0000b310: 2020 6e75 6d62 6572 3d35 2c0a 2020 2020    number=5,.    
-0000b320: 2020 2020 656e 756d 3d54 7970 652c 0a20      enum=Type,. 
-0000b330: 2020 2029 0a20 2020 206f 6e5f 6368 616e     ).    on_chan
-0000b340: 6765 5f61 6374 696f 6e3a 2022 4163 7469  ge_action: "Acti
-0000b350: 6f6e 2220 3d20 7072 6f74 6f2e 4669 656c  on" = proto.Fiel
-0000b360: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
-0000b370: 2e4d 4553 5341 4745 2c0a 2020 2020 2020  .MESSAGE,.      
-0000b380: 2020 6e75 6d62 6572 3d36 2c0a 2020 2020    number=6,.    
-0000b390: 2020 2020 6d65 7373 6167 653d 2241 6374      message="Act
-0000b3a0: 696f 6e22 2c0a 2020 2020 290a 2020 2020  ion",.    ).    
-0000b3b0: 696e 6974 6961 6c5f 7375 6767 6573 7469  initial_suggesti
-0000b3c0: 6f6e 733a 2022 5375 6767 6573 7469 6f6e  ons: "Suggestion
-0000b3d0: 7322 203d 2070 726f 746f 2e46 6965 6c64  s" = proto.Field
-0000b3e0: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
-0000b3f0: 4d45 5353 4147 452c 0a20 2020 2020 2020  MESSAGE,.       
-0000b400: 206e 756d 6265 723d 372c 0a20 2020 2020   number=7,.     
-0000b410: 2020 206d 6573 7361 6765 3d22 5375 6767     message="Sugg
-0000b420: 6573 7469 6f6e 7322 2c0a 2020 2020 290a  estions",.    ).
-0000b430: 2020 2020 6175 746f 5f63 6f6d 706c 6574      auto_complet
-0000b440: 655f 6163 7469 6f6e 3a20 2241 6374 696f  e_action: "Actio
-0000b450: 6e22 203d 2070 726f 746f 2e46 6965 6c64  n" = proto.Field
-0000b460: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
-0000b470: 4d45 5353 4147 452c 0a20 2020 2020 2020  MESSAGE,.       
-0000b480: 206e 756d 6265 723d 382c 0a20 2020 2020   number=8,.     
-0000b490: 2020 206d 6573 7361 6765 3d22 4163 7469     message="Acti
-0000b4a0: 6f6e 222c 0a20 2020 2029 0a20 2020 2070  on",.    ).    p
-0000b4b0: 6c61 6365 686f 6c64 6572 5f74 6578 743a  laceholder_text:
-0000b4c0: 2073 7472 203d 2070 726f 746f 2e46 6965   str = proto.Fie
-0000b4d0: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
-0000b4e0: 6f2e 5354 5249 4e47 2c0a 2020 2020 2020  o.STRING,.      
-0000b4f0: 2020 6e75 6d62 6572 3d31 322c 0a20 2020    number=12,.   
-0000b500: 2029 0a0a 0a63 6c61 7373 2053 7567 6765   )...class Sugge
-0000b510: 7374 696f 6e73 2870 726f 746f 2e4d 6573  stions(proto.Mes
-0000b520: 7361 6765 293a 0a20 2020 2072 2222 2253  sage):.    r"""S
-0000b530: 7567 6765 7374 6564 2076 616c 7565 7320  uggested values 
-0000b540: 7468 6174 2075 7365 7273 2063 616e 2065  that users can e
-0000b550: 6e74 6572 2e20 5468 6573 6520 7661 6c75  nter. These valu
-0000b560: 6573 2061 7070 6561 7220 7768 656e 0a20  es appear when. 
-0000b570: 2020 2075 7365 7273 2063 6c69 636b 2069     users click i
-0000b580: 6e73 6964 6520 7468 6520 7465 7874 2069  nside the text i
-0000b590: 6e70 7574 2066 6965 6c64 2e20 4173 2075  nput field. As u
-0000b5a0: 7365 7273 2074 7970 652c 2074 6865 0a20  sers type, the. 
-0000b5b0: 2020 2073 7567 6765 7374 6564 2076 616c     suggested val
-0000b5c0: 7565 7320 6479 6e61 6d69 6361 6c6c 7920  ues dynamically 
-0000b5d0: 6669 6c74 6572 2074 6f20 6d61 7463 6820  filter to match 
-0000b5e0: 7768 6174 2074 6865 2075 7365 7273 2068  what the users h
-0000b5f0: 6176 650a 2020 2020 7479 7065 642e 0a0a  ave.    typed...
-0000b600: 2020 2020 466f 7220 6578 616d 706c 652c      For example,
-0000b610: 2061 2074 6578 7420 696e 7075 7420 6669   a text input fi
-0000b620: 656c 6420 666f 7220 7072 6f67 7261 6d6d  eld for programm
-0000b630: 696e 6720 6c61 6e67 7561 6765 206d 6967  ing language mig
-0000b640: 6874 0a20 2020 2073 7567 6765 7374 204a  ht.    suggest J
-0000b650: 6176 612c 204a 6176 6153 6372 6970 742c  ava, JavaScript,
-0000b660: 2050 7974 686f 6e2c 2061 6e64 2043 2b2b   Python, and C++
-0000b670: 2e20 5768 656e 2075 7365 7273 2073 7461  . When users sta
-0000b680: 7274 2074 7970 696e 670a 2020 2020 6060  rt typing.    ``
-0000b690: 4a61 7660 602c 2074 6865 206c 6973 7420  Jav``, the list 
-0000b6a0: 6f66 2073 7567 6765 7374 696f 6e73 2066  of suggestions f
-0000b6b0: 696c 7465 7273 2074 6f20 7368 6f77 2060  ilters to show `
-0000b6c0: 604a 6176 6160 6020 616e 640a 2020 2020  `Java`` and.    
-0000b6d0: 6060 4a61 7661 5363 7269 7074 6060 2e0a  ``JavaScript``..
-0000b6e0: 0a20 2020 2053 7567 6765 7374 6564 2076  .    Suggested v
-0000b6f0: 616c 7565 7320 6865 6c70 2067 7569 6465  alues help guide
-0000b700: 2075 7365 7273 2074 6f20 656e 7465 7220   users to enter 
-0000b710: 7661 6c75 6573 2074 6861 7420 796f 7572  values that your
-0000b720: 2061 7070 2063 616e 0a20 2020 206d 616b   app can.    mak
-0000b730: 6520 7365 6e73 6520 6f66 2e20 5768 656e  e sense of. When
-0000b740: 2072 6566 6572 7269 6e67 2074 6f20 4a61   referring to Ja
-0000b750: 7661 5363 7269 7074 2c20 736f 6d65 2075  vaScript, some u
-0000b760: 7365 7273 206d 6967 6874 2065 6e74 6572  sers might enter
-0000b770: 0a20 2020 2060 606a 6176 6173 6372 6970  .    ``javascrip
-0000b780: 7460 6020 616e 6420 6f74 6865 7273 2060  t`` and others `
-0000b790: 606a 6176 6120 7363 7269 7074 6060 2e20  `java script``. 
-0000b7a0: 5375 6767 6573 7469 6e67 2060 604a 6176  Suggesting ``Jav
-0000b7b0: 6153 6372 6970 7460 600a 2020 2020 6361  aScript``.    ca
-0000b7c0: 6e20 7374 616e 6461 7264 697a 6520 686f  n standardize ho
-0000b7d0: 7720 7573 6572 7320 696e 7465 7261 6374  w users interact
-0000b7e0: 2077 6974 6820 796f 7572 2061 7070 2e0a   with your app..
-0000b7f0: 0a20 2020 2057 6865 6e20 7370 6563 6966  .    When specif
-0000b800: 6965 642c 2060 6054 6578 7449 6e70 7574  ied, ``TextInput
-0000b810: 2e74 7970 6560 6020 6973 2061 6c77 6179  .type`` is alway
-0000b820: 7320 6060 5349 4e47 4c45 5f4c 494e 4560  s ``SINGLE_LINE`
-0000b830: 602c 2065 7665 6e0a 2020 2020 6966 2069  `, even.    if i
-0000b840: 7427 7320 7365 7420 746f 2060 604d 554c  t's set to ``MUL
-0000b850: 5449 504c 455f 4c49 4e45 6060 2e0a 0a20  TIPLE_LINE``... 
-0000b860: 2020 2060 476f 6f67 6c65 2057 6f72 6b73     `Google Works
-0000b870: 7061 6365 2041 6464 2d6f 6e73 2061 6e64  pace Add-ons and
-0000b880: 2043 6861 740a 2020 2020 6170 7073 203c   Chat.    apps <
-0000b890: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
-0000b8a0: 7273 2e67 6f6f 676c 652e 636f 6d2f 776f  rs.google.com/wo
-0000b8b0: 726b 7370 6163 652f 6578 7465 6e64 3e60  rkspace/extend>`
-0000b8c0: 5f5f 3a0a 0a20 2020 2041 7474 7269 6275  __:..    Attribu
-0000b8d0: 7465 733a 0a20 2020 2020 2020 2069 7465  tes:.        ite
-0000b8e0: 6d73 2028 4d75 7461 626c 6553 6571 7565  ms (MutableSeque
-0000b8f0: 6e63 655b 676f 6f67 6c65 2e61 7070 732e  nce[google.apps.
-0000b900: 6361 7264 5f76 312e 7479 7065 732e 5375  card_v1.types.Su
-0000b910: 6767 6573 7469 6f6e 732e 5375 6767 6573  ggestions.Sugges
-0000b920: 7469 6f6e 4974 656d 5d29 3a0a 2020 2020  tionItem]):.    
-0000b930: 2020 2020 2020 2020 4120 6c69 7374 206f          A list o
-0000b940: 6620 7375 6767 6573 7469 6f6e 7320 7573  f suggestions us
-0000b950: 6564 2066 6f72 2061 7574 6f63 6f6d 706c  ed for autocompl
-0000b960: 6574 650a 2020 2020 2020 2020 2020 2020  ete.            
-0000b970: 7265 636f 6d6d 656e 6461 7469 6f6e 7320  recommendations 
-0000b980: 696e 2074 6578 7420 696e 7075 7420 6669  in text input fi
-0000b990: 656c 6473 2e0a 2020 2020 2222 220a 0a20  elds..    """.. 
-0000b9a0: 2020 2063 6c61 7373 2053 7567 6765 7374     class Suggest
-0000b9b0: 696f 6e49 7465 6d28 7072 6f74 6f2e 4d65  ionItem(proto.Me
-0000b9c0: 7373 6167 6529 3a0a 2020 2020 2020 2020  ssage):.        
-0000b9d0: 7222 2222 4f6e 6520 7375 6767 6573 7465  r"""One suggeste
-0000b9e0: 6420 7661 6c75 6520 7468 6174 2075 7365  d value that use
-0000b9f0: 7273 2063 616e 2065 6e74 6572 2069 6e20  rs can enter in 
-0000ba00: 6120 7465 7874 2069 6e70 7574 2066 6965  a text input fie
-0000ba10: 6c64 2e0a 0a20 2020 2020 2020 2060 476f  ld...        `Go
-0000ba20: 6f67 6c65 2057 6f72 6b73 7061 6365 2041  ogle Workspace A
-0000ba30: 6464 2d6f 6e73 2061 6e64 2043 6861 740a  dd-ons and Chat.
-0000ba40: 2020 2020 2020 2020 6170 7073 203c 6874          apps <ht
-0000ba50: 7470 733a 2f2f 6465 7665 6c6f 7065 7273  tps://developers
-0000ba60: 2e67 6f6f 676c 652e 636f 6d2f 776f 726b  .google.com/work
-0000ba70: 7370 6163 652f 6578 7465 6e64 3e60 5f5f  space/extend>`__
-0000ba80: 3a0a 0a0a 2020 2020 2020 2020 2e2e 205f  :...        .. _
-0000ba90: 6f6e 656f 663a 2068 7474 7073 3a2f 2f70  oneof: https://p
-0000baa0: 726f 746f 2d70 6c75 732d 7079 7468 6f6e  roto-plus-python
-0000bab0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
-0000bac0: 656e 2f73 7461 626c 652f 6669 656c 6473  en/stable/fields
-0000bad0: 2e68 746d 6c23 6f6e 656f 6673 2d6d 7574  .html#oneofs-mut
-0000bae0: 7561 6c6c 792d 6578 636c 7573 6976 652d  ually-exclusive-
-0000baf0: 6669 656c 6473 0a0a 2020 2020 2020 2020  fields..        
-0000bb00: 4174 7472 6962 7574 6573 3a0a 2020 2020  Attributes:.    
-0000bb10: 2020 2020 2020 2020 7465 7874 2028 7374          text (st
-0000bb20: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-0000bb30: 2020 2020 5468 6520 7661 6c75 6520 6f66      The value of
-0000bb40: 2061 2073 7567 6765 7374 6564 2069 6e70   a suggested inp
-0000bb50: 7574 2074 6f20 6120 7465 7874 0a20 2020  ut to a text.   
-0000bb60: 2020 2020 2020 2020 2020 2020 2069 6e70               inp
-0000bb70: 7574 2066 6965 6c64 2e20 5468 6973 2069  ut field. This i
-0000bb80: 7320 6571 7569 7661 6c65 6e74 2074 6f20  s equivalent to 
-0000bb90: 7768 6174 2075 7365 7273 0a20 2020 2020  what users.     
-0000bba0: 2020 2020 2020 2020 2020 2065 6e74 6572             enter
-0000bbb0: 2074 6865 6d73 656c 7665 732e 0a0a 2020   themselves...  
-0000bbc0: 2020 2020 2020 2020 2020 2020 2020 5468                Th
-0000bbd0: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
-0000bbe0: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
-0000bbf0: 2060 6063 6f6e 7465 6e74 6060 2e0a 2020   ``content``..  
-0000bc00: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-0000bc10: 2020 2074 6578 743a 2073 7472 203d 2070     text: str = p
-0000bc20: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
-0000bc30: 2020 2020 2020 2020 7072 6f74 6f2e 5354          proto.ST
-0000bc40: 5249 4e47 2c0a 2020 2020 2020 2020 2020  RING,.          
-0000bc50: 2020 6e75 6d62 6572 3d31 2c0a 2020 2020    number=1,.    
-0000bc60: 2020 2020 2020 2020 6f6e 656f 663d 2263          oneof="c
-0000bc70: 6f6e 7465 6e74 222c 0a20 2020 2020 2020  ontent",.       
-0000bc80: 2029 0a0a 2020 2020 6974 656d 733a 204d   )..    items: M
-0000bc90: 7574 6162 6c65 5365 7175 656e 6365 5b53  utableSequence[S
-0000bca0: 7567 6765 7374 696f 6e49 7465 6d5d 203d  uggestionItem] =
-0000bcb0: 2070 726f 746f 2e52 6570 6561 7465 6446   proto.RepeatedF
-0000bcc0: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
-0000bcd0: 6f74 6f2e 4d45 5353 4147 452c 0a20 2020  oto.MESSAGE,.   
-0000bce0: 2020 2020 206e 756d 6265 723d 312c 0a20       number=1,. 
-0000bcf0: 2020 2020 2020 206d 6573 7361 6765 3d53         message=S
-0000bd00: 7567 6765 7374 696f 6e49 7465 6d2c 0a20  uggestionItem,. 
-0000bd10: 2020 2029 0a0a 0a63 6c61 7373 2042 7574     )...class But
-0000bd20: 746f 6e4c 6973 7428 7072 6f74 6f2e 4d65  tonList(proto.Me
-0000bd30: 7373 6167 6529 3a0a 2020 2020 7222 2222  ssage):.    r"""
-0000bd40: 4120 6c69 7374 206f 6620 6275 7474 6f6e  A list of button
-0000bd50: 7320 6c61 7965 6420 6f75 7420 686f 7269  s layed out hori
-0000bd60: 7a6f 6e74 616c 6c79 2e20 466f 7220 616e  zontally. For an
-0000bd70: 2065 7861 6d70 6c65 2069 6e20 476f 6f67   example in Goog
-0000bd80: 6c65 0a20 2020 2043 6861 7420 6170 7073  le.    Chat apps
-0000bd90: 2c20 7365 6520 6042 7574 746f 6e0a 2020  , see `Button.  
-0000bda0: 2020 6c69 7374 203c 6874 7470 733a 2f2f    list <https://
-0000bdb0: 6465 7665 6c6f 7065 7273 2e67 6f6f 676c  developers.googl
-0000bdc0: 652e 636f 6d2f 6368 6174 2f75 692f 7769  e.com/chat/ui/wi
-0000bdd0: 6467 6574 732f 6275 7474 6f6e 2d6c 6973  dgets/button-lis
-0000bde0: 743e 605f 5f2e 0a0a 2020 2020 6047 6f6f  t>`__...    `Goo
-0000bdf0: 676c 6520 576f 726b 7370 6163 6520 4164  gle Workspace Ad
-0000be00: 642d 6f6e 7320 616e 6420 4368 6174 0a20  d-ons and Chat. 
-0000be10: 2020 2061 7070 7320 3c68 7474 7073 3a2f     apps <https:/
-0000be20: 2f64 6576 656c 6f70 6572 732e 676f 6f67  /developers.goog
-0000be30: 6c65 2e63 6f6d 2f77 6f72 6b73 7061 6365  le.com/workspace
-0000be40: 2f65 7874 656e 643e 605f 5f3a 0a0a 2020  /extend>`__:..  
-0000be50: 2020 4174 7472 6962 7574 6573 3a0a 2020    Attributes:.  
-0000be60: 2020 2020 2020 6275 7474 6f6e 7320 284d        buttons (M
-0000be70: 7574 6162 6c65 5365 7175 656e 6365 5b67  utableSequence[g
-0000be80: 6f6f 676c 652e 6170 7073 2e63 6172 645f  oogle.apps.card_
-0000be90: 7631 2e74 7970 6573 2e42 7574 746f 6e5d  v1.types.Button]
-0000bea0: 293a 0a20 2020 2020 2020 2020 2020 2041  ):.            A
-0000beb0: 6e20 6172 7261 7920 6f66 2062 7574 746f  n array of butto
-0000bec0: 6e73 2e0a 2020 2020 2222 220a 0a20 2020  ns..    """..   
-0000bed0: 2062 7574 746f 6e73 3a20 4d75 7461 626c   buttons: Mutabl
-0000bee0: 6553 6571 7565 6e63 655b 2242 7574 746f  eSequence["Butto
-0000bef0: 6e22 5d20 3d20 7072 6f74 6f2e 5265 7065  n"] = proto.Repe
-0000bf00: 6174 6564 4669 656c 6428 0a20 2020 2020  atedField(.     
-0000bf10: 2020 2070 726f 746f 2e4d 4553 5341 4745     proto.MESSAGE
-0000bf20: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
-0000bf30: 3d31 2c0a 2020 2020 2020 2020 6d65 7373  =1,.        mess
-0000bf40: 6167 653d 2242 7574 746f 6e22 2c0a 2020  age="Button",.  
-0000bf50: 2020 290a 0a0a 636c 6173 7320 5365 6c65    )...class Sele
-0000bf60: 6374 696f 6e49 6e70 7574 2870 726f 746f  ctionInput(proto
-0000bf70: 2e4d 6573 7361 6765 293a 0a20 2020 2072  .Message):.    r
-0000bf80: 2222 2241 2077 6964 6765 7420 7468 6174  """A widget that
-0000bf90: 2063 7265 6174 6573 206f 6e65 206f 7220   creates one or 
-0000bfa0: 6d6f 7265 2055 4920 6974 656d 7320 7468  more UI items th
-0000bfb0: 6174 2075 7365 7273 2063 616e 2073 656c  at users can sel
-0000bfc0: 6563 742e 0a20 2020 2046 6f72 2065 7861  ect..    For exa
-0000bfd0: 6d70 6c65 2c20 6120 6472 6f70 646f 776e  mple, a dropdown
-0000bfe0: 206d 656e 7520 6f72 2063 6865 636b 626f   menu or checkbo
-0000bff0: 7865 732e 2059 6f75 2063 616e 2075 7365  xes. You can use
-0000c000: 2074 6869 7320 7769 6467 6574 0a20 2020   this widget.   
-0000c010: 2074 6f20 636f 6c6c 6563 7420 6461 7461   to collect data
-0000c020: 2074 6861 7420 6361 6e20 6265 2070 7265   that can be pre
-0000c030: 6469 6374 6564 206f 7220 656e 756d 6572  dicted or enumer
-0000c040: 6174 6564 2e20 466f 7220 616e 2065 7861  ated. For an exa
-0000c050: 6d70 6c65 0a20 2020 2069 6e20 476f 6f67  mple.    in Goog
-0000c060: 6c65 2043 6861 7420 6170 7073 2c20 7365  le Chat apps, se
-0000c070: 6520 6053 656c 6563 7469 6f6e 0a20 2020  e `Selection.   
-0000c080: 2069 6e70 7574 203c 6874 7470 733a 2f2f   input <https://
-0000c090: 6465 7665 6c6f 7065 7273 2e67 6f6f 676c  developers.googl
-0000c0a0: 652e 636f 6d2f 6368 6174 2f75 692f 7769  e.com/chat/ui/wi
-0000c0b0: 6467 6574 732f 7365 6c65 6374 696f 6e2d  dgets/selection-
-0000c0c0: 696e 7075 743e 605f 5f2e 0a0a 2020 2020  input>`__...    
-0000c0d0: 4368 6174 2061 7070 7320 6361 6e20 7072  Chat apps can pr
-0000c0e0: 6f63 6573 7320 7468 6520 7661 6c75 6520  ocess the value 
-0000c0f0: 6f66 2069 7465 6d73 2074 6861 7420 7573  of items that us
-0000c100: 6572 7320 7365 6c65 6374 206f 7220 696e  ers select or in
-0000c110: 7075 742e 0a20 2020 2046 6f72 2064 6574  put..    For det
-0000c120: 6169 6c73 2061 626f 7574 2077 6f72 6b69  ails about worki
-0000c130: 6e67 2077 6974 6820 666f 726d 2069 6e70  ng with form inp
-0000c140: 7574 732c 2073 6565 2060 5265 6365 6976  uts, see `Receiv
-0000c150: 6520 666f 726d 0a20 2020 2064 6174 6120  e form.    data 
-0000c160: 3c68 7474 7073 3a2f 2f64 6576 656c 6f70  <https://develop
-0000c170: 6572 732e 676f 6f67 6c65 2e63 6f6d 2f63  ers.google.com/c
-0000c180: 6861 742f 7569 2f72 6561 642d 666f 726d  hat/ui/read-form
-0000c190: 2d64 6174 613e 605f 5f2e 0a0a 2020 2020  -data>`__...    
-0000c1a0: 546f 2063 6f6c 6c65 6374 2075 6e64 6566  To collect undef
-0000c1b0: 696e 6564 206f 7220 6162 7374 7261 6374  ined or abstract
-0000c1c0: 2064 6174 6120 6672 6f6d 2075 7365 7273   data from users
-0000c1d0: 2c20 7573 6520 7468 650a 2020 2020 5b54  , use the.    [T
-0000c1e0: 6578 7449 6e70 7574 5d5b 676f 6f67 6c65  extInput][google
-0000c1f0: 2e61 7070 732e 6361 7264 2e76 312e 5465  .apps.card.v1.Te
-0000c200: 7874 496e 7075 745d 2077 6964 6765 742e  xtInput] widget.
-0000c210: 0a0a 2020 2020 6047 6f6f 676c 6520 576f  ..    `Google Wo
-0000c220: 726b 7370 6163 6520 4164 642d 6f6e 7320  rkspace Add-ons 
-0000c230: 616e 6420 4368 6174 0a20 2020 2061 7070  and Chat.    app
-0000c240: 7320 3c68 7474 7073 3a2f 2f64 6576 656c  s <https://devel
-0000c250: 6f70 6572 732e 676f 6f67 6c65 2e63 6f6d  opers.google.com
-0000c260: 2f77 6f72 6b73 7061 6365 2f65 7874 656e  /workspace/exten
-0000c270: 643e 605f 5f3a 0a0a 2020 2020 5468 6973  d>`__:..    This
-0000c280: 206d 6573 7361 6765 2068 6173 2060 6f6e   message has `on
-0000c290: 656f 6660 5f20 6669 656c 6473 2028 6d75  eof`_ fields (mu
-0000c2a0: 7475 616c 6c79 2065 7863 6c75 7369 7665  tually exclusive
-0000c2b0: 2066 6965 6c64 7329 2e0a 2020 2020 466f   fields)..    Fo
-0000c2c0: 7220 6561 6368 206f 6e65 6f66 2c20 6174  r each oneof, at
-0000c2d0: 206d 6f73 7420 6f6e 6520 6d65 6d62 6572   most one member
-0000c2e0: 2066 6965 6c64 2063 616e 2062 6520 7365   field can be se
-0000c2f0: 7420 6174 2074 6865 2073 616d 6520 7469  t at the same ti
-0000c300: 6d65 2e0a 2020 2020 5365 7474 696e 6720  me..    Setting 
-0000c310: 616e 7920 6d65 6d62 6572 206f 6620 7468  any member of th
-0000c320: 6520 6f6e 656f 6620 6175 746f 6d61 7469  e oneof automati
-0000c330: 6361 6c6c 7920 636c 6561 7273 2061 6c6c  cally clears all
-0000c340: 206f 7468 6572 0a20 2020 206d 656d 6265   other.    membe
-0000c350: 7273 2e0a 0a20 2020 202e 2e20 5f6f 6e65  rs...    .. _one
-0000c360: 6f66 3a20 6874 7470 733a 2f2f 7072 6f74  of: https://prot
-0000c370: 6f2d 706c 7573 2d70 7974 686f 6e2e 7265  o-plus-python.re
-0000c380: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-0000c390: 7374 6162 6c65 2f66 6965 6c64 732e 6874  stable/fields.ht
-0000c3a0: 6d6c 236f 6e65 6f66 732d 6d75 7475 616c  ml#oneofs-mutual
-0000c3b0: 6c79 2d65 7863 6c75 7369 7665 2d66 6965  ly-exclusive-fie
-0000c3c0: 6c64 730a 0a20 2020 2041 7474 7269 6275  lds..    Attribu
-0000c3d0: 7465 733a 0a20 2020 2020 2020 206e 616d  tes:.        nam
-0000c3e0: 6520 2873 7472 293a 0a20 2020 2020 2020  e (str):.       
-0000c3f0: 2020 2020 2054 6865 206e 616d 6520 7468       The name th
-0000c400: 6174 2069 6465 6e74 6966 6965 7320 7468  at identifies th
-0000c410: 6520 7365 6c65 6374 696f 6e20 696e 7075  e selection inpu
-0000c420: 7420 696e 2061 2066 6f72 6d20 696e 7075  t in a form inpu
-0000c430: 740a 2020 2020 2020 2020 2020 2020 6576  t.            ev
-0000c440: 656e 742e 0a0a 2020 2020 2020 2020 2020  ent...          
-0000c450: 2020 466f 7220 6465 7461 696c 7320 6162    For details ab
-0000c460: 6f75 7420 776f 726b 696e 6720 7769 7468  out working with
-0000c470: 2066 6f72 6d20 696e 7075 7473 2c20 7365   form inputs, se
-0000c480: 6520 6052 6563 6569 7665 0a20 2020 2020  e `Receive.     
-0000c490: 2020 2020 2020 2066 6f72 6d0a 2020 2020         form.    
-0000c4a0: 2020 2020 2020 2020 6461 7461 203c 6874          data <ht
-0000c4b0: 7470 733a 2f2f 6465 7665 6c6f 7065 7273  tps://developers
-0000c4c0: 2e67 6f6f 676c 652e 636f 6d2f 6368 6174  .google.com/chat
-0000c4d0: 2f75 692f 7265 6164 2d66 6f72 6d2d 6461  /ui/read-form-da
-0000c4e0: 7461 3e60 5f5f 2e0a 2020 2020 2020 2020  ta>`__..        
-0000c4f0: 6c61 6265 6c20 2873 7472 293a 0a20 2020  label (str):.   
-0000c500: 2020 2020 2020 2020 2054 6865 2074 6578           The tex
-0000c510: 7420 7468 6174 2061 7070 6561 7273 2061  t that appears a
-0000c520: 626f 7665 2074 6865 2073 656c 6563 7469  bove the selecti
-0000c530: 6f6e 0a20 2020 2020 2020 2020 2020 2069  on.            i
-0000c540: 6e70 7574 2066 6965 6c64 2069 6e20 7468  nput field in th
-0000c550: 6520 7573 6572 2069 6e74 6572 6661 6365  e user interface
-0000c560: 2e0a 0a20 2020 2020 2020 2020 2020 2053  ...            S
-0000c570: 7065 6369 6679 2074 6578 7420 7468 6174  pecify text that
-0000c580: 2068 656c 7073 2074 6865 2075 7365 7220   helps the user 
-0000c590: 656e 7465 7220 7468 650a 2020 2020 2020  enter the.      
-0000c5a0: 2020 2020 2020 696e 666f 726d 6174 696f        informatio
-0000c5b0: 6e20 796f 7572 2061 7070 206e 6565 6473  n your app needs
-0000c5c0: 2e20 466f 7220 6578 616d 706c 652c 2069  . For example, i
-0000c5d0: 660a 2020 2020 2020 2020 2020 2020 7573  f.            us
-0000c5e0: 6572 7320 6172 6520 7365 6c65 6374 696e  ers are selectin
-0000c5f0: 6720 7468 6520 7572 6765 6e63 7920 6f66  g the urgency of
-0000c600: 2061 2077 6f72 6b20 7469 636b 6574 0a20   a work ticket. 
-0000c610: 2020 2020 2020 2020 2020 2066 726f 6d20             from 
-0000c620: 6120 6472 6f70 2d64 6f77 6e20 6d65 6e75  a drop-down menu
-0000c630: 2c20 7468 6520 6c61 6265 6c20 6d69 6768  , the label migh
-0000c640: 7420 6265 0a20 2020 2020 2020 2020 2020  t be.           
-0000c650: 2022 5572 6765 6e63 7922 206f 7220 2253   "Urgency" or "S
-0000c660: 656c 6563 7420 7572 6765 6e63 7922 2e0a  elect urgency"..
-0000c670: 2020 2020 2020 2020 7479 7065 5f20 2867          type_ (g
-0000c680: 6f6f 676c 652e 6170 7073 2e63 6172 645f  oogle.apps.card_
-0000c690: 7631 2e74 7970 6573 2e53 656c 6563 7469  v1.types.Selecti
-0000c6a0: 6f6e 496e 7075 742e 5365 6c65 6374 696f  onInput.Selectio
-0000c6b0: 6e54 7970 6529 3a0a 2020 2020 2020 2020  nType):.        
-0000c6c0: 2020 2020 5468 6520 7479 7065 206f 6620      The type of 
-0000c6d0: 6974 656d 7320 7468 6174 2061 7265 2064  items that are d
-0000c6e0: 6973 706c 6179 6564 2074 6f20 7573 6572  isplayed to user
-0000c6f0: 7320 696e 2061 0a20 2020 2020 2020 2020  s in a.         
-0000c700: 2020 2060 6053 656c 6563 7469 6f6e 496e     ``SelectionIn
-0000c710: 7075 7460 6020 7769 6467 6574 2e20 5365  put`` widget. Se
-0000c720: 6c65 6374 696f 6e20 7479 7065 7320 7375  lection types su
-0000c730: 7070 6f72 7420 6469 6666 6572 656e 740a  pport different.
-0000c740: 2020 2020 2020 2020 2020 2020 7479 7065              type
-0000c750: 7320 6f66 2069 6e74 6572 6163 7469 6f6e  s of interaction
-0000c760: 732e 2046 6f72 2065 7861 6d70 6c65 2c20  s. For example, 
-0000c770: 7573 6572 7320 6361 6e20 7365 6c65 6374  users can select
-0000c780: 206f 6e65 206f 720a 2020 2020 2020 2020   one or.        
-0000c790: 2020 2020 6d6f 7265 2063 6865 636b 626f      more checkbo
-0000c7a0: 7865 732c 2062 7574 2074 6865 7920 6361  xes, but they ca
-0000c7b0: 6e20 6f6e 6c79 2073 656c 6563 7420 6f6e  n only select on
-0000c7c0: 6520 7661 6c75 6520 6672 6f6d 2061 0a20  e value from a. 
-0000c7d0: 2020 2020 2020 2020 2020 2064 726f 7064             dropd
-0000c7e0: 6f77 6e20 6d65 6e75 2e0a 2020 2020 2020  own menu..      
-0000c7f0: 2020 6974 656d 7320 284d 7574 6162 6c65    items (Mutable
-0000c800: 5365 7175 656e 6365 5b67 6f6f 676c 652e  Sequence[google.
-0000c810: 6170 7073 2e63 6172 645f 7631 2e74 7970  apps.card_v1.typ
-0000c820: 6573 2e53 656c 6563 7469 6f6e 496e 7075  es.SelectionInpu
-0000c830: 742e 5365 6c65 6374 696f 6e49 7465 6d5d  t.SelectionItem]
-0000c840: 293a 0a20 2020 2020 2020 2020 2020 2041  ):.            A
-0000c850: 6e20 6172 7261 7920 6f66 2073 656c 6563  n array of selec
-0000c860: 7461 626c 6520 6974 656d 732e 2046 6f72  table items. For
-0000c870: 2065 7861 6d70 6c65 2c20 616e 0a20 2020   example, an.   
-0000c880: 2020 2020 2020 2020 2061 7272 6179 206f           array o
-0000c890: 6620 7261 6469 6f20 6275 7474 6f6e 7320  f radio buttons 
-0000c8a0: 6f72 2063 6865 636b 626f 7865 732e 2053  or checkboxes. S
-0000c8b0: 7570 706f 7274 730a 2020 2020 2020 2020  upports.        
-0000c8c0: 2020 2020 7570 2074 6f20 3130 3020 6974      up to 100 it
-0000c8d0: 656d 732e 0a20 2020 2020 2020 206f 6e5f  ems..        on_
-0000c8e0: 6368 616e 6765 5f61 6374 696f 6e20 2867  change_action (g
-0000c8f0: 6f6f 676c 652e 6170 7073 2e63 6172 645f  oogle.apps.card_
-0000c900: 7631 2e74 7970 6573 2e41 6374 696f 6e29  v1.types.Action)
-0000c910: 3a0a 2020 2020 2020 2020 2020 2020 4966  :.            If
-0000c920: 2073 7065 6369 6669 6564 2c20 7468 6520   specified, the 
-0000c930: 666f 726d 2069 7320 7375 626d 6974 7465  form is submitte
-0000c940: 6420 7768 656e 2074 6865 2073 656c 6563  d when the selec
-0000c950: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
-0000c960: 2063 6861 6e67 6573 2e20 4966 206e 6f74   changes. If not
-0000c970: 2073 7065 6369 6669 6564 2c20 796f 7520   specified, you 
-0000c980: 6d75 7374 2073 7065 6369 6679 2061 2073  must specify a s
-0000c990: 6570 6172 6174 650a 2020 2020 2020 2020  eparate.        
-0000c9a0: 2020 2020 6275 7474 6f6e 2074 6861 7420      button that 
-0000c9b0: 7375 626d 6974 7320 7468 6520 666f 726d  submits the form
-0000c9c0: 2e0a 0a20 2020 2020 2020 2020 2020 2046  ...            F
-0000c9d0: 6f72 2064 6574 6169 6c73 2061 626f 7574  or details about
-0000c9e0: 2077 6f72 6b69 6e67 2077 6974 6820 666f   working with fo
-0000c9f0: 726d 2069 6e70 7574 732c 2073 6565 2060  rm inputs, see `
-0000ca00: 5265 6365 6976 650a 2020 2020 2020 2020  Receive.        
-0000ca10: 2020 2020 666f 726d 0a20 2020 2020 2020      form.       
-0000ca20: 2020 2020 2064 6174 6120 3c68 7474 7073       data <https
-0000ca30: 3a2f 2f64 6576 656c 6f70 6572 732e 676f  ://developers.go
-0000ca40: 6f67 6c65 2e63 6f6d 2f63 6861 742f 7569  ogle.com/chat/ui
-0000ca50: 2f72 6561 642d 666f 726d 2d64 6174 613e  /read-form-data>
-0000ca60: 605f 5f2e 0a20 2020 2020 2020 206d 756c  `__..        mul
-0000ca70: 7469 5f73 656c 6563 745f 6d61 785f 7365  ti_select_max_se
-0000ca80: 6c65 6374 6564 5f69 7465 6d73 2028 696e  lected_items (in
-0000ca90: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
-0000caa0: 466f 7220 6d75 6c74 6973 656c 6563 7420  For multiselect 
-0000cab0: 6d65 6e75 732c 2074 6865 206d 6178 696d  menus, the maxim
-0000cac0: 756d 206e 756d 6265 7220 6f66 0a20 2020  um number of.   
-0000cad0: 2020 2020 2020 2020 2069 7465 6d73 2074           items t
-0000cae0: 6861 7420 6120 7573 6572 2063 616e 2073  hat a user can s
-0000caf0: 656c 6563 742e 204d 696e 696d 756d 2076  elect. Minimum v
-0000cb00: 616c 7565 2069 7320 310a 2020 2020 2020  alue is 1.      
-0000cb10: 2020 2020 2020 6974 656d 2e20 4966 2075        item. If u
-0000cb20: 6e73 7065 6369 6669 6564 2c20 6465 6661  nspecified, defa
-0000cb30: 756c 7473 2074 6f20 3320 6974 656d 732e  ults to 3 items.
-0000cb40: 0a20 2020 2020 2020 206d 756c 7469 5f73  .        multi_s
-0000cb50: 656c 6563 745f 6d69 6e5f 7175 6572 795f  elect_min_query_
-0000cb60: 6c65 6e67 7468 2028 696e 7429 3a0a 2020  length (int):.  
-0000cb70: 2020 2020 2020 2020 2020 466f 7220 6d75            For mu
-0000cb80: 6c74 6973 656c 6563 7420 6d65 6e75 732c  ltiselect menus,
-0000cb90: 2074 6865 206e 756d 6265 7220 6f66 2074   the number of t
-0000cba0: 6578 740a 2020 2020 2020 2020 2020 2020  ext.            
-0000cbb0: 6368 6172 6163 7465 7273 2074 6861 7420  characters that 
-0000cbc0: 6120 7573 6572 2069 6e70 7574 7320 6265  a user inputs be
-0000cbd0: 666f 7265 2074 6865 2043 6861 740a 2020  fore the Chat.  
-0000cbe0: 2020 2020 2020 2020 2020 6170 7020 7175            app qu
-0000cbf0: 6572 6965 7320 6175 746f 636f 6d70 6c65  eries autocomple
-0000cc00: 7465 2061 6e64 2064 6973 706c 6179 7320  te and displays 
-0000cc10: 7375 6767 6573 7465 640a 2020 2020 2020  suggested.      
-0000cc20: 2020 2020 2020 6974 656d 7320 696e 2074        items in t
-0000cc30: 6865 206d 656e 752e 0a0a 2020 2020 2020  he menu...      
-0000cc40: 2020 2020 2020 4966 2075 6e73 7065 6369        If unspeci
-0000cc50: 6669 6564 2c20 6465 6661 756c 7473 2074  fied, defaults t
-0000cc60: 6f20 3020 6368 6172 6163 7465 7273 2066  o 0 characters f
-0000cc70: 6f72 0a20 2020 2020 2020 2020 2020 2073  or.            s
-0000cc80: 7461 7469 6320 6461 7461 2073 6f75 7263  tatic data sourc
-0000cc90: 6573 2061 6e64 2033 2063 6861 7261 6374  es and 3 charact
-0000cca0: 6572 7320 666f 720a 2020 2020 2020 2020  ers for.        
-0000ccb0: 2020 2020 6578 7465 726e 616c 2064 6174      external dat
-0000ccc0: 6120 736f 7572 6365 732e 0a20 2020 2020  a sources..     
-0000ccd0: 2020 2065 7874 6572 6e61 6c5f 6461 7461     external_data
-0000cce0: 5f73 6f75 7263 6520 2867 6f6f 676c 652e  _source (google.
-0000ccf0: 6170 7073 2e63 6172 645f 7631 2e74 7970  apps.card_v1.typ
-0000cd00: 6573 2e41 6374 696f 6e29 3a0a 2020 2020  es.Action):.    
-0000cd10: 2020 2020 2020 2020 416e 2065 7874 6572          An exter
-0000cd20: 6e61 6c20 6461 7461 2073 6f75 7263 652c  nal data source,
-0000cd30: 2073 7563 6820 6173 2061 2072 656c 6174   such as a relat
-0000cd40: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
-0000cd50: 2020 6461 7461 2062 6173 652e 0a0a 2020    data base...  
-0000cd60: 2020 2020 2020 2020 2020 5468 6973 2066            This f
-0000cd70: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
-0000cd80: 206f 6620 606f 6e65 6f66 605f 2060 606d   of `oneof`_ ``m
-0000cd90: 756c 7469 5f73 656c 6563 745f 6461 7461  ulti_select_data
-0000cda0: 5f73 6f75 7263 6560 602e 0a20 2020 2020  _source``..     
-0000cdb0: 2020 2070 6c61 7466 6f72 6d5f 6461 7461     platform_data
-0000cdc0: 5f73 6f75 7263 6520 2867 6f6f 676c 652e  _source (google.
-0000cdd0: 6170 7073 2e63 6172 645f 7631 2e74 7970  apps.card_v1.typ
-0000cde0: 6573 2e53 656c 6563 7469 6f6e 496e 7075  es.SelectionInpu
-0000cdf0: 742e 506c 6174 666f 726d 4461 7461 536f  t.PlatformDataSo
-0000ce00: 7572 6365 293a 0a20 2020 2020 2020 2020  urce):.         
-0000ce10: 2020 2041 2064 6174 6120 736f 7572 6365     A data source
-0000ce20: 2066 726f 6d20 476f 6f67 6c65 2057 6f72   from Google Wor
-0000ce30: 6b73 7061 6365 2e0a 0a20 2020 2020 2020  kspace...       
-0000ce40: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
-0000ce50: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
-0000ce60: 6f6e 656f 6660 5f20 6060 6d75 6c74 695f  oneof`_ ``multi_
-0000ce70: 7365 6c65 6374 5f64 6174 615f 736f 7572  select_data_sour
-0000ce80: 6365 6060 2e0a 2020 2020 2222 220a 0a20  ce``..    """.. 
-0000ce90: 2020 2063 6c61 7373 2053 656c 6563 7469     class Selecti
-0000cea0: 6f6e 5479 7065 2870 726f 746f 2e45 6e75  onType(proto.Enu
-0000ceb0: 6d29 3a0a 2020 2020 2020 2020 7222 2222  m):.        r"""
-0000cec0: 5468 6520 666f 726d 6174 2066 6f72 2074  The format for t
-0000ced0: 6865 2069 7465 6d73 2074 6861 7420 7573  he items that us
-0000cee0: 6572 7320 6361 6e20 7365 6c65 6374 2e20  ers can select. 
-0000cef0: 4469 6666 6572 656e 7420 6f70 7469 6f6e  Different option
-0000cf00: 730a 2020 2020 2020 2020 7375 7070 6f72  s.        suppor
-0000cf10: 7420 6469 6666 6572 656e 7420 7479 7065  t different type
-0000cf20: 7320 6f66 2069 6e74 6572 6163 7469 6f6e  s of interaction
-0000cf30: 732e 2046 6f72 2065 7861 6d70 6c65 2c20  s. For example, 
-0000cf40: 7573 6572 7320 6361 6e0a 2020 2020 2020  users can.      
-0000cf50: 2020 7365 6c65 6374 206d 756c 7469 706c    select multipl
-0000cf60: 6520 6368 6563 6b62 6f78 6573 2c20 6275  e checkboxes, bu
-0000cf70: 7420 6361 6e20 6f6e 6c79 2073 656c 6563  t can only selec
-0000cf80: 7420 6f6e 6520 6974 656d 2066 726f 6d20  t one item from 
-0000cf90: 610a 2020 2020 2020 2020 6472 6f70 646f  a.        dropdo
-0000cfa0: 776e 206d 656e 752e 0a0a 2020 2020 2020  wn menu...      
-0000cfb0: 2020 4561 6368 2073 656c 6563 7469 6f6e    Each selection
-0000cfc0: 2069 6e70 7574 2073 7570 706f 7274 7320   input supports 
-0000cfd0: 6f6e 6520 7479 7065 206f 6620 7365 6c65  one type of sele
-0000cfe0: 6374 696f 6e2e 204d 6978 696e 670a 2020  ction. Mixing.  
-0000cff0: 2020 2020 2020 6368 6563 6b62 6f78 6573        checkboxes
-0000d000: 2061 6e64 2073 7769 7463 6865 732c 2066   and switches, f
-0000d010: 6f72 2065 7861 6d70 6c65 2c20 6973 6e27  or example, isn'
-0000d020: 7420 7375 7070 6f72 7465 642e 0a0a 2020  t supported...  
-0000d030: 2020 2020 2020 6047 6f6f 676c 6520 576f        `Google Wo
-0000d040: 726b 7370 6163 6520 4164 642d 6f6e 7320  rkspace Add-ons 
-0000d050: 616e 6420 4368 6174 0a20 2020 2020 2020  and Chat.       
-0000d060: 2061 7070 7320 3c68 7474 7073 3a2f 2f64   apps <https://d
-0000d070: 6576 656c 6f70 6572 732e 676f 6f67 6c65  evelopers.google
-0000d080: 2e63 6f6d 2f77 6f72 6b73 7061 6365 2f65  .com/workspace/e
-0000d090: 7874 656e 643e 605f 5f3a 0a0a 2020 2020  xtend>`__:..    
-0000d0a0: 2020 2020 5661 6c75 6573 3a0a 2020 2020      Values:.    
-0000d0b0: 2020 2020 2020 2020 4348 4543 4b5f 424f          CHECK_BO
-0000d0c0: 5820 2830 293a 0a20 2020 2020 2020 2020  X (0):.         
-0000d0d0: 2020 2020 2020 2041 2073 6574 206f 6620         A set of 
-0000d0e0: 6368 6563 6b62 6f78 6573 2e20 5573 6572  checkboxes. User
-0000d0f0: 7320 6361 6e20 7365 6c65 6374 206f 6e65  s can select one
-0000d100: 206f 720a 2020 2020 2020 2020 2020 2020   or.            
-0000d110: 2020 2020 6d6f 7265 2063 6865 636b 626f      more checkbo
-0000d120: 7865 732e 0a20 2020 2020 2020 2020 2020  xes..           
-0000d130: 2052 4144 494f 5f42 5554 544f 4e20 2831   RADIO_BUTTON (1
-0000d140: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000d150: 2020 2041 2073 6574 206f 6620 7261 6469     A set of radi
-0000d160: 6f20 6275 7474 6f6e 732e 2055 7365 7273  o buttons. Users
-0000d170: 2063 616e 2073 656c 6563 7420 6f6e 650a   can select one.
-0000d180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d190: 7261 6469 6f20 6275 7474 6f6e 2e0a 2020  radio button..  
-0000d1a0: 2020 2020 2020 2020 2020 5357 4954 4348            SWITCH
-0000d1b0: 2028 3229 3a0a 2020 2020 2020 2020 2020   (2):.          
-0000d1c0: 2020 2020 2020 4120 7365 7420 6f66 2073        A set of s
-0000d1d0: 7769 7463 6865 732e 2055 7365 7273 2063  witches. Users c
-0000d1e0: 616e 2074 7572 6e20 6f6e 206f 6e65 206f  an turn on one o
-0000d1f0: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
-0000d200: 2020 6d6f 7265 2073 7769 7463 6865 732e    more switches.
-0000d210: 0a20 2020 2020 2020 2020 2020 2044 524f  .            DRO
-0000d220: 5044 4f57 4e20 2833 293a 0a20 2020 2020  PDOWN (3):.     
-0000d230: 2020 2020 2020 2020 2020 2041 2064 726f             A dro
-0000d240: 7064 6f77 6e20 6d65 6e75 2e20 5573 6572  pdown menu. User
-0000d250: 7320 6361 6e20 7365 6c65 6374 206f 6e65  s can select one
-0000d260: 2069 7465 6d0a 2020 2020 2020 2020 2020   item.          
-0000d270: 2020 2020 2020 6672 6f6d 2074 6865 206d        from the m
-0000d280: 656e 752e 0a20 2020 2020 2020 2020 2020  enu..           
-0000d290: 204d 554c 5449 5f53 454c 4543 5420 2834   MULTI_SELECT (4
-0000d2a0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000d2b0: 2020 2041 206d 756c 7469 7365 6c65 6374     A multiselect
-0000d2c0: 206d 656e 7520 666f 7220 7374 6174 6963   menu for static
-0000d2d0: 206f 7220 6479 6e61 6d69 6320 6461 7461   or dynamic data
-0000d2e0: 2e20 4672 6f6d 2074 6865 206d 656e 750a  . From the menu.
-0000d2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d300: 6261 722c 2075 7365 7273 2073 656c 6563  bar, users selec
-0000d310: 7420 6f6e 6520 6f72 206d 6f72 6520 6974  t one or more it
-0000d320: 656d 732e 2055 7365 7273 2063 616e 2061  ems. Users can a
-0000d330: 6c73 6f20 696e 7075 740a 2020 2020 2020  lso input.      
-0000d340: 2020 2020 2020 2020 2020 7661 6c75 6573            values
-0000d350: 2074 6f20 706f 7075 6c61 7465 2064 796e   to populate dyn
-0000d360: 616d 6963 2064 6174 612e 2046 6f72 2065  amic data. For e
-0000d370: 7861 6d70 6c65 2c20 7573 6572 7320 6361  xample, users ca
-0000d380: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-0000d390: 2020 7374 6172 7420 7479 7069 6e67 2074    start typing t
-0000d3a0: 6865 206e 616d 6520 6f66 2061 2047 6f6f  he name of a Goo
-0000d3b0: 676c 6520 4368 6174 2073 7061 6365 2061  gle Chat space a
-0000d3c0: 6e64 2074 6865 2077 6964 6765 740a 2020  nd the widget.  
-0000d3d0: 2020 2020 2020 2020 2020 2020 2020 6175                au
-0000d3e0: 746f 7375 6767 6573 7473 2074 6865 2073  tosuggests the s
-0000d3f0: 7061 6365 2e0a 0a20 2020 2020 2020 2020  pace...         
-0000d400: 2020 2020 2020 2054 6f20 706f 7075 6c61         To popula
-0000d410: 7465 2069 7465 6d73 2066 6f72 2061 206d  te items for a m
-0000d420: 756c 7469 7365 6c65 6374 206d 656e 752c  ultiselect menu,
-0000d430: 2079 6f75 2063 616e 2075 7365 206f 6e65   you can use one
-0000d440: 206f 660a 2020 2020 2020 2020 2020 2020   of.            
-0000d450: 2020 2020 7468 6520 666f 6c6c 6f77 696e      the followin
-0000d460: 6720 7479 7065 7320 6f66 2064 6174 6120  g types of data 
-0000d470: 736f 7572 6365 733a 0a0a 2020 2020 2020  sources:..      
-0000d480: 2020 2020 2020 2020 2020 2d20 2053 7461            -  Sta
-0000d490: 7469 6320 6461 7461 3a20 4974 656d 7320  tic data: Items 
-0000d4a0: 6172 6520 7370 6563 6966 6965 6420 6173  are specified as
-0000d4b0: 2060 6053 656c 6563 7469 6f6e 4974 656d   ``SelectionItem
-0000d4c0: 6060 0a20 2020 2020 2020 2020 2020 2020  ``.             
-0000d4d0: 2020 2020 2020 6f62 6a65 6374 7320 696e        objects in
-0000d4e0: 2074 6865 2077 6964 6765 742e 2055 7020   the widget. Up 
-0000d4f0: 746f 2031 3030 2069 7465 6d73 2e0a 2020  to 100 items..  
-0000d500: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
-0000d510: 2047 6f6f 676c 6520 576f 726b 7370 6163   Google Workspac
-0000d520: 6520 6461 7461 3a20 4974 656d 7320 6172  e data: Items ar
-0000d530: 6520 706f 7075 6c61 7465 6420 7573 696e  e populated usin
-0000d540: 6720 6461 7461 0a20 2020 2020 2020 2020  g data.         
-0000d550: 2020 2020 2020 2020 2020 6672 6f6d 2047            from G
-0000d560: 6f6f 676c 6520 576f 726b 7370 6163 652c  oogle Workspace,
-0000d570: 2073 7563 6820 6173 2047 6f6f 676c 6520   such as Google 
-0000d580: 576f 726b 7370 6163 6520 7573 6572 7320  Workspace users 
-0000d590: 6f72 0a20 2020 2020 2020 2020 2020 2020  or.             
-0000d5a0: 2020 2020 2020 476f 6f67 6c65 2043 6861        Google Cha
-0000d5b0: 7420 7370 6163 6573 2e0a 2020 2020 2020  t spaces..      
-0000d5c0: 2020 2020 2020 2020 2020 2d20 2045 7874            -  Ext
-0000d5d0: 6572 6e61 6c20 6461 7461 3a20 4974 656d  ernal data: Item
-0000d5e0: 7320 6172 6520 706f 7075 6c61 7465 6420  s are populated 
-0000d5f0: 6672 6f6d 2061 6e20 6578 7465 726e 616c  from an external
-0000d600: 2064 6174 610a 2020 2020 2020 2020 2020   data.          
-0000d610: 2020 2020 2020 2020 2073 6f75 7263 6520           source 
-0000d620: 6f75 7473 6964 6520 6f66 2047 6f6f 676c  outside of Googl
-0000d630: 6520 576f 726b 7370 6163 652e 0a0a 2020  e Workspace...  
-0000d640: 2020 2020 2020 2020 2020 2020 2020 466f                Fo
-0000d650: 7220 6578 616d 706c 6573 206f 6620 686f  r examples of ho
-0000d660: 7720 746f 2069 6d70 6c65 6d65 6e74 206d  w to implement m
-0000d670: 756c 7469 7365 6c65 6374 206d 656e 7573  ultiselect menus
-0000d680: 2c20 7365 6520 7468 650a 2020 2020 2020  , see the.      
-0000d690: 2020 2020 2020 2020 2020 6060 6053 656c            ```Sel
-0000d6a0: 6563 7469 6f6e 496e 7075 7460 6020 7769  ectionInput`` wi
-0000d6b0: 6467 6574 0a20 2020 2020 2020 2020 2020  dget.           
-0000d6c0: 2020 2020 2070 6167 6520 3c68 7474 7073       page <https
-0000d6d0: 3a2f 2f64 6576 656c 6f70 6572 732e 676f  ://developers.go
-0000d6e0: 6f67 6c65 2e63 6f6d 2f63 6861 742f 7569  ogle.com/chat/ui
-0000d6f0: 2f77 6964 6765 7473 2f73 656c 6563 7469  /widgets/selecti
-0000d700: 6f6e 2d69 6e70 7574 236d 756c 7469 7365  on-input#multise
-0000d710: 6c65 6374 2d6d 656e 753e 605f 5f2e 0a0a  lect-menu>`__...
-0000d720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d730: 6047 6f6f 676c 6520 576f 726b 7370 6163  `Google Workspac
-0000d740: 6520 4164 642d 6f6e 7320 616e 6420 4368  e Add-ons and Ch
-0000d750: 6174 0a20 2020 2020 2020 2020 2020 2020  at.             
-0000d760: 2020 2061 7070 7320 3c68 7474 7073 3a2f     apps <https:/
-0000d770: 2f64 6576 656c 6f70 6572 732e 676f 6f67  /developers.goog
-0000d780: 6c65 2e63 6f6d 2f77 6f72 6b73 7061 6365  le.com/workspace
-0000d790: 2f65 7874 656e 643e 605f 5f3a 0a20 2020  /extend>`__:.   
-0000d7a0: 2020 2020 2020 2020 2020 2020 206d 756c               mul
-0000d7b0: 7469 7365 6c65 6374 2066 6f72 2047 6f6f  tiselect for Goo
-0000d7c0: 676c 6520 576f 726b 7370 6163 6520 4164  gle Workspace Ad
-0000d7d0: 642d 6f6e 7320 6172 6520 696e 2060 4465  d-ons are in `De
-0000d7e0: 7665 6c6f 7065 720a 2020 2020 2020 2020  veloper.        
-0000d7f0: 2020 2020 2020 2020 5072 6576 6965 7720          Preview 
-0000d800: 3c68 7474 7073 3a2f 2f64 6576 656c 6f70  <https://develop
-0000d810: 6572 732e 676f 6f67 6c65 2e63 6f6d 2f77  ers.google.com/w
-0000d820: 6f72 6b73 7061 6365 2f70 7265 7669 6577  orkspace/preview
-0000d830: 3e60 5f5f 2e0a 2020 2020 2020 2020 2222  >`__..        ""
-0000d840: 220a 2020 2020 2020 2020 4348 4543 4b5f  ".        CHECK_
-0000d850: 424f 5820 3d20 300a 2020 2020 2020 2020  BOX = 0.        
-0000d860: 5241 4449 4f5f 4255 5454 4f4e 203d 2031  RADIO_BUTTON = 1
-0000d870: 0a20 2020 2020 2020 2053 5749 5443 4820  .        SWITCH 
-0000d880: 3d20 320a 2020 2020 2020 2020 4452 4f50  = 2.        DROP
-0000d890: 444f 574e 203d 2033 0a20 2020 2020 2020  DOWN = 3.       
-0000d8a0: 204d 554c 5449 5f53 454c 4543 5420 3d20   MULTI_SELECT = 
-0000d8b0: 340a 0a20 2020 2063 6c61 7373 2053 656c  4..    class Sel
-0000d8c0: 6563 7469 6f6e 4974 656d 2870 726f 746f  ectionItem(proto
-0000d8d0: 2e4d 6573 7361 6765 293a 0a20 2020 2020  .Message):.     
-0000d8e0: 2020 2072 2222 2241 6e20 6974 656d 2074     r"""An item t
-0000d8f0: 6861 7420 7573 6572 7320 6361 6e20 7365  hat users can se
-0000d900: 6c65 6374 2069 6e20 6120 7365 6c65 6374  lect in a select
-0000d910: 696f 6e20 696e 7075 742c 2073 7563 6820  ion input, such 
-0000d920: 6173 2061 0a20 2020 2020 2020 2063 6865  as a.        che
-0000d930: 636b 626f 7820 6f72 2073 7769 7463 682e  ckbox or switch.
-0000d940: 0a0a 2020 2020 2020 2020 6047 6f6f 676c  ..        `Googl
-0000d950: 6520 576f 726b 7370 6163 6520 4164 642d  e Workspace Add-
-0000d960: 6f6e 7320 616e 6420 4368 6174 0a20 2020  ons and Chat.   
-0000d970: 2020 2020 2061 7070 7320 3c68 7474 7073       apps <https
-0000d980: 3a2f 2f64 6576 656c 6f70 6572 732e 676f  ://developers.go
-0000d990: 6f67 6c65 2e63 6f6d 2f77 6f72 6b73 7061  ogle.com/workspa
-0000d9a0: 6365 2f65 7874 656e 643e 605f 5f3a 0a0a  ce/extend>`__:..
-0000d9b0: 2020 2020 2020 2020 4174 7472 6962 7574          Attribut
-0000d9c0: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
-0000d9d0: 7465 7874 2028 7374 7229 3a0a 2020 2020  text (str):.    
-0000d9e0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-0000d9f0: 7465 7874 2074 6861 7420 6964 656e 7469  text that identi
-0000da00: 6669 6573 206f 7220 6465 7363 7269 6265  fies or describe
-0000da10: 7320 7468 650a 2020 2020 2020 2020 2020  s the.          
-0000da20: 2020 2020 2020 6974 656d 2074 6f20 7573        item to us
-0000da30: 6572 732e 0a20 2020 2020 2020 2020 2020  ers..           
-0000da40: 2076 616c 7565 2028 7374 7229 3a0a 2020   value (str):.  
-0000da50: 2020 2020 2020 2020 2020 2020 2020 5468                Th
-0000da60: 6520 7661 6c75 6520 6173 736f 6369 6174  e value associat
-0000da70: 6564 2077 6974 6820 7468 6973 2069 7465  ed with this ite
-0000da80: 6d2e 2054 6865 2063 6c69 656e 7420 7368  m. The client sh
-0000da90: 6f75 6c64 2075 7365 0a20 2020 2020 2020  ould use.       
-0000daa0: 2020 2020 2020 2020 2074 6869 7320 6173           this as
-0000dab0: 2061 2066 6f72 6d20 696e 7075 7420 7661   a form input va
-0000dac0: 6c75 652e 0a0a 2020 2020 2020 2020 2020  lue...          
-0000dad0: 2020 2020 2020 466f 7220 6465 7461 696c        For detail
-0000dae0: 7320 6162 6f75 7420 776f 726b 696e 6720  s about working 
-0000daf0: 7769 7468 2066 6f72 6d20 696e 7075 7473  with form inputs
-0000db00: 2c20 7365 6520 6052 6563 6569 7665 0a20  , see `Receive. 
-0000db10: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000db20: 6f72 6d0a 2020 2020 2020 2020 2020 2020  orm.            
-0000db30: 2020 2020 6461 7461 203c 6874 7470 733a      data <https:
-0000db40: 2f2f 6465 7665 6c6f 7065 7273 2e67 6f6f  //developers.goo
-0000db50: 676c 652e 636f 6d2f 6368 6174 2f75 692f  gle.com/chat/ui/
-0000db60: 7265 6164 2d66 6f72 6d2d 6461 7461 3e60  read-form-data>`
-0000db70: 5f5f 2e0a 2020 2020 2020 2020 2020 2020  __..            
-0000db80: 7365 6c65 6374 6564 2028 626f 6f6c 293a  selected (bool):
-0000db90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dba0: 2057 6865 7468 6572 2074 6865 2069 7465   Whether the ite
-0000dbb0: 6d20 6973 2073 656c 6563 7465 6420 6279  m is selected by
-0000dbc0: 2064 6566 6175 6c74 2e20 4966 0a20 2020   default. If.   
-0000dbd0: 2020 2020 2020 2020 2020 2020 2074 6865               the
-0000dbe0: 2073 656c 6563 7469 6f6e 2069 6e70 7574   selection input
-0000dbf0: 206f 6e6c 7920 6163 6365 7074 7320 6f6e   only accepts on
-0000dc00: 6520 7661 6c75 6520 2873 7563 680a 2020  e value (such.  
-0000dc10: 2020 2020 2020 2020 2020 2020 2020 6173                as
-0000dc20: 2066 6f72 2072 6164 696f 2062 7574 746f   for radio butto
-0000dc30: 6e73 206f 7220 6120 6472 6f70 646f 776e  ns or a dropdown
-0000dc40: 206d 656e 7529 2c20 6f6e 6c79 0a20 2020   menu), only.   
-0000dc50: 2020 2020 2020 2020 2020 2020 2073 6574               set
-0000dc60: 2074 6869 7320 6669 656c 6420 666f 7220   this field for 
-0000dc70: 6f6e 6520 6974 656d 2e0a 2020 2020 2020  one item..      
-0000dc80: 2020 2020 2020 7374 6172 745f 6963 6f6e        start_icon
-0000dc90: 5f75 7269 2028 7374 7229 3a0a 2020 2020  _uri (str):.    
-0000dca0: 2020 2020 2020 2020 2020 2020 466f 7220              For 
-0000dcb0: 6d75 6c74 6973 656c 6563 7420 6d65 6e75  multiselect menu
-0000dcc0: 732c 2074 6865 2055 524c 2066 6f72 2074  s, the URL for t
-0000dcd0: 6865 2069 636f 6e20 6469 7370 6c61 7965  he icon displaye
-0000dce0: 6420 6e65 7874 0a20 2020 2020 2020 2020  d next.         
-0000dcf0: 2020 2020 2020 2074 6f20 7468 6520 6974         to the it
-0000dd00: 656d 2773 2060 6074 6578 7460 6020 6669  em's ``text`` fi
-0000dd10: 656c 642e 2053 7570 706f 7274 7320 504e  eld. Supports PN
-0000dd20: 4720 616e 6420 4a50 4547 2066 696c 6573  G and JPEG files
-0000dd30: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000dd40: 2020 4d75 7374 2062 6520 616e 2060 6048    Must be an ``H
-0000dd50: 5454 5053 6060 2055 524c 2e20 466f 7220  TTPS`` URL. For 
-0000dd60: 6578 616d 706c 652c 0a20 2020 2020 2020  example,.       
-0000dd70: 2020 2020 2020 2020 2060 6068 7474 7073           ``https
-0000dd80: 3a2f 2f64 6576 656c 6f70 6572 732e 676f  ://developers.go
-0000dd90: 6f67 6c65 2e63 6f6d 2f63 6861 742f 696d  ogle.com/chat/im
-0000dda0: 6167 6573 2f71 7569 636b 7374 6172 742d  ages/quickstart-
-0000ddb0: 6170 702d 6176 6174 6172 2e70 6e67 6060  app-avatar.png``
-0000ddc0: 2e0a 2020 2020 2020 2020 2020 2020 626f  ..            bo
-0000ddd0: 7474 6f6d 5f74 6578 7420 2873 7472 293a  ttom_text (str):
-0000dde0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ddf0: 2046 6f72 206d 756c 7469 7365 6c65 6374   For multiselect
-0000de00: 206d 656e 7573 2c20 6120 7465 7874 2064   menus, a text d
-0000de10: 6573 6372 6970 7469 6f6e 206f 7220 6c61  escription or la
-0000de20: 6265 6c20 7468 6174 2773 0a20 2020 2020  bel that's.     
-0000de30: 2020 2020 2020 2020 2020 2064 6973 706c             displ
-0000de40: 6179 6564 2062 656c 6f77 2074 6865 2069  ayed below the i
-0000de50: 7465 6d27 7320 6060 7465 7874 6060 2066  tem's ``text`` f
-0000de60: 6965 6c64 2e0a 2020 2020 2020 2020 2222  ield..        ""
-0000de70: 220a 0a20 2020 2020 2020 2074 6578 743a  "..        text:
-0000de80: 2073 7472 203d 2070 726f 746f 2e46 6965   str = proto.Fie
-0000de90: 6c64 280a 2020 2020 2020 2020 2020 2020  ld(.            
-0000dea0: 7072 6f74 6f2e 5354 5249 4e47 2c0a 2020  proto.STRING,.  
-0000deb0: 2020 2020 2020 2020 2020 6e75 6d62 6572            number
-0000dec0: 3d31 2c0a 2020 2020 2020 2020 290a 2020  =1,.        ).  
-0000ded0: 2020 2020 2020 7661 6c75 653a 2073 7472        value: str
-0000dee0: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
-0000def0: 2020 2020 2020 2020 2020 2020 7072 6f74              prot
-0000df00: 6f2e 5354 5249 4e47 2c0a 2020 2020 2020  o.STRING,.      
-0000df10: 2020 2020 2020 6e75 6d62 6572 3d32 2c0a        number=2,.
-0000df20: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000df30: 2020 7365 6c65 6374 6564 3a20 626f 6f6c    selected: bool
-0000df40: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
-0000df50: 2020 2020 2020 2020 2020 2020 7072 6f74              prot
-0000df60: 6f2e 424f 4f4c 2c0a 2020 2020 2020 2020  o.BOOL,.        
-0000df70: 2020 2020 6e75 6d62 6572 3d33 2c0a 2020      number=3,.  
-0000df80: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000df90: 7374 6172 745f 6963 6f6e 5f75 7269 3a20  start_icon_uri: 
-0000dfa0: 7374 7220 3d20 7072 6f74 6f2e 4669 656c  str = proto.Fiel
-0000dfb0: 6428 0a20 2020 2020 2020 2020 2020 2070  d(.            p
-0000dfc0: 726f 746f 2e53 5452 494e 472c 0a20 2020  roto.STRING,.   
-0000dfd0: 2020 2020 2020 2020 206e 756d 6265 723d           number=
-0000dfe0: 342c 0a20 2020 2020 2020 2029 0a20 2020  4,.        ).   
-0000dff0: 2020 2020 2062 6f74 746f 6d5f 7465 7874       bottom_text
-0000e000: 3a20 7374 7220 3d20 7072 6f74 6f2e 4669  : str = proto.Fi
-0000e010: 656c 6428 0a20 2020 2020 2020 2020 2020  eld(.           
-0000e020: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
-0000e030: 2020 2020 2020 2020 2020 206e 756d 6265             numbe
-0000e040: 723d 352c 0a20 2020 2020 2020 2029 0a0a  r=5,.        )..
-0000e050: 2020 2020 636c 6173 7320 506c 6174 666f      class Platfo
-0000e060: 726d 4461 7461 536f 7572 6365 2870 726f  rmDataSource(pro
-0000e070: 746f 2e4d 6573 7361 6765 293a 0a20 2020  to.Message):.   
-0000e080: 2020 2020 2072 2222 2246 6f72 2061 205b       r"""For a [
-0000e090: 6060 5365 6c65 6374 696f 6e49 6e70 7574  ``SelectionInput
-0000e0a0: 6060 5d5b 676f 6f67 6c65 2e61 7070 732e  ``][google.apps.
-0000e0b0: 6361 7264 2e76 312e 5365 6c65 6374 696f  card.v1.Selectio
-0000e0c0: 6e49 6e70 7574 5d0a 2020 2020 2020 2020  nInput].        
-0000e0d0: 7769 6467 6574 2074 6861 7420 7573 6573  widget that uses
-0000e0e0: 2061 206d 756c 7469 7365 6c65 6374 206d   a multiselect m
-0000e0f0: 656e 752c 2061 2064 6174 6120 736f 7572  enu, a data sour
-0000e100: 6365 2066 726f 6d20 476f 6f67 6c65 0a20  ce from Google. 
-0000e110: 2020 2020 2020 2057 6f72 6b73 7061 6365         Workspace
-0000e120: 2e20 5573 6564 2074 6f20 706f 7075 6c61  . Used to popula
-0000e130: 7465 2069 7465 6d73 2069 6e20 6120 6d75  te items in a mu
-0000e140: 6c74 6973 656c 6563 7420 6d65 6e75 2e0a  ltiselect menu..
-0000e150: 0a20 2020 2020 2020 2060 476f 6f67 6c65  .        `Google
-0000e160: 2043 6861 7420 6170 7073 203c 6874 7470   Chat apps <http
-0000e170: 733a 2f2f 6465 7665 6c6f 7065 7273 2e67  s://developers.g
-0000e180: 6f6f 676c 652e 636f 6d2f 6368 6174 3e60  oogle.com/chat>`
-0000e190: 5f5f 3a0a 0a0a 2020 2020 2020 2020 2e2e  __:...        ..
-0000e1a0: 205f 6f6e 656f 663a 2068 7474 7073 3a2f   _oneof: https:/
-0000e1b0: 2f70 726f 746f 2d70 6c75 732d 7079 7468  /proto-plus-pyth
-0000e1c0: 6f6e 2e72 6561 6474 6865 646f 6373 2e69  on.readthedocs.i
-0000e1d0: 6f2f 656e 2f73 7461 626c 652f 6669 656c  o/en/stable/fiel
-0000e1e0: 6473 2e68 746d 6c23 6f6e 656f 6673 2d6d  ds.html#oneofs-m
-0000e1f0: 7574 7561 6c6c 792d 6578 636c 7573 6976  utually-exclusiv
-0000e200: 652d 6669 656c 6473 0a0a 2020 2020 2020  e-fields..      
-0000e210: 2020 4174 7472 6962 7574 6573 3a0a 2020    Attributes:.  
-0000e220: 2020 2020 2020 2020 2020 636f 6d6d 6f6e            common
-0000e230: 5f64 6174 615f 736f 7572 6365 2028 676f  _data_source (go
-0000e240: 6f67 6c65 2e61 7070 732e 6361 7264 5f76  ogle.apps.card_v
-0000e250: 312e 7479 7065 732e 5365 6c65 6374 696f  1.types.Selectio
-0000e260: 6e49 6e70 7574 2e50 6c61 7466 6f72 6d44  nInput.PlatformD
-0000e270: 6174 6153 6f75 7263 652e 436f 6d6d 6f6e  ataSource.Common
-0000e280: 4461 7461 536f 7572 6365 293a 0a20 2020  DataSource):.   
-0000e290: 2020 2020 2020 2020 2020 2020 2041 2064               A d
-0000e2a0: 6174 6120 736f 7572 6365 2073 6861 7265  ata source share
-0000e2b0: 6420 6279 2061 6c6c 2047 6f6f 676c 6520  d by all Google 
-0000e2c0: 576f 726b 7370 6163 650a 2020 2020 2020  Workspace.      
-0000e2d0: 2020 2020 2020 2020 2020 6170 706c 6963            applic
-0000e2e0: 6174 696f 6e73 2c20 7375 6368 2061 7320  ations, such as 
-0000e2f0: 7573 6572 7320 696e 2061 2047 6f6f 676c  users in a Googl
-0000e300: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-0000e310: 2020 576f 726b 7370 6163 6520 6f72 6761    Workspace orga
-0000e320: 6e69 7a61 7469 6f6e 2e0a 0a20 2020 2020  nization...     
-0000e330: 2020 2020 2020 2020 2020 2054 6869 7320             This 
-0000e340: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
-0000e350: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
-0000e360: 6461 7461 5f73 6f75 7263 6560 602e 0a20  data_source``.. 
-0000e370: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
-0000e380: 2020 2020 636c 6173 7320 436f 6d6d 6f6e      class Common
-0000e390: 4461 7461 536f 7572 6365 2870 726f 746f  DataSource(proto
-0000e3a0: 2e45 6e75 6d29 3a0a 2020 2020 2020 2020  .Enum):.        
-0000e3b0: 2020 2020 7222 2222 4120 6461 7461 2073      r"""A data s
-0000e3c0: 6f75 7263 6520 7368 6172 6564 2062 7920  ource shared by 
-0000e3d0: 616c 6c20 5b47 6f6f 676c 6520 576f 726b  all [Google Work
-0000e3e0: 7370 6163 6520 6170 706c 6963 6174 696f  space applicatio
-0000e3f0: 6e73 5d0a 2020 2020 2020 2020 2020 2020  ns].            
-0000e400: 2868 7474 7073 3a2f 2f64 6576 656c 6f70  (https://develop
-0000e410: 6572 732e 676f 6f67 6c65 2e63 6f6d 2f63  ers.google.com/c
-0000e420: 6861 742f 6170 692f 7265 6665 7265 6e63  hat/api/referenc
-0000e430: 652f 7265 7374 2f76 312f 486f 7374 4170  e/rest/v1/HostAp
-0000e440: 7029 2e0a 0a20 2020 2020 2020 2020 2020  p)...           
-0000e450: 2060 476f 6f67 6c65 2043 6861 7420 6170   `Google Chat ap
-0000e460: 7073 203c 6874 7470 733a 2f2f 6465 7665  ps <https://deve
-0000e470: 6c6f 7065 7273 2e67 6f6f 676c 652e 636f  lopers.google.co
-0000e480: 6d2f 6368 6174 3e60 5f5f 3a0a 0a20 2020  m/chat>`__:..   
-0000e490: 2020 2020 2020 2020 2056 616c 7565 733a           Values:
-0000e4a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e4b0: 2055 4e4b 4e4f 574e 2028 3029 3a0a 2020   UNKNOWN (0):.  
-0000e4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e4d0: 2020 4465 6661 756c 7420 7661 6c75 652e    Default value.
-0000e4e0: 2044 6f6e 2774 2075 7365 2e0a 2020 2020   Don't use..    
-0000e4f0: 2020 2020 2020 2020 2020 2020 5553 4552              USER
-0000e500: 2028 3129 3a0a 2020 2020 2020 2020 2020   (1):.          
-0000e510: 2020 2020 2020 2020 2020 476f 6f67 6c65            Google
-0000e520: 2057 6f72 6b73 7061 6365 2075 7365 7273   Workspace users
-0000e530: 2e20 5468 6520 7573 6572 2063 616e 206f  . The user can o
-0000e540: 6e6c 790a 2020 2020 2020 2020 2020 2020  nly.            
-0000e550: 2020 2020 2020 2020 7669 6577 2061 6e64          view and
-0000e560: 2073 656c 6563 7420 7573 6572 7320 6672   select users fr
-0000e570: 6f6d 2074 6865 6972 2047 6f6f 676c 650a  om their Google.
-0000e580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e590: 2020 2020 576f 726b 7370 6163 6520 6f72      Workspace or
-0000e5a0: 6761 6e69 7a61 7469 6f6e 2e0a 2020 2020  ganization..    
-0000e5b0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000e5c0: 2020 2020 2020 2020 554e 4b4e 4f57 4e20          UNKNOWN 
-0000e5d0: 3d20 300a 2020 2020 2020 2020 2020 2020  = 0.            
-0000e5e0: 5553 4552 203d 2031 0a0a 2020 2020 2020  USER = 1..      
-0000e5f0: 2020 636f 6d6d 6f6e 5f64 6174 615f 736f    common_data_so
-0000e600: 7572 6365 3a20 2253 656c 6563 7469 6f6e  urce: "Selection
-0000e610: 496e 7075 742e 506c 6174 666f 726d 4461  Input.PlatformDa
-0000e620: 7461 536f 7572 6365 2e43 6f6d 6d6f 6e44  taSource.CommonD
-0000e630: 6174 6153 6f75 7263 6522 203d 2028 0a20  ataSource" = (. 
-0000e640: 2020 2020 2020 2020 2020 2070 726f 746f             proto
-0000e650: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
-0000e660: 2020 2020 2020 2020 7072 6f74 6f2e 454e          proto.EN
-0000e670: 554d 2c0a 2020 2020 2020 2020 2020 2020  UM,.            
-0000e680: 2020 2020 6e75 6d62 6572 3d31 2c0a 2020      number=1,.  
-0000e690: 2020 2020 2020 2020 2020 2020 2020 6f6e                on
-0000e6a0: 656f 663d 2264 6174 615f 736f 7572 6365  eof="data_source
-0000e6b0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-0000e6c0: 2020 2065 6e75 6d3d 2253 656c 6563 7469     enum="Selecti
-0000e6d0: 6f6e 496e 7075 742e 506c 6174 666f 726d  onInput.Platform
-0000e6e0: 4461 7461 536f 7572 6365 2e43 6f6d 6d6f  DataSource.Commo
-0000e6f0: 6e44 6174 6153 6f75 7263 6522 2c0a 2020  nDataSource",.  
-0000e700: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000e710: 2020 2020 290a 0a20 2020 206e 616d 653a      )..    name:
-0000e720: 2073 7472 203d 2070 726f 746f 2e46 6965   str = proto.Fie
-0000e730: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
-0000e740: 6f2e 5354 5249 4e47 2c0a 2020 2020 2020  o.STRING,.      
-0000e750: 2020 6e75 6d62 6572 3d31 2c0a 2020 2020    number=1,.    
-0000e760: 290a 2020 2020 6c61 6265 6c3a 2073 7472  ).    label: str
-0000e770: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
-0000e780: 2020 2020 2020 2020 7072 6f74 6f2e 5354          proto.ST
-0000e790: 5249 4e47 2c0a 2020 2020 2020 2020 6e75  RING,.        nu
-0000e7a0: 6d62 6572 3d32 2c0a 2020 2020 290a 2020  mber=2,.    ).  
-0000e7b0: 2020 7479 7065 5f3a 2053 656c 6563 7469    type_: Selecti
-0000e7c0: 6f6e 5479 7065 203d 2070 726f 746f 2e46  onType = proto.F
-0000e7d0: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
-0000e7e0: 6f74 6f2e 454e 554d 2c0a 2020 2020 2020  oto.ENUM,.      
-0000e7f0: 2020 6e75 6d62 6572 3d33 2c0a 2020 2020    number=3,.    
-0000e800: 2020 2020 656e 756d 3d53 656c 6563 7469      enum=Selecti
-0000e810: 6f6e 5479 7065 2c0a 2020 2020 290a 2020  onType,.    ).  
-0000e820: 2020 6974 656d 733a 204d 7574 6162 6c65    items: Mutable
-0000e830: 5365 7175 656e 6365 5b53 656c 6563 7469  Sequence[Selecti
-0000e840: 6f6e 4974 656d 5d20 3d20 7072 6f74 6f2e  onItem] = proto.
-0000e850: 5265 7065 6174 6564 4669 656c 6428 0a20  RepeatedField(. 
-0000e860: 2020 2020 2020 2070 726f 746f 2e4d 4553         proto.MES
-0000e870: 5341 4745 2c0a 2020 2020 2020 2020 6e75  SAGE,.        nu
-0000e880: 6d62 6572 3d34 2c0a 2020 2020 2020 2020  mber=4,.        
-0000e890: 6d65 7373 6167 653d 5365 6c65 6374 696f  message=Selectio
-0000e8a0: 6e49 7465 6d2c 0a20 2020 2029 0a20 2020  nItem,.    ).   
-0000e8b0: 206f 6e5f 6368 616e 6765 5f61 6374 696f   on_change_actio
-0000e8c0: 6e3a 2022 4163 7469 6f6e 2220 3d20 7072  n: "Action" = pr
-0000e8d0: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
-0000e8e0: 2020 2070 726f 746f 2e4d 4553 5341 4745     proto.MESSAGE
-0000e8f0: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
-0000e900: 3d35 2c0a 2020 2020 2020 2020 6d65 7373  =5,.        mess
-0000e910: 6167 653d 2241 6374 696f 6e22 2c0a 2020  age="Action",.  
-0000e920: 2020 290a 2020 2020 6d75 6c74 695f 7365    ).    multi_se
-0000e930: 6c65 6374 5f6d 6178 5f73 656c 6563 7465  lect_max_selecte
-0000e940: 645f 6974 656d 733a 2069 6e74 203d 2070  d_items: int = p
-0000e950: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
-0000e960: 2020 2020 7072 6f74 6f2e 494e 5433 322c      proto.INT32,
-0000e970: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
-0000e980: 362c 0a20 2020 2029 0a20 2020 206d 756c  6,.    ).    mul
-0000e990: 7469 5f73 656c 6563 745f 6d69 6e5f 7175  ti_select_min_qu
-0000e9a0: 6572 795f 6c65 6e67 7468 3a20 696e 7420  ery_length: int 
-0000e9b0: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
-0000e9c0: 2020 2020 2020 2070 726f 746f 2e49 4e54         proto.INT
-0000e9d0: 3332 2c0a 2020 2020 2020 2020 6e75 6d62  32,.        numb
-0000e9e0: 6572 3d37 2c0a 2020 2020 290a 2020 2020  er=7,.    ).    
-0000e9f0: 6578 7465 726e 616c 5f64 6174 615f 736f  external_data_so
-0000ea00: 7572 6365 3a20 2241 6374 696f 6e22 203d  urce: "Action" =
-0000ea10: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
-0000ea20: 2020 2020 2020 7072 6f74 6f2e 4d45 5353        proto.MESS
-0000ea30: 4147 452c 0a20 2020 2020 2020 206e 756d  AGE,.        num
-0000ea40: 6265 723d 382c 0a20 2020 2020 2020 206f  ber=8,.        o
-0000ea50: 6e65 6f66 3d22 6d75 6c74 695f 7365 6c65  neof="multi_sele
-0000ea60: 6374 5f64 6174 615f 736f 7572 6365 222c  ct_data_source",
-0000ea70: 0a20 2020 2020 2020 206d 6573 7361 6765  .        message
-0000ea80: 3d22 4163 7469 6f6e 222c 0a20 2020 2029  ="Action",.    )
-0000ea90: 0a20 2020 2070 6c61 7466 6f72 6d5f 6461  .    platform_da
-0000eaa0: 7461 5f73 6f75 7263 653a 2050 6c61 7466  ta_source: Platf
-0000eab0: 6f72 6d44 6174 6153 6f75 7263 6520 3d20  ormDataSource = 
-0000eac0: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
-0000ead0: 2020 2020 2070 726f 746f 2e4d 4553 5341       proto.MESSA
-0000eae0: 4745 2c0a 2020 2020 2020 2020 6e75 6d62  GE,.        numb
-0000eaf0: 6572 3d39 2c0a 2020 2020 2020 2020 6f6e  er=9,.        on
-0000eb00: 656f 663d 226d 756c 7469 5f73 656c 6563  eof="multi_selec
-0000eb10: 745f 6461 7461 5f73 6f75 7263 6522 2c0a  t_data_source",.
-0000eb20: 2020 2020 2020 2020 6d65 7373 6167 653d          message=
-0000eb30: 506c 6174 666f 726d 4461 7461 536f 7572  PlatformDataSour
-0000eb40: 6365 2c0a 2020 2020 290a 0a0a 636c 6173  ce,.    )...clas
-0000eb50: 7320 4461 7465 5469 6d65 5069 636b 6572  s DateTimePicker
-0000eb60: 2870 726f 746f 2e4d 6573 7361 6765 293a  (proto.Message):
-0000eb70: 0a20 2020 2072 2222 224c 6574 7320 7573  .    r"""Lets us
-0000eb80: 6572 7320 696e 7075 7420 6120 6461 7465  ers input a date
-0000eb90: 2c20 6120 7469 6d65 2c20 6f72 2062 6f74  , a time, or bot
-0000eba0: 6820 6120 6461 7465 2061 6e64 2061 2074  h a date and a t
-0000ebb0: 696d 652e 2046 6f72 2061 6e0a 2020 2020  ime. For an.    
-0000ebc0: 6578 616d 706c 6520 696e 2047 6f6f 676c  example in Googl
-0000ebd0: 6520 4368 6174 2061 7070 732c 2073 6565  e Chat apps, see
-0000ebe0: 2060 4461 7465 2074 696d 650a 2020 2020   `Date time.    
-0000ebf0: 7069 636b 6572 203c 6874 7470 733a 2f2f  picker <https://
-0000ec00: 6465 7665 6c6f 7065 7273 2e67 6f6f 676c  developers.googl
-0000ec10: 652e 636f 6d2f 6368 6174 2f75 692f 7769  e.com/chat/ui/wi
-0000ec20: 6467 6574 732f 6461 7465 2d74 696d 652d  dgets/date-time-
-0000ec30: 7069 636b 6572 3e60 5f5f 2e0a 0a20 2020  picker>`__...   
-0000ec40: 2055 7365 7273 2063 616e 2069 6e70 7574   Users can input
-0000ec50: 2074 6578 7420 6f72 2075 7365 2074 6865   text or use the
-0000ec60: 2070 6963 6b65 7220 746f 2073 656c 6563   picker to selec
-0000ec70: 7420 6461 7465 7320 616e 6420 7469 6d65  t dates and time
-0000ec80: 732e 2049 660a 2020 2020 7573 6572 7320  s. If.    users 
-0000ec90: 696e 7075 7420 616e 2069 6e76 616c 6964  input an invalid
-0000eca0: 2064 6174 6520 6f72 2074 696d 652c 2074   date or time, t
-0000ecb0: 6865 2070 6963 6b65 7220 7368 6f77 7320  he picker shows 
-0000ecc0: 616e 2065 7272 6f72 2074 6861 740a 2020  an error that.  
-0000ecd0: 2020 7072 6f6d 7074 7320 7573 6572 7320    prompts users 
-0000ece0: 746f 2069 6e70 7574 2074 6865 2069 6e66  to input the inf
-0000ecf0: 6f72 6d61 7469 6f6e 2063 6f72 7265 6374  ormation correct
-0000ed00: 6c79 2e0a 0a20 2020 2060 476f 6f67 6c65  ly...    `Google
-0000ed10: 2057 6f72 6b73 7061 6365 2041 6464 2d6f   Workspace Add-o
-0000ed20: 6e73 2061 6e64 2043 6861 740a 2020 2020  ns and Chat.    
-0000ed30: 6170 7073 203c 6874 7470 733a 2f2f 6465  apps <https://de
-0000ed40: 7665 6c6f 7065 7273 2e67 6f6f 676c 652e  velopers.google.
-0000ed50: 636f 6d2f 776f 726b 7370 6163 652f 6578  com/workspace/ex
-0000ed60: 7465 6e64 3e60 5f5f 3a0a 0a20 2020 2041  tend>`__:..    A
-0000ed70: 7474 7269 6275 7465 733a 0a20 2020 2020  ttributes:.     
-0000ed80: 2020 206e 616d 6520 2873 7472 293a 0a20     name (str):. 
-0000ed90: 2020 2020 2020 2020 2020 2054 6865 206e             The n
-0000eda0: 616d 6520 6279 2077 6869 6368 2074 6865  ame by which the
-0000edb0: 2060 6044 6174 6554 696d 6550 6963 6b65   ``DateTimePicke
-0000edc0: 7260 6020 6973 2069 6465 6e74 6966 6965  r`` is identifie
-0000edd0: 6420 696e 2061 0a20 2020 2020 2020 2020  d in a.         
-0000ede0: 2020 2066 6f72 6d20 696e 7075 7420 6576     form input ev
-0000edf0: 656e 742e 0a0a 2020 2020 2020 2020 2020  ent...          
-0000ee00: 2020 466f 7220 6465 7461 696c 7320 6162    For details ab
-0000ee10: 6f75 7420 776f 726b 696e 6720 7769 7468  out working with
-0000ee20: 2066 6f72 6d20 696e 7075 7473 2c20 7365   form inputs, se
-0000ee30: 6520 6052 6563 6569 7665 0a20 2020 2020  e `Receive.     
-0000ee40: 2020 2020 2020 2066 6f72 6d0a 2020 2020         form.    
-0000ee50: 2020 2020 2020 2020 6461 7461 203c 6874          data <ht
-0000ee60: 7470 733a 2f2f 6465 7665 6c6f 7065 7273  tps://developers
-0000ee70: 2e67 6f6f 676c 652e 636f 6d2f 6368 6174  .google.com/chat
-0000ee80: 2f75 692f 7265 6164 2d66 6f72 6d2d 6461  /ui/read-form-da
-0000ee90: 7461 3e60 5f5f 2e0a 2020 2020 2020 2020  ta>`__..        
-0000eea0: 6c61 6265 6c20 2873 7472 293a 0a20 2020  label (str):.   
-0000eeb0: 2020 2020 2020 2020 2054 6865 2074 6578           The tex
-0000eec0: 7420 7468 6174 2070 726f 6d70 7473 2075  t that prompts u
-0000eed0: 7365 7273 2074 6f20 696e 7075 7420 6120  sers to input a 
-0000eee0: 6461 7465 2c20 6120 7469 6d65 2c20 6f72  date, a time, or
-0000eef0: 2061 0a20 2020 2020 2020 2020 2020 2064   a.            d
-0000ef00: 6174 6520 616e 6420 7469 6d65 2e20 466f  ate and time. Fo
-0000ef10: 7220 6578 616d 706c 652c 2069 6620 7573  r example, if us
-0000ef20: 6572 7320 6172 6520 7363 6865 6475 6c69  ers are scheduli
-0000ef30: 6e67 2061 6e0a 2020 2020 2020 2020 2020  ng an.          
-0000ef40: 2020 6170 706f 696e 746d 656e 742c 2075    appointment, u
-0000ef50: 7365 2061 206c 6162 656c 2073 7563 6820  se a label such 
-0000ef60: 6173 2060 6041 7070 6f69 6e74 6d65 6e74  as ``Appointment
-0000ef70: 2064 6174 6560 6020 6f72 0a20 2020 2020   date`` or.     
-0000ef80: 2020 2020 2020 2060 6041 7070 6f69 6e74         ``Appoint
-0000ef90: 6d65 6e74 2064 6174 6520 616e 6420 7469  ment date and ti
-0000efa0: 6d65 6060 2e0a 2020 2020 2020 2020 7479  me``..        ty
-0000efb0: 7065 5f20 2867 6f6f 676c 652e 6170 7073  pe_ (google.apps
-0000efc0: 2e63 6172 645f 7631 2e74 7970 6573 2e44  .card_v1.types.D
-0000efd0: 6174 6554 696d 6550 6963 6b65 722e 4461  ateTimePicker.Da
-0000efe0: 7465 5469 6d65 5069 636b 6572 5479 7065  teTimePickerType
-0000eff0: 293a 0a20 2020 2020 2020 2020 2020 2057  ):.            W
-0000f000: 6865 7468 6572 2074 6865 2077 6964 6765  hether the widge
-0000f010: 7420 7375 7070 6f72 7473 2069 6e70 7574  t supports input
-0000f020: 7469 6e67 2061 2064 6174 652c 0a20 2020  ting a date,.   
-0000f030: 2020 2020 2020 2020 2061 2074 696d 652c           a time,
-0000f040: 206f 7220 7468 6520 6461 7465 2061 6e64   or the date and
-0000f050: 2074 696d 652e 0a20 2020 2020 2020 2076   time..        v
-0000f060: 616c 7565 5f6d 735f 6570 6f63 6820 2869  alue_ms_epoch (i
-0000f070: 6e74 293a 0a20 2020 2020 2020 2020 2020  nt):.           
-0000f080: 2054 6865 2064 6566 6175 6c74 2076 616c   The default val
-0000f090: 7565 2064 6973 706c 6179 6564 2069 6e20  ue displayed in 
-0000f0a0: 7468 6520 7769 6467 6574 2c20 696e 206d  the widget, in m
-0000f0b0: 696c 6c69 7365 636f 6e64 730a 2020 2020  illiseconds.    
-0000f0c0: 2020 2020 2020 2020 7369 6e63 6520 6055          since `U
-0000f0d0: 6e69 7820 6570 6f63 680a 2020 2020 2020  nix epoch.      
-0000f0e0: 2020 2020 2020 7469 6d65 203c 6874 7470        time <http
-0000f0f0: 733a 2f2f 656e 2e77 696b 6970 6564 6961  s://en.wikipedia
-0000f100: 2e6f 7267 2f77 696b 692f 556e 6978 5f74  .org/wiki/Unix_t
-0000f110: 696d 653e 605f 5f2e 0a0a 2020 2020 2020  ime>`__...      
-0000f120: 2020 2020 2020 5370 6563 6966 7920 7468        Specify th
-0000f130: 6520 7661 6c75 6520 6261 7365 6420 6f6e  e value based on
-0000f140: 2074 6865 2074 7970 6520 6f66 2070 6963   the type of pic
-0000f150: 6b65 720a 2020 2020 2020 2020 2020 2020  ker.            
-0000f160: 2860 6044 6174 6554 696d 6550 6963 6b65  (``DateTimePicke
-0000f170: 7254 7970 6560 6029 3a0a 0a20 2020 2020  rType``):..     
-0000f180: 2020 2020 2020 202d 2020 6060 4441 5445         -  ``DATE
-0000f190: 5f41 4e44 5f54 494d 4560 603a 2061 2063  _AND_TIME``: a c
-0000f1a0: 616c 656e 6461 7220 6461 7465 2061 6e64  alendar date and
-0000f1b0: 2074 696d 6520 696e 2055 5443 2e20 466f   time in UTC. Fo
-0000f1c0: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
-0000f1d0: 2065 7861 6d70 6c65 2c20 746f 2072 6570   example, to rep
-0000f1e0: 7265 7365 6e74 204a 616e 7561 7279 2031  resent January 1
-0000f1f0: 2c20 3230 3233 2061 7420 3132 3a30 3020  , 2023 at 12:00 
-0000f200: 504d 2055 5443 2c0a 2020 2020 2020 2020  PM UTC,.        
-0000f210: 2020 2020 2020 2075 7365 2060 6031 3637         use ``167
-0000f220: 3235 3734 3430 3030 3030 6060 2e0a 2020  2574400000``..  
-0000f230: 2020 2020 2020 2020 2020 2d20 2060 6044            -  ``D
-0000f240: 4154 455f 4f4e 4c59 6060 3a20 6120 6361  ATE_ONLY``: a ca
-0000f250: 6c65 6e64 6172 2064 6174 6520 6174 2030  lendar date at 0
-0000f260: 303a 3030 3a30 3020 5554 432e 2046 6f72  0:00:00 UTC. For
-0000f270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f280: 6578 616d 706c 652c 2074 6f20 7265 7072  example, to repr
-0000f290: 6573 656e 7420 4a61 6e75 6172 7920 312c  esent January 1,
-0000f2a0: 2032 3032 332c 2075 7365 0a20 2020 2020   2023, use.     
-0000f2b0: 2020 2020 2020 2020 2020 6060 3136 3732            ``1672
-0000f2c0: 3533 3132 3030 3030 3060 602e 0a20 2020  531200000``..   
-0000f2d0: 2020 2020 2020 2020 202d 2020 6060 5449           -  ``TI
-0000f2e0: 4d45 5f4f 4e4c 5960 603a 2061 2074 696d  ME_ONLY``: a tim
-0000f2f0: 6520 696e 2055 5443 2e20 466f 7220 6578  e in UTC. For ex
-0000f300: 616d 706c 652c 2074 6f20 7265 7072 6573  ample, to repres
-0000f310: 656e 740a 2020 2020 2020 2020 2020 2020  ent.            
-0000f320: 2020 2031 323a 3030 2050 4d2c 2075 7365     12:00 PM, use
-0000f330: 2060 6034 3332 3030 3030 3060 6020 286f   ``43200000`` (o
-0000f340: 7220 6060 3132 202a 2036 3020 2a20 3630  r ``12 * 60 * 60
-0000f350: 202a 2031 3030 3060 6029 2e0a 2020 2020   * 1000``)..    
-0000f360: 2020 2020 7469 6d65 7a6f 6e65 5f6f 6666      timezone_off
-0000f370: 7365 745f 6461 7465 2028 696e 7429 3a0a  set_date (int):.
-0000f380: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-0000f390: 6e75 6d62 6572 2072 6570 7265 7365 6e74  number represent
-0000f3a0: 696e 6720 7468 6520 7469 6d65 207a 6f6e  ing the time zon
-0000f3b0: 6520 6f66 6673 6574 2066 726f 6d20 5554  e offset from UT
-0000f3c0: 432c 2069 6e0a 2020 2020 2020 2020 2020  C, in.          
-0000f3d0: 2020 6d69 6e75 7465 732e 2049 6620 7365    minutes. If se
-0000f3e0: 742c 2074 6865 2060 6076 616c 7565 5f6d  t, the ``value_m
-0000f3f0: 735f 6570 6f63 6860 6020 6973 2064 6973  s_epoch`` is dis
-0000f400: 706c 6179 6564 2069 6e20 7468 650a 2020  played in the.  
-0000f410: 2020 2020 2020 2020 2020 7370 6563 6966            specif
-0000f420: 6965 6420 7469 6d65 207a 6f6e 652e 2049  ied time zone. I
-0000f430: 6620 756e 7365 742c 2074 6865 2076 616c  f unset, the val
-0000f440: 7565 2064 6566 6175 6c74 7320 746f 2074  ue defaults to t
-0000f450: 6865 0a20 2020 2020 2020 2020 2020 2075  he.            u
-0000f460: 7365 7227 7320 7469 6d65 207a 6f6e 6520  ser's time zone 
-0000f470: 7365 7474 696e 672e 0a20 2020 2020 2020  setting..       
-0000f480: 206f 6e5f 6368 616e 6765 5f61 6374 696f   on_change_actio
-0000f490: 6e20 2867 6f6f 676c 652e 6170 7073 2e63  n (google.apps.c
-0000f4a0: 6172 645f 7631 2e74 7970 6573 2e41 6374  ard_v1.types.Act
-0000f4b0: 696f 6e29 3a0a 2020 2020 2020 2020 2020  ion):.          
-0000f4c0: 2020 5472 6967 6765 7265 6420 7768 656e    Triggered when
-0000f4d0: 2074 6865 2075 7365 7220 636c 6963 6b73   the user clicks
-0000f4e0: 202a 2a53 6176 652a 2a20 6f72 202a 2a43   **Save** or **C
-0000f4f0: 6c65 6172 2a2a 2066 726f 6d0a 2020 2020  lear** from.    
-0000f500: 2020 2020 2020 2020 7468 6520 6060 4461          the ``Da
-0000f510: 7465 5469 6d65 5069 636b 6572 6060 2069  teTimePicker`` i
-0000f520: 6e74 6572 6661 6365 2e0a 2020 2020 2222  nterface..    ""
-0000f530: 220a 0a20 2020 2063 6c61 7373 2044 6174  "..    class Dat
-0000f540: 6554 696d 6550 6963 6b65 7254 7970 6528  eTimePickerType(
-0000f550: 7072 6f74 6f2e 456e 756d 293a 0a20 2020  proto.Enum):.   
-0000f560: 2020 2020 2072 2222 2254 6865 2066 6f72       r"""The for
-0000f570: 6d61 7420 666f 7220 7468 6520 6461 7465  mat for the date
-0000f580: 2061 6e64 2074 696d 6520 696e 2074 6865   and time in the
-0000f590: 2060 6044 6174 6554 696d 6550 6963 6b65   ``DateTimePicke
-0000f5a0: 7260 6020 7769 6467 6574 2e0a 2020 2020  r`` widget..    
-0000f5b0: 2020 2020 4465 7465 726d 696e 6573 2077      Determines w
-0000f5c0: 6865 7468 6572 2075 7365 7273 2063 616e  hether users can
-0000f5d0: 2069 6e70 7574 2061 2064 6174 652c 2061   input a date, a
-0000f5e0: 2074 696d 652c 206f 7220 626f 7468 2061   time, or both a
-0000f5f0: 2064 6174 650a 2020 2020 2020 2020 616e   date.        an
-0000f600: 6420 7469 6d65 2e0a 0a20 2020 2020 2020  d time...       
-0000f610: 2060 476f 6f67 6c65 2057 6f72 6b73 7061   `Google Workspa
-0000f620: 6365 2041 6464 2d6f 6e73 2061 6e64 2043  ce Add-ons and C
-0000f630: 6861 740a 2020 2020 2020 2020 6170 7073  hat.        apps
-0000f640: 203c 6874 7470 733a 2f2f 6465 7665 6c6f   <https://develo
-0000f650: 7065 7273 2e67 6f6f 676c 652e 636f 6d2f  pers.google.com/
-0000f660: 776f 726b 7370 6163 652f 6578 7465 6e64  workspace/extend
-0000f670: 3e60 5f5f 3a0a 0a20 2020 2020 2020 2056  >`__:..        V
-0000f680: 616c 7565 733a 0a20 2020 2020 2020 2020  alues:.         
-0000f690: 2020 2044 4154 455f 414e 445f 5449 4d45     DATE_AND_TIME
-0000f6a0: 2028 3029 3a0a 2020 2020 2020 2020 2020   (0):.          
-0000f6b0: 2020 2020 2020 5573 6572 7320 696e 7075        Users inpu
-0000f6c0: 7420 6120 6461 7465 2061 6e64 2074 696d  t a date and tim
-0000f6d0: 652e 0a20 2020 2020 2020 2020 2020 2044  e..            D
-0000f6e0: 4154 455f 4f4e 4c59 2028 3129 3a0a 2020  ATE_ONLY (1):.  
-0000f6f0: 2020 2020 2020 2020 2020 2020 2020 5573                Us
-0000f700: 6572 7320 696e 7075 7420 6120 6461 7465  ers input a date
-0000f710: 2e0a 2020 2020 2020 2020 2020 2020 5449  ..            TI
-0000f720: 4d45 5f4f 4e4c 5920 2832 293a 0a20 2020  ME_ONLY (2):.   
-0000f730: 2020 2020 2020 2020 2020 2020 2055 7365               Use
-0000f740: 7273 2069 6e70 7574 2061 2074 696d 652e  rs input a time.
-0000f750: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000f760: 2020 2020 2044 4154 455f 414e 445f 5449       DATE_AND_TI
-0000f770: 4d45 203d 2030 0a20 2020 2020 2020 2044  ME = 0.        D
-0000f780: 4154 455f 4f4e 4c59 203d 2031 0a20 2020  ATE_ONLY = 1.   
-0000f790: 2020 2020 2054 494d 455f 4f4e 4c59 203d       TIME_ONLY =
-0000f7a0: 2032 0a0a 2020 2020 6e61 6d65 3a20 7374   2..    name: st
-0000f7b0: 7220 3d20 7072 6f74 6f2e 4669 656c 6428  r = proto.Field(
-0000f7c0: 0a20 2020 2020 2020 2070 726f 746f 2e53  .        proto.S
-0000f7d0: 5452 494e 472c 0a20 2020 2020 2020 206e  TRING,.        n
-0000f7e0: 756d 6265 723d 312c 0a20 2020 2029 0a20  umber=1,.    ). 
-0000f7f0: 2020 206c 6162 656c 3a20 7374 7220 3d20     label: str = 
-0000f800: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
-0000f810: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
-0000f820: 472c 0a20 2020 2020 2020 206e 756d 6265  G,.        numbe
-0000f830: 723d 322c 0a20 2020 2029 0a20 2020 2074  r=2,.    ).    t
-0000f840: 7970 655f 3a20 4461 7465 5469 6d65 5069  ype_: DateTimePi
-0000f850: 636b 6572 5479 7065 203d 2070 726f 746f  ckerType = proto
-0000f860: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
-0000f870: 7072 6f74 6f2e 454e 554d 2c0a 2020 2020  proto.ENUM,.    
-0000f880: 2020 2020 6e75 6d62 6572 3d33 2c0a 2020      number=3,.  
-0000f890: 2020 2020 2020 656e 756d 3d44 6174 6554        enum=DateT
-0000f8a0: 696d 6550 6963 6b65 7254 7970 652c 0a20  imePickerType,. 
-0000f8b0: 2020 2029 0a20 2020 2076 616c 7565 5f6d     ).    value_m
-0000f8c0: 735f 6570 6f63 683a 2069 6e74 203d 2070  s_epoch: int = p
-0000f8d0: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
-0000f8e0: 2020 2020 7072 6f74 6f2e 494e 5436 342c      proto.INT64,
-0000f8f0: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
-0000f900: 342c 0a20 2020 2029 0a20 2020 2074 696d  4,.    ).    tim
-0000f910: 657a 6f6e 655f 6f66 6673 6574 5f64 6174  ezone_offset_dat
-0000f920: 653a 2069 6e74 203d 2070 726f 746f 2e46  e: int = proto.F
-0000f930: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
-0000f940: 6f74 6f2e 494e 5433 322c 0a20 2020 2020  oto.INT32,.     
-0000f950: 2020 206e 756d 6265 723d 352c 0a20 2020     number=5,.   
-0000f960: 2029 0a20 2020 206f 6e5f 6368 616e 6765   ).    on_change
-0000f970: 5f61 6374 696f 6e3a 2022 4163 7469 6f6e  _action: "Action
-0000f980: 2220 3d20 7072 6f74 6f2e 4669 656c 6428  " = proto.Field(
-0000f990: 0a20 2020 2020 2020 2070 726f 746f 2e4d  .        proto.M
-0000f9a0: 4553 5341 4745 2c0a 2020 2020 2020 2020  ESSAGE,.        
-0000f9b0: 6e75 6d62 6572 3d36 2c0a 2020 2020 2020  number=6,.      
-0000f9c0: 2020 6d65 7373 6167 653d 2241 6374 696f    message="Actio
-0000f9d0: 6e22 2c0a 2020 2020 290a 0a0a 636c 6173  n",.    )...clas
-0000f9e0: 7320 4275 7474 6f6e 2870 726f 746f 2e4d  s Button(proto.M
-0000f9f0: 6573 7361 6765 293a 0a20 2020 2072 2222  essage):.    r""
-0000fa00: 2241 2074 6578 742c 2069 636f 6e2c 206f  "A text, icon, o
-0000fa10: 7220 7465 7874 2061 6e64 2069 636f 6e20  r text and icon 
-0000fa20: 6275 7474 6f6e 2074 6861 7420 7573 6572  button that user
-0000fa30: 7320 6361 6e20 636c 6963 6b2e 2046 6f72  s can click. For
-0000fa40: 2061 6e0a 2020 2020 6578 616d 706c 6520   an.    example 
-0000fa50: 696e 2047 6f6f 676c 6520 4368 6174 2061  in Google Chat a
-0000fa60: 7070 732c 2073 6565 2060 4275 7474 6f6e  pps, see `Button
-0000fa70: 0a20 2020 206c 6973 7420 3c68 7474 7073  .    list <https
-0000fa80: 3a2f 2f64 6576 656c 6f70 6572 732e 676f  ://developers.go
-0000fa90: 6f67 6c65 2e63 6f6d 2f63 6861 742f 7569  ogle.com/chat/ui
-0000faa0: 2f77 6964 6765 7473 2f62 7574 746f 6e2d  /widgets/button-
-0000fab0: 6c69 7374 3e60 5f5f 2e0a 0a20 2020 2054  list>`__...    T
-0000fac0: 6f20 6d61 6b65 2061 6e20 696d 6167 6520  o make an image 
-0000fad0: 6120 636c 6963 6b61 626c 6520 6275 7474  a clickable butt
-0000fae0: 6f6e 2c20 7370 6563 6966 7920 616e 0a20  on, specify an. 
-0000faf0: 2020 205b 6060 496d 6167 6560 605d 5b67     [``Image``][g
-0000fb00: 6f6f 676c 652e 6170 7073 2e63 6172 642e  oogle.apps.card.
-0000fb10: 7631 2e49 6d61 6765 5d20 286e 6f74 2061  v1.Image] (not a
-0000fb20: 6e0a 2020 2020 5b60 6049 6d61 6765 436f  n.    [``ImageCo
-0000fb30: 6d70 6f6e 656e 7460 605d 5b67 6f6f 676c  mponent``][googl
-0000fb40: 652e 6170 7073 2e63 6172 642e 7631 2e49  e.apps.card.v1.I
-0000fb50: 6d61 6765 436f 6d70 6f6e 656e 745d 2920  mageComponent]) 
-0000fb60: 616e 6420 7365 7420 616e 0a20 2020 2060  and set an.    `
-0000fb70: 606f 6e43 6c69 636b 6060 2061 6374 696f  `onClick`` actio
-0000fb80: 6e2e 0a0a 2020 2020 6047 6f6f 676c 6520  n...    `Google 
-0000fb90: 576f 726b 7370 6163 6520 4164 642d 6f6e  Workspace Add-on
-0000fba0: 7320 616e 6420 4368 6174 0a20 2020 2061  s and Chat.    a
-0000fbb0: 7070 7320 3c68 7474 7073 3a2f 2f64 6576  pps <https://dev
-0000fbc0: 656c 6f70 6572 732e 676f 6f67 6c65 2e63  elopers.google.c
-0000fbd0: 6f6d 2f77 6f72 6b73 7061 6365 2f65 7874  om/workspace/ext
-0000fbe0: 656e 643e 605f 5f3a 0a0a 2020 2020 4174  end>`__:..    At
-0000fbf0: 7472 6962 7574 6573 3a0a 2020 2020 2020  tributes:.      
-0000fc00: 2020 7465 7874 2028 7374 7229 3a0a 2020    text (str):.  
-0000fc10: 2020 2020 2020 2020 2020 5468 6520 7465            The te
-0000fc20: 7874 2064 6973 706c 6179 6564 2069 6e73  xt displayed ins
-0000fc30: 6964 6520 7468 6520 6275 7474 6f6e 2e0a  ide the button..
-0000fc40: 2020 2020 2020 2020 6963 6f6e 2028 676f          icon (go
-0000fc50: 6f67 6c65 2e61 7070 732e 6361 7264 5f76  ogle.apps.card_v
-0000fc60: 312e 7479 7065 732e 4963 6f6e 293a 0a20  1.types.Icon):. 
-0000fc70: 2020 2020 2020 2020 2020 2054 6865 2069             The i
-0000fc80: 636f 6e20 696d 6167 652e 2049 6620 626f  con image. If bo
-0000fc90: 7468 2060 6069 636f 6e60 6020 616e 6420  th ``icon`` and 
-0000fca0: 6060 7465 7874 6060 2061 7265 2073 6574  ``text`` are set
-0000fcb0: 2c20 7468 656e 0a20 2020 2020 2020 2020  , then.         
-0000fcc0: 2020 2074 6865 2069 636f 6e20 6170 7065     the icon appe
-0000fcd0: 6172 7320 6265 666f 7265 2074 6865 2074  ars before the t
-0000fce0: 6578 742e 0a20 2020 2020 2020 2063 6f6c  ext..        col
-0000fcf0: 6f72 2028 676f 6f67 6c65 2e74 7970 652e  or (google.type.
-0000fd00: 636f 6c6f 725f 7062 322e 436f 6c6f 7229  color_pb2.Color)
-0000fd10: 3a0a 2020 2020 2020 2020 2020 2020 4966  :.            If
-0000fd20: 2073 6574 2c20 7468 6520 6275 7474 6f6e   set, the button
-0000fd30: 2069 7320 6669 6c6c 6564 2077 6974 6820   is filled with 
-0000fd40: 6120 736f 6c69 6420 6261 636b 6772 6f75  a solid backgrou
-0000fd50: 6e64 2063 6f6c 6f72 0a20 2020 2020 2020  nd color.       
-0000fd60: 2020 2020 2061 6e64 2074 6865 2066 6f6e       and the fon
-0000fd70: 7420 636f 6c6f 7220 6368 616e 6765 7320  t color changes 
-0000fd80: 746f 206d 6169 6e74 6169 6e20 636f 6e74  to maintain cont
-0000fd90: 7261 7374 2077 6974 6820 7468 650a 2020  rast with the.  
-0000fda0: 2020 2020 2020 2020 2020 6261 636b 6772            backgr
-0000fdb0: 6f75 6e64 2063 6f6c 6f72 2e20 466f 7220  ound color. For 
-0000fdc0: 6578 616d 706c 652c 2073 6574 7469 6e67  example, setting
-0000fdd0: 2061 2062 6c75 6520 6261 636b 6772 6f75   a blue backgrou
-0000fde0: 6e64 0a20 2020 2020 2020 2020 2020 206c  nd.            l
-0000fdf0: 696b 656c 7920 7265 7375 6c74 7320 696e  ikely results in
-0000fe00: 2077 6869 7465 2074 6578 742e 0a0a 2020   white text...  
-0000fe10: 2020 2020 2020 2020 2020 4966 2075 6e73            If uns
-0000fe20: 6574 2c20 7468 6520 696d 6167 6520 6261  et, the image ba
-0000fe30: 636b 6772 6f75 6e64 2069 7320 7768 6974  ckground is whit
-0000fe40: 6520 616e 6420 7468 6520 666f 6e74 2063  e and the font c
-0000fe50: 6f6c 6f72 0a20 2020 2020 2020 2020 2020  olor.           
-0000fe60: 2069 7320 626c 7565 2e0a 0a20 2020 2020   is blue...     
-0000fe70: 2020 2020 2020 2046 6f72 2072 6564 2c20         For red, 
-0000fe80: 6772 6565 6e2c 2061 6e64 2062 6c75 652c  green, and blue,
-0000fe90: 2074 6865 2076 616c 7565 206f 6620 6561   the value of ea
-0000fea0: 6368 2066 6965 6c64 2069 7320 610a 2020  ch field is a.  
-0000feb0: 2020 2020 2020 2020 2020 6060 666c 6f61            ``floa
-0000fec0: 7460 6020 6e75 6d62 6572 2074 6861 7420  t`` number that 
-0000fed0: 796f 7520 6361 6e20 6578 7072 6573 7320  you can express 
-0000fee0: 696e 2065 6974 6865 7220 6f66 2074 776f  in either of two
-0000fef0: 2077 6179 733a 0a20 2020 2020 2020 2020   ways:.         
-0000ff00: 2020 2061 7320 6120 6e75 6d62 6572 2062     as a number b
-0000ff10: 6574 7765 656e 2030 2061 6e64 2032 3535  etween 0 and 255
-0000ff20: 2064 6976 6964 6564 2062 7920 3235 3520   divided by 255 
-0000ff30: 2831 3533 2f32 3535 292c 206f 720a 2020  (153/255), or.  
-0000ff40: 2020 2020 2020 2020 2020 6173 2061 2076            as a v
-0000ff50: 616c 7565 2062 6574 7765 656e 2030 2061  alue between 0 a
-0000ff60: 6e64 2031 2028 302e 3629 2e20 3020 7265  nd 1 (0.6). 0 re
-0000ff70: 7072 6573 656e 7473 2074 6865 2061 6273  presents the abs
-0000ff80: 656e 6365 0a20 2020 2020 2020 2020 2020  ence.           
-0000ff90: 206f 6620 6120 636f 6c6f 7220 616e 6420   of a color and 
-0000ffa0: 3120 6f72 2032 3535 2f32 3535 2072 6570  1 or 255/255 rep
-0000ffb0: 7265 7365 6e74 2074 6865 2066 756c 6c20  resent the full 
-0000ffc0: 7072 6573 656e 6365 206f 660a 2020 2020  presence of.    
-0000ffd0: 2020 2020 2020 2020 7468 6174 2063 6f6c          that col
-0000ffe0: 6f72 206f 6e20 7468 6520 5247 4220 7363  or on the RGB sc
-0000fff0: 616c 652e 0a0a 2020 2020 2020 2020 2020  ale...          
-00010000: 2020 4f70 7469 6f6e 616c 6c79 2073 6574    Optionally set
-00010010: 2060 6061 6c70 6861 6060 2c20 7768 6963   ``alpha``, whic
-00010020: 6820 7365 7473 2061 206c 6576 656c 206f  h sets a level o
-00010030: 6620 7472 616e 7370 6172 656e 6379 0a20  f transparency. 
-00010040: 2020 2020 2020 2020 2020 2075 7369 6e67             using
-00010050: 2074 6869 7320 6571 7561 7469 6f6e 3a0a   this equation:.
-00010060: 0a20 2020 2020 2020 2020 2020 203a 3a0a  .            ::.
-00010070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010080: 7069 7865 6c20 636f 6c6f 7220 3d20 616c  pixel color = al
-00010090: 7068 6120 2a20 2874 6869 7320 636f 6c6f  pha * (this colo
-000100a0: 7229 202b 2028 312e 3020 2d20 616c 7068  r) + (1.0 - alph
-000100b0: 6129 202a 2028 6261 636b 6772 6f75 6e64  a) * (background
-000100c0: 2063 6f6c 6f72 290a 0a20 2020 2020 2020   color)..       
-000100d0: 2020 2020 2046 6f72 2060 6061 6c70 6861       For ``alpha
-000100e0: 6060 2c20 6120 7661 6c75 6520 6f66 2060  ``, a value of `
-000100f0: 6031 6060 2063 6f72 7265 7370 6f6e 6473  `1`` corresponds
-00010100: 2077 6974 6820 6120 736f 6c69 640a 2020   with a solid.  
-00010110: 2020 2020 2020 2020 2020 636f 6c6f 722c            color,
-00010120: 2061 6e64 2061 2076 616c 7565 206f 6620   and a value of 
-00010130: 6060 3060 6020 636f 7272 6573 706f 6e64  ``0`` correspond
-00010140: 7320 7769 7468 2061 2063 6f6d 706c 6574  s with a complet
-00010150: 656c 790a 2020 2020 2020 2020 2020 2020  ely.            
-00010160: 7472 616e 7370 6172 656e 7420 636f 6c6f  transparent colo
-00010170: 722e 0a0a 2020 2020 2020 2020 2020 2020  r...            
-00010180: 466f 7220 6578 616d 706c 652c 2074 6865  For example, the
-00010190: 2066 6f6c 6c6f 7769 6e67 2063 6f6c 6f72   following color
-000101a0: 2072 6570 7265 7365 6e74 7320 6120 6861   represents a ha
-000101b0: 6c66 0a20 2020 2020 2020 2020 2020 2074  lf.            t
-000101c0: 7261 6e73 7061 7265 6e74 2072 6564 3a0a  ransparent red:.
-000101d0: 0a20 2020 2020 2020 2020 2020 203a 3a0a  .            ::.
-000101e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000101f0: 2263 6f6c 6f72 223a 207b 0a20 2020 2020  "color": {.     
-00010200: 2020 2020 2020 2020 2020 2020 2022 7265               "re
-00010210: 6422 3a20 312c 0a20 2020 2020 2020 2020  d": 1,.         
-00010220: 2020 2020 2020 2020 2022 6772 6565 6e22           "green"
-00010230: 3a20 302c 0a20 2020 2020 2020 2020 2020  : 0,.           
-00010240: 2020 2020 2020 2022 626c 7565 223a 2030         "blue": 0
-00010250: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00010260: 2020 2020 2261 6c70 6861 223a 2030 2e35      "alpha": 0.5
-00010270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010280: 7d0a 2020 2020 2020 2020 6f6e 5f63 6c69  }.        on_cli
-00010290: 636b 2028 676f 6f67 6c65 2e61 7070 732e  ck (google.apps.
-000102a0: 6361 7264 5f76 312e 7479 7065 732e 4f6e  card_v1.types.On
-000102b0: 436c 6963 6b29 3a0a 2020 2020 2020 2020  Click):.        
-000102c0: 2020 2020 5265 7175 6972 6564 2e20 5468      Required. Th
-000102d0: 6520 6163 7469 6f6e 2074 6f20 7065 7266  e action to perf
-000102e0: 6f72 6d20 7768 656e 2061 2075 7365 720a  orm when a user.
-000102f0: 2020 2020 2020 2020 2020 2020 636c 6963              clic
-00010300: 6b73 2074 6865 2062 7574 746f 6e2c 2073  ks the button, s
-00010310: 7563 6820 6173 206f 7065 6e69 6e67 2061  uch as opening a
-00010320: 2068 7970 6572 6c69 6e6b 0a20 2020 2020   hyperlink.     
-00010330: 2020 2020 2020 206f 7220 7275 6e6e 696e         or runnin
-00010340: 6720 6120 6375 7374 6f6d 2066 756e 6374  g a custom funct
-00010350: 696f 6e2e 0a20 2020 2020 2020 2064 6973  ion..        dis
-00010360: 6162 6c65 6420 2862 6f6f 6c29 3a0a 2020  abled (bool):.  
-00010370: 2020 2020 2020 2020 2020 4966 2060 6074            If ``t
-00010380: 7275 6560 602c 2074 6865 2062 7574 746f  rue``, the butto
-00010390: 6e20 6973 2064 6973 706c 6179 6564 2069  n is displayed i
-000103a0: 6e20 616e 2069 6e61 6374 6976 6520 7374  n an inactive st
-000103b0: 6174 650a 2020 2020 2020 2020 2020 2020  ate.            
-000103c0: 616e 6420 646f 6573 6e27 7420 7265 7370  and doesn't resp
-000103d0: 6f6e 6420 746f 2075 7365 7220 6163 7469  ond to user acti
-000103e0: 6f6e 732e 0a20 2020 2020 2020 2061 6c74  ons..        alt
-000103f0: 5f74 6578 7420 2873 7472 293a 0a20 2020  _text (str):.   
-00010400: 2020 2020 2020 2020 2054 6865 2061 6c74           The alt
-00010410: 6572 6e61 7469 7665 2074 6578 7420 7468  ernative text th
-00010420: 6174 2773 2075 7365 6420 666f 720a 2020  at's used for.  
-00010430: 2020 2020 2020 2020 2020 6163 6365 7373            access
-00010440: 6962 696c 6974 792e 0a20 2020 2020 2020  ibility..       
-00010450: 2020 2020 2053 6574 2064 6573 6372 6970       Set descrip
-00010460: 7469 7665 2074 6578 7420 7468 6174 206c  tive text that l
-00010470: 6574 7320 7573 6572 7320 6b6e 6f77 2077  ets users know w
-00010480: 6861 740a 2020 2020 2020 2020 2020 2020  hat.            
-00010490: 7468 6520 6275 7474 6f6e 2064 6f65 732e  the button does.
-000104a0: 2046 6f72 2065 7861 6d70 6c65 2c20 6966   For example, if
-000104b0: 2061 2062 7574 746f 6e20 6f70 656e 730a   a button opens.
-000104c0: 2020 2020 2020 2020 2020 2020 6120 6879              a hy
-000104d0: 7065 726c 696e 6b2c 2079 6f75 206d 6967  perlink, you mig
-000104e0: 6874 2077 7269 7465 3a20 224f 7065 6e73  ht write: "Opens
-000104f0: 2061 206e 6577 0a20 2020 2020 2020 2020   a new.         
-00010500: 2020 2062 726f 7773 6572 2074 6162 2061     browser tab a
-00010510: 6e64 206e 6176 6967 6174 6573 2074 6f20  nd navigates to 
-00010520: 7468 6520 476f 6f67 6c65 2043 6861 740a  the Google Chat.
-00010530: 2020 2020 2020 2020 2020 2020 6465 7665              deve
-00010540: 6c6f 7065 7220 646f 6375 6d65 6e74 6174  loper documentat
-00010550: 696f 6e20 6174 0a20 2020 2020 2020 2020  ion at.         
-00010560: 2020 2068 7474 7073 3a2f 2f64 6576 656c     https://devel
-00010570: 6f70 6572 732e 676f 6f67 6c65 2e63 6f6d  opers.google.com
-00010580: 2f63 6861 7422 2e0a 2020 2020 2222 220a  /chat"..    """.
-00010590: 0a20 2020 2074 6578 743a 2073 7472 203d  .    text: str =
-000105a0: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
-000105b0: 2020 2020 2020 7072 6f74 6f2e 5354 5249        proto.STRI
-000105c0: 4e47 2c0a 2020 2020 2020 2020 6e75 6d62  NG,.        numb
-000105d0: 6572 3d31 2c0a 2020 2020 290a 2020 2020  er=1,.    ).    
-000105e0: 6963 6f6e 3a20 2249 636f 6e22 203d 2070  icon: "Icon" = p
-000105f0: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
-00010600: 2020 2020 7072 6f74 6f2e 4d45 5353 4147      proto.MESSAG
-00010610: 452c 0a20 2020 2020 2020 206e 756d 6265  E,.        numbe
-00010620: 723d 322c 0a20 2020 2020 2020 206d 6573  r=2,.        mes
-00010630: 7361 6765 3d22 4963 6f6e 222c 0a20 2020  sage="Icon",.   
-00010640: 2029 0a20 2020 2063 6f6c 6f72 3a20 636f   ).    color: co
-00010650: 6c6f 725f 7062 322e 436f 6c6f 7220 3d20  lor_pb2.Color = 
-00010660: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
-00010670: 2020 2020 2070 726f 746f 2e4d 4553 5341       proto.MESSA
-00010680: 4745 2c0a 2020 2020 2020 2020 6e75 6d62  GE,.        numb
-00010690: 6572 3d33 2c0a 2020 2020 2020 2020 6d65  er=3,.        me
-000106a0: 7373 6167 653d 636f 6c6f 725f 7062 322e  ssage=color_pb2.
-000106b0: 436f 6c6f 722c 0a20 2020 2029 0a20 2020  Color,.    ).   
-000106c0: 206f 6e5f 636c 6963 6b3a 2022 4f6e 436c   on_click: "OnCl
-000106d0: 6963 6b22 203d 2070 726f 746f 2e46 6965  ick" = proto.Fie
-000106e0: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
-000106f0: 6f2e 4d45 5353 4147 452c 0a20 2020 2020  o.MESSAGE,.     
-00010700: 2020 206e 756d 6265 723d 342c 0a20 2020     number=4,.   
-00010710: 2020 2020 206d 6573 7361 6765 3d22 4f6e       message="On
-00010720: 436c 6963 6b22 2c0a 2020 2020 290a 2020  Click",.    ).  
-00010730: 2020 6469 7361 626c 6564 3a20 626f 6f6c    disabled: bool
-00010740: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
-00010750: 2020 2020 2020 2020 7072 6f74 6f2e 424f          proto.BO
-00010760: 4f4c 2c0a 2020 2020 2020 2020 6e75 6d62  OL,.        numb
-00010770: 6572 3d35 2c0a 2020 2020 290a 2020 2020  er=5,.    ).    
-00010780: 616c 745f 7465 7874 3a20 7374 7220 3d20  alt_text: str = 
-00010790: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
-000107a0: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
-000107b0: 472c 0a20 2020 2020 2020 206e 756d 6265  G,.        numbe
-000107c0: 723d 362c 0a20 2020 2029 0a0a 0a63 6c61  r=6,.    )...cla
-000107d0: 7373 2049 636f 6e28 7072 6f74 6f2e 4d65  ss Icon(proto.Me
-000107e0: 7373 6167 6529 3a0a 2020 2020 7222 2222  ssage):.    r"""
-000107f0: 416e 2069 636f 6e20 6469 7370 6c61 7965  An icon displaye
-00010800: 6420 696e 2061 2077 6964 6765 7420 6f6e  d in a widget on
-00010810: 2061 2063 6172 642e 2046 6f72 2061 6e20   a card. For an 
-00010820: 6578 616d 706c 6520 696e 2047 6f6f 676c  example in Googl
-00010830: 650a 2020 2020 4368 6174 2061 7070 732c  e.    Chat apps,
-00010840: 2073 6565 0a20 2020 2060 4963 6f6e 203c   see.    `Icon <
-00010850: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
-00010860: 7273 2e67 6f6f 676c 652e 636f 6d2f 6368  rs.google.com/ch
-00010870: 6174 2f75 692f 7769 6467 6574 732f 6963  at/ui/widgets/ic
-00010880: 6f6e 3e60 5f5f 2e0a 0a20 2020 2053 7570  on>`__...    Sup
-00010890: 706f 7274 730a 2020 2020 6062 7569 6c74  ports.    `built
-000108a0: 2d69 6e20 3c68 7474 7073 3a2f 2f64 6576  -in <https://dev
-000108b0: 656c 6f70 6572 732e 676f 6f67 6c65 2e63  elopers.google.c
-000108c0: 6f6d 2f63 6861 742f 666f 726d 6174 2d6d  om/chat/format-m
-000108d0: 6573 7361 6765 7323 6275 696c 7469 6e69  essages#builtini
-000108e0: 636f 6e73 3e60 5f5f 0a20 2020 2061 6e64  cons>`__.    and
-000108f0: 0a20 2020 2060 6375 7374 6f6d 203c 6874  .    `custom <ht
-00010900: 7470 733a 2f2f 6465 7665 6c6f 7065 7273  tps://developers
-00010910: 2e67 6f6f 676c 652e 636f 6d2f 6368 6174  .google.com/chat
-00010920: 2f66 6f72 6d61 742d 6d65 7373 6167 6573  /format-messages
-00010930: 2363 7573 746f 6d69 636f 6e73 3e60 5f5f  #customicons>`__
-00010940: 0a20 2020 2069 636f 6e73 2e0a 0a20 2020  .    icons...   
-00010950: 2060 476f 6f67 6c65 2057 6f72 6b73 7061   `Google Workspa
-00010960: 6365 2041 6464 2d6f 6e73 2061 6e64 2043  ce Add-ons and C
-00010970: 6861 740a 2020 2020 6170 7073 203c 6874  hat.    apps <ht
-00010980: 7470 733a 2f2f 6465 7665 6c6f 7065 7273  tps://developers
-00010990: 2e67 6f6f 676c 652e 636f 6d2f 776f 726b  .google.com/work
-000109a0: 7370 6163 652f 6578 7465 6e64 3e60 5f5f  space/extend>`__
-000109b0: 3a0a 0a20 2020 2054 6869 7320 6d65 7373  :..    This mess
-000109c0: 6167 6520 6861 7320 606f 6e65 6f66 605f  age has `oneof`_
-000109d0: 2066 6965 6c64 7320 286d 7574 7561 6c6c   fields (mutuall
-000109e0: 7920 6578 636c 7573 6976 6520 6669 656c  y exclusive fiel
-000109f0: 6473 292e 0a20 2020 2046 6f72 2065 6163  ds)..    For eac
-00010a00: 6820 6f6e 656f 662c 2061 7420 6d6f 7374  h oneof, at most
-00010a10: 206f 6e65 206d 656d 6265 7220 6669 656c   one member fiel
-00010a20: 6420 6361 6e20 6265 2073 6574 2061 7420  d can be set at 
-00010a30: 7468 6520 7361 6d65 2074 696d 652e 0a20  the same time.. 
-00010a40: 2020 2053 6574 7469 6e67 2061 6e79 206d     Setting any m
-00010a50: 656d 6265 7220 6f66 2074 6865 206f 6e65  ember of the one
-00010a60: 6f66 2061 7574 6f6d 6174 6963 616c 6c79  of automatically
-00010a70: 2063 6c65 6172 7320 616c 6c20 6f74 6865   clears all othe
-00010a80: 720a 2020 2020 6d65 6d62 6572 732e 0a0a  r.    members...
-00010a90: 2020 2020 2e2e 205f 6f6e 656f 663a 2068      .. _oneof: h
-00010aa0: 7474 7073 3a2f 2f70 726f 746f 2d70 6c75  ttps://proto-plu
-00010ab0: 732d 7079 7468 6f6e 2e72 6561 6474 6865  s-python.readthe
-00010ac0: 646f 6373 2e69 6f2f 656e 2f73 7461 626c  docs.io/en/stabl
-00010ad0: 652f 6669 656c 6473 2e68 746d 6c23 6f6e  e/fields.html#on
-00010ae0: 656f 6673 2d6d 7574 7561 6c6c 792d 6578  eofs-mutually-ex
-00010af0: 636c 7573 6976 652d 6669 656c 6473 0a0a  clusive-fields..
-00010b00: 2020 2020 4174 7472 6962 7574 6573 3a0a      Attributes:.
-00010b10: 2020 2020 2020 2020 6b6e 6f77 6e5f 6963          known_ic
-00010b20: 6f6e 2028 7374 7229 3a0a 2020 2020 2020  on (str):.      
-00010b30: 2020 2020 2020 4469 7370 6c61 7920 6f6e        Display on
-00010b40: 6520 6f66 2074 6865 2062 7569 6c74 2d69  e of the built-i
-00010b50: 6e20 6963 6f6e 7320 7072 6f76 6964 6564  n icons provided
-00010b60: 2062 7920 476f 6f67 6c65 0a20 2020 2020   by Google.     
-00010b70: 2020 2020 2020 2057 6f72 6b73 7061 6365         Workspace
-00010b80: 2e0a 0a20 2020 2020 2020 2020 2020 2046  ...            F
-00010b90: 6f72 2065 7861 6d70 6c65 2c20 746f 2064  or example, to d
-00010ba0: 6973 706c 6179 2061 6e20 6169 7270 6c61  isplay an airpla
-00010bb0: 6e65 2069 636f 6e2c 2073 7065 6369 6679  ne icon, specify
-00010bc0: 0a20 2020 2020 2020 2020 2020 2060 6041  .            ``A
-00010bd0: 4952 504c 414e 4560 602e 2046 6f72 2061  IRPLANE``. For a
-00010be0: 2062 7573 2c20 7370 6563 6966 7920 6060   bus, specify ``
-00010bf0: 4255 5360 602e 0a0a 2020 2020 2020 2020  BUS``...        
-00010c00: 2020 2020 466f 7220 6120 6675 6c6c 206c      For a full l
-00010c10: 6973 7420 6f66 2073 7570 706f 7274 6564  ist of supported
-00010c20: 2069 636f 6e73 2c20 7365 6520 6062 7569   icons, see `bui
-00010c30: 6c74 2d69 6e0a 2020 2020 2020 2020 2020  lt-in.          
-00010c40: 2020 6963 6f6e 7320 3c68 7474 7073 3a2f    icons <https:/
-00010c50: 2f64 6576 656c 6f70 6572 732e 676f 6f67  /developers.goog
-00010c60: 6c65 2e63 6f6d 2f63 6861 742f 666f 726d  le.com/chat/form
-00010c70: 6174 2d6d 6573 7361 6765 7323 6275 696c  at-messages#buil
-00010c80: 7469 6e69 636f 6e73 3e60 5f5f 2e0a 0a20  tinicons>`__... 
-00010c90: 2020 2020 2020 2020 2020 2054 6869 7320             This 
-00010ca0: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
-00010cb0: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
-00010cc0: 6963 6f6e 7360 602e 0a20 2020 2020 2020  icons``..       
-00010cd0: 2069 636f 6e5f 7572 6c20 2873 7472 293a   icon_url (str):
-00010ce0: 0a20 2020 2020 2020 2020 2020 2044 6973  .            Dis
-00010cf0: 706c 6179 2061 2063 7573 746f 6d20 6963  play a custom ic
-00010d00: 6f6e 2068 6f73 7465 6420 6174 2061 6e20  on hosted at an 
-00010d10: 4854 5450 5320 5552 4c2e 0a0a 2020 2020  HTTPS URL...    
-00010d20: 2020 2020 2020 2020 466f 7220 6578 616d          For exam
-00010d30: 706c 653a 0a0a 2020 2020 2020 2020 2020  ple:..          
-00010d40: 2020 3a3a 0a0a 2020 2020 2020 2020 2020    ::..          
-00010d50: 2020 2020 2022 6963 6f6e 5572 6c22 3a0a       "iconUrl":.
-00010d60: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00010d70: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
-00010d80: 7273 2e67 6f6f 676c 652e 636f 6d2f 6368  rs.google.com/ch
-00010d90: 6174 2f69 6d61 6765 732f 7175 6963 6b73  at/images/quicks
-00010da0: 7461 7274 2d61 7070 2d61 7661 7461 722e  tart-app-avatar.
-00010db0: 706e 6722 0a0a 2020 2020 2020 2020 2020  png"..          
-00010dc0: 2020 5375 7070 6f72 7465 6420 6669 6c65    Supported file
-00010dd0: 2074 7970 6573 2069 6e63 6c75 6465 2060   types include `
-00010de0: 602e 706e 6760 6020 616e 6420 6060 2e6a  `.png`` and ``.j
-00010df0: 7067 6060 2e0a 0a20 2020 2020 2020 2020  pg``...         
-00010e00: 2020 2054 6869 7320 6669 656c 6420 6973     This field is
-00010e10: 2061 206d 656d 6265 7220 6f66 2060 6f6e   a member of `on
-00010e20: 656f 6660 5f20 6060 6963 6f6e 7360 602e  eof`_ ``icons``.
-00010e30: 0a20 2020 2020 2020 2061 6c74 5f74 6578  .        alt_tex
-00010e40: 7420 2873 7472 293a 0a20 2020 2020 2020  t (str):.       
-00010e50: 2020 2020 204f 7074 696f 6e61 6c2e 2041       Optional. A
-00010e60: 2064 6573 6372 6970 7469 6f6e 206f 6620   description of 
-00010e70: 7468 6520 6963 6f6e 2075 7365 6420 666f  the icon used fo
-00010e80: 7220 6163 6365 7373 6962 696c 6974 792e  r accessibility.
-00010e90: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
-00010ea0: 756e 7370 6563 6966 6965 642c 2074 6865  unspecified, the
-00010eb0: 2064 6566 6175 6c74 2076 616c 7565 2060   default value `
-00010ec0: 6042 7574 746f 6e60 6020 6973 2070 726f  `Button`` is pro
-00010ed0: 7669 6465 642e 2041 730a 2020 2020 2020  vided. As.      
-00010ee0: 2020 2020 2020 6120 6265 7374 2070 7261        a best pra
-00010ef0: 6374 6963 652c 2079 6f75 2073 686f 756c  ctice, you shoul
-00010f00: 6420 7365 7420 6120 6865 6c70 6675 6c20  d set a helpful 
-00010f10: 6465 7363 7269 7074 696f 6e20 666f 720a  description for.
-00010f20: 2020 2020 2020 2020 2020 2020 7768 6174              what
-00010f30: 2074 6865 2069 636f 6e20 6469 7370 6c61   the icon displa
-00010f40: 7973 2c20 616e 6420 6966 2061 7070 6c69  ys, and if appli
-00010f50: 6361 626c 652c 2077 6861 7420 6974 2064  cable, what it d
-00010f60: 6f65 732e 2046 6f72 0a20 2020 2020 2020  oes. For.       
-00010f70: 2020 2020 2065 7861 6d70 6c65 2c20 6060       example, ``
-00010f80: 4120 7573 6572 2773 2061 6363 6f75 6e74  A user's account
-00010f90: 2070 6f72 7472 6169 7460 602c 206f 720a   portrait``, or.
-00010fa0: 2020 2020 2020 2020 2020 2020 6060 4f70              ``Op
-00010fb0: 656e 7320 6120 6e65 7720 6272 6f77 7365  ens a new browse
-00010fc0: 7220 7461 6220 616e 6420 6e61 7669 6761  r tab and naviga
-00010fd0: 7465 7320 746f 2074 6865 2047 6f6f 676c  tes to the Googl
-00010fe0: 6520 4368 6174 2064 6576 656c 6f70 6572  e Chat developer
-00010ff0: 2064 6f63 756d 656e 7461 7469 6f6e 2061   documentation a
-00011000: 7420 6874 7470 733a 2f2f 6465 7665 6c6f  t https://develo
-00011010: 7065 7273 2e67 6f6f 676c 652e 636f 6d2f  pers.google.com/
-00011020: 6368 6174 6060 2e0a 0a20 2020 2020 2020  chat``...       
-00011030: 2020 2020 2049 6620 7468 6520 6963 6f6e       If the icon
-00011040: 2069 7320 7365 7420 696e 2061 0a20 2020   is set in a.   
-00011050: 2020 2020 2020 2020 205b 6060 4275 7474           [``Butt
-00011060: 6f6e 6060 5d5b 676f 6f67 6c65 2e61 7070  on``][google.app
-00011070: 732e 6361 7264 2e76 312e 4275 7474 6f6e  s.card.v1.Button
-00011080: 5d2c 2074 6865 2060 6061 6c74 5465 7874  ], the ``altText
-00011090: 6060 0a20 2020 2020 2020 2020 2020 2061  ``.            a
-000110a0: 7070 6561 7273 2061 7320 6865 6c70 6572  ppears as helper
-000110b0: 2074 6578 7420 7768 656e 2074 6865 2075   text when the u
-000110c0: 7365 7220 686f 7665 7273 206f 7665 7220  ser hovers over 
-000110d0: 7468 6520 6275 7474 6f6e 2e0a 2020 2020  the button..    
-000110e0: 2020 2020 2020 2020 486f 7765 7665 722c          However,
-000110f0: 2069 6620 7468 6520 6275 7474 6f6e 2061   if the button a
-00011100: 6c73 6f20 7365 7473 2060 6074 6578 7460  lso sets ``text`
-00011110: 602c 2074 6865 2069 636f 6e27 730a 2020  `, the icon's.  
-00011120: 2020 2020 2020 2020 2020 6060 616c 7454            ``altT
-00011130: 6578 7460 6020 6973 2069 676e 6f72 6564  ext`` is ignored
-00011140: 2e0a 2020 2020 2020 2020 696d 6167 655f  ..        image_
-00011150: 7479 7065 2028 676f 6f67 6c65 2e61 7070  type (google.app
-00011160: 732e 6361 7264 5f76 312e 7479 7065 732e  s.card_v1.types.
-00011170: 5769 6467 6574 2e49 6d61 6765 5479 7065  Widget.ImageType
-00011180: 293a 0a20 2020 2020 2020 2020 2020 2054  ):.            T
-00011190: 6865 2063 726f 7020 7374 796c 6520 6170  he crop style ap
-000111a0: 706c 6965 6420 746f 2074 6865 2069 6d61  plied to the ima
-000111b0: 6765 2e20 496e 2073 6f6d 6520 6361 7365  ge. In some case
-000111c0: 732c 2061 7070 6c79 696e 670a 2020 2020  s, applying.    
-000111d0: 2020 2020 2020 2020 6120 6060 4349 5243          a ``CIRC
-000111e0: 4c45 6060 2063 726f 7020 6361 7573 6573  LE`` crop causes
-000111f0: 2074 6865 2069 6d61 6765 2074 6f20 6265   the image to be
-00011200: 2064 7261 776e 206c 6172 6765 7220 7468   drawn larger th
-00011210: 616e 2061 0a20 2020 2020 2020 2020 2020  an a.           
-00011220: 2062 7569 6c74 2d69 6e20 6963 6f6e 2e0a   built-in icon..
-00011230: 2020 2020 2222 220a 0a20 2020 206b 6e6f      """..    kno
-00011240: 776e 5f69 636f 6e3a 2073 7472 203d 2070  wn_icon: str = p
-00011250: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
-00011260: 2020 2020 7072 6f74 6f2e 5354 5249 4e47      proto.STRING
-00011270: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
-00011280: 3d31 2c0a 2020 2020 2020 2020 6f6e 656f  =1,.        oneo
-00011290: 663d 2269 636f 6e73 222c 0a20 2020 2029  f="icons",.    )
-000112a0: 0a20 2020 2069 636f 6e5f 7572 6c3a 2073  .    icon_url: s
-000112b0: 7472 203d 2070 726f 746f 2e46 6965 6c64  tr = proto.Field
-000112c0: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
-000112d0: 5354 5249 4e47 2c0a 2020 2020 2020 2020  STRING,.        
-000112e0: 6e75 6d62 6572 3d32 2c0a 2020 2020 2020  number=2,.      
-000112f0: 2020 6f6e 656f 663d 2269 636f 6e73 222c    oneof="icons",
-00011300: 0a20 2020 2029 0a20 2020 2061 6c74 5f74  .    ).    alt_t
-00011310: 6578 743a 2073 7472 203d 2070 726f 746f  ext: str = proto
-00011320: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
-00011330: 7072 6f74 6f2e 5354 5249 4e47 2c0a 2020  proto.STRING,.  
-00011340: 2020 2020 2020 6e75 6d62 6572 3d33 2c0a        number=3,.
-00011350: 2020 2020 290a 2020 2020 696d 6167 655f      ).    image_
-00011360: 7479 7065 3a20 2257 6964 6765 742e 496d  type: "Widget.Im
-00011370: 6167 6554 7970 6522 203d 2070 726f 746f  ageType" = proto
-00011380: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
-00011390: 7072 6f74 6f2e 454e 554d 2c0a 2020 2020  proto.ENUM,.    
-000113a0: 2020 2020 6e75 6d62 6572 3d34 2c0a 2020      number=4,.  
-000113b0: 2020 2020 2020 656e 756d 3d22 5769 6467        enum="Widg
-000113c0: 6574 2e49 6d61 6765 5479 7065 222c 0a20  et.ImageType",. 
-000113d0: 2020 2029 0a0a 0a63 6c61 7373 2049 6d61     )...class Ima
-000113e0: 6765 4372 6f70 5374 796c 6528 7072 6f74  geCropStyle(prot
-000113f0: 6f2e 4d65 7373 6167 6529 3a0a 2020 2020  o.Message):.    
-00011400: 7222 2222 5265 7072 6573 656e 7473 2074  r"""Represents t
-00011410: 6865 2063 726f 7020 7374 796c 6520 6170  he crop style ap
-00011420: 706c 6965 6420 746f 2061 6e20 696d 6167  plied to an imag
-00011430: 652e 0a0a 2020 2020 6047 6f6f 676c 6520  e...    `Google 
-00011440: 576f 726b 7370 6163 6520 4164 642d 6f6e  Workspace Add-on
-00011450: 7320 616e 6420 4368 6174 0a20 2020 2061  s and Chat.    a
-00011460: 7070 7320 3c68 7474 7073 3a2f 2f64 6576  pps <https://dev
-00011470: 656c 6f70 6572 732e 676f 6f67 6c65 2e63  elopers.google.c
-00011480: 6f6d 2f77 6f72 6b73 7061 6365 2f65 7874  om/workspace/ext
-00011490: 656e 643e 605f 5f3a 0a0a 2020 2020 466f  end>`__:..    Fo
-000114a0: 7220 6578 616d 706c 652c 2068 6572 6527  r example, here'
-000114b0: 7320 686f 7720 746f 2061 7070 6c79 2061  s how to apply a
-000114c0: 2031 363a 3920 6173 7065 6374 2072 6174   16:9 aspect rat
-000114d0: 696f 3a0a 0a20 2020 203a 3a0a 0a20 2020  io:..    ::..   
-000114e0: 2020 2020 6372 6f70 5374 796c 6520 7b0a      cropStyle {.
-000114f0: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
-00011500: 2252 4543 5441 4e47 4c45 5f43 5553 544f  "RECTANGLE_CUSTO
-00011510: 4d22 2c0a 2020 2020 2020 2020 2261 7370  M",.        "asp
-00011520: 6563 7452 6174 696f 223a 2031 362f 390a  ectRatio": 16/9.
-00011530: 2020 2020 2020 207d 0a0a 2020 2020 4174         }..    At
-00011540: 7472 6962 7574 6573 3a0a 2020 2020 2020  tributes:.      
-00011550: 2020 7479 7065 5f20 2867 6f6f 676c 652e    type_ (google.
-00011560: 6170 7073 2e63 6172 645f 7631 2e74 7970  apps.card_v1.typ
-00011570: 6573 2e49 6d61 6765 4372 6f70 5374 796c  es.ImageCropStyl
-00011580: 652e 496d 6167 6543 726f 7054 7970 6529  e.ImageCropType)
-00011590: 3a0a 2020 2020 2020 2020 2020 2020 5468  :.            Th
-000115a0: 6520 6372 6f70 2074 7970 652e 0a20 2020  e crop type..   
-000115b0: 2020 2020 2061 7370 6563 745f 7261 7469       aspect_rati
-000115c0: 6f20 2866 6c6f 6174 293a 0a20 2020 2020  o (float):.     
-000115d0: 2020 2020 2020 2054 6865 2061 7370 6563         The aspec
-000115e0: 7420 7261 7469 6f20 746f 2075 7365 2069  t ratio to use i
-000115f0: 6620 7468 6520 6372 6f70 2074 7970 6520  f the crop type 
-00011600: 6973 0a20 2020 2020 2020 2020 2020 2060  is.            `
-00011610: 6052 4543 5441 4e47 4c45 5f43 5553 544f  `RECTANGLE_CUSTO
-00011620: 4d60 602e 0a0a 2020 2020 2020 2020 2020  M``...          
-00011630: 2020 466f 7220 6578 616d 706c 652c 2068    For example, h
-00011640: 6572 6527 7320 686f 7720 746f 2061 7070  ere's how to app
-00011650: 6c79 2061 2031 363a 3920 6173 7065 6374  ly a 16:9 aspect
-00011660: 2072 6174 696f 3a0a 0a20 2020 2020 2020   ratio:..       
-00011670: 2020 2020 203a 3a0a 0a20 2020 2020 2020       ::..       
-00011680: 2020 2020 2020 2020 6372 6f70 5374 796c          cropStyl
-00011690: 6520 7b0a 2020 2020 2020 2020 2020 2020  e {.            
-000116a0: 2020 2020 2274 7970 6522 3a20 2252 4543      "type": "REC
-000116b0: 5441 4e47 4c45 5f43 5553 544f 4d22 2c0a  TANGLE_CUSTOM",.
-000116c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000116d0: 2261 7370 6563 7452 6174 696f 223a 2031  "aspectRatio": 1
-000116e0: 362f 390a 2020 2020 2020 2020 2020 2020  6/9.            
-000116f0: 2020 207d 0a20 2020 2022 2222 0a0a 2020     }.    """..  
-00011700: 2020 636c 6173 7320 496d 6167 6543 726f    class ImageCro
-00011710: 7054 7970 6528 7072 6f74 6f2e 456e 756d  pType(proto.Enum
-00011720: 293a 0a20 2020 2020 2020 2072 2222 2252  ):.        r"""R
-00011730: 6570 7265 7365 6e74 7320 7468 6520 6372  epresents the cr
-00011740: 6f70 2073 7479 6c65 2061 7070 6c69 6564  op style applied
-00011750: 2074 6f20 616e 2069 6d61 6765 2e0a 0a20   to an image... 
-00011760: 2020 2020 2020 2060 476f 6f67 6c65 2057         `Google W
-00011770: 6f72 6b73 7061 6365 2041 6464 2d6f 6e73  orkspace Add-ons
-00011780: 2061 6e64 2043 6861 740a 2020 2020 2020   and Chat.      
-00011790: 2020 6170 7073 203c 6874 7470 733a 2f2f    apps <https://
-000117a0: 6465 7665 6c6f 7065 7273 2e67 6f6f 676c  developers.googl
-000117b0: 652e 636f 6d2f 776f 726b 7370 6163 652f  e.com/workspace/
-000117c0: 6578 7465 6e64 3e60 5f5f 3a0a 0a20 2020  extend>`__:..   
-000117d0: 2020 2020 2056 616c 7565 733a 0a20 2020       Values:.   
-000117e0: 2020 2020 2020 2020 2049 4d41 4745 5f43           IMAGE_C
-000117f0: 524f 505f 5459 5045 5f55 4e53 5045 4349  ROP_TYPE_UNSPECI
-00011800: 4649 4544 2028 3029 3a0a 2020 2020 2020  FIED (0):.      
-00011810: 2020 2020 2020 2020 2020 446f 6e27 7420            Don't 
-00011820: 7573 652e 2055 6e73 7065 6369 6669 6564  use. Unspecified
-00011830: 2e0a 2020 2020 2020 2020 2020 2020 5351  ..            SQ
-00011840: 5541 5245 2028 3129 3a0a 2020 2020 2020  UARE (1):.      
-00011850: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
-00011860: 7420 7661 6c75 652e 2041 7070 6c69 6573  t value. Applies
-00011870: 2061 2073 7175 6172 6520 6372 6f70 2e0a   a square crop..
-00011880: 2020 2020 2020 2020 2020 2020 4349 5243              CIRC
-00011890: 4c45 2028 3229 3a0a 2020 2020 2020 2020  LE (2):.        
-000118a0: 2020 2020 2020 2020 4170 706c 6965 7320          Applies 
-000118b0: 6120 6369 7263 756c 6172 2063 726f 702e  a circular crop.
-000118c0: 0a20 2020 2020 2020 2020 2020 2052 4543  .            REC
-000118d0: 5441 4e47 4c45 5f43 5553 544f 4d20 2833  TANGLE_CUSTOM (3
-000118e0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000118f0: 2020 2041 7070 6c69 6573 2061 2072 6563     Applies a rec
-00011900: 7461 6e67 756c 6172 2063 726f 7020 7769  tangular crop wi
-00011910: 7468 2061 2063 7573 746f 6d20 6173 7065  th a custom aspe
-00011920: 6374 2072 6174 696f 2e20 5365 740a 2020  ct ratio. Set.  
-00011930: 2020 2020 2020 2020 2020 2020 2020 7468                th
-00011940: 6520 6375 7374 6f6d 2061 7370 6563 7420  e custom aspect 
-00011950: 7261 7469 6f20 7769 7468 2060 6061 7370  ratio with ``asp
-00011960: 6563 7452 6174 696f 6060 2e0a 2020 2020  ectRatio``..    
-00011970: 2020 2020 2020 2020 5245 4354 414e 474c          RECTANGL
-00011980: 455f 345f 3320 2834 293a 0a20 2020 2020  E_4_3 (4):.     
-00011990: 2020 2020 2020 2020 2020 2041 7070 6c69             Appli
-000119a0: 6573 2061 2072 6563 7461 6e67 756c 6172  es a rectangular
-000119b0: 2063 726f 7020 7769 7468 2061 2034 3a33   crop with a 4:3
-000119c0: 2061 7370 6563 740a 2020 2020 2020 2020   aspect.        
-000119d0: 2020 2020 2020 2020 7261 7469 6f2e 0a20          ratio.. 
-000119e0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000119f0: 2020 2049 4d41 4745 5f43 524f 505f 5459     IMAGE_CROP_TY
-00011a00: 5045 5f55 4e53 5045 4349 4649 4544 203d  PE_UNSPECIFIED =
-00011a10: 2030 0a20 2020 2020 2020 2053 5155 4152   0.        SQUAR
-00011a20: 4520 3d20 310a 2020 2020 2020 2020 4349  E = 1.        CI
-00011a30: 5243 4c45 203d 2032 0a20 2020 2020 2020  RCLE = 2.       
-00011a40: 2052 4543 5441 4e47 4c45 5f43 5553 544f   RECTANGLE_CUSTO
-00011a50: 4d20 3d20 330a 2020 2020 2020 2020 5245  M = 3.        RE
-00011a60: 4354 414e 474c 455f 345f 3320 3d20 340a  CTANGLE_4_3 = 4.
-00011a70: 0a20 2020 2074 7970 655f 3a20 496d 6167  .    type_: Imag
-00011a80: 6543 726f 7054 7970 6520 3d20 7072 6f74  eCropType = prot
-00011a90: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-00011aa0: 2070 726f 746f 2e45 4e55 4d2c 0a20 2020   proto.ENUM,.   
-00011ab0: 2020 2020 206e 756d 6265 723d 312c 0a20       number=1,. 
-00011ac0: 2020 2020 2020 2065 6e75 6d3d 496d 6167         enum=Imag
-00011ad0: 6543 726f 7054 7970 652c 0a20 2020 2029  eCropType,.    )
-00011ae0: 0a20 2020 2061 7370 6563 745f 7261 7469  .    aspect_rati
-00011af0: 6f3a 2066 6c6f 6174 203d 2070 726f 746f  o: float = proto
-00011b00: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
-00011b10: 7072 6f74 6f2e 444f 5542 4c45 2c0a 2020  proto.DOUBLE,.  
-00011b20: 2020 2020 2020 6e75 6d62 6572 3d32 2c0a        number=2,.
-00011b30: 2020 2020 290a 0a0a 636c 6173 7320 426f      )...class Bo
-00011b40: 7264 6572 5374 796c 6528 7072 6f74 6f2e  rderStyle(proto.
-00011b50: 4d65 7373 6167 6529 3a0a 2020 2020 7222  Message):.    r"
-00011b60: 2222 5468 6520 7374 796c 6520 6f70 7469  ""The style opti
-00011b70: 6f6e 7320 666f 7220 7468 6520 626f 7264  ons for the bord
-00011b80: 6572 206f 6620 6120 6361 7264 206f 7220  er of a card or 
-00011b90: 7769 6467 6574 2c20 696e 636c 7564 696e  widget, includin
-00011ba0: 6720 7468 650a 2020 2020 626f 7264 6572  g the.    border
-00011bb0: 2074 7970 6520 616e 6420 636f 6c6f 722e   type and color.
-00011bc0: 0a0a 2020 2020 6047 6f6f 676c 6520 576f  ..    `Google Wo
-00011bd0: 726b 7370 6163 6520 4164 642d 6f6e 7320  rkspace Add-ons 
-00011be0: 616e 6420 4368 6174 0a20 2020 2061 7070  and Chat.    app
-00011bf0: 7320 3c68 7474 7073 3a2f 2f64 6576 656c  s <https://devel
-00011c00: 6f70 6572 732e 676f 6f67 6c65 2e63 6f6d  opers.google.com
-00011c10: 2f77 6f72 6b73 7061 6365 2f65 7874 656e  /workspace/exten
-00011c20: 643e 605f 5f3a 0a0a 2020 2020 4174 7472  d>`__:..    Attr
-00011c30: 6962 7574 6573 3a0a 2020 2020 2020 2020  ibutes:.        
-00011c40: 7479 7065 5f20 2867 6f6f 676c 652e 6170  type_ (google.ap
-00011c50: 7073 2e63 6172 645f 7631 2e74 7970 6573  ps.card_v1.types
-00011c60: 2e42 6f72 6465 7253 7479 6c65 2e42 6f72  .BorderStyle.Bor
-00011c70: 6465 7254 7970 6529 3a0a 2020 2020 2020  derType):.      
-00011c80: 2020 2020 2020 5468 6520 626f 7264 6572        The border
-00011c90: 2074 7970 652e 0a20 2020 2020 2020 2073   type..        s
-00011ca0: 7472 6f6b 655f 636f 6c6f 7220 2867 6f6f  troke_color (goo
-00011cb0: 676c 652e 7479 7065 2e63 6f6c 6f72 5f70  gle.type.color_p
-00011cc0: 6232 2e43 6f6c 6f72 293a 0a20 2020 2020  b2.Color):.     
-00011cd0: 2020 2020 2020 2054 6865 2063 6f6c 6f72         The color
-00011ce0: 7320 746f 2075 7365 2077 6865 6e20 7468  s to use when th
-00011cf0: 6520 7479 7065 2069 7320 6060 424f 5244  e type is ``BORD
-00011d00: 4552 5f54 5950 455f 5354 524f 4b45 6060  ER_TYPE_STROKE``
-00011d10: 2e0a 2020 2020 2020 2020 636f 726e 6572  ..        corner
-00011d20: 5f72 6164 6975 7320 2869 6e74 293a 0a20  _radius (int):. 
-00011d30: 2020 2020 2020 2020 2020 2054 6865 2063             The c
-00011d40: 6f72 6e65 7220 7261 6469 7573 2066 6f72  orner radius for
-00011d50: 2074 6865 2062 6f72 6465 722e 0a20 2020   the border..   
-00011d60: 2022 2222 0a0a 2020 2020 636c 6173 7320   """..    class 
-00011d70: 426f 7264 6572 5479 7065 2870 726f 746f  BorderType(proto
-00011d80: 2e45 6e75 6d29 3a0a 2020 2020 2020 2020  .Enum):.        
-00011d90: 7222 2222 5265 7072 6573 656e 7473 2074  r"""Represents t
-00011da0: 6865 2062 6f72 6465 7220 7479 7065 7320  he border types 
-00011db0: 6170 706c 6965 6420 746f 2077 6964 6765  applied to widge
-00011dc0: 7473 2e0a 0a20 2020 2020 2020 2060 476f  ts...        `Go
-00011dd0: 6f67 6c65 2057 6f72 6b73 7061 6365 2041  ogle Workspace A
-00011de0: 6464 2d6f 6e73 2061 6e64 2043 6861 740a  dd-ons and Chat.
-00011df0: 2020 2020 2020 2020 6170 7073 203c 6874          apps <ht
-00011e00: 7470 733a 2f2f 6465 7665 6c6f 7065 7273  tps://developers
-00011e10: 2e67 6f6f 676c 652e 636f 6d2f 776f 726b  .google.com/work
-00011e20: 7370 6163 652f 6578 7465 6e64 3e60 5f5f  space/extend>`__
-00011e30: 3a0a 0a20 2020 2020 2020 2056 616c 7565  :..        Value
-00011e40: 733a 0a20 2020 2020 2020 2020 2020 2042  s:.            B
-00011e50: 4f52 4445 525f 5459 5045 5f55 4e53 5045  ORDER_TYPE_UNSPE
-00011e60: 4349 4649 4544 2028 3029 3a0a 2020 2020  CIFIED (0):.    
-00011e70: 2020 2020 2020 2020 2020 2020 446f 6e27              Don'
-00011e80: 7420 7573 652e 2055 6e73 7065 6369 6669  t use. Unspecifi
-00011e90: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
-00011ea0: 4e4f 5f42 4f52 4445 5220 2831 293a 0a20  NO_BORDER (1):. 
-00011eb0: 2020 2020 2020 2020 2020 2020 2020 2044                 D
-00011ec0: 6566 6175 6c74 2076 616c 7565 2e20 4e6f  efault value. No
-00011ed0: 2062 6f72 6465 722e 0a20 2020 2020 2020   border..       
-00011ee0: 2020 2020 2053 5452 4f4b 4520 2832 293a       STROKE (2):
-00011ef0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011f00: 204f 7574 6c69 6e65 2e0a 2020 2020 2020   Outline..      
-00011f10: 2020 2222 220a 2020 2020 2020 2020 424f    """.        BO
-00011f20: 5244 4552 5f54 5950 455f 554e 5350 4543  RDER_TYPE_UNSPEC
-00011f30: 4946 4945 4420 3d20 300a 2020 2020 2020  IFIED = 0.      
-00011f40: 2020 4e4f 5f42 4f52 4445 5220 3d20 310a    NO_BORDER = 1.
-00011f50: 2020 2020 2020 2020 5354 524f 4b45 203d          STROKE =
-00011f60: 2032 0a0a 2020 2020 7479 7065 5f3a 2042   2..    type_: B
-00011f70: 6f72 6465 7254 7970 6520 3d20 7072 6f74  orderType = prot
-00011f80: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-00011f90: 2070 726f 746f 2e45 4e55 4d2c 0a20 2020   proto.ENUM,.   
-00011fa0: 2020 2020 206e 756d 6265 723d 312c 0a20       number=1,. 
-00011fb0: 2020 2020 2020 2065 6e75 6d3d 426f 7264         enum=Bord
-00011fc0: 6572 5479 7065 2c0a 2020 2020 290a 2020  erType,.    ).  
-00011fd0: 2020 7374 726f 6b65 5f63 6f6c 6f72 3a20    stroke_color: 
-00011fe0: 636f 6c6f 725f 7062 322e 436f 6c6f 7220  color_pb2.Color 
-00011ff0: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
-00012000: 2020 2020 2020 2070 726f 746f 2e4d 4553         proto.MES
-00012010: 5341 4745 2c0a 2020 2020 2020 2020 6e75  SAGE,.        nu
-00012020: 6d62 6572 3d32 2c0a 2020 2020 2020 2020  mber=2,.        
-00012030: 6d65 7373 6167 653d 636f 6c6f 725f 7062  message=color_pb
-00012040: 322e 436f 6c6f 722c 0a20 2020 2029 0a20  2.Color,.    ). 
-00012050: 2020 2063 6f72 6e65 725f 7261 6469 7573     corner_radius
-00012060: 3a20 696e 7420 3d20 7072 6f74 6f2e 4669  : int = proto.Fi
-00012070: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
-00012080: 746f 2e49 4e54 3332 2c0a 2020 2020 2020  to.INT32,.      
-00012090: 2020 6e75 6d62 6572 3d33 2c0a 2020 2020    number=3,.    
-000120a0: 290a 0a0a 636c 6173 7320 496d 6167 6543  )...class ImageC
-000120b0: 6f6d 706f 6e65 6e74 2870 726f 746f 2e4d  omponent(proto.M
-000120c0: 6573 7361 6765 293a 0a20 2020 2072 2222  essage):.    r""
-000120d0: 2252 6570 7265 7365 6e74 7320 616e 2069  "Represents an i
-000120e0: 6d61 6765 2e0a 0a20 2020 2060 476f 6f67  mage...    `Goog
-000120f0: 6c65 2057 6f72 6b73 7061 6365 2041 6464  le Workspace Add
-00012100: 2d6f 6e73 2061 6e64 2043 6861 740a 2020  -ons and Chat.  
-00012110: 2020 6170 7073 203c 6874 7470 733a 2f2f    apps <https://
-00012120: 6465 7665 6c6f 7065 7273 2e67 6f6f 676c  developers.googl
-00012130: 652e 636f 6d2f 776f 726b 7370 6163 652f  e.com/workspace/
-00012140: 6578 7465 6e64 3e60 5f5f 3a0a 0a20 2020  extend>`__:..   
-00012150: 2041 7474 7269 6275 7465 733a 0a20 2020   Attributes:.   
-00012160: 2020 2020 2069 6d61 6765 5f75 7269 2028       image_uri (
-00012170: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
-00012180: 2020 5468 6520 696d 6167 6520 5552 4c2e    The image URL.
-00012190: 0a20 2020 2020 2020 2061 6c74 5f74 6578  .        alt_tex
-000121a0: 7420 2873 7472 293a 0a20 2020 2020 2020  t (str):.       
-000121b0: 2020 2020 2054 6865 2061 6363 6573 7369       The accessi
-000121c0: 6269 6c69 7479 206c 6162 656c 2066 6f72  bility label for
-000121d0: 2074 6865 2069 6d61 6765 2e0a 2020 2020   the image..    
-000121e0: 2020 2020 6372 6f70 5f73 7479 6c65 2028      crop_style (
-000121f0: 676f 6f67 6c65 2e61 7070 732e 6361 7264  google.apps.card
-00012200: 5f76 312e 7479 7065 732e 496d 6167 6543  _v1.types.ImageC
-00012210: 726f 7053 7479 6c65 293a 0a20 2020 2020  ropStyle):.     
-00012220: 2020 2020 2020 2054 6865 2063 726f 7020         The crop 
-00012230: 7374 796c 6520 746f 2061 7070 6c79 2074  style to apply t
-00012240: 6f20 7468 6520 696d 6167 652e 0a20 2020  o the image..   
-00012250: 2020 2020 2062 6f72 6465 725f 7374 796c       border_styl
-00012260: 6520 2867 6f6f 676c 652e 6170 7073 2e63  e (google.apps.c
-00012270: 6172 645f 7631 2e74 7970 6573 2e42 6f72  ard_v1.types.Bor
-00012280: 6465 7253 7479 6c65 293a 0a20 2020 2020  derStyle):.     
-00012290: 2020 2020 2020 2054 6865 2062 6f72 6465         The borde
-000122a0: 7220 7374 796c 6520 746f 2061 7070 6c79  r style to apply
-000122b0: 2074 6f20 7468 6520 696d 6167 652e 0a20   to the image.. 
-000122c0: 2020 2022 2222 0a0a 2020 2020 696d 6167     """..    imag
-000122d0: 655f 7572 693a 2073 7472 203d 2070 726f  e_uri: str = pro
-000122e0: 746f 2e46 6965 6c64 280a 2020 2020 2020  to.Field(.      
-000122f0: 2020 7072 6f74 6f2e 5354 5249 4e47 2c0a    proto.STRING,.
-00012300: 2020 2020 2020 2020 6e75 6d62 6572 3d31          number=1
-00012310: 2c0a 2020 2020 290a 2020 2020 616c 745f  ,.    ).    alt_
-00012320: 7465 7874 3a20 7374 7220 3d20 7072 6f74  text: str = prot
-00012330: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-00012340: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
-00012350: 2020 2020 2020 206e 756d 6265 723d 322c         number=2,
-00012360: 0a20 2020 2029 0a20 2020 2063 726f 705f  .    ).    crop_
-00012370: 7374 796c 653a 2022 496d 6167 6543 726f  style: "ImageCro
-00012380: 7053 7479 6c65 2220 3d20 7072 6f74 6f2e  pStyle" = proto.
-00012390: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
-000123a0: 726f 746f 2e4d 4553 5341 4745 2c0a 2020  roto.MESSAGE,.  
-000123b0: 2020 2020 2020 6e75 6d62 6572 3d33 2c0a        number=3,.
-000123c0: 2020 2020 2020 2020 6d65 7373 6167 653d          message=
-000123d0: 2249 6d61 6765 4372 6f70 5374 796c 6522  "ImageCropStyle"
-000123e0: 2c0a 2020 2020 290a 2020 2020 626f 7264  ,.    ).    bord
-000123f0: 6572 5f73 7479 6c65 3a20 2242 6f72 6465  er_style: "Borde
-00012400: 7253 7479 6c65 2220 3d20 7072 6f74 6f2e  rStyle" = proto.
-00012410: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
-00012420: 726f 746f 2e4d 4553 5341 4745 2c0a 2020  roto.MESSAGE,.  
-00012430: 2020 2020 2020 6e75 6d62 6572 3d34 2c0a        number=4,.
-00012440: 2020 2020 2020 2020 6d65 7373 6167 653d          message=
-00012450: 2242 6f72 6465 7253 7479 6c65 222c 0a20  "BorderStyle",. 
-00012460: 2020 2029 0a0a 0a63 6c61 7373 2047 7269     )...class Gri
-00012470: 6428 7072 6f74 6f2e 4d65 7373 6167 6529  d(proto.Message)
-00012480: 3a0a 2020 2020 7222 2222 4469 7370 6c61  :.    r"""Displa
-00012490: 7973 2061 2067 7269 6420 7769 7468 2061  ys a grid with a
-000124a0: 2063 6f6c 6c65 6374 696f 6e20 6f66 2069   collection of i
-000124b0: 7465 6d73 2e20 4974 656d 7320 6361 6e20  tems. Items can 
-000124c0: 6f6e 6c79 2069 6e63 6c75 6465 0a20 2020  only include.   
-000124d0: 2074 6578 7420 6f72 2069 6d61 6765 732e   text or images.
-000124e0: 2046 6f72 2072 6573 706f 6e73 6976 6520   For responsive 
-000124f0: 636f 6c75 6d6e 732c 206f 7220 746f 2069  columns, or to i
-00012500: 6e63 6c75 6465 206d 6f72 6520 7468 616e  nclude more than
-00012510: 2074 6578 740a 2020 2020 6f72 2069 6d61   text.    or ima
-00012520: 6765 732c 2075 7365 205b 6060 436f 6c75  ges, use [``Colu
-00012530: 6d6e 7360 605d 5b67 6f6f 676c 652e 6170  mns``][google.ap
-00012540: 7073 2e63 6172 642e 7631 2e43 6f6c 756d  ps.card.v1.Colum
-00012550: 6e73 5d2e 2046 6f72 2061 6e0a 2020 2020  ns]. For an.    
-00012560: 6578 616d 706c 6520 696e 2047 6f6f 676c  example in Googl
-00012570: 6520 4368 6174 2061 7070 732c 2073 6565  e Chat apps, see
-00012580: 0a20 2020 2060 4772 6964 203c 6874 7470  .    `Grid <http
-00012590: 733a 2f2f 6465 7665 6c6f 7065 7273 2e67  s://developers.g
-000125a0: 6f6f 676c 652e 636f 6d2f 6368 6174 2f75  oogle.com/chat/u
-000125b0: 692f 7769 6467 6574 732f 6772 6964 3e60  i/widgets/grid>`
-000125c0: 5f5f 2e0a 0a20 2020 2041 2067 7269 6420  __...    A grid 
-000125d0: 7375 7070 6f72 7473 2061 6e79 206e 756d  supports any num
-000125e0: 6265 7220 6f66 2063 6f6c 756d 6e73 2061  ber of columns a
-000125f0: 6e64 2069 7465 6d73 2e20 5468 6520 6e75  nd items. The nu
-00012600: 6d62 6572 206f 6620 726f 7773 0a20 2020  mber of rows.   
-00012610: 2069 7320 6465 7465 726d 696e 6564 2062   is determined b
-00012620: 7920 6974 656d 7320 6469 7669 6465 6420  y items divided 
-00012630: 6279 2063 6f6c 756d 6e73 2e20 4120 6772  by columns. A gr
-00012640: 6964 2077 6974 6820 3130 2069 7465 6d73  id with 10 items
-00012650: 2061 6e64 0a20 2020 2032 2063 6f6c 756d   and.    2 colum
-00012660: 6e73 2068 6173 2035 2072 6f77 732e 2041  ns has 5 rows. A
-00012670: 2067 7269 6420 7769 7468 2031 3120 6974   grid with 11 it
-00012680: 656d 7320 616e 6420 3220 636f 6c75 6d6e  ems and 2 column
-00012690: 7320 6861 7320 3620 726f 7773 2e0a 0a20  s has 6 rows... 
-000126a0: 2020 2060 476f 6f67 6c65 2057 6f72 6b73     `Google Works
-000126b0: 7061 6365 2041 6464 2d6f 6e73 2061 6e64  pace Add-ons and
-000126c0: 2043 6861 740a 2020 2020 6170 7073 203c   Chat.    apps <
-000126d0: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
-000126e0: 7273 2e67 6f6f 676c 652e 636f 6d2f 776f  rs.google.com/wo
-000126f0: 726b 7370 6163 652f 6578 7465 6e64 3e60  rkspace/extend>`
-00012700: 5f5f 3a0a 0a20 2020 2046 6f72 2065 7861  __:..    For exa
-00012710: 6d70 6c65 2c20 7468 6520 666f 6c6c 6f77  mple, the follow
-00012720: 696e 6720 4a53 4f4e 2063 7265 6174 6573  ing JSON creates
-00012730: 2061 2032 2063 6f6c 756d 6e20 6772 6964   a 2 column grid
-00012740: 2077 6974 6820 610a 2020 2020 7369 6e67   with a.    sing
-00012750: 6c65 2069 7465 6d3a 0a0a 2020 2020 3a3a  le item:..    ::
-00012760: 0a0a 2020 2020 2020 2022 6772 6964 223a  ..       "grid":
-00012770: 207b 0a20 2020 2020 2020 2020 2274 6974   {.         "tit
-00012780: 6c65 223a 2022 4120 6669 6e65 2063 6f6c  le": "A fine col
-00012790: 6c65 6374 696f 6e20 6f66 2069 7465 6d73  lection of items
-000127a0: 222c 0a20 2020 2020 2020 2020 2263 6f6c  ",.         "col
-000127b0: 756d 6e43 6f75 6e74 223a 2032 2c0a 2020  umnCount": 2,.  
-000127c0: 2020 2020 2020 2022 626f 7264 6572 5374         "borderSt
-000127d0: 796c 6522 3a20 7b0a 2020 2020 2020 2020  yle": {.        
-000127e0: 2020 2022 7479 7065 223a 2022 5354 524f     "type": "STRO
-000127f0: 4b45 222c 0a20 2020 2020 2020 2020 2020  KE",.           
-00012800: 2263 6f72 6e65 7252 6164 6975 7322 3a20  "cornerRadius": 
-00012810: 340a 2020 2020 2020 2020 207d 2c0a 2020  4.         },.  
-00012820: 2020 2020 2020 2022 6974 656d 7322 3a20         "items": 
-00012830: 5b0a 2020 2020 2020 2020 2020 207b 0a20  [.           {. 
-00012840: 2020 2020 2020 2020 2020 2020 2269 6d61              "ima
-00012850: 6765 223a 207b 0a20 2020 2020 2020 2020  ge": {.         
-00012860: 2020 2020 2020 2269 6d61 6765 5572 6922        "imageUri"
-00012870: 3a20 2268 7474 7073 3a2f 2f77 7777 2e65  : "https://www.e
-00012880: 7861 6d70 6c65 2e63 6f6d 2f69 6d61 6765  xample.com/image
-00012890: 2e70 6e67 222c 0a20 2020 2020 2020 2020  .png",.         
-000128a0: 2020 2020 2020 2263 726f 7053 7479 6c65        "cropStyle
-000128b0: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-000128c0: 2020 2020 2020 2274 7970 6522 3a20 2253        "type": "S
-000128d0: 5155 4152 4522 0a20 2020 2020 2020 2020  QUARE".         
-000128e0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-000128f0: 2020 2020 2020 2020 2262 6f72 6465 7253          "borderS
-00012900: 7479 6c65 223a 207b 0a20 2020 2020 2020  tyle": {.       
-00012910: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
-00012920: 3a20 2253 5452 4f4b 4522 0a20 2020 2020  : "STROKE".     
-00012930: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-00012940: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00012950: 2020 2020 2020 2020 2022 7469 746c 6522           "title"
-00012960: 3a20 2241 6e20 6974 656d 222c 0a20 2020  : "An item",.   
-00012970: 2020 2020 2020 2020 2020 2274 6578 7441            "textA
-00012980: 6c69 676e 6d65 6e74 223a 2022 4345 4e54  lignment": "CENT
-00012990: 4552 220a 2020 2020 2020 2020 2020 207d  ER".           }
-000129a0: 0a20 2020 2020 2020 2020 5d2c 0a20 2020  .         ],.   
-000129b0: 2020 2020 2020 226f 6e43 6c69 636b 223a        "onClick":
-000129c0: 207b 0a20 2020 2020 2020 2020 2020 226f   {.           "o
-000129d0: 7065 6e4c 696e 6b22 3a20 7b0a 2020 2020  penLink": {.    
-000129e0: 2020 2020 2020 2020 2022 7572 6c22 3a20           "url": 
-000129f0: 2268 7474 7073 3a2f 2f77 7777 2e65 7861  "https://www.exa
-00012a00: 6d70 6c65 2e63 6f6d 220a 2020 2020 2020  mple.com".      
-00012a10: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
-00012a20: 7d0a 2020 2020 2020 207d 0a0a 2020 2020  }.       }..    
-00012a30: 4174 7472 6962 7574 6573 3a0a 2020 2020  Attributes:.    
-00012a40: 2020 2020 7469 746c 6520 2873 7472 293a      title (str):
-00012a50: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
-00012a60: 2074 6578 7420 7468 6174 2064 6973 706c   text that displ
-00012a70: 6179 7320 696e 2074 6865 2067 7269 6420  ays in the grid 
-00012a80: 6865 6164 6572 2e0a 2020 2020 2020 2020  header..        
-00012a90: 6974 656d 7320 284d 7574 6162 6c65 5365  items (MutableSe
-00012aa0: 7175 656e 6365 5b67 6f6f 676c 652e 6170  quence[google.ap
-00012ab0: 7073 2e63 6172 645f 7631 2e74 7970 6573  ps.card_v1.types
-00012ac0: 2e47 7269 642e 4772 6964 4974 656d 5d29  .Grid.GridItem])
-00012ad0: 3a0a 2020 2020 2020 2020 2020 2020 5468  :.            Th
-00012ae0: 6520 6974 656d 7320 746f 2064 6973 706c  e items to displ
-00012af0: 6179 2069 6e20 7468 6520 6772 6964 2e0a  ay in the grid..
-00012b00: 2020 2020 2020 2020 626f 7264 6572 5f73          border_s
-00012b10: 7479 6c65 2028 676f 6f67 6c65 2e61 7070  tyle (google.app
-00012b20: 732e 6361 7264 5f76 312e 7479 7065 732e  s.card_v1.types.
-00012b30: 426f 7264 6572 5374 796c 6529 3a0a 2020  BorderStyle):.  
-00012b40: 2020 2020 2020 2020 2020 5468 6520 626f            The bo
-00012b50: 7264 6572 2073 7479 6c65 2074 6f20 6170  rder style to ap
-00012b60: 706c 7920 746f 2065 6163 6820 6772 6964  ply to each grid
-00012b70: 2069 7465 6d2e 0a20 2020 2020 2020 2063   item..        c
-00012b80: 6f6c 756d 6e5f 636f 756e 7420 2869 6e74  olumn_count (int
-00012b90: 293a 0a20 2020 2020 2020 2020 2020 2054  ):.            T
-00012ba0: 6865 206e 756d 6265 7220 6f66 2063 6f6c  he number of col
-00012bb0: 756d 6e73 2074 6f20 6469 7370 6c61 7920  umns to display 
-00012bc0: 696e 2074 6865 2067 7269 642e 0a20 2020  in the grid..   
-00012bd0: 2020 2020 2020 2020 2041 2064 6566 6175           A defau
-00012be0: 6c74 2076 616c 7565 2069 7320 7573 6564  lt value is used
-00012bf0: 2069 6620 7468 6973 2066 6965 6c64 2069   if this field i
-00012c00: 736e 2774 0a20 2020 2020 2020 2020 2020  sn't.           
-00012c10: 2073 7065 6369 6669 6564 2c20 616e 6420   specified, and 
-00012c20: 7468 6174 2064 6566 6175 6c74 2076 616c  that default val
-00012c30: 7565 2069 7320 6469 6666 6572 656e 740a  ue is different.
-00012c40: 2020 2020 2020 2020 2020 2020 6465 7065              depe
-00012c50: 6e64 696e 6720 6f6e 2077 6865 7265 2074  nding on where t
-00012c60: 6865 2067 7269 6420 6973 2073 686f 776e  he grid is shown
-00012c70: 2028 6469 616c 6f67 0a20 2020 2020 2020   (dialog.       
-00012c80: 2020 2020 2076 6572 7375 7320 636f 6d70       versus comp
-00012c90: 616e 696f 6e29 2e0a 2020 2020 2020 2020  anion)..        
-00012ca0: 6f6e 5f63 6c69 636b 2028 676f 6f67 6c65  on_click (google
-00012cb0: 2e61 7070 732e 6361 7264 5f76 312e 7479  .apps.card_v1.ty
-00012cc0: 7065 732e 4f6e 436c 6963 6b29 3a0a 2020  pes.OnClick):.  
-00012cd0: 2020 2020 2020 2020 2020 5468 6973 2063            This c
-00012ce0: 616c 6c62 6163 6b20 6973 2072 6575 7365  allback is reuse
-00012cf0: 6420 6279 2065 6163 6820 696e 6469 7669  d by each indivi
-00012d00: 6475 616c 0a20 2020 2020 2020 2020 2020  dual.           
-00012d10: 2067 7269 6420 6974 656d 2c20 6275 7420   grid item, but 
-00012d20: 7769 7468 2074 6865 2069 7465 6d27 7320  with the item's 
-00012d30: 6964 656e 7469 6669 6572 2061 6e64 0a20  identifier and. 
-00012d40: 2020 2020 2020 2020 2020 2069 6e64 6578             index
-00012d50: 2069 6e20 7468 6520 6974 656d 7320 6c69   in the items li
-00012d60: 7374 2061 6464 6564 2074 6f20 7468 6520  st added to the 
-00012d70: 6361 6c6c 6261 636b 2773 0a20 2020 2020  callback's.     
-00012d80: 2020 2020 2020 2070 6172 616d 6574 6572         parameter
-00012d90: 732e 0a20 2020 2022 2222 0a0a 2020 2020  s..    """..    
-00012da0: 636c 6173 7320 4772 6964 4974 656d 2870  class GridItem(p
-00012db0: 726f 746f 2e4d 6573 7361 6765 293a 0a20  roto.Message):. 
-00012dc0: 2020 2020 2020 2072 2222 2252 6570 7265         r"""Repre
-00012dd0: 7365 6e74 7320 616e 2069 7465 6d20 696e  sents an item in
-00012de0: 2061 2067 7269 6420 6c61 796f 7574 2e20   a grid layout. 
-00012df0: 4974 656d 7320 6361 6e20 636f 6e74 6169  Items can contai
-00012e00: 6e20 7465 7874 2c20 616e 0a20 2020 2020  n text, an.     
-00012e10: 2020 2069 6d61 6765 2c20 6f72 2062 6f74     image, or bot
-00012e20: 6820 7465 7874 2061 6e64 2061 6e20 696d  h text and an im
-00012e30: 6167 652e 0a0a 2020 2020 2020 2020 6047  age...        `G
-00012e40: 6f6f 676c 6520 576f 726b 7370 6163 6520  oogle Workspace 
-00012e50: 4164 642d 6f6e 7320 616e 6420 4368 6174  Add-ons and Chat
-00012e60: 0a20 2020 2020 2020 2061 7070 7320 3c68  .        apps <h
-00012e70: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
-00012e80: 732e 676f 6f67 6c65 2e63 6f6d 2f77 6f72  s.google.com/wor
-00012e90: 6b73 7061 6365 2f65 7874 656e 643e 605f  kspace/extend>`_
-00012ea0: 5f3a 0a0a 2020 2020 2020 2020 4174 7472  _:..        Attr
-00012eb0: 6962 7574 6573 3a0a 2020 2020 2020 2020  ibutes:.        
-00012ec0: 2020 2020 6964 2028 7374 7229 3a0a 2020      id (str):.  
-00012ed0: 2020 2020 2020 2020 2020 2020 2020 4120                A 
-00012ee0: 7573 6572 2d73 7065 6369 6669 6564 2069  user-specified i
-00012ef0: 6465 6e74 6966 6965 7220 666f 7220 7468  dentifier for th
-00012f00: 6973 2067 7269 6420 6974 656d 2e20 5468  is grid item. Th
-00012f10: 6973 0a20 2020 2020 2020 2020 2020 2020  is.             
-00012f20: 2020 2069 6465 6e74 6966 6965 7220 6973     identifier is
-00012f30: 2072 6574 7572 6e65 6420 696e 2074 6865   returned in the
-00012f40: 2070 6172 656e 7420 6772 6964 2773 2060   parent grid's `
-00012f50: 606f 6e43 6c69 636b 6060 0a20 2020 2020  `onClick``.     
-00012f60: 2020 2020 2020 2020 2020 2063 616c 6c62             callb
-00012f70: 6163 6b20 7061 7261 6d65 7465 7273 2e0a  ack parameters..
-00012f80: 2020 2020 2020 2020 2020 2020 696d 6167              imag
-00012f90: 6520 2867 6f6f 676c 652e 6170 7073 2e63  e (google.apps.c
-00012fa0: 6172 645f 7631 2e74 7970 6573 2e49 6d61  ard_v1.types.Ima
-00012fb0: 6765 436f 6d70 6f6e 656e 7429 3a0a 2020  geComponent):.  
-00012fc0: 2020 2020 2020 2020 2020 2020 2020 5468                Th
-00012fd0: 6520 696d 6167 6520 7468 6174 2064 6973  e image that dis
-00012fe0: 706c 6179 7320 696e 2074 6865 2067 7269  plays in the gri
-00012ff0: 6420 6974 656d 2e0a 2020 2020 2020 2020  d item..        
-00013000: 2020 2020 7469 746c 6520 2873 7472 293a      title (str):
-00013010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013020: 2054 6865 2067 7269 6420 6974 656d 2773   The grid item's
-00013030: 2074 6974 6c65 2e0a 2020 2020 2020 2020   title..        
-00013040: 2020 2020 7375 6274 6974 6c65 2028 7374      subtitle (st
-00013050: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-00013060: 2020 2020 5468 6520 6772 6964 2069 7465      The grid ite
-00013070: 6d27 7320 7375 6274 6974 6c65 2e0a 2020  m's subtitle..  
-00013080: 2020 2020 2020 2020 2020 6c61 796f 7574            layout
-00013090: 2028 676f 6f67 6c65 2e61 7070 732e 6361   (google.apps.ca
-000130a0: 7264 5f76 312e 7479 7065 732e 4772 6964  rd_v1.types.Grid
-000130b0: 2e47 7269 6449 7465 6d2e 4772 6964 4974  .GridItem.GridIt
-000130c0: 656d 4c61 796f 7574 293a 0a20 2020 2020  emLayout):.     
-000130d0: 2020 2020 2020 2020 2020 2054 6865 206c             The l
-000130e0: 6179 6f75 7420 746f 2075 7365 2066 6f72  ayout to use for
-000130f0: 2074 6865 2067 7269 6420 6974 656d 2e0a   the grid item..
-00013100: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
-00013110: 2020 2020 2063 6c61 7373 2047 7269 6449       class GridI
-00013120: 7465 6d4c 6179 6f75 7428 7072 6f74 6f2e  temLayout(proto.
-00013130: 456e 756d 293a 0a20 2020 2020 2020 2020  Enum):.         
-00013140: 2020 2072 2222 2252 6570 7265 7365 6e74     r"""Represent
-00013150: 7320 7468 6520 7661 7269 6f75 7320 6c61  s the various la
-00013160: 796f 7574 206f 7074 696f 6e73 2061 7661  yout options ava
-00013170: 696c 6162 6c65 2066 6f72 2061 2067 7269  ilable for a gri
-00013180: 6420 6974 656d 2e0a 0a20 2020 2020 2020  d item...       
-00013190: 2020 2020 2060 476f 6f67 6c65 2057 6f72       `Google Wor
-000131a0: 6b73 7061 6365 2041 6464 2d6f 6e73 2061  kspace Add-ons a
-000131b0: 6e64 2043 6861 740a 2020 2020 2020 2020  nd Chat.        
-000131c0: 2020 2020 6170 7073 203c 6874 7470 733a      apps <https:
-000131d0: 2f2f 6465 7665 6c6f 7065 7273 2e67 6f6f  //developers.goo
-000131e0: 676c 652e 636f 6d2f 776f 726b 7370 6163  gle.com/workspac
-000131f0: 652f 6578 7465 6e64 3e60 5f5f 3a0a 0a20  e/extend>`__:.. 
-00013200: 2020 2020 2020 2020 2020 2056 616c 7565             Value
-00013210: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-00013220: 2020 2047 5249 445f 4954 454d 5f4c 4159     GRID_ITEM_LAY
-00013230: 4f55 545f 554e 5350 4543 4946 4945 4420  OUT_UNSPECIFIED 
-00013240: 2830 293a 0a20 2020 2020 2020 2020 2020  (0):.           
-00013250: 2020 2020 2020 2020 2044 6f6e 2774 2075           Don't u
-00013260: 7365 2e20 556e 7370 6563 6966 6965 642e  se. Unspecified.
-00013270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013280: 2054 4558 545f 4245 4c4f 5720 2831 293a   TEXT_BELOW (1):
-00013290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000132a0: 2020 2020 2054 6865 2074 6974 6c65 2061       The title a
-000132b0: 6e64 2073 7562 7469 746c 6520 6172 6520  nd subtitle are 
-000132c0: 7368 6f77 6e20 6265 6c6f 7720 7468 650a  shown below the.
-000132d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000132e0: 2020 2020 6772 6964 2069 7465 6d27 7320      grid item's 
-000132f0: 696d 6167 652e 0a20 2020 2020 2020 2020  image..         
-00013300: 2020 2020 2020 2054 4558 545f 4142 4f56         TEXT_ABOV
-00013310: 4520 2832 293a 0a20 2020 2020 2020 2020  E (2):.         
-00013320: 2020 2020 2020 2020 2020 2054 6865 2074             The t
-00013330: 6974 6c65 2061 6e64 2073 7562 7469 746c  itle and subtitl
-00013340: 6520 6172 6520 7368 6f77 6e20 6162 6f76  e are shown abov
-00013350: 6520 7468 650a 2020 2020 2020 2020 2020  e the.          
-00013360: 2020 2020 2020 2020 2020 6772 6964 2069            grid i
-00013370: 7465 6d27 7320 696d 6167 652e 0a20 2020  tem's image..   
-00013380: 2020 2020 2020 2020 2022 2222 0a20 2020           """.   
-00013390: 2020 2020 2020 2020 2047 5249 445f 4954           GRID_IT
-000133a0: 454d 5f4c 4159 4f55 545f 554e 5350 4543  EM_LAYOUT_UNSPEC
-000133b0: 4946 4945 4420 3d20 300a 2020 2020 2020  IFIED = 0.      
-000133c0: 2020 2020 2020 5445 5854 5f42 454c 4f57        TEXT_BELOW
-000133d0: 203d 2031 0a20 2020 2020 2020 2020 2020   = 1.           
-000133e0: 2054 4558 545f 4142 4f56 4520 3d20 320a   TEXT_ABOVE = 2.
-000133f0: 0a20 2020 2020 2020 2069 643a 2073 7472  .        id: str
-00013400: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
-00013410: 2020 2020 2020 2020 2020 2020 7072 6f74              prot
-00013420: 6f2e 5354 5249 4e47 2c0a 2020 2020 2020  o.STRING,.      
-00013430: 2020 2020 2020 6e75 6d62 6572 3d31 2c0a        number=1,.
-00013440: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00013450: 2020 696d 6167 653a 2022 496d 6167 6543    image: "ImageC
-00013460: 6f6d 706f 6e65 6e74 2220 3d20 7072 6f74  omponent" = prot
-00013470: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-00013480: 2020 2020 2070 726f 746f 2e4d 4553 5341       proto.MESSA
-00013490: 4745 2c0a 2020 2020 2020 2020 2020 2020  GE,.            
-000134a0: 6e75 6d62 6572 3d32 2c0a 2020 2020 2020  number=2,.      
-000134b0: 2020 2020 2020 6d65 7373 6167 653d 2249        message="I
-000134c0: 6d61 6765 436f 6d70 6f6e 656e 7422 2c0a  mageComponent",.
-000134d0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000134e0: 2020 7469 746c 653a 2073 7472 203d 2070    title: str = p
-000134f0: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
-00013500: 2020 2020 2020 2020 7072 6f74 6f2e 5354          proto.ST
-00013510: 5249 4e47 2c0a 2020 2020 2020 2020 2020  RING,.          
-00013520: 2020 6e75 6d62 6572 3d33 2c0a 2020 2020    number=3,.    
-00013530: 2020 2020 290a 2020 2020 2020 2020 7375      ).        su
-00013540: 6274 6974 6c65 3a20 7374 7220 3d20 7072  btitle: str = pr
-00013550: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
-00013560: 2020 2020 2020 2070 726f 746f 2e53 5452         proto.STR
-00013570: 494e 472c 0a20 2020 2020 2020 2020 2020  ING,.           
-00013580: 206e 756d 6265 723d 342c 0a20 2020 2020   number=4,.     
-00013590: 2020 2029 0a20 2020 2020 2020 206c 6179     ).        lay
-000135a0: 6f75 743a 2022 4772 6964 2e47 7269 6449  out: "Grid.GridI
-000135b0: 7465 6d2e 4772 6964 4974 656d 4c61 796f  tem.GridItemLayo
-000135c0: 7574 2220 3d20 7072 6f74 6f2e 4669 656c  ut" = proto.Fiel
-000135d0: 6428 0a20 2020 2020 2020 2020 2020 2070  d(.            p
-000135e0: 726f 746f 2e45 4e55 4d2c 0a20 2020 2020  roto.ENUM,.     
-000135f0: 2020 2020 2020 206e 756d 6265 723d 392c         number=9,
-00013600: 0a20 2020 2020 2020 2020 2020 2065 6e75  .            enu
-00013610: 6d3d 2247 7269 642e 4772 6964 4974 656d  m="Grid.GridItem
-00013620: 2e47 7269 6449 7465 6d4c 6179 6f75 7422  .GridItemLayout"
-00013630: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-00013640: 2074 6974 6c65 3a20 7374 7220 3d20 7072   title: str = pr
-00013650: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
-00013660: 2020 2070 726f 746f 2e53 5452 494e 472c     proto.STRING,
-00013670: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
-00013680: 312c 0a20 2020 2029 0a20 2020 2069 7465  1,.    ).    ite
-00013690: 6d73 3a20 4d75 7461 626c 6553 6571 7565  ms: MutableSeque
-000136a0: 6e63 655b 4772 6964 4974 656d 5d20 3d20  nce[GridItem] = 
-000136b0: 7072 6f74 6f2e 5265 7065 6174 6564 4669  proto.RepeatedFi
-000136c0: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
-000136d0: 746f 2e4d 4553 5341 4745 2c0a 2020 2020  to.MESSAGE,.    
-000136e0: 2020 2020 6e75 6d62 6572 3d32 2c0a 2020      number=2,.  
-000136f0: 2020 2020 2020 6d65 7373 6167 653d 4772        message=Gr
-00013700: 6964 4974 656d 2c0a 2020 2020 290a 2020  idItem,.    ).  
-00013710: 2020 626f 7264 6572 5f73 7479 6c65 3a20    border_style: 
-00013720: 2242 6f72 6465 7253 7479 6c65 2220 3d20  "BorderStyle" = 
-00013730: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
-00013740: 2020 2020 2070 726f 746f 2e4d 4553 5341       proto.MESSA
-00013750: 4745 2c0a 2020 2020 2020 2020 6e75 6d62  GE,.        numb
-00013760: 6572 3d33 2c0a 2020 2020 2020 2020 6d65  er=3,.        me
-00013770: 7373 6167 653d 2242 6f72 6465 7253 7479  ssage="BorderSty
-00013780: 6c65 222c 0a20 2020 2029 0a20 2020 2063  le",.    ).    c
-00013790: 6f6c 756d 6e5f 636f 756e 743a 2069 6e74  olumn_count: int
-000137a0: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
-000137b0: 2020 2020 2020 2020 7072 6f74 6f2e 494e          proto.IN
-000137c0: 5433 322c 0a20 2020 2020 2020 206e 756d  T32,.        num
-000137d0: 6265 723d 342c 0a20 2020 2029 0a20 2020  ber=4,.    ).   
-000137e0: 206f 6e5f 636c 6963 6b3a 2022 4f6e 436c   on_click: "OnCl
-000137f0: 6963 6b22 203d 2070 726f 746f 2e46 6965  ick" = proto.Fie
-00013800: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
-00013810: 6f2e 4d45 5353 4147 452c 0a20 2020 2020  o.MESSAGE,.     
-00013820: 2020 206e 756d 6265 723d 352c 0a20 2020     number=5,.   
-00013830: 2020 2020 206d 6573 7361 6765 3d22 4f6e       message="On
-00013840: 436c 6963 6b22 2c0a 2020 2020 290a 0a0a  Click",.    )...
-00013850: 636c 6173 7320 436f 6c75 6d6e 7328 7072  class Columns(pr
-00013860: 6f74 6f2e 4d65 7373 6167 6529 3a0a 2020  oto.Message):.  
-00013870: 2020 7222 2222 5468 6520 6060 436f 6c75    r"""The ``Colu
-00013880: 6d6e 7360 6020 7769 6467 6574 2064 6973  mns`` widget dis
-00013890: 706c 6179 7320 7570 2074 6f20 3220 636f  plays up to 2 co
-000138a0: 6c75 6d6e 7320 696e 2061 2063 6172 6420  lumns in a card 
-000138b0: 6f72 2064 6961 6c6f 672e 0a20 2020 2059  or dialog..    Y
-000138c0: 6f75 2063 616e 2061 6464 2077 6964 6765  ou can add widge
-000138d0: 7473 2074 6f20 6561 6368 2063 6f6c 756d  ts to each colum
-000138e0: 6e3b 2074 6865 2077 6964 6765 7473 2061  n; the widgets a
-000138f0: 7070 6561 7220 696e 2074 6865 206f 7264  ppear in the ord
-00013900: 6572 0a20 2020 2074 6861 7420 7468 6579  er.    that they
-00013910: 2061 7265 2073 7065 6369 6669 6564 2e20   are specified. 
-00013920: 466f 7220 616e 2065 7861 6d70 6c65 2069  For an example i
-00013930: 6e20 476f 6f67 6c65 2043 6861 7420 6170  n Google Chat ap
-00013940: 7073 2c20 7365 650a 2020 2020 6043 6f6c  ps, see.    `Col
-00013950: 756d 6e73 203c 6874 7470 733a 2f2f 6465  umns <https://de
-00013960: 7665 6c6f 7065 7273 2e67 6f6f 676c 652e  velopers.google.
-00013970: 636f 6d2f 6368 6174 2f75 692f 7769 6467  com/chat/ui/widg
-00013980: 6574 732f 636f 6c75 6d6e 733e 605f 5f2e  ets/columns>`__.
-00013990: 0a0a 2020 2020 5468 6520 6865 6967 6874  ..    The height
-000139a0: 206f 6620 6561 6368 2063 6f6c 756d 6e20   of each column 
-000139b0: 6973 2064 6574 6572 6d69 6e65 6420 6279  is determined by
-000139c0: 2074 6865 2074 616c 6c65 7220 636f 6c75   the taller colu
-000139d0: 6d6e 2e20 466f 720a 2020 2020 6578 616d  mn. For.    exam
-000139e0: 706c 652c 2069 6620 7468 6520 6669 7273  ple, if the firs
-000139f0: 7420 636f 6c75 6d6e 2069 7320 7461 6c6c  t column is tall
-00013a00: 6572 2074 6861 6e20 7468 6520 7365 636f  er than the seco
-00013a10: 6e64 2063 6f6c 756d 6e2c 2062 6f74 680a  nd column, both.
-00013a20: 2020 2020 636f 6c75 6d6e 7320 6861 7665      columns have
-00013a30: 2074 6865 2068 6569 6768 7420 6f66 2074   the height of t
-00013a40: 6865 2066 6972 7374 2063 6f6c 756d 6e2e  he first column.
-00013a50: 2042 6563 6175 7365 2065 6163 6820 636f   Because each co
-00013a60: 6c75 6d6e 2063 616e 0a20 2020 2063 6f6e  lumn can.    con
-00013a70: 7461 696e 2061 2064 6966 6665 7265 6e74  tain a different
-00013a80: 206e 756d 6265 7220 6f66 2077 6964 6765   number of widge
-00013a90: 7473 2c20 796f 7520 6361 6e27 7420 6465  ts, you can't de
-00013aa0: 6669 6e65 2072 6f77 7320 6f72 0a20 2020  fine rows or.   
-00013ab0: 2061 6c69 676e 2077 6964 6765 7473 2062   align widgets b
-00013ac0: 6574 7765 656e 2074 6865 2063 6f6c 756d  etween the colum
-00013ad0: 6e73 2e0a 0a20 2020 2043 6f6c 756d 6e73  ns...    Columns
-00013ae0: 2061 7265 2064 6973 706c 6179 6564 2073   are displayed s
-00013af0: 6964 652d 6279 2d73 6964 652e 2059 6f75  ide-by-side. You
-00013b00: 2063 616e 2063 7573 746f 6d69 7a65 2074   can customize t
-00013b10: 6865 2077 6964 7468 206f 660a 2020 2020  he width of.    
-00013b20: 6561 6368 2063 6f6c 756d 6e20 7573 696e  each column usin
-00013b30: 6720 7468 6520 6060 486f 7269 7a6f 6e74  g the ``Horizont
-00013b40: 616c 5369 7a65 5374 796c 6560 6020 6669  alSizeStyle`` fi
-00013b50: 656c 642e 2049 6620 7468 6520 7573 6572  eld. If the user
-00013b60: 2773 0a20 2020 2073 6372 6565 6e20 7769  's.    screen wi
-00013b70: 6474 6820 6973 2074 6f6f 206e 6172 726f  dth is too narro
-00013b80: 772c 2074 6865 2073 6563 6f6e 6420 636f  w, the second co
-00013b90: 6c75 6d6e 2077 7261 7073 2062 656c 6f77  lumn wraps below
-00013ba0: 2074 6865 2066 6972 7374 3a0a 0a20 2020   the first:..   
-00013bb0: 202d 2020 4f6e 2077 6562 2c20 7468 6520   -  On web, the 
-00013bc0: 7365 636f 6e64 2063 6f6c 756d 6e20 7772  second column wr
-00013bd0: 6170 7320 6966 2074 6865 2073 6372 6565  aps if the scree
-00013be0: 6e20 7769 6474 6820 6973 206c 6573 7320  n width is less 
-00013bf0: 7468 616e 0a20 2020 2020 2020 6f72 2065  than.       or e
-00013c00: 7175 616c 2074 6f20 3438 3020 7069 7865  qual to 480 pixe
-00013c10: 6c73 2e0a 2020 2020 2d20 204f 6e20 694f  ls..    -  On iO
-00013c20: 5320 6465 7669 6365 732c 2074 6865 2073  S devices, the s
-00013c30: 6563 6f6e 6420 636f 6c75 6d6e 2077 7261  econd column wra
-00013c40: 7073 2069 6620 7468 6520 7363 7265 656e  ps if the screen
-00013c50: 2077 6964 7468 2069 730a 2020 2020 2020   width is.      
-00013c60: 206c 6573 7320 7468 616e 206f 7220 6571   less than or eq
-00013c70: 7561 6c20 746f 2033 3030 2070 742e 0a20  ual to 300 pt.. 
-00013c80: 2020 202d 2020 4f6e 2041 6e64 726f 6964     -  On Android
-00013c90: 2064 6576 6963 6573 2c20 7468 6520 7365   devices, the se
-00013ca0: 636f 6e64 2063 6f6c 756d 6e20 7772 6170  cond column wrap
-00013cb0: 7320 6966 2074 6865 2073 6372 6565 6e20  s if the screen 
-00013cc0: 7769 6474 680a 2020 2020 2020 2069 7320  width.       is 
-00013cd0: 6c65 7373 2074 6861 6e20 6f72 2065 7175  less than or equ
-00013ce0: 616c 2074 6f20 3332 3020 6470 2e0a 0a20  al to 320 dp... 
-00013cf0: 2020 2054 6f20 696e 636c 7564 6520 6d6f     To include mo
-00013d00: 7265 2074 6861 6e20 3220 636f 6c75 6d6e  re than 2 column
-00013d10: 732c 206f 7220 746f 2075 7365 2072 6f77  s, or to use row
-00013d20: 732c 2075 7365 2074 6865 0a20 2020 205b  s, use the.    [
-00013d30: 6060 4772 6964 6060 5d5b 676f 6f67 6c65  ``Grid``][google
-00013d40: 2e61 7070 732e 6361 7264 2e76 312e 4772  .apps.card.v1.Gr
-00013d50: 6964 5d20 7769 6467 6574 2e0a 0a20 2020  id] widget...   
-00013d60: 2060 476f 6f67 6c65 2057 6f72 6b73 7061   `Google Workspa
-00013d70: 6365 2041 6464 2d6f 6e73 2061 6e64 2043  ce Add-ons and C
-00013d80: 6861 740a 2020 2020 6170 7073 203c 6874  hat.    apps <ht
-00013d90: 7470 733a 2f2f 6465 7665 6c6f 7065 7273  tps://developers
-00013da0: 2e67 6f6f 676c 652e 636f 6d2f 776f 726b  .google.com/work
-00013db0: 7370 6163 652f 6578 7465 6e64 3e60 5f5f  space/extend>`__
-00013dc0: 3a20 436f 6c75 6d6e 730a 2020 2020 666f  : Columns.    fo
-00013dd0: 7220 476f 6f67 6c65 2057 6f72 6b73 7061  r Google Workspa
-00013de0: 6365 2041 6464 2d6f 6e73 2061 7265 2069  ce Add-ons are i
-00013df0: 6e20 6044 6576 656c 6f70 6572 0a20 2020  n `Developer.   
-00013e00: 2050 7265 7669 6577 203c 6874 7470 733a   Preview <https:
-00013e10: 2f2f 6465 7665 6c6f 7065 7273 2e67 6f6f  //developers.goo
-00013e20: 676c 652e 636f 6d2f 776f 726b 7370 6163  gle.com/workspac
-00013e30: 652f 7072 6576 6965 773e 605f 5f2e 0a0a  e/preview>`__...
-00013e40: 2020 2020 4174 7472 6962 7574 6573 3a0a      Attributes:.
-00013e50: 2020 2020 2020 2020 636f 6c75 6d6e 5f69          column_i
-00013e60: 7465 6d73 2028 4d75 7461 626c 6553 6571  tems (MutableSeq
-00013e70: 7565 6e63 655b 676f 6f67 6c65 2e61 7070  uence[google.app
-00013e80: 732e 6361 7264 5f76 312e 7479 7065 732e  s.card_v1.types.
-00013e90: 436f 6c75 6d6e 732e 436f 6c75 6d6e 5d29  Columns.Column])
-00013ea0: 3a0a 2020 2020 2020 2020 2020 2020 416e  :.            An
-00013eb0: 2061 7272 6179 206f 6620 636f 6c75 6d6e   array of column
-00013ec0: 732e 2059 6f75 2063 616e 2069 6e63 6c75  s. You can inclu
-00013ed0: 6465 2075 7020 746f 2032 0a20 2020 2020  de up to 2.     
-00013ee0: 2020 2020 2020 2063 6f6c 756d 6e73 2069         columns i
-00013ef0: 6e20 6120 6361 7264 206f 7220 6469 616c  n a card or dial
-00013f00: 6f67 2e0a 2020 2020 2222 220a 0a20 2020  og..    """..   
-00013f10: 2063 6c61 7373 2043 6f6c 756d 6e28 7072   class Column(pr
-00013f20: 6f74 6f2e 4d65 7373 6167 6529 3a0a 2020  oto.Message):.  
-00013f30: 2020 2020 2020 7222 2222 4120 636f 6c75        r"""A colu
-00013f40: 6d6e 2e0a 0a20 2020 2020 2020 2060 476f  mn...        `Go
-00013f50: 6f67 6c65 2043 6861 7420 6170 7073 203c  ogle Chat apps <
-00013f60: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
-00013f70: 7273 2e67 6f6f 676c 652e 636f 6d2f 6368  rs.google.com/ch
-00013f80: 6174 3e60 5f5f 3a0a 0a20 2020 2020 2020  at>`__:..       
-00013f90: 2041 7474 7269 6275 7465 733a 0a20 2020   Attributes:.   
-00013fa0: 2020 2020 2020 2020 2068 6f72 697a 6f6e           horizon
-00013fb0: 7461 6c5f 7369 7a65 5f73 7479 6c65 2028  tal_size_style (
-00013fc0: 676f 6f67 6c65 2e61 7070 732e 6361 7264  google.apps.card
-00013fd0: 5f76 312e 7479 7065 732e 436f 6c75 6d6e  _v1.types.Column
-00013fe0: 732e 436f 6c75 6d6e 2e48 6f72 697a 6f6e  s.Column.Horizon
-00013ff0: 7461 6c53 697a 6553 7479 6c65 293a 0a20  talSizeStyle):. 
-00014000: 2020 2020 2020 2020 2020 2020 2020 2053                 S
-00014010: 7065 6369 6669 6573 2068 6f77 2061 2063  pecifies how a c
-00014020: 6f6c 756d 6e20 6669 6c6c 7320 7468 6520  olumn fills the 
-00014030: 7769 6474 6820 6f66 2074 6865 2063 6172  width of the car
-00014040: 642e 0a0a 2020 2020 2020 2020 2020 2020  d...            
-00014050: 2020 2020 6047 6f6f 676c 6520 4368 6174      `Google Chat
-00014060: 2061 7070 7320 3c68 7474 7073 3a2f 2f64   apps <https://d
-00014070: 6576 656c 6f70 6572 732e 676f 6f67 6c65  evelopers.google
-00014080: 2e63 6f6d 2f63 6861 743e 605f 5f3a 0a20  .com/chat>`__:. 
-00014090: 2020 2020 2020 2020 2020 2068 6f72 697a             horiz
-000140a0: 6f6e 7461 6c5f 616c 6967 6e6d 656e 7420  ontal_alignment 
-000140b0: 2867 6f6f 676c 652e 6170 7073 2e63 6172  (google.apps.car
-000140c0: 645f 7631 2e74 7970 6573 2e57 6964 6765  d_v1.types.Widge
-000140d0: 742e 486f 7269 7a6f 6e74 616c 416c 6967  t.HorizontalAlig
-000140e0: 6e6d 656e 7429 3a0a 2020 2020 2020 2020  nment):.        
-000140f0: 2020 2020 2020 2020 5370 6563 6966 6965          Specifie
-00014100: 7320 7768 6574 6865 7220 7769 6467 6574  s whether widget
-00014110: 7320 616c 6967 6e20 746f 2074 6865 206c  s align to the l
-00014120: 6566 742c 0a20 2020 2020 2020 2020 2020  eft,.           
-00014130: 2020 2020 2072 6967 6874 2c20 6f72 2063       right, or c
-00014140: 656e 7465 7220 6f66 2061 2063 6f6c 756d  enter of a colum
-00014150: 6e2e 0a20 2020 2020 2020 2020 2020 2076  n..            v
-00014160: 6572 7469 6361 6c5f 616c 6967 6e6d 656e  ertical_alignmen
-00014170: 7420 2867 6f6f 676c 652e 6170 7073 2e63  t (google.apps.c
-00014180: 6172 645f 7631 2e74 7970 6573 2e43 6f6c  ard_v1.types.Col
-00014190: 756d 6e73 2e43 6f6c 756d 6e2e 5665 7274  umns.Column.Vert
-000141a0: 6963 616c 416c 6967 6e6d 656e 7429 3a0a  icalAlignment):.
-000141b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000141c0: 5370 6563 6966 6965 7320 7768 6574 6865  Specifies whethe
-000141d0: 7220 7769 6467 6574 7320 616c 6967 6e20  r widgets align 
-000141e0: 746f 2074 6865 2074 6f70 2c20 626f 7474  to the top, bott
-000141f0: 6f6d 2c20 6f72 0a20 2020 2020 2020 2020  om, or.         
-00014200: 2020 2020 2020 2063 656e 7465 7220 6f66         center of
-00014210: 2061 2063 6f6c 756d 6e2e 0a0a 2020 2020   a column...    
-00014220: 2020 2020 2020 2020 2020 2020 6047 6f6f              `Goo
-00014230: 676c 6520 4368 6174 2061 7070 7320 3c68  gle Chat apps <h
-00014240: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
-00014250: 732e 676f 6f67 6c65 2e63 6f6d 2f63 6861  s.google.com/cha
-00014260: 743e 605f 5f3a 0a20 2020 2020 2020 2020  t>`__:.         
-00014270: 2020 2077 6964 6765 7473 2028 4d75 7461     widgets (Muta
-00014280: 626c 6553 6571 7565 6e63 655b 676f 6f67  bleSequence[goog
-00014290: 6c65 2e61 7070 732e 6361 7264 5f76 312e  le.apps.card_v1.
-000142a0: 7479 7065 732e 436f 6c75 6d6e 732e 436f  types.Columns.Co
-000142b0: 6c75 6d6e 2e57 6964 6765 7473 5d29 3a0a  lumn.Widgets]):.
-000142c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000142d0: 416e 2061 7272 6179 206f 6620 7769 6467  An array of widg
-000142e0: 6574 7320 696e 636c 7564 6564 2069 6e20  ets included in 
-000142f0: 6120 636f 6c75 6d6e 2e0a 2020 2020 2020  a column..      
-00014300: 2020 2020 2020 2020 2020 5769 6467 6574            Widget
-00014310: 7320 6170 7065 6172 2069 6e20 7468 6520  s appear in the 
-00014320: 6f72 6465 7220 7468 6174 2074 6865 7920  order that they 
-00014330: 6172 650a 2020 2020 2020 2020 2020 2020  are.            
-00014340: 2020 2020 7370 6563 6966 6965 642e 0a20      specified.. 
-00014350: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
-00014360: 2020 2020 636c 6173 7320 486f 7269 7a6f      class Horizo
-00014370: 6e74 616c 5369 7a65 5374 796c 6528 7072  ntalSizeStyle(pr
-00014380: 6f74 6f2e 456e 756d 293a 0a20 2020 2020  oto.Enum):.     
-00014390: 2020 2020 2020 2072 2222 2253 7065 6369         r"""Speci
-000143a0: 6669 6573 2068 6f77 2061 2063 6f6c 756d  fies how a colum
-000143b0: 6e20 6669 6c6c 7320 7468 6520 7769 6474  n fills the widt
-000143c0: 6820 6f66 2074 6865 2063 6172 642e 2054  h of the card. T
-000143d0: 6865 2077 6964 7468 206f 660a 2020 2020  he width of.    
-000143e0: 2020 2020 2020 2020 6561 6368 2063 6f6c          each col
-000143f0: 756d 6e20 6465 7065 6e64 7320 6f6e 2062  umn depends on b
-00014400: 6f74 6820 7468 6520 6060 486f 7269 7a6f  oth the ``Horizo
-00014410: 6e74 616c 5369 7a65 5374 796c 6560 6020  ntalSizeStyle`` 
-00014420: 616e 6420 7468 650a 2020 2020 2020 2020  and the.        
-00014430: 2020 2020 7769 6474 6820 6f66 2074 6865      width of the
-00014440: 2077 6964 6765 7473 2077 6974 6869 6e20   widgets within 
-00014450: 7468 6520 636f 6c75 6d6e 2e0a 0a20 2020  the column...   
-00014460: 2020 2020 2020 2020 2060 476f 6f67 6c65           `Google
-00014470: 2043 6861 7420 6170 7073 203c 6874 7470   Chat apps <http
-00014480: 733a 2f2f 6465 7665 6c6f 7065 7273 2e67  s://developers.g
-00014490: 6f6f 676c 652e 636f 6d2f 6368 6174 3e60  oogle.com/chat>`
-000144a0: 5f5f 3a0a 0a20 2020 2020 2020 2020 2020  __:..           
-000144b0: 2056 616c 7565 733a 0a20 2020 2020 2020   Values:.       
-000144c0: 2020 2020 2020 2020 2048 4f52 495a 4f4e           HORIZON
-000144d0: 5441 4c5f 5349 5a45 5f53 5459 4c45 5f55  TAL_SIZE_STYLE_U
-000144e0: 4e53 5045 4349 4649 4544 2028 3029 3a0a  NSPECIFIED (0):.
-000144f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014500: 2020 2020 446f 6e27 7420 7573 652e 2055      Don't use. U
-00014510: 6e73 7065 6369 6669 6564 2e0a 2020 2020  nspecified..    
-00014520: 2020 2020 2020 2020 2020 2020 4649 4c4c              FILL
-00014530: 5f41 5641 494c 4142 4c45 5f53 5041 4345  _AVAILABLE_SPACE
-00014540: 2028 3129 3a0a 2020 2020 2020 2020 2020   (1):.          
-00014550: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
-00014560: 7420 7661 6c75 652e 2043 6f6c 756d 6e20  t value. Column 
-00014570: 6669 6c6c 7320 7468 6520 6176 6169 6c61  fills the availa
-00014580: 626c 6520 7370 6163 652c 2075 7020 746f  ble space, up to
-00014590: 2037 3025 0a20 2020 2020 2020 2020 2020   70%.           
-000145a0: 2020 2020 2020 2020 206f 6620 7468 6520           of the 
-000145b0: 6361 7264 2773 2077 6964 7468 2e20 4966  card's width. If
-000145c0: 2062 6f74 6820 636f 6c75 6d6e 7320 6172   both columns ar
-000145d0: 6520 7365 7420 746f 0a20 2020 2020 2020  e set to.       
-000145e0: 2020 2020 2020 2020 2020 2020 2060 6046               ``F
-000145f0: 494c 4c5f 4156 4149 4c41 424c 455f 5350  ILL_AVAILABLE_SP
-00014600: 4143 4560 602c 2065 6163 6820 636f 6c75  ACE``, each colu
-00014610: 6d6e 2066 696c 6c73 2035 3025 206f 6620  mn fills 50% of 
-00014620: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
-00014630: 2020 2020 2020 2020 7370 6163 652e 0a20          space.. 
-00014640: 2020 2020 2020 2020 2020 2020 2020 2046                 F
-00014650: 494c 4c5f 4d49 4e49 4d55 4d5f 5350 4143  ILL_MINIMUM_SPAC
-00014660: 4520 2832 293a 0a20 2020 2020 2020 2020  E (2):.         
-00014670: 2020 2020 2020 2020 2020 2043 6f6c 756d             Colum
-00014680: 6e20 6669 6c6c 7320 7468 6520 6c65 6173  n fills the leas
-00014690: 7420 616d 6f75 6e74 206f 6620 7370 6163  t amount of spac
-000146a0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-000146b0: 2020 2020 2020 706f 7373 6962 6c65 2061        possible a
-000146c0: 6e64 206e 6f20 6d6f 7265 2074 6861 6e20  nd no more than 
-000146d0: 3330 2520 6f66 2074 6865 2063 6172 6427  30% of the card'
-000146e0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-000146f0: 2020 2020 2020 7769 6474 682e 0a20 2020        width..   
-00014700: 2020 2020 2020 2020 2022 2222 0a20 2020           """.   
-00014710: 2020 2020 2020 2020 2048 4f52 495a 4f4e           HORIZON
-00014720: 5441 4c5f 5349 5a45 5f53 5459 4c45 5f55  TAL_SIZE_STYLE_U
-00014730: 4e53 5045 4349 4649 4544 203d 2030 0a20  NSPECIFIED = 0. 
-00014740: 2020 2020 2020 2020 2020 2046 494c 4c5f             FILL_
-00014750: 4156 4149 4c41 424c 455f 5350 4143 4520  AVAILABLE_SPACE 
-00014760: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
-00014770: 4649 4c4c 5f4d 494e 494d 554d 5f53 5041  FILL_MINIMUM_SPA
-00014780: 4345 203d 2032 0a0a 2020 2020 2020 2020  CE = 2..        
-00014790: 636c 6173 7320 5665 7274 6963 616c 416c  class VerticalAl
-000147a0: 6967 6e6d 656e 7428 7072 6f74 6f2e 456e  ignment(proto.En
-000147b0: 756d 293a 0a20 2020 2020 2020 2020 2020  um):.           
-000147c0: 2072 2222 2253 7065 6369 6669 6573 2077   r"""Specifies w
-000147d0: 6865 7468 6572 2077 6964 6765 7473 2061  hether widgets a
-000147e0: 6c69 676e 2074 6f20 7468 6520 746f 702c  lign to the top,
-000147f0: 2062 6f74 746f 6d2c 206f 7220 6365 6e74   bottom, or cent
-00014800: 6572 206f 6620 610a 2020 2020 2020 2020  er of a.        
-00014810: 2020 2020 636f 6c75 6d6e 2e0a 0a20 2020      column...   
-00014820: 2020 2020 2020 2020 2060 476f 6f67 6c65           `Google
-00014830: 2043 6861 7420 6170 7073 203c 6874 7470   Chat apps <http
-00014840: 733a 2f2f 6465 7665 6c6f 7065 7273 2e67  s://developers.g
-00014850: 6f6f 676c 652e 636f 6d2f 6368 6174 3e60  oogle.com/chat>`
-00014860: 5f5f 3a0a 0a20 2020 2020 2020 2020 2020  __:..           
-00014870: 2056 616c 7565 733a 0a20 2020 2020 2020   Values:.       
-00014880: 2020 2020 2020 2020 2056 4552 5449 4341           VERTICA
-00014890: 4c5f 414c 4947 4e4d 454e 545f 554e 5350  L_ALIGNMENT_UNSP
-000148a0: 4543 4946 4945 4420 2830 293a 0a20 2020  ECIFIED (0):.   
-000148b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000148c0: 2044 6f6e 2774 2075 7365 2e20 556e 7370   Don't use. Unsp
-000148d0: 6563 6966 6965 642e 0a20 2020 2020 2020  ecified..       
-000148e0: 2020 2020 2020 2020 2043 454e 5445 5220           CENTER 
-000148f0: 2831 293a 0a20 2020 2020 2020 2020 2020  (1):.           
-00014900: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
-00014910: 2076 616c 7565 2e20 416c 6967 6e73 2077   value. Aligns w
-00014920: 6964 6765 7473 2074 6f20 7468 6520 6365  idgets to the ce
-00014930: 6e74 6572 0a20 2020 2020 2020 2020 2020  nter.           
-00014940: 2020 2020 2020 2020 206f 6620 6120 636f           of a co
-00014950: 6c75 6d6e 2e0a 2020 2020 2020 2020 2020  lumn..          
-00014960: 2020 2020 2020 544f 5020 2832 293a 0a20        TOP (2):. 
-00014970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014980: 2020 2041 6c69 676e 7320 7769 6467 6574     Aligns widget
-00014990: 7320 746f 2074 6865 2074 6f70 206f 6620  s to the top of 
-000149a0: 6120 636f 6c75 6d6e 2e0a 2020 2020 2020  a column..      
-000149b0: 2020 2020 2020 2020 2020 424f 5454 4f4d            BOTTOM
-000149c0: 2028 3329 3a0a 2020 2020 2020 2020 2020   (3):.          
-000149d0: 2020 2020 2020 2020 2020 416c 6967 6e73            Aligns
-000149e0: 2077 6964 6765 7473 2074 6f20 7468 6520   widgets to the 
-000149f0: 626f 7474 6f6d 206f 6620 6120 636f 6c75  bottom of a colu
-00014a00: 6d6e 2e0a 2020 2020 2020 2020 2020 2020  mn..            
-00014a10: 2222 220a 2020 2020 2020 2020 2020 2020  """.            
-00014a20: 5645 5254 4943 414c 5f41 4c49 474e 4d45  VERTICAL_ALIGNME
-00014a30: 4e54 5f55 4e53 5045 4349 4649 4544 203d  NT_UNSPECIFIED =
-00014a40: 2030 0a20 2020 2020 2020 2020 2020 2043   0.            C
-00014a50: 454e 5445 5220 3d20 310a 2020 2020 2020  ENTER = 1.      
-00014a60: 2020 2020 2020 544f 5020 3d20 320a 2020        TOP = 2.  
-00014a70: 2020 2020 2020 2020 2020 424f 5454 4f4d            BOTTOM
-00014a80: 203d 2033 0a0a 2020 2020 2020 2020 636c   = 3..        cl
-00014a90: 6173 7320 5769 6467 6574 7328 7072 6f74  ass Widgets(prot
-00014aa0: 6f2e 4d65 7373 6167 6529 3a0a 2020 2020  o.Message):.    
-00014ab0: 2020 2020 2020 2020 7222 2222 5468 6520          r"""The 
-00014ac0: 7375 7070 6f72 7465 6420 7769 6467 6574  supported widget
-00014ad0: 7320 7468 6174 2079 6f75 2063 616e 2069  s that you can i
-00014ae0: 6e63 6c75 6465 2069 6e20 6120 636f 6c75  nclude in a colu
-00014af0: 6d6e 2e0a 0a20 2020 2020 2020 2020 2020  mn...           
-00014b00: 2060 476f 6f67 6c65 2043 6861 7420 6170   `Google Chat ap
-00014b10: 7073 203c 6874 7470 733a 2f2f 6465 7665  ps <https://deve
-00014b20: 6c6f 7065 7273 2e67 6f6f 676c 652e 636f  lopers.google.co
-00014b30: 6d2f 6368 6174 3e60 5f5f 3a0a 0a20 2020  m/chat>`__:..   
-00014b40: 2020 2020 2020 2020 2054 6869 7320 6d65           This me
-00014b50: 7373 6167 6520 6861 7320 606f 6e65 6f66  ssage has `oneof
-00014b60: 605f 2066 6965 6c64 7320 286d 7574 7561  `_ fields (mutua
-00014b70: 6c6c 7920 6578 636c 7573 6976 6520 6669  lly exclusive fi
-00014b80: 656c 6473 292e 0a20 2020 2020 2020 2020  elds)..         
-00014b90: 2020 2046 6f72 2065 6163 6820 6f6e 656f     For each oneo
-00014ba0: 662c 2061 7420 6d6f 7374 206f 6e65 206d  f, at most one m
-00014bb0: 656d 6265 7220 6669 656c 6420 6361 6e20  ember field can 
-00014bc0: 6265 2073 6574 2061 7420 7468 6520 7361  be set at the sa
-00014bd0: 6d65 2074 696d 652e 0a20 2020 2020 2020  me time..       
-00014be0: 2020 2020 2053 6574 7469 6e67 2061 6e79       Setting any
-00014bf0: 206d 656d 6265 7220 6f66 2074 6865 206f   member of the o
-00014c00: 6e65 6f66 2061 7574 6f6d 6174 6963 616c  neof automatical
-00014c10: 6c79 2063 6c65 6172 7320 616c 6c20 6f74  ly clears all ot
-00014c20: 6865 720a 2020 2020 2020 2020 2020 2020  her.            
-00014c30: 6d65 6d62 6572 732e 0a0a 2020 2020 2020  members...      
-00014c40: 2020 2020 2020 2e2e 205f 6f6e 656f 663a        .. _oneof:
-00014c50: 2068 7474 7073 3a2f 2f70 726f 746f 2d70   https://proto-p
-00014c60: 6c75 732d 7079 7468 6f6e 2e72 6561 6474  lus-python.readt
-00014c70: 6865 646f 6373 2e69 6f2f 656e 2f73 7461  hedocs.io/en/sta
-00014c80: 626c 652f 6669 656c 6473 2e68 746d 6c23  ble/fields.html#
-00014c90: 6f6e 656f 6673 2d6d 7574 7561 6c6c 792d  oneofs-mutually-
-00014ca0: 6578 636c 7573 6976 652d 6669 656c 6473  exclusive-fields
-00014cb0: 0a0a 2020 2020 2020 2020 2020 2020 4174  ..            At
-00014cc0: 7472 6962 7574 6573 3a0a 2020 2020 2020  tributes:.      
-00014cd0: 2020 2020 2020 2020 2020 7465 7874 5f70            text_p
-00014ce0: 6172 6167 7261 7068 2028 676f 6f67 6c65  aragraph (google
-00014cf0: 2e61 7070 732e 6361 7264 5f76 312e 7479  .apps.card_v1.ty
-00014d00: 7065 732e 5465 7874 5061 7261 6772 6170  pes.TextParagrap
-00014d10: 6829 3a0a 2020 2020 2020 2020 2020 2020  h):.            
-00014d20: 2020 2020 2020 2020 5b54 6578 7450 6172          [TextPar
-00014d30: 6167 7261 7068 5d5b 676f 6f67 6c65 2e61  agraph][google.a
-00014d40: 7070 732e 6361 7264 2e76 312e 5465 7874  pps.card.v1.Text
-00014d50: 5061 7261 6772 6170 685d 2077 6964 6765  Paragraph] widge
-00014d60: 742e 0a0a 2020 2020 2020 2020 2020 2020  t...            
-00014d70: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
-00014d80: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
-00014d90: 6620 606f 6e65 6f66 605f 2060 6064 6174  f `oneof`_ ``dat
-00014da0: 6160 602e 0a20 2020 2020 2020 2020 2020  a``..           
-00014db0: 2020 2020 2069 6d61 6765 2028 676f 6f67       image (goog
-00014dc0: 6c65 2e61 7070 732e 6361 7264 5f76 312e  le.apps.card_v1.
-00014dd0: 7479 7065 732e 496d 6167 6529 3a0a 2020  types.Image):.  
-00014de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014df0: 2020 5b49 6d61 6765 5d5b 676f 6f67 6c65    [Image][google
-00014e00: 2e61 7070 732e 6361 7264 2e76 312e 496d  .apps.card.v1.Im
-00014e10: 6167 655d 2077 6964 6765 742e 0a0a 2020  age] widget...  
-00014e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014e30: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
-00014e40: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
-00014e50: 6f66 605f 2060 6064 6174 6160 602e 0a20  of`_ ``data``.. 
-00014e60: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00014e70: 6563 6f72 6174 6564 5f74 6578 7420 2867  ecorated_text (g
-00014e80: 6f6f 676c 652e 6170 7073 2e63 6172 645f  oogle.apps.card_
-00014e90: 7631 2e74 7970 6573 2e44 6563 6f72 6174  v1.types.Decorat
-00014ea0: 6564 5465 7874 293a 0a20 2020 2020 2020  edText):.       
-00014eb0: 2020 2020 2020 2020 2020 2020 205b 4465               [De
-00014ec0: 636f 7261 7465 6454 6578 745d 5b67 6f6f  coratedText][goo
-00014ed0: 676c 652e 6170 7073 2e63 6172 642e 7631  gle.apps.card.v1
-00014ee0: 2e44 6563 6f72 6174 6564 5465 7874 5d20  .DecoratedText] 
-00014ef0: 7769 6467 6574 2e0a 0a20 2020 2020 2020  widget...       
-00014f00: 2020 2020 2020 2020 2020 2020 2054 6869               Thi
-00014f10: 7320 6669 656c 6420 6973 2061 206d 656d  s field is a mem
-00014f20: 6265 7220 6f66 2060 6f6e 656f 6660 5f20  ber of `oneof`_ 
-00014f30: 6060 6461 7461 6060 2e0a 2020 2020 2020  ``data``..      
-00014f40: 2020 2020 2020 2020 2020 6275 7474 6f6e            button
-00014f50: 5f6c 6973 7420 2867 6f6f 676c 652e 6170  _list (google.ap
-00014f60: 7073 2e63 6172 645f 7631 2e74 7970 6573  ps.card_v1.types
-00014f70: 2e42 7574 746f 6e4c 6973 7429 3a0a 2020  .ButtonList):.  
-00014f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014f90: 2020 5b42 7574 746f 6e4c 6973 745d 5b67    [ButtonList][g
-00014fa0: 6f6f 676c 652e 6170 7073 2e63 6172 642e  oogle.apps.card.
-00014fb0: 7631 2e42 7574 746f 6e4c 6973 745d 2077  v1.ButtonList] w
-00014fc0: 6964 6765 742e 0a0a 2020 2020 2020 2020  idget...        
-00014fd0: 2020 2020 2020 2020 2020 2020 5468 6973              This
-00014fe0: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
-00014ff0: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
-00015000: 6064 6174 6160 602e 0a20 2020 2020 2020  `data``..       
-00015010: 2020 2020 2020 2020 2074 6578 745f 696e           text_in
-00015020: 7075 7420 2867 6f6f 676c 652e 6170 7073  put (google.apps
-00015030: 2e63 6172 645f 7631 2e74 7970 6573 2e54  .card_v1.types.T
-00015040: 6578 7449 6e70 7574 293a 0a20 2020 2020  extInput):.     
-00015050: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-00015060: 5465 7874 496e 7075 745d 5b67 6f6f 676c  TextInput][googl
-00015070: 652e 6170 7073 2e63 6172 642e 7631 2e54  e.apps.card.v1.T
-00015080: 6578 7449 6e70 7574 5d20 7769 6467 6574  extInput] widget
-00015090: 2e0a 0a20 2020 2020 2020 2020 2020 2020  ...             
-000150a0: 2020 2020 2020 2054 6869 7320 6669 656c         This fiel
-000150b0: 6420 6973 2061 206d 656d 6265 7220 6f66  d is a member of
-000150c0: 2060 6f6e 656f 6660 5f20 6060 6461 7461   `oneof`_ ``data
-000150d0: 6060 2e0a 2020 2020 2020 2020 2020 2020  ``..            
-000150e0: 2020 2020 7365 6c65 6374 696f 6e5f 696e      selection_in
-000150f0: 7075 7420 2867 6f6f 676c 652e 6170 7073  put (google.apps
-00015100: 2e63 6172 645f 7631 2e74 7970 6573 2e53  .card_v1.types.S
-00015110: 656c 6563 7469 6f6e 496e 7075 7429 3a0a  electionInput):.
-00015120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015130: 2020 2020 5b53 656c 6563 7469 6f6e 496e      [SelectionIn
-00015140: 7075 745d 5b67 6f6f 676c 652e 6170 7073  put][google.apps
-00015150: 2e63 6172 642e 7631 2e53 656c 6563 7469  .card.v1.Selecti
-00015160: 6f6e 496e 7075 745d 2077 6964 6765 742e  onInput] widget.
-00015170: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015180: 2020 2020 2020 5468 6973 2066 6965 6c64        This field
-00015190: 2069 7320 6120 6d65 6d62 6572 206f 6620   is a member of 
-000151a0: 606f 6e65 6f66 605f 2060 6064 6174 6160  `oneof`_ ``data`
-000151b0: 602e 0a20 2020 2020 2020 2020 2020 2020  `..             
-000151c0: 2020 2064 6174 655f 7469 6d65 5f70 6963     date_time_pic
-000151d0: 6b65 7220 2867 6f6f 676c 652e 6170 7073  ker (google.apps
-000151e0: 2e63 6172 645f 7631 2e74 7970 6573 2e44  .card_v1.types.D
-000151f0: 6174 6554 696d 6550 6963 6b65 7229 3a0a  ateTimePicker):.
-00015200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015210: 2020 2020 5b44 6174 6554 696d 6550 6963      [DateTimePic
-00015220: 6b65 725d 5b67 6f6f 676c 652e 6170 7073  ker][google.apps
-00015230: 2e63 6172 642e 7631 2e44 6174 6554 696d  .card.v1.DateTim
-00015240: 6550 6963 6b65 725d 2077 6964 6765 742e  ePicker] widget.
-00015250: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015260: 2020 2020 2020 5468 6973 2066 6965 6c64        This field
-00015270: 2069 7320 6120 6d65 6d62 6572 206f 6620   is a member of 
-00015280: 606f 6e65 6f66 605f 2060 6064 6174 6160  `oneof`_ ``data`
-00015290: 602e 0a20 2020 2020 2020 2020 2020 2022  `..            "
-000152a0: 2222 0a0a 2020 2020 2020 2020 2020 2020  ""..            
-000152b0: 7465 7874 5f70 6172 6167 7261 7068 3a20  text_paragraph: 
-000152c0: 2254 6578 7450 6172 6167 7261 7068 2220  "TextParagraph" 
-000152d0: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
-000152e0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000152f0: 726f 746f 2e4d 4553 5341 4745 2c0a 2020  roto.MESSAGE,.  
-00015300: 2020 2020 2020 2020 2020 2020 2020 6e75                nu
-00015310: 6d62 6572 3d31 2c0a 2020 2020 2020 2020  mber=1,.        
-00015320: 2020 2020 2020 2020 6f6e 656f 663d 2264          oneof="d
-00015330: 6174 6122 2c0a 2020 2020 2020 2020 2020  ata",.          
-00015340: 2020 2020 2020 6d65 7373 6167 653d 2254        message="T
-00015350: 6578 7450 6172 6167 7261 7068 222c 0a20  extParagraph",. 
-00015360: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00015370: 2020 2020 2020 2020 2069 6d61 6765 3a20           image: 
-00015380: 2249 6d61 6765 2220 3d20 7072 6f74 6f2e  "Image" = proto.
-00015390: 4669 656c 6428 0a20 2020 2020 2020 2020  Field(.         
-000153a0: 2020 2020 2020 2070 726f 746f 2e4d 4553         proto.MES
-000153b0: 5341 4745 2c0a 2020 2020 2020 2020 2020  SAGE,.          
-000153c0: 2020 2020 2020 6e75 6d62 6572 3d32 2c0a        number=2,.
-000153d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000153e0: 6f6e 656f 663d 2264 6174 6122 2c0a 2020  oneof="data",.  
-000153f0: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-00015400: 7373 6167 653d 2249 6d61 6765 222c 0a20  ssage="Image",. 
-00015410: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00015420: 2020 2020 2020 2020 2064 6563 6f72 6174           decorat
-00015430: 6564 5f74 6578 743a 2022 4465 636f 7261  ed_text: "Decora
-00015440: 7465 6454 6578 7422 203d 2070 726f 746f  tedText" = proto
-00015450: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
-00015460: 2020 2020 2020 2020 7072 6f74 6f2e 4d45          proto.ME
-00015470: 5353 4147 452c 0a20 2020 2020 2020 2020  SSAGE,.         
-00015480: 2020 2020 2020 206e 756d 6265 723d 332c         number=3,
-00015490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000154a0: 206f 6e65 6f66 3d22 6461 7461 222c 0a20   oneof="data",. 
-000154b0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-000154c0: 6573 7361 6765 3d22 4465 636f 7261 7465  essage="Decorate
-000154d0: 6454 6578 7422 2c0a 2020 2020 2020 2020  dText",.        
-000154e0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-000154f0: 2020 6275 7474 6f6e 5f6c 6973 743a 2022    button_list: "
-00015500: 4275 7474 6f6e 4c69 7374 2220 3d20 7072  ButtonList" = pr
-00015510: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
-00015520: 2020 2020 2020 2020 2020 2070 726f 746f             proto
-00015530: 2e4d 4553 5341 4745 2c0a 2020 2020 2020  .MESSAGE,.      
-00015540: 2020 2020 2020 2020 2020 6e75 6d62 6572            number
-00015550: 3d34 2c0a 2020 2020 2020 2020 2020 2020  =4,.            
-00015560: 2020 2020 6f6e 656f 663d 2264 6174 6122      oneof="data"
-00015570: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00015580: 2020 6d65 7373 6167 653d 2242 7574 746f    message="Butto
-00015590: 6e4c 6973 7422 2c0a 2020 2020 2020 2020  nList",.        
-000155a0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-000155b0: 2020 7465 7874 5f69 6e70 7574 3a20 2254    text_input: "T
-000155c0: 6578 7449 6e70 7574 2220 3d20 7072 6f74  extInput" = prot
-000155d0: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-000155e0: 2020 2020 2020 2020 2070 726f 746f 2e4d           proto.M
-000155f0: 4553 5341 4745 2c0a 2020 2020 2020 2020  ESSAGE,.        
-00015600: 2020 2020 2020 2020 6e75 6d62 6572 3d35          number=5
-00015610: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00015620: 2020 6f6e 656f 663d 2264 6174 6122 2c0a    oneof="data",.
-00015630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015640: 6d65 7373 6167 653d 2254 6578 7449 6e70  message="TextInp
-00015650: 7574 222c 0a20 2020 2020 2020 2020 2020  ut",.           
-00015660: 2029 0a20 2020 2020 2020 2020 2020 2073   ).            s
-00015670: 656c 6563 7469 6f6e 5f69 6e70 7574 3a20  election_input: 
-00015680: 2253 656c 6563 7469 6f6e 496e 7075 7422  "SelectionInput"
-00015690: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
-000156a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000156b0: 7072 6f74 6f2e 4d45 5353 4147 452c 0a20  proto.MESSAGE,. 
-000156c0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-000156d0: 756d 6265 723d 362c 0a20 2020 2020 2020  umber=6,.       
-000156e0: 2020 2020 2020 2020 206f 6e65 6f66 3d22           oneof="
-000156f0: 6461 7461 222c 0a20 2020 2020 2020 2020  data",.         
-00015700: 2020 2020 2020 206d 6573 7361 6765 3d22         message="
-00015710: 5365 6c65 6374 696f 6e49 6e70 7574 222c  SelectionInput",
-00015720: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00015730: 2020 2020 2020 2020 2020 2064 6174 655f             date_
-00015740: 7469 6d65 5f70 6963 6b65 723a 2022 4461  time_picker: "Da
-00015750: 7465 5469 6d65 5069 636b 6572 2220 3d20  teTimePicker" = 
-00015760: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
-00015770: 2020 2020 2020 2020 2020 2020 2070 726f               pro
-00015780: 746f 2e4d 4553 5341 4745 2c0a 2020 2020  to.MESSAGE,.    
-00015790: 2020 2020 2020 2020 2020 2020 6e75 6d62              numb
-000157a0: 6572 3d37 2c0a 2020 2020 2020 2020 2020  er=7,.          
-000157b0: 2020 2020 2020 6f6e 656f 663d 2264 6174        oneof="dat
-000157c0: 6122 2c0a 2020 2020 2020 2020 2020 2020  a",.            
-000157d0: 2020 2020 6d65 7373 6167 653d 2244 6174      message="Dat
-000157e0: 6554 696d 6550 6963 6b65 7222 2c0a 2020  eTimePicker",.  
-000157f0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-00015800: 2020 2020 2068 6f72 697a 6f6e 7461 6c5f       horizontal_
-00015810: 7369 7a65 5f73 7479 6c65 3a20 2243 6f6c  size_style: "Col
-00015820: 756d 6e73 2e43 6f6c 756d 6e2e 486f 7269  umns.Column.Hori
-00015830: 7a6f 6e74 616c 5369 7a65 5374 796c 6522  zontalSizeStyle"
-00015840: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
-00015850: 2020 2020 2020 2020 2020 2020 7072 6f74              prot
-00015860: 6f2e 454e 554d 2c0a 2020 2020 2020 2020  o.ENUM,.        
-00015870: 2020 2020 6e75 6d62 6572 3d31 2c0a 2020      number=1,.  
-00015880: 2020 2020 2020 2020 2020 656e 756d 3d22            enum="
-00015890: 436f 6c75 6d6e 732e 436f 6c75 6d6e 2e48  Columns.Column.H
-000158a0: 6f72 697a 6f6e 7461 6c53 697a 6553 7479  orizontalSizeSty
-000158b0: 6c65 222c 0a20 2020 2020 2020 2029 0a20  le",.        ). 
-000158c0: 2020 2020 2020 2068 6f72 697a 6f6e 7461         horizonta
-000158d0: 6c5f 616c 6967 6e6d 656e 743a 2022 5769  l_alignment: "Wi
-000158e0: 6467 6574 2e48 6f72 697a 6f6e 7461 6c41  dget.HorizontalA
-000158f0: 6c69 676e 6d65 6e74 2220 3d20 7072 6f74  lignment" = prot
-00015900: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-00015910: 2020 2020 2070 726f 746f 2e45 4e55 4d2c       proto.ENUM,
-00015920: 0a20 2020 2020 2020 2020 2020 206e 756d  .            num
-00015930: 6265 723d 322c 0a20 2020 2020 2020 2020  ber=2,.         
-00015940: 2020 2065 6e75 6d3d 2257 6964 6765 742e     enum="Widget.
-00015950: 486f 7269 7a6f 6e74 616c 416c 6967 6e6d  HorizontalAlignm
-00015960: 656e 7422 2c0a 2020 2020 2020 2020 290a  ent",.        ).
-00015970: 2020 2020 2020 2020 7665 7274 6963 616c          vertical
-00015980: 5f61 6c69 676e 6d65 6e74 3a20 2243 6f6c  _alignment: "Col
-00015990: 756d 6e73 2e43 6f6c 756d 6e2e 5665 7274  umns.Column.Vert
-000159a0: 6963 616c 416c 6967 6e6d 656e 7422 203d  icalAlignment" =
-000159b0: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
-000159c0: 2020 2020 2020 2020 2020 7072 6f74 6f2e            proto.
-000159d0: 454e 554d 2c0a 2020 2020 2020 2020 2020  ENUM,.          
-000159e0: 2020 6e75 6d62 6572 3d33 2c0a 2020 2020    number=3,.    
-000159f0: 2020 2020 2020 2020 656e 756d 3d22 436f          enum="Co
-00015a00: 6c75 6d6e 732e 436f 6c75 6d6e 2e56 6572  lumns.Column.Ver
-00015a10: 7469 6361 6c41 6c69 676e 6d65 6e74 222c  ticalAlignment",
-00015a20: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00015a30: 2020 2077 6964 6765 7473 3a20 4d75 7461     widgets: Muta
-00015a40: 626c 6553 6571 7565 6e63 655b 2243 6f6c  bleSequence["Col
-00015a50: 756d 6e73 2e43 6f6c 756d 6e2e 5769 6467  umns.Column.Widg
-00015a60: 6574 7322 5d20 3d20 7072 6f74 6f2e 5265  ets"] = proto.Re
-00015a70: 7065 6174 6564 4669 656c 6428 0a20 2020  peatedField(.   
-00015a80: 2020 2020 2020 2020 2070 726f 746f 2e4d           proto.M
-00015a90: 4553 5341 4745 2c0a 2020 2020 2020 2020  ESSAGE,.        
-00015aa0: 2020 2020 6e75 6d62 6572 3d34 2c0a 2020      number=4,.  
-00015ab0: 2020 2020 2020 2020 2020 6d65 7373 6167            messag
-00015ac0: 653d 2243 6f6c 756d 6e73 2e43 6f6c 756d  e="Columns.Colum
-00015ad0: 6e2e 5769 6467 6574 7322 2c0a 2020 2020  n.Widgets",.    
-00015ae0: 2020 2020 290a 0a20 2020 2063 6f6c 756d      )..    colum
-00015af0: 6e5f 6974 656d 733a 204d 7574 6162 6c65  n_items: Mutable
-00015b00: 5365 7175 656e 6365 5b43 6f6c 756d 6e5d  Sequence[Column]
-00015b10: 203d 2070 726f 746f 2e52 6570 6561 7465   = proto.Repeate
-00015b20: 6446 6965 6c64 280a 2020 2020 2020 2020  dField(.        
-00015b30: 7072 6f74 6f2e 4d45 5353 4147 452c 0a20  proto.MESSAGE,. 
-00015b40: 2020 2020 2020 206e 756d 6265 723d 322c         number=2,
-00015b50: 0a20 2020 2020 2020 206d 6573 7361 6765  .        message
-00015b60: 3d43 6f6c 756d 6e2c 0a20 2020 2029 0a0a  =Column,.    )..
-00015b70: 0a63 6c61 7373 204f 6e43 6c69 636b 2870  .class OnClick(p
-00015b80: 726f 746f 2e4d 6573 7361 6765 293a 0a20  roto.Message):. 
-00015b90: 2020 2072 2222 2252 6570 7265 7365 6e74     r"""Represent
-00015ba0: 7320 686f 7720 746f 2072 6573 706f 6e64  s how to respond
-00015bb0: 2077 6865 6e20 7573 6572 7320 636c 6963   when users clic
-00015bc0: 6b20 616e 2069 6e74 6572 6163 7469 7665  k an interactive
-00015bd0: 2065 6c65 6d65 6e74 206f 6e0a 2020 2020   element on.    
-00015be0: 6120 6361 7264 2c20 7375 6368 2061 7320  a card, such as 
-00015bf0: 6120 6275 7474 6f6e 2e0a 0a20 2020 2060  a button...    `
-00015c00: 476f 6f67 6c65 2057 6f72 6b73 7061 6365  Google Workspace
-00015c10: 2041 6464 2d6f 6e73 2061 6e64 2043 6861   Add-ons and Cha
-00015c20: 740a 2020 2020 6170 7073 203c 6874 7470  t.    apps <http
-00015c30: 733a 2f2f 6465 7665 6c6f 7065 7273 2e67  s://developers.g
-00015c40: 6f6f 676c 652e 636f 6d2f 776f 726b 7370  oogle.com/worksp
-00015c50: 6163 652f 6578 7465 6e64 3e60 5f5f 3a0a  ace/extend>`__:.
-00015c60: 0a20 2020 2054 6869 7320 6d65 7373 6167  .    This messag
-00015c70: 6520 6861 7320 606f 6e65 6f66 605f 2066  e has `oneof`_ f
-00015c80: 6965 6c64 7320 286d 7574 7561 6c6c 7920  ields (mutually 
-00015c90: 6578 636c 7573 6976 6520 6669 656c 6473  exclusive fields
-00015ca0: 292e 0a20 2020 2046 6f72 2065 6163 6820  )..    For each 
-00015cb0: 6f6e 656f 662c 2061 7420 6d6f 7374 206f  oneof, at most o
-00015cc0: 6e65 206d 656d 6265 7220 6669 656c 6420  ne member field 
-00015cd0: 6361 6e20 6265 2073 6574 2061 7420 7468  can be set at th
-00015ce0: 6520 7361 6d65 2074 696d 652e 0a20 2020  e same time..   
-00015cf0: 2053 6574 7469 6e67 2061 6e79 206d 656d   Setting any mem
-00015d00: 6265 7220 6f66 2074 6865 206f 6e65 6f66  ber of the oneof
-00015d10: 2061 7574 6f6d 6174 6963 616c 6c79 2063   automatically c
-00015d20: 6c65 6172 7320 616c 6c20 6f74 6865 720a  lears all other.
-00015d30: 2020 2020 6d65 6d62 6572 732e 0a0a 2020      members...  
-00015d40: 2020 2e2e 205f 6f6e 656f 663a 2068 7474    .. _oneof: htt
-00015d50: 7073 3a2f 2f70 726f 746f 2d70 6c75 732d  ps://proto-plus-
-00015d60: 7079 7468 6f6e 2e72 6561 6474 6865 646f  python.readthedo
-00015d70: 6373 2e69 6f2f 656e 2f73 7461 626c 652f  cs.io/en/stable/
-00015d80: 6669 656c 6473 2e68 746d 6c23 6f6e 656f  fields.html#oneo
-00015d90: 6673 2d6d 7574 7561 6c6c 792d 6578 636c  fs-mutually-excl
-00015da0: 7573 6976 652d 6669 656c 6473 0a0a 2020  usive-fields..  
-00015db0: 2020 4174 7472 6962 7574 6573 3a0a 2020    Attributes:.  
-00015dc0: 2020 2020 2020 6163 7469 6f6e 2028 676f        action (go
-00015dd0: 6f67 6c65 2e61 7070 732e 6361 7264 5f76  ogle.apps.card_v
-00015de0: 312e 7479 7065 732e 4163 7469 6f6e 293a  1.types.Action):
-00015df0: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
-00015e00: 7370 6563 6966 6965 642c 2061 6e20 6163  specified, an ac
-00015e10: 7469 6f6e 2069 7320 7472 6967 6765 7265  tion is triggere
-00015e20: 6420 6279 2074 6869 7320 6060 6f6e 436c  d by this ``onCl
-00015e30: 6963 6b60 602e 0a0a 2020 2020 2020 2020  ick``...        
-00015e40: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
-00015e50: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
-00015e60: 6e65 6f66 605f 2060 6064 6174 6160 602e  neof`_ ``data``.
-00015e70: 0a20 2020 2020 2020 206f 7065 6e5f 6c69  .        open_li
-00015e80: 6e6b 2028 676f 6f67 6c65 2e61 7070 732e  nk (google.apps.
-00015e90: 6361 7264 5f76 312e 7479 7065 732e 4f70  card_v1.types.Op
-00015ea0: 656e 4c69 6e6b 293a 0a20 2020 2020 2020  enLink):.       
-00015eb0: 2020 2020 2049 6620 7370 6563 6966 6965       If specifie
-00015ec0: 642c 2074 6869 7320 6060 6f6e 436c 6963  d, this ``onClic
-00015ed0: 6b60 6020 7472 6967 6765 7273 2061 6e20  k`` triggers an 
-00015ee0: 6f70 656e 206c 696e 6b20 6163 7469 6f6e  open link action
-00015ef0: 2e0a 0a20 2020 2020 2020 2020 2020 2054  ...            T
-00015f00: 6869 7320 6669 656c 6420 6973 2061 206d  his field is a m
-00015f10: 656d 6265 7220 6f66 2060 6f6e 656f 6660  ember of `oneof`
-00015f20: 5f20 6060 6461 7461 6060 2e0a 2020 2020  _ ``data``..    
-00015f30: 2020 2020 6f70 656e 5f64 796e 616d 6963      open_dynamic
-00015f40: 5f6c 696e 6b5f 6163 7469 6f6e 2028 676f  _link_action (go
-00015f50: 6f67 6c65 2e61 7070 732e 6361 7264 5f76  ogle.apps.card_v
-00015f60: 312e 7479 7065 732e 4163 7469 6f6e 293a  1.types.Action):
-00015f70: 0a20 2020 2020 2020 2020 2020 2041 6e20  .            An 
-00015f80: 6164 642d 6f6e 2074 7269 6767 6572 7320  add-on triggers 
-00015f90: 7468 6973 2061 6374 696f 6e20 7768 656e  this action when
-00015fa0: 2074 6865 2061 6374 696f 6e20 6e65 6564   the action need
-00015fb0: 7320 746f 206f 7065 6e0a 2020 2020 2020  s to open.      
-00015fc0: 2020 2020 2020 6120 6c69 6e6b 2e20 5468        a link. Th
-00015fd0: 6973 2064 6966 6665 7273 2066 726f 6d20  is differs from 
-00015fe0: 7468 6520 6060 6f70 656e 5f6c 696e 6b60  the ``open_link`
-00015ff0: 6020 6162 6f76 6520 696e 2074 6861 740a  ` above in that.
-00016000: 2020 2020 2020 2020 2020 2020 7468 6973              this
-00016010: 206e 6565 6473 2074 6f20 7461 6c6b 2074   needs to talk t
-00016020: 6f20 7365 7276 6572 2074 6f20 6765 7420  o server to get 
-00016030: 7468 6520 6c69 6e6b 2e20 5468 7573 2073  the link. Thus s
-00016040: 6f6d 650a 2020 2020 2020 2020 2020 2020  ome.            
-00016050: 7072 6570 6172 6174 696f 6e20 776f 726b  preparation work
-00016060: 2069 7320 7265 7175 6972 6564 2066 6f72   is required for
-00016070: 2077 6562 2063 6c69 656e 7420 746f 2064   web client to d
-00016080: 6f20 6265 666f 7265 2074 6865 0a20 2020  o before the.   
-00016090: 2020 2020 2020 2020 206f 7065 6e20 6c69           open li
-000160a0: 6e6b 2061 6374 696f 6e20 7265 7370 6f6e  nk action respon
-000160b0: 7365 2063 6f6d 6573 2062 6163 6b2e 0a0a  se comes back...
-000160c0: 2020 2020 2020 2020 2020 2020 6047 6f6f              `Goo
-000160d0: 676c 6520 576f 726b 7370 6163 650a 2020  gle Workspace.  
-000160e0: 2020 2020 2020 2020 2020 4164 642d 6f6e            Add-on
-000160f0: 7320 3c68 7474 7073 3a2f 2f64 6576 656c  s <https://devel
-00016100: 6f70 6572 732e 676f 6f67 6c65 2e63 6f6d  opers.google.com
-00016110: 2f77 6f72 6b73 7061 6365 2f61 6464 2d6f  /workspace/add-o
-00016120: 6e73 3e60 5f5f 3a0a 0a20 2020 2020 2020  ns>`__:..       
-00016130: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
-00016140: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
-00016150: 6f6e 656f 6660 5f20 6060 6461 7461 6060  oneof`_ ``data``
-00016160: 2e0a 2020 2020 2020 2020 6361 7264 2028  ..        card (
-00016170: 676f 6f67 6c65 2e61 7070 732e 6361 7264  google.apps.card
-00016180: 5f76 312e 7479 7065 732e 4361 7264 293a  _v1.types.Card):
-00016190: 0a20 2020 2020 2020 2020 2020 2041 206e  .            A n
-000161a0: 6577 2063 6172 6420 6973 2070 7573 6865  ew card is pushe
-000161b0: 6420 746f 2074 6865 2063 6172 6420 7374  d to the card st
-000161c0: 6163 6b20 6166 7465 7220 636c 6963 6b69  ack after clicki
-000161d0: 6e67 2069 660a 2020 2020 2020 2020 2020  ng if.          
-000161e0: 2020 7370 6563 6966 6965 642e 0a0a 2020    specified...  
-000161f0: 2020 2020 2020 2020 2020 6047 6f6f 676c            `Googl
-00016200: 6520 576f 726b 7370 6163 650a 2020 2020  e Workspace.    
-00016210: 2020 2020 2020 2020 4164 642d 6f6e 7320          Add-ons 
-00016220: 3c68 7474 7073 3a2f 2f64 6576 656c 6f70  <https://develop
-00016230: 6572 732e 676f 6f67 6c65 2e63 6f6d 2f77  ers.google.com/w
-00016240: 6f72 6b73 7061 6365 2f61 6464 2d6f 6e73  orkspace/add-ons
-00016250: 3e60 5f5f 3a0a 0a20 2020 2020 2020 2020  >`__:..         
-00016260: 2020 2054 6869 7320 6669 656c 6420 6973     This field is
-00016270: 2061 206d 656d 6265 7220 6f66 2060 6f6e   a member of `on
-00016280: 656f 6660 5f20 6060 6461 7461 6060 2e0a  eof`_ ``data``..
-00016290: 2020 2020 2222 220a 0a20 2020 2061 6374      """..    act
-000162a0: 696f 6e3a 2022 4163 7469 6f6e 2220 3d20  ion: "Action" = 
-000162b0: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
-000162c0: 2020 2020 2070 726f 746f 2e4d 4553 5341       proto.MESSA
-000162d0: 4745 2c0a 2020 2020 2020 2020 6e75 6d62  GE,.        numb
-000162e0: 6572 3d31 2c0a 2020 2020 2020 2020 6f6e  er=1,.        on
-000162f0: 656f 663d 2264 6174 6122 2c0a 2020 2020  eof="data",.    
-00016300: 2020 2020 6d65 7373 6167 653d 2241 6374      message="Act
-00016310: 696f 6e22 2c0a 2020 2020 290a 2020 2020  ion",.    ).    
-00016320: 6f70 656e 5f6c 696e 6b3a 2022 4f70 656e  open_link: "Open
-00016330: 4c69 6e6b 2220 3d20 7072 6f74 6f2e 4669  Link" = proto.Fi
-00016340: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
-00016350: 746f 2e4d 4553 5341 4745 2c0a 2020 2020  to.MESSAGE,.    
-00016360: 2020 2020 6e75 6d62 6572 3d32 2c0a 2020      number=2,.  
-00016370: 2020 2020 2020 6f6e 656f 663d 2264 6174        oneof="dat
-00016380: 6122 2c0a 2020 2020 2020 2020 6d65 7373  a",.        mess
-00016390: 6167 653d 224f 7065 6e4c 696e 6b22 2c0a  age="OpenLink",.
-000163a0: 2020 2020 290a 2020 2020 6f70 656e 5f64      ).    open_d
-000163b0: 796e 616d 6963 5f6c 696e 6b5f 6163 7469  ynamic_link_acti
-000163c0: 6f6e 3a20 2241 6374 696f 6e22 203d 2070  on: "Action" = p
-000163d0: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
-000163e0: 2020 2020 7072 6f74 6f2e 4d45 5353 4147      proto.MESSAG
-000163f0: 452c 0a20 2020 2020 2020 206e 756d 6265  E,.        numbe
-00016400: 723d 332c 0a20 2020 2020 2020 206f 6e65  r=3,.        one
-00016410: 6f66 3d22 6461 7461 222c 0a20 2020 2020  of="data",.     
-00016420: 2020 206d 6573 7361 6765 3d22 4163 7469     message="Acti
-00016430: 6f6e 222c 0a20 2020 2029 0a20 2020 2063  on",.    ).    c
-00016440: 6172 643a 2022 4361 7264 2220 3d20 7072  ard: "Card" = pr
-00016450: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
-00016460: 2020 2070 726f 746f 2e4d 4553 5341 4745     proto.MESSAGE
-00016470: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
-00016480: 3d34 2c0a 2020 2020 2020 2020 6f6e 656f  =4,.        oneo
-00016490: 663d 2264 6174 6122 2c0a 2020 2020 2020  f="data",.      
-000164a0: 2020 6d65 7373 6167 653d 2243 6172 6422    message="Card"
-000164b0: 2c0a 2020 2020 290a 0a0a 636c 6173 7320  ,.    )...class 
-000164c0: 4f70 656e 4c69 6e6b 2870 726f 746f 2e4d  OpenLink(proto.M
-000164d0: 6573 7361 6765 293a 0a20 2020 2072 2222  essage):.    r""
-000164e0: 2252 6570 7265 7365 6e74 7320 616e 2060  "Represents an `
-000164f0: 606f 6e43 6c69 636b 6060 2065 7665 6e74  `onClick`` event
-00016500: 2074 6861 7420 6f70 656e 7320 6120 6879   that opens a hy
-00016510: 7065 726c 696e 6b2e 0a0a 2020 2020 6047  perlink...    `G
-00016520: 6f6f 676c 6520 576f 726b 7370 6163 6520  oogle Workspace 
-00016530: 4164 642d 6f6e 7320 616e 6420 4368 6174  Add-ons and Chat
-00016540: 0a20 2020 2061 7070 7320 3c68 7474 7073  .    apps <https
-00016550: 3a2f 2f64 6576 656c 6f70 6572 732e 676f  ://developers.go
-00016560: 6f67 6c65 2e63 6f6d 2f77 6f72 6b73 7061  ogle.com/workspa
-00016570: 6365 2f65 7874 656e 643e 605f 5f3a 0a0a  ce/extend>`__:..
-00016580: 2020 2020 4174 7472 6962 7574 6573 3a0a      Attributes:.
-00016590: 2020 2020 2020 2020 7572 6c20 2873 7472          url (str
-000165a0: 293a 0a20 2020 2020 2020 2020 2020 2054  ):.            T
-000165b0: 6865 2055 524c 2074 6f20 6f70 656e 2e0a  he URL to open..
-000165c0: 2020 2020 2020 2020 6f70 656e 5f61 7320          open_as 
-000165d0: 2867 6f6f 676c 652e 6170 7073 2e63 6172  (google.apps.car
-000165e0: 645f 7631 2e74 7970 6573 2e4f 7065 6e4c  d_v1.types.OpenL
-000165f0: 696e 6b2e 4f70 656e 4173 293a 0a20 2020  ink.OpenAs):.   
-00016600: 2020 2020 2020 2020 2048 6f77 2074 6f20           How to 
-00016610: 6f70 656e 2061 206c 696e 6b2e 0a0a 2020  open a link...  
-00016620: 2020 2020 2020 2020 2020 6047 6f6f 676c            `Googl
-00016630: 6520 576f 726b 7370 6163 650a 2020 2020  e Workspace.    
-00016640: 2020 2020 2020 2020 4164 642d 6f6e 7320          Add-ons 
-00016650: 3c68 7474 7073 3a2f 2f64 6576 656c 6f70  <https://develop
-00016660: 6572 732e 676f 6f67 6c65 2e63 6f6d 2f77  ers.google.com/w
-00016670: 6f72 6b73 7061 6365 2f61 6464 2d6f 6e73  orkspace/add-ons
-00016680: 3e60 5f5f 3a0a 2020 2020 2020 2020 6f6e  >`__:.        on
-00016690: 5f63 6c6f 7365 2028 676f 6f67 6c65 2e61  _close (google.a
-000166a0: 7070 732e 6361 7264 5f76 312e 7479 7065  pps.card_v1.type
-000166b0: 732e 4f70 656e 4c69 6e6b 2e4f 6e43 6c6f  s.OpenLink.OnClo
-000166c0: 7365 293a 0a20 2020 2020 2020 2020 2020  se):.           
-000166d0: 2057 6865 7468 6572 2074 6865 2063 6c69   Whether the cli
-000166e0: 656e 7420 666f 7267 6574 7320 6162 6f75  ent forgets abou
-000166f0: 7420 6120 6c69 6e6b 2061 6674 6572 206f  t a link after o
-00016700: 7065 6e69 6e67 2069 742c 206f 720a 2020  pening it, or.  
-00016710: 2020 2020 2020 2020 2020 6f62 7365 7276            observ
-00016720: 6573 2069 7420 756e 7469 6c20 7468 6520  es it until the 
-00016730: 7769 6e64 6f77 2063 6c6f 7365 732e 0a0a  window closes...
-00016740: 2020 2020 2020 2020 2020 2020 6047 6f6f              `Goo
-00016750: 676c 6520 576f 726b 7370 6163 650a 2020  gle Workspace.  
-00016760: 2020 2020 2020 2020 2020 4164 642d 6f6e            Add-on
-00016770: 7320 3c68 7474 7073 3a2f 2f64 6576 656c  s <https://devel
-00016780: 6f70 6572 732e 676f 6f67 6c65 2e63 6f6d  opers.google.com
-00016790: 2f77 6f72 6b73 7061 6365 2f61 6464 2d6f  /workspace/add-o
-000167a0: 6e73 3e60 5f5f 3a0a 2020 2020 2222 220a  ns>`__:.    """.
-000167b0: 0a20 2020 2063 6c61 7373 204f 7065 6e41  .    class OpenA
-000167c0: 7328 7072 6f74 6f2e 456e 756d 293a 0a20  s(proto.Enum):. 
-000167d0: 2020 2020 2020 2072 2222 2257 6865 6e20         r"""When 
-000167e0: 616e 2060 604f 6e43 6c69 636b 6060 2061  an ``OnClick`` a
-000167f0: 6374 696f 6e20 6f70 656e 7320 6120 6c69  ction opens a li
-00016800: 6e6b 2c20 7468 656e 2074 6865 2063 6c69  nk, then the cli
-00016810: 656e 7420 6361 6e20 6569 7468 6572 0a20  ent can either. 
-00016820: 2020 2020 2020 206f 7065 6e20 6974 2061         open it a
-00016830: 7320 6120 6675 6c6c 2d73 697a 6520 7769  s a full-size wi
-00016840: 6e64 6f77 2028 6966 2074 6861 7427 7320  ndow (if that's 
-00016850: 7468 6520 6672 616d 6520 7573 6564 2062  the frame used b
-00016860: 7920 7468 650a 2020 2020 2020 2020 636c  y the.        cl
-00016870: 6965 6e74 292c 206f 7220 616e 206f 7665  ient), or an ove
-00016880: 726c 6179 2028 7375 6368 2061 7320 6120  rlay (such as a 
-00016890: 706f 702d 7570 292e 2054 6865 2069 6d70  pop-up). The imp
-000168a0: 6c65 6d65 6e74 6174 696f 6e0a 2020 2020  lementation.    
-000168b0: 2020 2020 6465 7065 6e64 7320 6f6e 2074      depends on t
-000168c0: 6865 2063 6c69 656e 7420 706c 6174 666f  he client platfo
-000168d0: 726d 2063 6170 6162 696c 6974 6965 732c  rm capabilities,
-000168e0: 2061 6e64 2074 6865 2076 616c 7565 2073   and the value s
-000168f0: 656c 6563 7465 640a 2020 2020 2020 2020  elected.        
-00016900: 6d69 6768 7420 6265 2069 676e 6f72 6564  might be ignored
-00016910: 2069 6620 7468 6520 636c 6965 6e74 2064   if the client d
-00016920: 6f65 736e 2774 2073 7570 706f 7274 2069  oesn't support i
-00016930: 742e 2060 6046 554c 4c5f 5349 5a45 6060  t. ``FULL_SIZE``
-00016940: 2069 730a 2020 2020 2020 2020 7375 7070   is.        supp
-00016950: 6f72 7465 6420 6279 2061 6c6c 2063 6c69  orted by all cli
-00016960: 656e 7473 2e0a 0a20 2020 2020 2020 2060  ents...        `
-00016970: 476f 6f67 6c65 2057 6f72 6b73 7061 6365  Google Workspace
-00016980: 0a20 2020 2020 2020 2041 6464 2d6f 6e73  .        Add-ons
-00016990: 203c 6874 7470 733a 2f2f 6465 7665 6c6f   <https://develo
-000169a0: 7065 7273 2e67 6f6f 676c 652e 636f 6d2f  pers.google.com/
-000169b0: 776f 726b 7370 6163 652f 6164 642d 6f6e  workspace/add-on
-000169c0: 733e 605f 5f3a 0a0a 2020 2020 2020 2020  s>`__:..        
-000169d0: 5661 6c75 6573 3a0a 2020 2020 2020 2020  Values:.        
-000169e0: 2020 2020 4655 4c4c 5f53 495a 4520 2830      FULL_SIZE (0
-000169f0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00016a00: 2020 2054 6865 206c 696e 6b20 6f70 656e     The link open
-00016a10: 7320 6173 2061 2066 756c 6c2d 7369 7a65  s as a full-size
-00016a20: 2077 696e 646f 7720 2869 660a 2020 2020   window (if.    
-00016a30: 2020 2020 2020 2020 2020 2020 7468 6174              that
-00016a40: 2773 2074 6865 2066 7261 6d65 2075 7365  's the frame use
-00016a50: 6420 6279 2074 6865 2063 6c69 656e 7429  d by the client)
-00016a60: 2e0a 2020 2020 2020 2020 2020 2020 4f56  ..            OV
-00016a70: 4552 4c41 5920 2831 293a 0a20 2020 2020  ERLAY (1):.     
-00016a80: 2020 2020 2020 2020 2020 2054 6865 206c             The l
-00016a90: 696e 6b20 6f70 656e 7320 6173 2061 6e20  ink opens as an 
-00016aa0: 6f76 6572 6c61 792c 2073 7563 6820 6173  overlay, such as
-00016ab0: 2061 0a20 2020 2020 2020 2020 2020 2020   a.             
-00016ac0: 2020 2070 6f70 2d75 702e 0a20 2020 2020     pop-up..     
-00016ad0: 2020 2022 2222 0a20 2020 2020 2020 2046     """.        F
-00016ae0: 554c 4c5f 5349 5a45 203d 2030 0a20 2020  ULL_SIZE = 0.   
-00016af0: 2020 2020 204f 5645 524c 4159 203d 2031       OVERLAY = 1
-00016b00: 0a0a 2020 2020 636c 6173 7320 4f6e 436c  ..    class OnCl
-00016b10: 6f73 6528 7072 6f74 6f2e 456e 756d 293a  ose(proto.Enum):
-00016b20: 0a20 2020 2020 2020 2072 2222 2257 6861  .        r"""Wha
-00016b30: 7420 7468 6520 636c 6965 6e74 2064 6f65  t the client doe
-00016b40: 7320 7768 656e 2061 206c 696e 6b20 6f70  s when a link op
-00016b50: 656e 6564 2062 7920 616e 2060 604f 6e43  ened by an ``OnC
-00016b60: 6c69 636b 6060 2061 6374 696f 6e20 6973  lick`` action is
-00016b70: 0a20 2020 2020 2020 2063 6c6f 7365 642e  .        closed.
-00016b80: 0a0a 2020 2020 2020 2020 496d 706c 656d  ..        Implem
-00016b90: 656e 7461 7469 6f6e 2064 6570 656e 6473  entation depends
-00016ba0: 206f 6e20 636c 6965 6e74 2070 6c61 7466   on client platf
-00016bb0: 6f72 6d20 6361 7061 6269 6c69 7469 6573  orm capabilities
-00016bc0: 2e20 466f 7220 6578 616d 706c 652c 0a20  . For example,. 
-00016bd0: 2020 2020 2020 2061 2077 6562 2062 726f         a web bro
-00016be0: 7773 6572 206d 6967 6874 206f 7065 6e20  wser might open 
-00016bf0: 6120 6c69 6e6b 2069 6e20 6120 706f 702d  a link in a pop-
-00016c00: 7570 2077 696e 646f 7720 7769 7468 2061  up window with a
-00016c10: 6e0a 2020 2020 2020 2020 6060 4f6e 436c  n.        ``OnCl
-00016c20: 6f73 6560 6020 6861 6e64 6c65 722e 0a0a  ose`` handler...
-00016c30: 2020 2020 2020 2020 4966 2062 6f74 6820          If both 
-00016c40: 6060 4f6e 4f70 656e 6060 2061 6e64 2060  ``OnOpen`` and `
-00016c50: 604f 6e43 6c6f 7365 6060 2068 616e 646c  `OnClose`` handl
-00016c60: 6572 7320 6172 6520 7365 742c 2061 6e64  ers are set, and
-00016c70: 2074 6865 2063 6c69 656e 740a 2020 2020   the client.    
-00016c80: 2020 2020 706c 6174 666f 726d 2063 616e      platform can
-00016c90: 2774 2073 7570 706f 7274 2062 6f74 6820  't support both 
-00016ca0: 7661 6c75 6573 2c20 6060 4f6e 436c 6f73  values, ``OnClos
-00016cb0: 6560 6020 7461 6b65 7320 7072 6563 6564  e`` takes preced
-00016cc0: 656e 6365 2e0a 0a20 2020 2020 2020 2060  ence...        `
-00016cd0: 476f 6f67 6c65 2057 6f72 6b73 7061 6365  Google Workspace
-00016ce0: 0a20 2020 2020 2020 2041 6464 2d6f 6e73  .        Add-ons
-00016cf0: 203c 6874 7470 733a 2f2f 6465 7665 6c6f   <https://develo
-00016d00: 7065 7273 2e67 6f6f 676c 652e 636f 6d2f  pers.google.com/
-00016d10: 776f 726b 7370 6163 652f 6164 642d 6f6e  workspace/add-on
-00016d20: 733e 605f 5f3a 0a0a 2020 2020 2020 2020  s>`__:..        
-00016d30: 5661 6c75 6573 3a0a 2020 2020 2020 2020  Values:.        
-00016d40: 2020 2020 4e4f 5448 494e 4720 2830 293a      NOTHING (0):
-00016d50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016d60: 2044 6566 6175 6c74 2076 616c 7565 2e20   Default value. 
-00016d70: 5468 6520 6361 7264 2064 6f65 736e 2774  The card doesn't
-00016d80: 2072 656c 6f61 643b 0a20 2020 2020 2020   reload;.       
-00016d90: 2020 2020 2020 2020 206e 6f74 6869 6e67           nothing
-00016da0: 2068 6170 7065 6e73 2e0a 2020 2020 2020   happens..      
-00016db0: 2020 2020 2020 5245 4c4f 4144 2028 3129        RELOAD (1)
-00016dc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00016dd0: 2020 5265 6c6f 6164 7320 7468 6520 6361    Reloads the ca
-00016de0: 7264 2061 6674 6572 2074 6865 2063 6869  rd after the chi
-00016df0: 6c64 2077 696e 646f 7720 636c 6f73 6573  ld window closes
-00016e00: 2e0a 0a20 2020 2020 2020 2020 2020 2020  ...             
-00016e10: 2020 2049 6620 7573 6564 2069 6e20 636f     If used in co
-00016e20: 6e6a 756e 6374 696f 6e20 7769 7468 0a20  njunction with. 
-00016e30: 2020 2020 2020 2020 2020 2020 2020 2060                 `
-00016e40: 6060 4f70 656e 4173 2e4f 5645 524c 4159  ``OpenAs.OVERLAY
-00016e50: 6060 203c 6874 7470 733a 2f2f 6465 7665  `` <https://deve
-00016e60: 6c6f 7065 7273 2e67 6f6f 676c 652e 636f  lopers.google.co
-00016e70: 6d2f 776f 726b 7370 6163 652f 6164 642d  m/workspace/add-
-00016e80: 6f6e 732f 7265 6665 7265 6e63 652f 7270  ons/reference/rp
-00016e90: 632f 676f 6f67 6c65 2e61 7070 732e 6361  c/google.apps.ca
-00016ea0: 7264 2e76 3123 6f70 656e 6173 3e60 5f5f  rd.v1#openas>`__
-00016eb0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00016ec0: 2020 7468 6520 6368 696c 6420 7769 6e64    the child wind
-00016ed0: 6f77 2061 6374 7320 6173 2061 206d 6f64  ow acts as a mod
-00016ee0: 616c 2064 6961 6c6f 6720 616e 6420 7468  al dialog and th
-00016ef0: 6520 7061 7265 6e74 2063 6172 640a 2020  e parent card.  
-00016f00: 2020 2020 2020 2020 2020 2020 2020 6973                is
-00016f10: 2062 6c6f 636b 6564 2075 6e74 696c 2074   blocked until t
-00016f20: 6865 2063 6869 6c64 2077 696e 646f 7720  he child window 
-00016f30: 636c 6f73 6573 2e0a 2020 2020 2020 2020  closes..        
-00016f40: 2222 220a 2020 2020 2020 2020 4e4f 5448  """.        NOTH
-00016f50: 494e 4720 3d20 300a 2020 2020 2020 2020  ING = 0.        
-00016f60: 5245 4c4f 4144 203d 2031 0a0a 2020 2020  RELOAD = 1..    
-00016f70: 7572 6c3a 2073 7472 203d 2070 726f 746f  url: str = proto
-00016f80: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
-00016f90: 7072 6f74 6f2e 5354 5249 4e47 2c0a 2020  proto.STRING,.  
-00016fa0: 2020 2020 2020 6e75 6d62 6572 3d31 2c0a        number=1,.
-00016fb0: 2020 2020 290a 2020 2020 6f70 656e 5f61      ).    open_a
-00016fc0: 733a 204f 7065 6e41 7320 3d20 7072 6f74  s: OpenAs = prot
-00016fd0: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-00016fe0: 2070 726f 746f 2e45 4e55 4d2c 0a20 2020   proto.ENUM,.   
-00016ff0: 2020 2020 206e 756d 6265 723d 322c 0a20       number=2,. 
-00017000: 2020 2020 2020 2065 6e75 6d3d 4f70 656e         enum=Open
-00017010: 4173 2c0a 2020 2020 290a 2020 2020 6f6e  As,.    ).    on
-00017020: 5f63 6c6f 7365 3a20 4f6e 436c 6f73 6520  _close: OnClose 
-00017030: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
-00017040: 2020 2020 2020 2070 726f 746f 2e45 4e55         proto.ENU
-00017050: 4d2c 0a20 2020 2020 2020 206e 756d 6265  M,.        numbe
-00017060: 723d 332c 0a20 2020 2020 2020 2065 6e75  r=3,.        enu
-00017070: 6d3d 4f6e 436c 6f73 652c 0a20 2020 2029  m=OnClose,.    )
-00017080: 0a0a 0a63 6c61 7373 2041 6374 696f 6e28  ...class Action(
-00017090: 7072 6f74 6f2e 4d65 7373 6167 6529 3a0a  proto.Message):.
-000170a0: 2020 2020 7222 2222 416e 2061 6374 696f      r"""An actio
-000170b0: 6e20 7468 6174 2064 6573 6372 6962 6573  n that describes
-000170c0: 2074 6865 2062 6568 6176 696f 7220 7768   the behavior wh
-000170d0: 656e 2074 6865 2066 6f72 6d20 6973 2073  en the form is s
-000170e0: 7562 6d69 7474 6564 2e0a 2020 2020 466f  ubmitted..    Fo
-000170f0: 7220 6578 616d 706c 652c 2079 6f75 2063  r example, you c
-00017100: 616e 2069 6e76 6f6b 6520 616e 2041 7070  an invoke an App
-00017110: 7320 5363 7269 7074 2073 6372 6970 7420  s Script script 
-00017120: 746f 2068 616e 646c 6520 7468 650a 2020  to handle the.  
-00017130: 2020 666f 726d 2e20 4966 2074 6865 2061    form. If the a
-00017140: 6374 696f 6e20 6973 2074 7269 6767 6572  ction is trigger
-00017150: 6564 2c20 7468 6520 666f 726d 2076 616c  ed, the form val
-00017160: 7565 7320 6172 6520 7365 6e74 2074 6f20  ues are sent to 
-00017170: 7468 650a 2020 2020 7365 7276 6572 2e0a  the.    server..
-00017180: 0a20 2020 2060 476f 6f67 6c65 2057 6f72  .    `Google Wor
-00017190: 6b73 7061 6365 2041 6464 2d6f 6e73 2061  kspace Add-ons a
-000171a0: 6e64 2043 6861 740a 2020 2020 6170 7073  nd Chat.    apps
-000171b0: 203c 6874 7470 733a 2f2f 6465 7665 6c6f   <https://develo
-000171c0: 7065 7273 2e67 6f6f 676c 652e 636f 6d2f  pers.google.com/
-000171d0: 776f 726b 7370 6163 652f 6578 7465 6e64  workspace/extend
-000171e0: 3e60 5f5f 3a0a 0a20 2020 2041 7474 7269  >`__:..    Attri
-000171f0: 6275 7465 733a 0a20 2020 2020 2020 2066  butes:.        f
-00017200: 756e 6374 696f 6e20 2873 7472 293a 0a20  unction (str):. 
-00017210: 2020 2020 2020 2020 2020 2041 2063 7573             A cus
-00017220: 746f 6d20 6675 6e63 7469 6f6e 2074 6f20  tom function to 
-00017230: 696e 766f 6b65 2077 6865 6e20 7468 6520  invoke when the 
-00017240: 636f 6e74 6169 6e69 6e67 2065 6c65 6d65  containing eleme
-00017250: 6e74 2069 730a 2020 2020 2020 2020 2020  nt is.          
-00017260: 2020 636c 6963 6b65 6420 6f72 206f 7468    clicked or oth
-00017270: 7277 6973 6520 6163 7469 7661 7465 642e  rwise activated.
-00017280: 0a0a 2020 2020 2020 2020 2020 2020 466f  ..            Fo
-00017290: 7220 6578 616d 706c 6520 7573 6167 652c  r example usage,
-000172a0: 2073 6565 2060 4372 6561 7465 2069 6e74   see `Create int
-000172b0: 6572 6163 7469 7665 0a20 2020 2020 2020  eractive.       
-000172c0: 2020 2020 2063 6172 6473 203c 6874 7470       cards <http
-000172d0: 733a 2f2f 6465 7665 6c6f 7065 7273 2e67  s://developers.g
-000172e0: 6f6f 676c 652e 636f 6d2f 6368 6174 2f68  oogle.com/chat/h
-000172f0: 6f77 2d74 6f73 2f63 6172 6473 2d6f 6e63  ow-tos/cards-onc
-00017300: 6c69 636b 3e60 5f5f 2e0a 2020 2020 2020  lick>`__..      
-00017310: 2020 7061 7261 6d65 7465 7273 2028 4d75    parameters (Mu
-00017320: 7461 626c 6553 6571 7565 6e63 655b 676f  tableSequence[go
-00017330: 6f67 6c65 2e61 7070 732e 6361 7264 5f76  ogle.apps.card_v
-00017340: 312e 7479 7065 732e 4163 7469 6f6e 2e41  1.types.Action.A
-00017350: 6374 696f 6e50 6172 616d 6574 6572 5d29  ctionParameter])
-00017360: 3a0a 2020 2020 2020 2020 2020 2020 4c69  :.            Li
-00017370: 7374 206f 6620 6163 7469 6f6e 2070 6172  st of action par
-00017380: 616d 6574 6572 732e 0a20 2020 2020 2020  ameters..       
-00017390: 206c 6f61 645f 696e 6469 6361 746f 7220   load_indicator 
-000173a0: 2867 6f6f 676c 652e 6170 7073 2e63 6172  (google.apps.car
-000173b0: 645f 7631 2e74 7970 6573 2e41 6374 696f  d_v1.types.Actio
-000173c0: 6e2e 4c6f 6164 496e 6469 6361 746f 7229  n.LoadIndicator)
-000173d0: 3a0a 2020 2020 2020 2020 2020 2020 5370  :.            Sp
-000173e0: 6563 6966 6965 7320 7468 6520 6c6f 6164  ecifies the load
-000173f0: 696e 6720 696e 6469 6361 746f 7220 7468  ing indicator th
-00017400: 6174 2074 6865 0a20 2020 2020 2020 2020  at the.         
-00017410: 2020 2061 6374 696f 6e20 6469 7370 6c61     action displa
-00017420: 7973 2077 6869 6c65 206d 616b 696e 6720  ys while making 
-00017430: 7468 6520 6361 6c6c 2074 6f20 7468 650a  the call to the.
-00017440: 2020 2020 2020 2020 2020 2020 6163 7469              acti
-00017450: 6f6e 2e0a 2020 2020 2020 2020 7065 7273  on..        pers
-00017460: 6973 745f 7661 6c75 6573 2028 626f 6f6c  ist_values (bool
-00017470: 293a 0a20 2020 2020 2020 2020 2020 2049  ):.            I
-00017480: 6e64 6963 6174 6573 2077 6865 7468 6572  ndicates whether
-00017490: 2066 6f72 6d20 7661 6c75 6573 2070 6572   form values per
-000174a0: 7369 7374 2061 6674 6572 2074 6865 2061  sist after the a
-000174b0: 6374 696f 6e2e 2054 6865 0a20 2020 2020  ction. The.     
-000174c0: 2020 2020 2020 2064 6566 6175 6c74 2076         default v
-000174d0: 616c 7565 2069 7320 6060 6661 6c73 6560  alue is ``false`
-000174e0: 602e 0a0a 2020 2020 2020 2020 2020 2020  `...            
-000174f0: 4966 2060 6074 7275 6560 602c 2066 6f72  If ``true``, for
-00017500: 6d20 7661 6c75 6573 2072 656d 6169 6e20  m values remain 
-00017510: 6166 7465 7220 7468 6520 6163 7469 6f6e  after the action
-00017520: 2069 730a 2020 2020 2020 2020 2020 2020   is.            
-00017530: 7472 6967 6765 7265 642e 2054 6f20 6c65  triggered. To le
-00017540: 7420 7468 6520 7573 6572 206d 616b 6520  t the user make 
-00017550: 6368 616e 6765 7320 7768 696c 6520 7468  changes while th
-00017560: 6520 6163 7469 6f6e 2069 730a 2020 2020  e action is.    
-00017570: 2020 2020 2020 2020 6265 696e 6720 7072          being pr
-00017580: 6f63 6573 7365 642c 2073 6574 0a20 2020  ocessed, set.   
-00017590: 2020 2020 2020 2020 2060 6060 4c6f 6164           ```Load
-000175a0: 496e 6469 6361 746f 7260 6020 3c68 7474  Indicator`` <htt
-000175b0: 7073 3a2f 2f64 6576 656c 6f70 6572 732e  ps://developers.
-000175c0: 676f 6f67 6c65 2e63 6f6d 2f77 6f72 6b73  google.com/works
-000175d0: 7061 6365 2f61 6464 2d6f 6e73 2f72 6566  pace/add-ons/ref
-000175e0: 6572 656e 6365 2f72 7063 2f67 6f6f 676c  erence/rpc/googl
-000175f0: 652e 6170 7073 2e63 6172 642e 7631 236c  e.apps.card.v1#l
-00017600: 6f61 6469 6e64 6963 6174 6f72 3e60 5f5f  oadindicator>`__
-00017610: 0a20 2020 2020 2020 2020 2020 2074 6f20  .            to 
-00017620: 6060 4e4f 4e45 6060 2e20 466f 7220 6063  ``NONE``. For `c
-00017630: 6172 640a 2020 2020 2020 2020 2020 2020  ard.            
-00017640: 6d65 7373 6167 6573 203c 6874 7470 733a  messages <https:
-00017650: 2f2f 6465 7665 6c6f 7065 7273 2e67 6f6f  //developers.goo
-00017660: 676c 652e 636f 6d2f 6368 6174 2f61 7069  gle.com/chat/api
-00017670: 2f67 7569 6465 732f 7631 2f6d 6573 7361  /guides/v1/messa
-00017680: 6765 732f 6372 6561 7465 2363 7265 6174  ges/create#creat
-00017690: 653e 605f 5f0a 2020 2020 2020 2020 2020  e>`__.          
-000176a0: 2020 696e 2043 6861 7420 6170 7073 2c20    in Chat apps, 
-000176b0: 796f 7520 6d75 7374 2061 6c73 6f20 7365  you must also se
-000176c0: 7420 7468 6520 6163 7469 6f6e 2773 0a20  t the action's. 
-000176d0: 2020 2020 2020 2020 2020 2060 6060 5265             ```Re
-000176e0: 7370 6f6e 7365 5479 7065 6060 203c 6874  sponseType`` <ht
-000176f0: 7470 733a 2f2f 6465 7665 6c6f 7065 7273  tps://developers
-00017700: 2e67 6f6f 676c 652e 636f 6d2f 6368 6174  .google.com/chat
-00017710: 2f61 7069 2f72 6566 6572 656e 6365 2f72  /api/reference/r
-00017720: 6573 742f 7631 2f73 7061 6365 732e 6d65  est/v1/spaces.me
-00017730: 7373 6167 6573 2372 6573 706f 6e73 6574  ssages#responset
-00017740: 7970 653e 605f 5f0a 2020 2020 2020 2020  ype>`__.        
-00017750: 2020 2020 746f 2060 6055 5044 4154 455f      to ``UPDATE_
-00017760: 4d45 5353 4147 4560 6020 616e 6420 7573  MESSAGE`` and us
-00017770: 6520 7468 6520 7361 6d65 0a20 2020 2020  e the same.     
-00017780: 2020 2020 2020 2060 6060 6361 7264 5f69         ```card_i
-00017790: 6460 6020 3c68 7474 7073 3a2f 2f64 6576  d`` <https://dev
-000177a0: 656c 6f70 6572 732e 676f 6f67 6c65 2e63  elopers.google.c
-000177b0: 6f6d 2f63 6861 742f 6170 692f 7265 6665  om/chat/api/refe
-000177c0: 7265 6e63 652f 7265 7374 2f76 312f 7370  rence/rest/v1/sp
-000177d0: 6163 6573 2e6d 6573 7361 6765 7323 4361  aces.messages#Ca
-000177e0: 7264 5769 7468 4964 3e60 5f5f 0a20 2020  rdWithId>`__.   
-000177f0: 2020 2020 2020 2020 2066 726f 6d20 7468           from th
-00017800: 6520 6361 7264 2074 6861 7420 636f 6e74  e card that cont
-00017810: 6169 6e65 6420 7468 6520 6163 7469 6f6e  ained the action
-00017820: 2e0a 0a20 2020 2020 2020 2020 2020 2049  ...            I
-00017830: 6620 6060 6661 6c73 6560 602c 2074 6865  f ``false``, the
-00017840: 2066 6f72 6d20 7661 6c75 6573 2061 7265   form values are
-00017850: 2063 6c65 6172 6564 2077 6865 6e20 7468   cleared when th
-00017860: 6520 6163 7469 6f6e 2069 730a 2020 2020  e action is.    
-00017870: 2020 2020 2020 2020 7472 6967 6765 7265          triggere
-00017880: 642e 2054 6f20 7072 6576 656e 7420 7468  d. To prevent th
-00017890: 6520 7573 6572 2066 726f 6d20 6d61 6b69  e user from maki
-000178a0: 6e67 2063 6861 6e67 6573 2077 6869 6c65  ng changes while
-000178b0: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
-000178c0: 2061 6374 696f 6e20 6973 2062 6569 6e67   action is being
-000178d0: 2070 726f 6365 7373 6564 2c20 7365 740a   processed, set.
-000178e0: 2020 2020 2020 2020 2020 2020 6060 604c              ```L
-000178f0: 6f61 6449 6e64 6963 6174 6f72 6060 203c  oadIndicator`` <
-00017900: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
-00017910: 7273 2e67 6f6f 676c 652e 636f 6d2f 776f  rs.google.com/wo
-00017920: 726b 7370 6163 652f 6164 642d 6f6e 732f  rkspace/add-ons/
-00017930: 7265 6665 7265 6e63 652f 7270 632f 676f  reference/rpc/go
-00017940: 6f67 6c65 2e61 7070 732e 6361 7264 2e76  ogle.apps.card.v
-00017950: 3123 6c6f 6164 696e 6469 6361 746f 723e  1#loadindicator>
-00017960: 605f 5f0a 2020 2020 2020 2020 2020 2020  `__.            
-00017970: 746f 2060 6053 5049 4e4e 4552 6060 2e0a  to ``SPINNER``..
-00017980: 2020 2020 2020 2020 696e 7465 7261 6374          interact
-00017990: 696f 6e20 2867 6f6f 676c 652e 6170 7073  ion (google.apps
-000179a0: 2e63 6172 645f 7631 2e74 7970 6573 2e41  .card_v1.types.A
-000179b0: 6374 696f 6e2e 496e 7465 7261 6374 696f  ction.Interactio
-000179c0: 6e29 3a0a 2020 2020 2020 2020 2020 2020  n):.            
-000179d0: 4f70 7469 6f6e 616c 2e20 5265 7175 6972  Optional. Requir
-000179e0: 6564 2077 6865 6e20 6f70 656e 696e 6720  ed when opening 
-000179f0: 610a 2020 2020 2020 2020 2020 2020 6064  a.            `d
-00017a00: 6961 6c6f 6720 3c68 7474 7073 3a2f 2f64  ialog <https://d
-00017a10: 6576 656c 6f70 6572 732e 676f 6f67 6c65  evelopers.google
-00017a20: 2e63 6f6d 2f63 6861 742f 686f 772d 746f  .com/chat/how-to
-00017a30: 732f 6469 616c 6f67 733e 605f 5f2e 0a0a  s/dialogs>`__...
-00017a40: 2020 2020 2020 2020 2020 2020 5768 6174              What
-00017a50: 2074 6f20 646f 2069 6e20 7265 7370 6f6e   to do in respon
-00017a60: 7365 2074 6f20 616e 2069 6e74 6572 6163  se to an interac
-00017a70: 7469 6f6e 2077 6974 6820 6120 7573 6572  tion with a user
-00017a80: 2c20 7375 6368 0a20 2020 2020 2020 2020  , such.         
-00017a90: 2020 2061 7320 6120 7573 6572 2063 6c69     as a user cli
-00017aa0: 636b 696e 6720 6120 6275 7474 6f6e 2069  cking a button i
-00017ab0: 6e20 6120 6361 7264 206d 6573 7361 6765  n a card message
-00017ac0: 2e0a 0a20 2020 2020 2020 2020 2020 2049  ...            I
-00017ad0: 6620 756e 7370 6563 6966 6965 642c 2074  f unspecified, t
-00017ae0: 6865 2061 7070 2072 6573 706f 6e64 7320  he app responds 
-00017af0: 6279 2065 7865 6375 7469 6e67 2061 6e0a  by executing an.
-00017b00: 2020 2020 2020 2020 2020 2020 6060 6163              ``ac
-00017b10: 7469 6f6e 6060 e280 946c 696b 6520 6f70  tion``...like op
-00017b20: 656e 696e 6720 6120 6c69 6e6b 206f 7220  ening a link or 
-00017b30: 7275 6e6e 696e 6720 6120 6675 6e63 7469  running a functi
-00017b40: 6f6e e280 9461 730a 2020 2020 2020 2020  on...as.        
-00017b50: 2020 2020 6e6f 726d 616c 2e0a 0a20 2020      normal...   
-00017b60: 2020 2020 2020 2020 2042 7920 7370 6563           By spec
-00017b70: 6966 7969 6e67 2061 6e20 6060 696e 7465  ifying an ``inte
-00017b80: 7261 6374 696f 6e60 602c 2074 6865 2061  raction``, the a
-00017b90: 7070 2063 616e 2072 6573 706f 6e64 2069  pp can respond i
-00017ba0: 6e0a 2020 2020 2020 2020 2020 2020 7370  n.            sp
-00017bb0: 6563 6961 6c20 696e 7465 7261 6374 6976  ecial interactiv
-00017bc0: 6520 7761 7973 2e20 466f 7220 6578 616d  e ways. For exam
-00017bd0: 706c 652c 2062 7920 7365 7474 696e 670a  ple, by setting.
-00017be0: 2020 2020 2020 2020 2020 2020 6060 696e              ``in
-00017bf0: 7465 7261 6374 696f 6e60 6020 746f 2060  teraction`` to `
-00017c00: 604f 5045 4e5f 4449 414c 4f47 6060 2c20  `OPEN_DIALOG``, 
-00017c10: 7468 6520 6170 7020 6361 6e20 6f70 656e  the app can open
-00017c20: 2061 0a20 2020 2020 2020 2020 2020 2060   a.            `
-00017c30: 6469 616c 6f67 203c 6874 7470 733a 2f2f  dialog <https://
-00017c40: 6465 7665 6c6f 7065 7273 2e67 6f6f 676c  developers.googl
-00017c50: 652e 636f 6d2f 6368 6174 2f68 6f77 2d74  e.com/chat/how-t
-00017c60: 6f73 2f64 6961 6c6f 6773 3e60 5f5f 2e0a  os/dialogs>`__..
-00017c70: 2020 2020 2020 2020 2020 2020 5768 656e              When
-00017c80: 2073 7065 6369 6669 6564 2c20 6120 6c6f   specified, a lo
-00017c90: 6164 696e 6720 696e 6469 6361 746f 7220  ading indicator 
-00017ca0: 6973 6e27 7420 7368 6f77 6e2e 2049 660a  isn't shown. If.
-00017cb0: 2020 2020 2020 2020 2020 2020 7370 6563              spec
-00017cc0: 6966 6965 6420 666f 7220 616e 2061 6464  ified for an add
-00017cd0: 2d6f 6e2c 2074 6865 2065 6e74 6972 6520  -on, the entire 
-00017ce0: 6361 7264 2069 7320 7374 7269 7070 6564  card is stripped
-00017cf0: 2061 6e64 0a20 2020 2020 2020 2020 2020   and.           
-00017d00: 206e 6f74 6869 6e67 2069 7320 7368 6f77   nothing is show
-00017d10: 6e20 696e 2074 6865 2063 6c69 656e 742e  n in the client.
-00017d20: 0a0a 2020 2020 2020 2020 2020 2020 6047  ..            `G
-00017d30: 6f6f 676c 6520 4368 6174 2061 7070 7320  oogle Chat apps 
-00017d40: 3c68 7474 7073 3a2f 2f64 6576 656c 6f70  <https://develop
-00017d50: 6572 732e 676f 6f67 6c65 2e63 6f6d 2f63  ers.google.com/c
-00017d60: 6861 743e 605f 5f3a 0a20 2020 2022 2222  hat>`__:.    """
-00017d70: 0a0a 2020 2020 636c 6173 7320 4c6f 6164  ..    class Load
-00017d80: 496e 6469 6361 746f 7228 7072 6f74 6f2e  Indicator(proto.
-00017d90: 456e 756d 293a 0a20 2020 2020 2020 2072  Enum):.        r
-00017da0: 2222 2253 7065 6369 6669 6573 2074 6865  """Specifies the
-00017db0: 206c 6f61 6469 6e67 2069 6e64 6963 6174   loading indicat
-00017dc0: 6f72 2074 6861 7420 7468 6520 6163 7469  or that the acti
-00017dd0: 6f6e 2064 6973 706c 6179 7320 7768 696c  on displays whil
-00017de0: 650a 2020 2020 2020 2020 6d61 6b69 6e67  e.        making
-00017df0: 2074 6865 2063 616c 6c20 746f 2074 6865   the call to the
-00017e00: 2061 6374 696f 6e2e 0a0a 2020 2020 2020   action...      
-00017e10: 2020 6047 6f6f 676c 6520 576f 726b 7370    `Google Worksp
-00017e20: 6163 6520 4164 642d 6f6e 7320 616e 6420  ace Add-ons and 
-00017e30: 4368 6174 0a20 2020 2020 2020 2061 7070  Chat.        app
-00017e40: 7320 3c68 7474 7073 3a2f 2f64 6576 656c  s <https://devel
-00017e50: 6f70 6572 732e 676f 6f67 6c65 2e63 6f6d  opers.google.com
-00017e60: 2f77 6f72 6b73 7061 6365 2f65 7874 656e  /workspace/exten
-00017e70: 643e 605f 5f3a 0a0a 2020 2020 2020 2020  d>`__:..        
-00017e80: 5661 6c75 6573 3a0a 2020 2020 2020 2020  Values:.        
-00017e90: 2020 2020 5350 494e 4e45 5220 2830 293a      SPINNER (0):
-00017ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017eb0: 2044 6973 706c 6179 7320 6120 7370 696e   Displays a spin
-00017ec0: 6e65 7220 746f 2069 6e64 6963 6174 6520  ner to indicate 
-00017ed0: 7468 6174 2063 6f6e 7465 6e74 0a20 2020  that content.   
-00017ee0: 2020 2020 2020 2020 2020 2020 2069 7320               is 
-00017ef0: 6c6f 6164 696e 672e 0a20 2020 2020 2020  loading..       
-00017f00: 2020 2020 204e 4f4e 4520 2831 293a 0a20       NONE (1):. 
-00017f10: 2020 2020 2020 2020 2020 2020 2020 204e                 N
-00017f20: 6f74 6869 6e67 2069 7320 6469 7370 6c61  othing is displa
-00017f30: 7965 642e 0a20 2020 2020 2020 2022 2222  yed..        """
-00017f40: 0a20 2020 2020 2020 2053 5049 4e4e 4552  .        SPINNER
-00017f50: 203d 2030 0a20 2020 2020 2020 204e 4f4e   = 0.        NON
-00017f60: 4520 3d20 310a 0a20 2020 2063 6c61 7373  E = 1..    class
-00017f70: 2049 6e74 6572 6163 7469 6f6e 2870 726f   Interaction(pro
-00017f80: 746f 2e45 6e75 6d29 3a0a 2020 2020 2020  to.Enum):.      
-00017f90: 2020 7222 2222 4f70 7469 6f6e 616c 2e20    r"""Optional. 
-00017fa0: 5265 7175 6972 6564 2077 6865 6e20 6f70  Required when op
-00017fb0: 656e 696e 6720 610a 2020 2020 2020 2020  ening a.        
-00017fc0: 6064 6961 6c6f 6720 3c68 7474 7073 3a2f  `dialog <https:/
-00017fd0: 2f64 6576 656c 6f70 6572 732e 676f 6f67  /developers.goog
-00017fe0: 6c65 2e63 6f6d 2f63 6861 742f 686f 772d  le.com/chat/how-
-00017ff0: 746f 732f 6469 616c 6f67 733e 605f 5f2e  tos/dialogs>`__.
-00018000: 0a0a 2020 2020 2020 2020 5768 6174 2074  ..        What t
-00018010: 6f20 646f 2069 6e20 7265 7370 6f6e 7365  o do in response
-00018020: 2074 6f20 616e 2069 6e74 6572 6163 7469   to an interacti
-00018030: 6f6e 2077 6974 6820 6120 7573 6572 2c20  on with a user, 
-00018040: 7375 6368 2061 7320 6120 7573 6572 0a20  such as a user. 
-00018050: 2020 2020 2020 2063 6c69 636b 696e 6720         clicking 
-00018060: 6120 6275 7474 6f6e 2069 6e20 6120 6361  a button in a ca
-00018070: 7264 206d 6573 7361 6765 2e0a 0a20 2020  rd message...   
-00018080: 2020 2020 2049 6620 756e 7370 6563 6966       If unspecif
-00018090: 6965 642c 2074 6865 2061 7070 2072 6573  ied, the app res
-000180a0: 706f 6e64 7320 6279 2065 7865 6375 7469  ponds by executi
-000180b0: 6e67 2061 6e20 6060 6163 7469 6f6e 6060  ng an ``action``
-000180c0: e280 946c 696b 650a 2020 2020 2020 2020  ...like.        
-000180d0: 6f70 656e 696e 6720 6120 6c69 6e6b 206f  opening a link o
-000180e0: 7220 7275 6e6e 696e 6720 6120 6675 6e63  r running a func
-000180f0: 7469 6f6e e280 9461 7320 6e6f 726d 616c  tion...as normal
-00018100: 2e0a 0a20 2020 2020 2020 2042 7920 7370  ...        By sp
-00018110: 6563 6966 7969 6e67 2061 6e20 6060 696e  ecifying an ``in
-00018120: 7465 7261 6374 696f 6e60 602c 2074 6865  teraction``, the
-00018130: 2061 7070 2063 616e 2072 6573 706f 6e64   app can respond
-00018140: 2069 6e20 7370 6563 6961 6c0a 2020 2020   in special.    
-00018150: 2020 2020 696e 7465 7261 6374 6976 6520      interactive 
-00018160: 7761 7973 2e20 466f 7220 6578 616d 706c  ways. For exampl
-00018170: 652c 2062 7920 7365 7474 696e 6720 6060  e, by setting ``
-00018180: 696e 7465 7261 6374 696f 6e60 6020 746f  interaction`` to
-00018190: 0a20 2020 2020 2020 2060 604f 5045 4e5f  .        ``OPEN_
-000181a0: 4449 414c 4f47 6060 2c20 7468 6520 6170  DIALOG``, the ap
-000181b0: 7020 6361 6e20 6f70 656e 2061 0a20 2020  p can open a.   
-000181c0: 2020 2020 2060 6469 616c 6f67 203c 6874       `dialog <ht
-000181d0: 7470 733a 2f2f 6465 7665 6c6f 7065 7273  tps://developers
-000181e0: 2e67 6f6f 676c 652e 636f 6d2f 6368 6174  .google.com/chat
-000181f0: 2f68 6f77 2d74 6f73 2f64 6961 6c6f 6773  /how-tos/dialogs
-00018200: 3e60 5f5f 2e0a 0a20 2020 2020 2020 2057  >`__...        W
-00018210: 6865 6e20 7370 6563 6966 6965 642c 2061  hen specified, a
-00018220: 206c 6f61 6469 6e67 2069 6e64 6963 6174   loading indicat
-00018230: 6f72 2069 736e 2774 2073 686f 776e 2e20  or isn't shown. 
-00018240: 4966 2073 7065 6369 6669 6564 2066 6f72  If specified for
-00018250: 2061 6e0a 2020 2020 2020 2020 6164 642d   an.        add-
-00018260: 6f6e 2c20 7468 6520 656e 7469 7265 2063  on, the entire c
-00018270: 6172 6420 6973 2073 7472 6970 7065 6420  ard is stripped 
-00018280: 616e 6420 6e6f 7468 696e 6720 6973 2073  and nothing is s
-00018290: 686f 776e 2069 6e20 7468 650a 2020 2020  hown in the.    
-000182a0: 2020 2020 636c 6965 6e74 2e0a 0a20 2020      client...   
-000182b0: 2020 2020 2060 476f 6f67 6c65 2043 6861       `Google Cha
-000182c0: 7420 6170 7073 203c 6874 7470 733a 2f2f  t apps <https://
-000182d0: 6465 7665 6c6f 7065 7273 2e67 6f6f 676c  developers.googl
-000182e0: 652e 636f 6d2f 6368 6174 3e60 5f5f 3a0a  e.com/chat>`__:.
-000182f0: 0a20 2020 2020 2020 2056 616c 7565 733a  .        Values:
-00018300: 0a20 2020 2020 2020 2020 2020 2049 4e54  .            INT
-00018310: 4552 4143 5449 4f4e 5f55 4e53 5045 4349  ERACTION_UNSPECI
-00018320: 4649 4544 2028 3029 3a0a 2020 2020 2020  FIED (0):.      
-00018330: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
-00018340: 7420 7661 6c75 652e 2054 6865 2060 6061  t value. The ``a
-00018350: 6374 696f 6e60 6020 6578 6563 7574 6573  ction`` executes
-00018360: 2061 7320 6e6f 726d 616c 2e0a 2020 2020   as normal..    
-00018370: 2020 2020 2020 2020 4f50 454e 5f44 4941          OPEN_DIA
-00018380: 4c4f 4720 2831 293a 0a20 2020 2020 2020  LOG (1):.       
-00018390: 2020 2020 2020 2020 204f 7065 6e73 2061           Opens a
-000183a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000183b0: 2060 6469 616c 6f67 203c 6874 7470 733a   `dialog <https:
-000183c0: 2f2f 6465 7665 6c6f 7065 7273 2e67 6f6f  //developers.goo
-000183d0: 676c 652e 636f 6d2f 6368 6174 2f68 6f77  gle.com/chat/how
-000183e0: 2d74 6f73 2f64 6961 6c6f 6773 3e60 5f5f  -tos/dialogs>`__
-000183f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00018400: 2020 6120 7769 6e64 6f77 6564 2c20 6361    a windowed, ca
-00018410: 7264 2d62 6173 6564 2069 6e74 6572 6661  rd-based interfa
-00018420: 6365 2074 6861 7420 4368 6174 2061 7070  ce that Chat app
-00018430: 7320 7573 6520 746f 0a20 2020 2020 2020  s use to.       
-00018440: 2020 2020 2020 2020 2069 6e74 6572 6163           interac
-00018450: 7420 7769 7468 2075 7365 7273 2e0a 0a20  t with users... 
-00018460: 2020 2020 2020 2020 2020 2020 2020 204f                 O
-00018470: 6e6c 7920 7375 7070 6f72 7465 6420 6279  nly supported by
-00018480: 2043 6861 7420 6170 7073 2069 6e20 7265   Chat apps in re
-00018490: 7370 6f6e 7365 2074 6f20 6275 7474 6f6e  sponse to button
-000184a0: 2d63 6c69 636b 7320 6f6e 0a20 2020 2020  -clicks on.     
-000184b0: 2020 2020 2020 2020 2020 2063 6172 6420             card 
-000184c0: 6d65 7373 6167 6573 2e20 4966 2073 7065  messages. If spe
-000184d0: 6369 6669 6564 2066 6f72 2061 6e20 6164  cified for an ad
-000184e0: 642d 6f6e 2c20 7468 6520 656e 7469 7265  d-on, the entire
-000184f0: 2063 6172 640a 2020 2020 2020 2020 2020   card.          
-00018500: 2020 2020 2020 6973 2073 7472 6970 7065        is strippe
-00018510: 6420 616e 6420 6e6f 7468 696e 6720 6973  d and nothing is
-00018520: 2073 686f 776e 2069 6e20 7468 6520 636c   shown in the cl
-00018530: 6965 6e74 2e0a 0a20 2020 2020 2020 2020  ient...         
-00018540: 2020 2020 2020 2060 476f 6f67 6c65 2043         `Google C
-00018550: 6861 7420 6170 7073 203c 6874 7470 733a  hat apps <https:
-00018560: 2f2f 6465 7665 6c6f 7065 7273 2e67 6f6f  //developers.goo
-00018570: 676c 652e 636f 6d2f 6368 6174 3e60 5f5f  gle.com/chat>`__
-00018580: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00018590: 2020 2020 2020 494e 5445 5241 4354 494f        INTERACTIO
-000185a0: 4e5f 554e 5350 4543 4946 4945 4420 3d20  N_UNSPECIFIED = 
-000185b0: 300a 2020 2020 2020 2020 4f50 454e 5f44  0.        OPEN_D
-000185c0: 4941 4c4f 4720 3d20 310a 0a20 2020 2063  IALOG = 1..    c
-000185d0: 6c61 7373 2041 6374 696f 6e50 6172 616d  lass ActionParam
-000185e0: 6574 6572 2870 726f 746f 2e4d 6573 7361  eter(proto.Messa
-000185f0: 6765 293a 0a20 2020 2020 2020 2072 2222  ge):.        r""
-00018600: 224c 6973 7420 6f66 2073 7472 696e 6720  "List of string 
-00018610: 7061 7261 6d65 7465 7273 2074 6f20 7375  parameters to su
-00018620: 7070 6c79 2077 6865 6e20 7468 6520 6163  pply when the ac
-00018630: 7469 6f6e 206d 6574 686f 6420 6973 0a20  tion method is. 
-00018640: 2020 2020 2020 2069 6e76 6f6b 6564 2e20         invoked. 
-00018650: 466f 7220 6578 616d 706c 652c 2063 6f6e  For example, con
-00018660: 7369 6465 7220 7468 7265 6520 736e 6f6f  sider three snoo
-00018670: 7a65 2062 7574 746f 6e73 3a20 736e 6f6f  ze buttons: snoo
-00018680: 7a65 206e 6f77 2c0a 2020 2020 2020 2020  ze now,.        
-00018690: 736e 6f6f 7a65 206f 6e65 2064 6179 2c20  snooze one day, 
-000186a0: 6f72 2073 6e6f 6f7a 6520 6e65 7874 2077  or snooze next w
-000186b0: 6565 6b2e 2059 6f75 206d 6967 6874 2075  eek. You might u
-000186c0: 7365 0a20 2020 2020 2020 2060 6061 6374  se.        ``act
-000186d0: 696f 6e20 6d65 7468 6f64 203d 2073 6e6f  ion method = sno
-000186e0: 6f7a 6528 2960 602c 2070 6173 7369 6e67  oze()``, passing
-000186f0: 2074 6865 2073 6e6f 6f7a 6520 7479 7065   the snooze type
-00018700: 2061 6e64 2073 6e6f 6f7a 650a 2020 2020   and snooze.    
-00018710: 2020 2020 7469 6d65 2069 6e20 7468 6520      time in the 
-00018720: 6c69 7374 206f 6620 7374 7269 6e67 2070  list of string p
-00018730: 6172 616d 6574 6572 732e 0a0a 2020 2020  arameters...    
-00018740: 2020 2020 546f 206c 6561 726e 206d 6f72      To learn mor
-00018750: 652c 2073 6565 0a20 2020 2020 2020 2060  e, see.        `
-00018760: 6060 436f 6d6d 6f6e 4576 656e 744f 626a  ``CommonEventObj
-00018770: 6563 7460 6020 3c68 7474 7073 3a2f 2f64  ect`` <https://d
-00018780: 6576 656c 6f70 6572 732e 676f 6f67 6c65  evelopers.google
-00018790: 2e63 6f6d 2f63 6861 742f 6170 692f 7265  .com/chat/api/re
-000187a0: 6665 7265 6e63 652f 7265 7374 2f76 312f  ference/rest/v1/
-000187b0: 4576 656e 7423 636f 6d6d 6f6e 6576 656e  Event#commoneven
-000187c0: 746f 626a 6563 743e 605f 5f2e 0a0a 2020  tobject>`__...  
-000187d0: 2020 2020 2020 6047 6f6f 676c 6520 576f        `Google Wo
-000187e0: 726b 7370 6163 6520 4164 642d 6f6e 7320  rkspace Add-ons 
-000187f0: 616e 6420 4368 6174 0a20 2020 2020 2020  and Chat.       
-00018800: 2061 7070 7320 3c68 7474 7073 3a2f 2f64   apps <https://d
-00018810: 6576 656c 6f70 6572 732e 676f 6f67 6c65  evelopers.google
-00018820: 2e63 6f6d 2f77 6f72 6b73 7061 6365 2f65  .com/workspace/e
-00018830: 7874 656e 643e 605f 5f3a 0a0a 2020 2020  xtend>`__:..    
-00018840: 2020 2020 4174 7472 6962 7574 6573 3a0a      Attributes:.
-00018850: 2020 2020 2020 2020 2020 2020 6b65 7920              key 
-00018860: 2873 7472 293a 0a20 2020 2020 2020 2020  (str):.         
-00018870: 2020 2020 2020 2054 6865 206e 616d 6520         The name 
-00018880: 6f66 2074 6865 2070 6172 616d 6574 6572  of the parameter
-00018890: 2066 6f72 2074 6865 2061 6374 696f 6e0a   for the action.
-000188a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000188b0: 7363 7269 7074 2e0a 2020 2020 2020 2020  script..        
-000188c0: 2020 2020 7661 6c75 6520 2873 7472 293a      value (str):
-000188d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000188e0: 2054 6865 2076 616c 7565 206f 6620 7468   The value of th
-000188f0: 6520 7061 7261 6d65 7465 722e 0a20 2020  e parameter..   
-00018900: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
-00018910: 2020 6b65 793a 2073 7472 203d 2070 726f    key: str = pro
-00018920: 746f 2e46 6965 6c64 280a 2020 2020 2020  to.Field(.      
-00018930: 2020 2020 2020 7072 6f74 6f2e 5354 5249        proto.STRI
-00018940: 4e47 2c0a 2020 2020 2020 2020 2020 2020  NG,.            
-00018950: 6e75 6d62 6572 3d31 2c0a 2020 2020 2020  number=1,.      
-00018960: 2020 290a 2020 2020 2020 2020 7661 6c75    ).        valu
-00018970: 653a 2073 7472 203d 2070 726f 746f 2e46  e: str = proto.F
-00018980: 6965 6c64 280a 2020 2020 2020 2020 2020  ield(.          
-00018990: 2020 7072 6f74 6f2e 5354 5249 4e47 2c0a    proto.STRING,.
-000189a0: 2020 2020 2020 2020 2020 2020 6e75 6d62              numb
-000189b0: 6572 3d32 2c0a 2020 2020 2020 2020 290a  er=2,.        ).
-000189c0: 0a20 2020 2066 756e 6374 696f 6e3a 2073  .    function: s
-000189d0: 7472 203d 2070 726f 746f 2e46 6965 6c64  tr = proto.Field
-000189e0: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
-000189f0: 5354 5249 4e47 2c0a 2020 2020 2020 2020  STRING,.        
-00018a00: 6e75 6d62 6572 3d31 2c0a 2020 2020 290a  number=1,.    ).
-00018a10: 2020 2020 7061 7261 6d65 7465 7273 3a20      parameters: 
-00018a20: 4d75 7461 626c 6553 6571 7565 6e63 655b  MutableSequence[
-00018a30: 4163 7469 6f6e 5061 7261 6d65 7465 725d  ActionParameter]
-00018a40: 203d 2070 726f 746f 2e52 6570 6561 7465   = proto.Repeate
-00018a50: 6446 6965 6c64 280a 2020 2020 2020 2020  dField(.        
-00018a60: 7072 6f74 6f2e 4d45 5353 4147 452c 0a20  proto.MESSAGE,. 
-00018a70: 2020 2020 2020 206e 756d 6265 723d 322c         number=2,
-00018a80: 0a20 2020 2020 2020 206d 6573 7361 6765  .        message
-00018a90: 3d41 6374 696f 6e50 6172 616d 6574 6572  =ActionParameter
-00018aa0: 2c0a 2020 2020 290a 2020 2020 6c6f 6164  ,.    ).    load
-00018ab0: 5f69 6e64 6963 6174 6f72 3a20 4c6f 6164  _indicator: Load
-00018ac0: 496e 6469 6361 746f 7220 3d20 7072 6f74  Indicator = prot
-00018ad0: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-00018ae0: 2070 726f 746f 2e45 4e55 4d2c 0a20 2020   proto.ENUM,.   
-00018af0: 2020 2020 206e 756d 6265 723d 332c 0a20       number=3,. 
-00018b00: 2020 2020 2020 2065 6e75 6d3d 4c6f 6164         enum=Load
-00018b10: 496e 6469 6361 746f 722c 0a20 2020 2029  Indicator,.    )
-00018b20: 0a20 2020 2070 6572 7369 7374 5f76 616c  .    persist_val
-00018b30: 7565 733a 2062 6f6f 6c20 3d20 7072 6f74  ues: bool = prot
-00018b40: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-00018b50: 2070 726f 746f 2e42 4f4f 4c2c 0a20 2020   proto.BOOL,.   
-00018b60: 2020 2020 206e 756d 6265 723d 342c 0a20       number=4,. 
-00018b70: 2020 2029 0a20 2020 2069 6e74 6572 6163     ).    interac
-00018b80: 7469 6f6e 3a20 496e 7465 7261 6374 696f  tion: Interactio
-00018b90: 6e20 3d20 7072 6f74 6f2e 4669 656c 6428  n = proto.Field(
-00018ba0: 0a20 2020 2020 2020 2070 726f 746f 2e45  .        proto.E
-00018bb0: 4e55 4d2c 0a20 2020 2020 2020 206e 756d  NUM,.        num
-00018bc0: 6265 723d 352c 0a20 2020 2020 2020 2065  ber=5,.        e
-00018bd0: 6e75 6d3d 496e 7465 7261 6374 696f 6e2c  num=Interaction,
-00018be0: 0a20 2020 2029 0a0a 0a5f 5f61 6c6c 5f5f  .    )...__all__
-00018bf0: 203d 2074 7570 6c65 2873 6f72 7465 6428   = tuple(sorted(
-00018c00: 5f5f 7072 6f74 6f62 7566 5f5f 2e6d 616e  __protobuf__.man
-00018c10: 6966 6573 7429 290a                      ifest)).
+00007650: 3d22 4465 636f 7261 7465 6454 6578 7422  ="DecoratedText"
+00007660: 2c0a 2020 2020 290a 2020 2020 6275 7474  ,.    ).    butt
+00007670: 6f6e 5f6c 6973 743a 2022 4275 7474 6f6e  on_list: "Button
+00007680: 4c69 7374 2220 3d20 7072 6f74 6f2e 4669  List" = proto.Fi
+00007690: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
+000076a0: 746f 2e4d 4553 5341 4745 2c0a 2020 2020  to.MESSAGE,.    
+000076b0: 2020 2020 6e75 6d62 6572 3d34 2c0a 2020      number=4,.  
+000076c0: 2020 2020 2020 6f6e 656f 663d 2264 6174        oneof="dat
+000076d0: 6122 2c0a 2020 2020 2020 2020 6d65 7373  a",.        mess
+000076e0: 6167 653d 2242 7574 746f 6e4c 6973 7422  age="ButtonList"
+000076f0: 2c0a 2020 2020 290a 2020 2020 7465 7874  ,.    ).    text
+00007700: 5f69 6e70 7574 3a20 2254 6578 7449 6e70  _input: "TextInp
+00007710: 7574 2220 3d20 7072 6f74 6f2e 4669 656c  ut" = proto.Fiel
+00007720: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
+00007730: 2e4d 4553 5341 4745 2c0a 2020 2020 2020  .MESSAGE,.      
+00007740: 2020 6e75 6d62 6572 3d35 2c0a 2020 2020    number=5,.    
+00007750: 2020 2020 6f6e 656f 663d 2264 6174 6122      oneof="data"
+00007760: 2c0a 2020 2020 2020 2020 6d65 7373 6167  ,.        messag
+00007770: 653d 2254 6578 7449 6e70 7574 222c 0a20  e="TextInput",. 
+00007780: 2020 2029 0a20 2020 2073 656c 6563 7469     ).    selecti
+00007790: 6f6e 5f69 6e70 7574 3a20 2253 656c 6563  on_input: "Selec
+000077a0: 7469 6f6e 496e 7075 7422 203d 2070 726f  tionInput" = pro
+000077b0: 746f 2e46 6965 6c64 280a 2020 2020 2020  to.Field(.      
+000077c0: 2020 7072 6f74 6f2e 4d45 5353 4147 452c    proto.MESSAGE,
+000077d0: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
+000077e0: 362c 0a20 2020 2020 2020 206f 6e65 6f66  6,.        oneof
+000077f0: 3d22 6461 7461 222c 0a20 2020 2020 2020  ="data",.       
+00007800: 206d 6573 7361 6765 3d22 5365 6c65 6374   message="Select
+00007810: 696f 6e49 6e70 7574 222c 0a20 2020 2029  ionInput",.    )
+00007820: 0a20 2020 2064 6174 655f 7469 6d65 5f70  .    date_time_p
+00007830: 6963 6b65 723a 2022 4461 7465 5469 6d65  icker: "DateTime
+00007840: 5069 636b 6572 2220 3d20 7072 6f74 6f2e  Picker" = proto.
+00007850: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
+00007860: 726f 746f 2e4d 4553 5341 4745 2c0a 2020  roto.MESSAGE,.  
+00007870: 2020 2020 2020 6e75 6d62 6572 3d37 2c0a        number=7,.
+00007880: 2020 2020 2020 2020 6f6e 656f 663d 2264          oneof="d
+00007890: 6174 6122 2c0a 2020 2020 2020 2020 6d65  ata",.        me
+000078a0: 7373 6167 653d 2244 6174 6554 696d 6550  ssage="DateTimeP
+000078b0: 6963 6b65 7222 2c0a 2020 2020 290a 2020  icker",.    ).  
+000078c0: 2020 6469 7669 6465 723a 2022 4469 7669    divider: "Divi
+000078d0: 6465 7222 203d 2070 726f 746f 2e46 6965  der" = proto.Fie
+000078e0: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
+000078f0: 6f2e 4d45 5353 4147 452c 0a20 2020 2020  o.MESSAGE,.     
+00007900: 2020 206e 756d 6265 723d 392c 0a20 2020     number=9,.   
+00007910: 2020 2020 206f 6e65 6f66 3d22 6461 7461       oneof="data
+00007920: 222c 0a20 2020 2020 2020 206d 6573 7361  ",.        messa
+00007930: 6765 3d22 4469 7669 6465 7222 2c0a 2020  ge="Divider",.  
+00007940: 2020 290a 2020 2020 6772 6964 3a20 2247    ).    grid: "G
+00007950: 7269 6422 203d 2070 726f 746f 2e46 6965  rid" = proto.Fie
+00007960: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
+00007970: 6f2e 4d45 5353 4147 452c 0a20 2020 2020  o.MESSAGE,.     
+00007980: 2020 206e 756d 6265 723d 3130 2c0a 2020     number=10,.  
+00007990: 2020 2020 2020 6f6e 656f 663d 2264 6174        oneof="dat
+000079a0: 6122 2c0a 2020 2020 2020 2020 6d65 7373  a",.        mess
+000079b0: 6167 653d 2247 7269 6422 2c0a 2020 2020  age="Grid",.    
+000079c0: 290a 2020 2020 636f 6c75 6d6e 733a 2022  ).    columns: "
+000079d0: 436f 6c75 6d6e 7322 203d 2070 726f 746f  Columns" = proto
+000079e0: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
+000079f0: 7072 6f74 6f2e 4d45 5353 4147 452c 0a20  proto.MESSAGE,. 
+00007a00: 2020 2020 2020 206e 756d 6265 723d 3131         number=11
+00007a10: 2c0a 2020 2020 2020 2020 6f6e 656f 663d  ,.        oneof=
+00007a20: 2264 6174 6122 2c0a 2020 2020 2020 2020  "data",.        
+00007a30: 6d65 7373 6167 653d 2243 6f6c 756d 6e73  message="Columns
+00007a40: 222c 0a20 2020 2029 0a20 2020 2068 6f72  ",.    ).    hor
+00007a50: 697a 6f6e 7461 6c5f 616c 6967 6e6d 656e  izontal_alignmen
+00007a60: 743a 2048 6f72 697a 6f6e 7461 6c41 6c69  t: HorizontalAli
+00007a70: 676e 6d65 6e74 203d 2070 726f 746f 2e46  gnment = proto.F
+00007a80: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
+00007a90: 6f74 6f2e 454e 554d 2c0a 2020 2020 2020  oto.ENUM,.      
+00007aa0: 2020 6e75 6d62 6572 3d38 2c0a 2020 2020    number=8,.    
+00007ab0: 2020 2020 656e 756d 3d48 6f72 697a 6f6e      enum=Horizon
+00007ac0: 7461 6c41 6c69 676e 6d65 6e74 2c0a 2020  talAlignment,.  
+00007ad0: 2020 290a 0a0a 636c 6173 7320 5465 7874    )...class Text
+00007ae0: 5061 7261 6772 6170 6828 7072 6f74 6f2e  Paragraph(proto.
+00007af0: 4d65 7373 6167 6529 3a0a 2020 2020 7222  Message):.    r"
+00007b00: 2222 4120 7061 7261 6772 6170 6820 6f66  ""A paragraph of
+00007b10: 2074 6578 7420 7468 6174 2073 7570 706f   text that suppo
+00007b20: 7274 7320 666f 726d 6174 7469 6e67 2e20  rts formatting. 
+00007b30: 466f 7220 616e 2065 7861 6d70 6c65 2069  For an example i
+00007b40: 6e0a 2020 2020 476f 6f67 6c65 2043 6861  n.    Google Cha
+00007b50: 7420 6170 7073 2c20 7365 6520 6041 6464  t apps, see `Add
+00007b60: 2061 2070 6172 6167 7261 7068 206f 6620   a paragraph of 
+00007b70: 666f 726d 6174 7465 640a 2020 2020 7465  formatted.    te
+00007b80: 7874 203c 6874 7470 733a 2f2f 6465 7665  xt <https://deve
+00007b90: 6c6f 7065 7273 2e67 6f6f 676c 652e 636f  lopers.google.co
+00007ba0: 6d2f 776f 726b 7370 6163 652f 6368 6174  m/workspace/chat
+00007bb0: 2f61 6464 2d74 6578 742d 696d 6167 652d  /add-text-image-
+00007bc0: 6361 7264 2d64 6961 6c6f 6723 6164 645f  card-dialog#add_
+00007bd0: 615f 7061 7261 6772 6170 685f 6f66 5f66  a_paragraph_of_f
+00007be0: 6f72 6d61 7474 6564 5f74 6578 743e 605f  ormatted_text>`_
+00007bf0: 5f2e 0a20 2020 2046 6f72 206d 6f72 6520  _..    For more 
+00007c00: 696e 666f 726d 6174 696f 6e20 6162 6f75  information abou
+00007c10: 7420 666f 726d 6174 7469 6e67 2074 6578  t formatting tex
+00007c20: 742c 2073 6565 2060 466f 726d 6174 7469  t, see `Formatti
+00007c30: 6e67 2074 6578 7420 696e 0a20 2020 2047  ng text in.    G
+00007c40: 6f6f 676c 6520 4368 6174 0a20 2020 2061  oogle Chat.    a
+00007c50: 7070 7320 3c68 7474 7073 3a2f 2f64 6576  pps <https://dev
+00007c60: 656c 6f70 6572 732e 676f 6f67 6c65 2e63  elopers.google.c
+00007c70: 6f6d 2f77 6f72 6b73 7061 6365 2f63 6861  om/workspace/cha
+00007c80: 742f 666f 726d 6174 2d6d 6573 7361 6765  t/format-message
+00007c90: 7323 6361 7264 2d66 6f72 6d61 7474 696e  s#card-formattin
+00007ca0: 673e 605f 5f0a 2020 2020 616e 6420 6046  g>`__.    and `F
+00007cb0: 6f72 6d61 7474 696e 6720 7465 7874 2069  ormatting text i
+00007cc0: 6e20 476f 6f67 6c65 2057 6f72 6b73 7061  n Google Workspa
+00007cd0: 6365 0a20 2020 2041 6464 2d6f 6e73 203c  ce.    Add-ons <
+00007ce0: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
+00007cf0: 7273 2e67 6f6f 676c 652e 636f 6d2f 6170  rs.google.com/ap
+00007d00: 7073 2d73 6372 6970 742f 6164 642d 6f6e  ps-script/add-on
+00007d10: 732f 636f 6e63 6570 7473 2f77 6964 6765  s/concepts/widge
+00007d20: 7473 2374 6578 745f 666f 726d 6174 7469  ts#text_formatti
+00007d30: 6e67 3e60 5f5f 2e0a 0a20 2020 2060 476f  ng>`__...    `Go
+00007d40: 6f67 6c65 2057 6f72 6b73 7061 6365 2041  ogle Workspace A
+00007d50: 6464 2d6f 6e73 2061 6e64 2043 6861 740a  dd-ons and Chat.
+00007d60: 2020 2020 6170 7073 203c 6874 7470 733a      apps <https:
+00007d70: 2f2f 6465 7665 6c6f 7065 7273 2e67 6f6f  //developers.goo
+00007d80: 676c 652e 636f 6d2f 776f 726b 7370 6163  gle.com/workspac
+00007d90: 652f 6578 7465 6e64 3e60 5f5f 3a0a 0a20  e/extend>`__:.. 
+00007da0: 2020 2041 7474 7269 6275 7465 733a 0a20     Attributes:. 
+00007db0: 2020 2020 2020 2074 6578 7420 2873 7472         text (str
+00007dc0: 293a 0a20 2020 2020 2020 2020 2020 2054  ):.            T
+00007dd0: 6865 2074 6578 7420 7468 6174 2773 2073  he text that's s
+00007de0: 686f 776e 2069 6e20 7468 6520 7769 6467  hown in the widg
+00007df0: 6574 2e0a 2020 2020 2222 220a 0a20 2020  et..    """..   
+00007e00: 2074 6578 743a 2073 7472 203d 2070 726f   text: str = pro
+00007e10: 746f 2e46 6965 6c64 280a 2020 2020 2020  to.Field(.      
+00007e20: 2020 7072 6f74 6f2e 5354 5249 4e47 2c0a    proto.STRING,.
+00007e30: 2020 2020 2020 2020 6e75 6d62 6572 3d31          number=1
+00007e40: 2c0a 2020 2020 290a 0a0a 636c 6173 7320  ,.    )...class 
+00007e50: 496d 6167 6528 7072 6f74 6f2e 4d65 7373  Image(proto.Mess
+00007e60: 6167 6529 3a0a 2020 2020 7222 2222 416e  age):.    r"""An
+00007e70: 2069 6d61 6765 2074 6861 7420 6973 2073   image that is s
+00007e80: 7065 6369 6669 6564 2062 7920 6120 5552  pecified by a UR
+00007e90: 4c20 616e 6420 6361 6e20 6861 7665 2061  L and can have a
+00007ea0: 6e20 6060 6f6e 436c 6963 6b60 600a 2020  n ``onClick``.  
+00007eb0: 2020 6163 7469 6f6e 2e20 466f 7220 616e    action. For an
+00007ec0: 2065 7861 6d70 6c65 2c20 7365 6520 6041   example, see `A
+00007ed0: 6464 2061 6e0a 2020 2020 696d 6167 6520  dd an.    image 
+00007ee0: 3c68 7474 7073 3a2f 2f64 6576 656c 6f70  <https://develop
+00007ef0: 6572 732e 676f 6f67 6c65 2e63 6f6d 2f77  ers.google.com/w
+00007f00: 6f72 6b73 7061 6365 2f63 6861 742f 6164  orkspace/chat/ad
+00007f10: 642d 7465 7874 2d69 6d61 6765 2d63 6172  d-text-image-car
+00007f20: 642d 6469 616c 6f67 2361 6464 5f61 6e5f  d-dialog#add_an_
+00007f30: 696d 6167 653e 605f 5f2e 0a0a 2020 2020  image>`__...    
+00007f40: 6047 6f6f 676c 6520 576f 726b 7370 6163  `Google Workspac
+00007f50: 6520 4164 642d 6f6e 7320 616e 6420 4368  e Add-ons and Ch
+00007f60: 6174 0a20 2020 2061 7070 7320 3c68 7474  at.    apps <htt
+00007f70: 7073 3a2f 2f64 6576 656c 6f70 6572 732e  ps://developers.
+00007f80: 676f 6f67 6c65 2e63 6f6d 2f77 6f72 6b73  google.com/works
+00007f90: 7061 6365 2f65 7874 656e 643e 605f 5f3a  pace/extend>`__:
+00007fa0: 0a0a 2020 2020 4174 7472 6962 7574 6573  ..    Attributes
+00007fb0: 3a0a 2020 2020 2020 2020 696d 6167 655f  :.        image_
+00007fc0: 7572 6c20 2873 7472 293a 0a20 2020 2020  url (str):.     
+00007fd0: 2020 2020 2020 2054 6865 2048 5454 5053         The HTTPS
+00007fe0: 2055 524c 2074 6861 7420 686f 7374 7320   URL that hosts 
+00007ff0: 7468 6520 696d 6167 652e 0a0a 2020 2020  the image...    
+00008000: 2020 2020 2020 2020 466f 7220 6578 616d          For exam
+00008010: 706c 653a 0a0a 2020 2020 2020 2020 2020  ple:..          
+00008020: 2020 3a3a 0a0a 2020 2020 2020 2020 2020    ::..          
+00008030: 2020 2020 2068 7474 7073 3a2f 2f64 6576       https://dev
+00008040: 656c 6f70 6572 732e 676f 6f67 6c65 2e63  elopers.google.c
+00008050: 6f6d 2f77 6f72 6b73 7061 6365 2f63 6861  om/workspace/cha
+00008060: 742f 696d 6167 6573 2f71 7569 636b 7374  t/images/quickst
+00008070: 6172 742d 6170 702d 6176 6174 6172 2e70  art-app-avatar.p
+00008080: 6e67 0a20 2020 2020 2020 206f 6e5f 636c  ng.        on_cl
+00008090: 6963 6b20 2867 6f6f 676c 652e 6170 7073  ick (google.apps
+000080a0: 2e63 6172 645f 7631 2e74 7970 6573 2e4f  .card_v1.types.O
+000080b0: 6e43 6c69 636b 293a 0a20 2020 2020 2020  nClick):.       
+000080c0: 2020 2020 2057 6865 6e20 6120 7573 6572       When a user
+000080d0: 2063 6c69 636b 7320 7468 6520 696d 6167   clicks the imag
+000080e0: 652c 2074 6865 2063 6c69 636b 0a20 2020  e, the click.   
+000080f0: 2020 2020 2020 2020 2074 7269 6767 6572           trigger
+00008100: 7320 7468 6973 2061 6374 696f 6e2e 0a20  s this action.. 
+00008110: 2020 2020 2020 2061 6c74 5f74 6578 7420         alt_text 
+00008120: 2873 7472 293a 0a20 2020 2020 2020 2020  (str):.         
+00008130: 2020 2054 6865 2061 6c74 6572 6e61 7469     The alternati
+00008140: 7665 2074 6578 7420 6f66 2074 6869 7320  ve text of this 
+00008150: 696d 6167 6520 7468 6174 2773 0a20 2020  image that's.   
+00008160: 2020 2020 2020 2020 2075 7365 6420 666f           used fo
+00008170: 7220 6163 6365 7373 6962 696c 6974 792e  r accessibility.
+00008180: 0a20 2020 2022 2222 0a0a 2020 2020 696d  .    """..    im
+00008190: 6167 655f 7572 6c3a 2073 7472 203d 2070  age_url: str = p
+000081a0: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
+000081b0: 2020 2020 7072 6f74 6f2e 5354 5249 4e47      proto.STRING
+000081c0: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
+000081d0: 3d31 2c0a 2020 2020 290a 2020 2020 6f6e  =1,.    ).    on
+000081e0: 5f63 6c69 636b 3a20 224f 6e43 6c69 636b  _click: "OnClick
+000081f0: 2220 3d20 7072 6f74 6f2e 4669 656c 6428  " = proto.Field(
+00008200: 0a20 2020 2020 2020 2070 726f 746f 2e4d  .        proto.M
+00008210: 4553 5341 4745 2c0a 2020 2020 2020 2020  ESSAGE,.        
+00008220: 6e75 6d62 6572 3d32 2c0a 2020 2020 2020  number=2,.      
+00008230: 2020 6d65 7373 6167 653d 224f 6e43 6c69    message="OnCli
+00008240: 636b 222c 0a20 2020 2029 0a20 2020 2061  ck",.    ).    a
+00008250: 6c74 5f74 6578 743a 2073 7472 203d 2070  lt_text: str = p
+00008260: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
+00008270: 2020 2020 7072 6f74 6f2e 5354 5249 4e47      proto.STRING
+00008280: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
+00008290: 3d33 2c0a 2020 2020 290a 0a0a 636c 6173  =3,.    )...clas
+000082a0: 7320 4469 7669 6465 7228 7072 6f74 6f2e  s Divider(proto.
+000082b0: 4d65 7373 6167 6529 3a0a 2020 2020 7222  Message):.    r"
+000082c0: 2222 4469 7370 6c61 7973 2061 2064 6976  ""Displays a div
+000082d0: 6964 6572 2062 6574 7765 656e 2077 6964  ider between wid
+000082e0: 6765 7473 2061 7320 6120 686f 7269 7a6f  gets as a horizo
+000082f0: 6e74 616c 206c 696e 652e 2046 6f72 2061  ntal line. For a
+00008300: 6e0a 2020 2020 6578 616d 706c 6520 696e  n.    example in
+00008310: 2047 6f6f 676c 6520 4368 6174 2061 7070   Google Chat app
+00008320: 732c 2073 6565 2060 4164 6420 6120 686f  s, see `Add a ho
+00008330: 7269 7a6f 6e74 616c 2064 6976 6964 6572  rizontal divider
+00008340: 2062 6574 7765 656e 0a20 2020 2077 6964   between.    wid
+00008350: 6765 7473 203c 6874 7470 733a 2f2f 6465  gets <https://de
+00008360: 7665 6c6f 7065 7273 2e67 6f6f 676c 652e  velopers.google.
+00008370: 636f 6d2f 776f 726b 7370 6163 652f 6368  com/workspace/ch
+00008380: 6174 2f66 6f72 6d61 742d 7374 7275 6374  at/format-struct
+00008390: 7572 652d 6361 7264 2d64 6961 6c6f 6723  ure-card-dialog#
+000083a0: 6164 645f 615f 686f 7269 7a6f 6e74 616c  add_a_horizontal
+000083b0: 5f64 6976 6964 6572 5f62 6574 7765 656e  _divider_between
+000083c0: 5f77 6964 6765 7473 3e60 5f5f 2e0a 0a20  _widgets>`__... 
+000083d0: 2020 2060 476f 6f67 6c65 2057 6f72 6b73     `Google Works
+000083e0: 7061 6365 2041 6464 2d6f 6e73 2061 6e64  pace Add-ons and
+000083f0: 2043 6861 740a 2020 2020 6170 7073 203c   Chat.    apps <
+00008400: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
+00008410: 7273 2e67 6f6f 676c 652e 636f 6d2f 776f  rs.google.com/wo
+00008420: 726b 7370 6163 652f 6578 7465 6e64 3e60  rkspace/extend>`
+00008430: 5f5f 3a0a 0a20 2020 2046 6f72 2065 7861  __:..    For exa
+00008440: 6d70 6c65 2c20 7468 6520 666f 6c6c 6f77  mple, the follow
+00008450: 696e 6720 4a53 4f4e 2063 7265 6174 6573  ing JSON creates
+00008460: 2061 2064 6976 6964 6572 3a0a 0a20 2020   a divider:..   
+00008470: 203a 3a0a 0a20 2020 2020 2020 2264 6976   ::..       "div
+00008480: 6964 6572 223a 207b 7d0a 0a20 2020 2022  ider": {}..    "
+00008490: 2222 0a0a 0a63 6c61 7373 2044 6563 6f72  ""...class Decor
+000084a0: 6174 6564 5465 7874 2870 726f 746f 2e4d  atedText(proto.M
+000084b0: 6573 7361 6765 293a 0a20 2020 2072 2222  essage):.    r""
+000084c0: 2241 2077 6964 6765 7420 7468 6174 2064  "A widget that d
+000084d0: 6973 706c 6179 7320 7465 7874 2077 6974  isplays text wit
+000084e0: 6820 6f70 7469 6f6e 616c 2064 6563 6f72  h optional decor
+000084f0: 6174 696f 6e73 2073 7563 6820 6173 2061  ations such as a
+00008500: 0a20 2020 206c 6162 656c 2061 626f 7665  .    label above
+00008510: 206f 7220 6265 6c6f 7720 7468 6520 7465   or below the te
+00008520: 7874 2c20 616e 2069 636f 6e20 696e 2066  xt, an icon in f
+00008530: 726f 6e74 206f 6620 7468 6520 7465 7874  ront of the text
+00008540: 2c20 610a 2020 2020 7365 6c65 6374 696f  , a.    selectio
+00008550: 6e20 7769 6467 6574 2c20 6f72 2061 2062  n widget, or a b
+00008560: 7574 746f 6e20 6166 7465 7220 7468 6520  utton after the 
+00008570: 7465 7874 2e20 466f 7220 616e 2065 7861  text. For an exa
+00008580: 6d70 6c65 2069 6e0a 2020 2020 476f 6f67  mple in.    Goog
+00008590: 6c65 2043 6861 7420 6170 7073 2c20 7365  le Chat apps, se
+000085a0: 6520 6044 6973 706c 6179 2074 6578 7420  e `Display text 
+000085b0: 7769 7468 2064 6563 6f72 6174 6976 650a  with decorative.
+000085c0: 2020 2020 7465 7874 203c 6874 7470 733a      text <https:
+000085d0: 2f2f 6465 7665 6c6f 7065 7273 2e67 6f6f  //developers.goo
+000085e0: 676c 652e 636f 6d2f 776f 726b 7370 6163  gle.com/workspac
+000085f0: 652f 6368 6174 2f61 6464 2d74 6578 742d  e/chat/add-text-
+00008600: 696d 6167 652d 6361 7264 2d64 6961 6c6f  image-card-dialo
+00008610: 6723 6469 7370 6c61 795f 7465 7874 5f77  g#display_text_w
+00008620: 6974 685f 6465 636f 7261 7469 7665 5f65  ith_decorative_e
+00008630: 6c65 6d65 6e74 733e 605f 5f2e 0a0a 2020  lements>`__...  
+00008640: 2020 6047 6f6f 676c 6520 576f 726b 7370    `Google Worksp
+00008650: 6163 6520 4164 642d 6f6e 7320 616e 6420  ace Add-ons and 
+00008660: 4368 6174 0a20 2020 2061 7070 7320 3c68  Chat.    apps <h
+00008670: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
+00008680: 732e 676f 6f67 6c65 2e63 6f6d 2f77 6f72  s.google.com/wor
+00008690: 6b73 7061 6365 2f65 7874 656e 643e 605f  kspace/extend>`_
+000086a0: 5f3a 0a0a 2020 2020 5468 6973 206d 6573  _:..    This mes
+000086b0: 7361 6765 2068 6173 2060 6f6e 656f 6660  sage has `oneof`
+000086c0: 5f20 6669 656c 6473 2028 6d75 7475 616c  _ fields (mutual
+000086d0: 6c79 2065 7863 6c75 7369 7665 2066 6965  ly exclusive fie
+000086e0: 6c64 7329 2e0a 2020 2020 466f 7220 6561  lds)..    For ea
+000086f0: 6368 206f 6e65 6f66 2c20 6174 206d 6f73  ch oneof, at mos
+00008700: 7420 6f6e 6520 6d65 6d62 6572 2066 6965  t one member fie
+00008710: 6c64 2063 616e 2062 6520 7365 7420 6174  ld can be set at
+00008720: 2074 6865 2073 616d 6520 7469 6d65 2e0a   the same time..
+00008730: 2020 2020 5365 7474 696e 6720 616e 7920      Setting any 
+00008740: 6d65 6d62 6572 206f 6620 7468 6520 6f6e  member of the on
+00008750: 656f 6620 6175 746f 6d61 7469 6361 6c6c  eof automaticall
+00008760: 7920 636c 6561 7273 2061 6c6c 206f 7468  y clears all oth
+00008770: 6572 0a20 2020 206d 656d 6265 7273 2e0a  er.    members..
+00008780: 0a20 2020 202e 2e20 5f6f 6e65 6f66 3a20  .    .. _oneof: 
+00008790: 6874 7470 733a 2f2f 7072 6f74 6f2d 706c  https://proto-pl
+000087a0: 7573 2d70 7974 686f 6e2e 7265 6164 7468  us-python.readth
+000087b0: 6564 6f63 732e 696f 2f65 6e2f 7374 6162  edocs.io/en/stab
+000087c0: 6c65 2f66 6965 6c64 732e 6874 6d6c 236f  le/fields.html#o
+000087d0: 6e65 6f66 732d 6d75 7475 616c 6c79 2d65  neofs-mutually-e
+000087e0: 7863 6c75 7369 7665 2d66 6965 6c64 730a  xclusive-fields.
+000087f0: 0a20 2020 2041 7474 7269 6275 7465 733a  .    Attributes:
+00008800: 0a20 2020 2020 2020 2069 636f 6e20 2867  .        icon (g
+00008810: 6f6f 676c 652e 6170 7073 2e63 6172 645f  oogle.apps.card_
+00008820: 7631 2e74 7970 6573 2e49 636f 6e29 3a0a  v1.types.Icon):.
+00008830: 2020 2020 2020 2020 2020 2020 4465 7072              Depr
+00008840: 6563 6174 6564 2069 6e20 6661 766f 7220  ecated in favor 
+00008850: 6f66 2060 6073 7461 7274 4963 6f6e 6060  of ``startIcon``
+00008860: 2e0a 2020 2020 2020 2020 7374 6172 745f  ..        start_
+00008870: 6963 6f6e 2028 676f 6f67 6c65 2e61 7070  icon (google.app
+00008880: 732e 6361 7264 5f76 312e 7479 7065 732e  s.card_v1.types.
+00008890: 4963 6f6e 293a 0a20 2020 2020 2020 2020  Icon):.         
+000088a0: 2020 2054 6865 2069 636f 6e20 6469 7370     The icon disp
+000088b0: 6c61 7965 6420 696e 2066 726f 6e74 206f  layed in front o
+000088c0: 6620 7468 6520 7465 7874 2e0a 2020 2020  f the text..    
+000088d0: 2020 2020 746f 705f 6c61 6265 6c20 2873      top_label (s
+000088e0: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
+000088f0: 2054 6865 2074 6578 7420 7468 6174 2061   The text that a
+00008900: 7070 6561 7273 2061 626f 7665 2060 6074  ppears above ``t
+00008910: 6578 7460 602e 2041 6c77 6179 7320 7472  ext``. Always tr
+00008920: 756e 6361 7465 732e 0a20 2020 2020 2020  uncates..       
+00008930: 2074 6578 7420 2873 7472 293a 0a20 2020   text (str):.   
+00008940: 2020 2020 2020 2020 2052 6571 7569 7265           Require
+00008950: 642e 2054 6865 2070 7269 6d61 7279 2074  d. The primary t
+00008960: 6578 742e 0a0a 2020 2020 2020 2020 2020  ext...          
+00008970: 2020 5375 7070 6f72 7473 2073 696d 706c    Supports simpl
+00008980: 6520 666f 726d 6174 7469 6e67 2e20 466f  e formatting. Fo
+00008990: 7220 6d6f 7265 2069 6e66 6f72 6d61 7469  r more informati
+000089a0: 6f6e 2061 626f 7574 0a20 2020 2020 2020  on about.       
+000089b0: 2020 2020 2066 6f72 6d61 7474 696e 6720       formatting 
+000089c0: 7465 7874 2c20 7365 6520 6046 6f72 6d61  text, see `Forma
+000089d0: 7474 696e 6720 7465 7874 2069 6e20 476f  tting text in Go
+000089e0: 6f67 6c65 2043 6861 740a 2020 2020 2020  ogle Chat.      
+000089f0: 2020 2020 2020 6170 7073 203c 6874 7470        apps <http
+00008a00: 733a 2f2f 6465 7665 6c6f 7065 7273 2e67  s://developers.g
+00008a10: 6f6f 676c 652e 636f 6d2f 776f 726b 7370  oogle.com/worksp
+00008a20: 6163 652f 6368 6174 2f66 6f72 6d61 742d  ace/chat/format-
+00008a30: 6d65 7373 6167 6573 2363 6172 642d 666f  messages#card-fo
+00008a40: 726d 6174 7469 6e67 3e60 5f5f 0a20 2020  rmatting>`__.   
+00008a50: 2020 2020 2020 2020 2061 6e64 2060 466f           and `Fo
+00008a60: 726d 6174 7469 6e67 2074 6578 7420 696e  rmatting text in
+00008a70: 2047 6f6f 676c 6520 576f 726b 7370 6163   Google Workspac
+00008a80: 650a 2020 2020 2020 2020 2020 2020 4164  e.            Ad
+00008a90: 642d 6f6e 7320 3c68 7474 7073 3a2f 2f64  d-ons <https://d
+00008aa0: 6576 656c 6f70 6572 732e 676f 6f67 6c65  evelopers.google
+00008ab0: 2e63 6f6d 2f61 7070 732d 7363 7269 7074  .com/apps-script
+00008ac0: 2f61 6464 2d6f 6e73 2f63 6f6e 6365 7074  /add-ons/concept
+00008ad0: 732f 7769 6467 6574 7323 7465 7874 5f66  s/widgets#text_f
+00008ae0: 6f72 6d61 7474 696e 673e 605f 5f2e 0a20  ormatting>`__.. 
+00008af0: 2020 2020 2020 2077 7261 705f 7465 7874         wrap_text
+00008b00: 2028 626f 6f6c 293a 0a20 2020 2020 2020   (bool):.       
+00008b10: 2020 2020 2054 6865 2077 7261 7020 7465       The wrap te
+00008b20: 7874 2073 6574 7469 6e67 2e20 4966 2060  xt setting. If `
+00008b30: 6074 7275 6560 602c 2074 6865 2074 6578  `true``, the tex
+00008b40: 7420 7772 6170 7320 616e 640a 2020 2020  t wraps and.    
+00008b50: 2020 2020 2020 2020 6469 7370 6c61 7973          displays
+00008b60: 206f 6e20 6d75 6c74 6970 6c65 206c 696e   on multiple lin
+00008b70: 6573 2e20 4f74 6865 7277 6973 652c 2074  es. Otherwise, t
+00008b80: 6865 2074 6578 7420 6973 0a20 2020 2020  he text is.     
+00008b90: 2020 2020 2020 2074 7275 6e63 6174 6564         truncated
+00008ba0: 2e0a 0a20 2020 2020 2020 2020 2020 204f  ...            O
+00008bb0: 6e6c 7920 6170 706c 6965 7320 746f 2060  nly applies to `
+00008bc0: 6074 6578 7460 602c 206e 6f74 2060 6074  `text``, not ``t
+00008bd0: 6f70 4c61 6265 6c60 6020 616e 640a 2020  opLabel`` and.  
+00008be0: 2020 2020 2020 2020 2020 6060 626f 7474            ``bott
+00008bf0: 6f6d 4c61 6265 6c60 602e 0a20 2020 2020  omLabel``..     
+00008c00: 2020 2062 6f74 746f 6d5f 6c61 6265 6c20     bottom_label 
+00008c10: 2873 7472 293a 0a20 2020 2020 2020 2020  (str):.         
+00008c20: 2020 2054 6865 2074 6578 7420 7468 6174     The text that
+00008c30: 2061 7070 6561 7273 2062 656c 6f77 2060   appears below `
+00008c40: 6074 6578 7460 602e 2041 6c77 6179 7320  `text``. Always 
+00008c50: 7772 6170 732e 0a20 2020 2020 2020 206f  wraps..        o
+00008c60: 6e5f 636c 6963 6b20 2867 6f6f 676c 652e  n_click (google.
+00008c70: 6170 7073 2e63 6172 645f 7631 2e74 7970  apps.card_v1.typ
+00008c80: 6573 2e4f 6e43 6c69 636b 293a 0a20 2020  es.OnClick):.   
+00008c90: 2020 2020 2020 2020 2054 6869 7320 6163           This ac
+00008ca0: 7469 6f6e 2069 7320 7472 6967 6765 7265  tion is triggere
+00008cb0: 6420 7768 656e 2075 7365 7273 2063 6c69  d when users cli
+00008cc0: 636b 2060 6074 6f70 4c61 6265 6c60 6020  ck ``topLabel`` 
+00008cd0: 6f72 0a20 2020 2020 2020 2020 2020 2060  or.            `
+00008ce0: 6062 6f74 746f 6d4c 6162 656c 6060 2e0a  `bottomLabel``..
+00008cf0: 2020 2020 2020 2020 6275 7474 6f6e 2028          button (
+00008d00: 676f 6f67 6c65 2e61 7070 732e 6361 7264  google.apps.card
+00008d10: 5f76 312e 7479 7065 732e 4275 7474 6f6e  _v1.types.Button
+00008d20: 293a 0a20 2020 2020 2020 2020 2020 2041  ):.            A
+00008d30: 2062 7574 746f 6e20 7468 6174 2061 2075   button that a u
+00008d40: 7365 7220 6361 6e20 636c 6963 6b20 746f  ser can click to
+00008d50: 2074 7269 6767 6572 2061 6e0a 2020 2020   trigger an.    
+00008d60: 2020 2020 2020 2020 6163 7469 6f6e 2e0a          action..
+00008d70: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
+00008d80: 7320 6669 656c 6420 6973 2061 206d 656d  s field is a mem
+00008d90: 6265 7220 6f66 2060 6f6e 656f 6660 5f20  ber of `oneof`_ 
+00008da0: 6060 636f 6e74 726f 6c60 602e 0a20 2020  ``control``..   
+00008db0: 2020 2020 2073 7769 7463 685f 636f 6e74       switch_cont
+00008dc0: 726f 6c20 2867 6f6f 676c 652e 6170 7073  rol (google.apps
+00008dd0: 2e63 6172 645f 7631 2e74 7970 6573 2e44  .card_v1.types.D
+00008de0: 6563 6f72 6174 6564 5465 7874 2e53 7769  ecoratedText.Swi
+00008df0: 7463 6843 6f6e 7472 6f6c 293a 0a20 2020  tchControl):.   
+00008e00: 2020 2020 2020 2020 2041 2073 7769 7463           A switc
+00008e10: 6820 7769 6467 6574 2074 6861 7420 6120  h widget that a 
+00008e20: 7573 6572 2063 616e 2063 6c69 636b 2074  user can click t
+00008e30: 6f0a 2020 2020 2020 2020 2020 2020 6368  o.            ch
+00008e40: 616e 6765 2069 7473 2073 7461 7465 2061  ange its state a
+00008e50: 6e64 2074 7269 6767 6572 2061 6e20 6163  nd trigger an ac
+00008e60: 7469 6f6e 2e0a 0a20 2020 2020 2020 2020  tion...         
+00008e70: 2020 2054 6869 7320 6669 656c 6420 6973     This field is
+00008e80: 2061 206d 656d 6265 7220 6f66 2060 6f6e   a member of `on
+00008e90: 656f 6660 5f20 6060 636f 6e74 726f 6c60  eof`_ ``control`
+00008ea0: 602e 0a20 2020 2020 2020 2065 6e64 5f69  `..        end_i
+00008eb0: 636f 6e20 2867 6f6f 676c 652e 6170 7073  con (google.apps
+00008ec0: 2e63 6172 645f 7631 2e74 7970 6573 2e49  .card_v1.types.I
+00008ed0: 636f 6e29 3a0a 2020 2020 2020 2020 2020  con):.          
+00008ee0: 2020 416e 2069 636f 6e20 6469 7370 6c61    An icon displa
+00008ef0: 7965 6420 6166 7465 7220 7468 6520 7465  yed after the te
+00008f00: 7874 2e0a 0a20 2020 2020 2020 2020 2020  xt...           
+00008f10: 2053 7570 706f 7274 730a 2020 2020 2020   Supports.      
+00008f20: 2020 2020 2020 6062 7569 6c74 2d69 6e20        `built-in 
+00008f30: 3c68 7474 7073 3a2f 2f64 6576 656c 6f70  <https://develop
+00008f40: 6572 732e 676f 6f67 6c65 2e63 6f6d 2f77  ers.google.com/w
+00008f50: 6f72 6b73 7061 6365 2f63 6861 742f 666f  orkspace/chat/fo
+00008f60: 726d 6174 2d6d 6573 7361 6765 7323 6275  rmat-messages#bu
+00008f70: 696c 7469 6e69 636f 6e73 3e60 5f5f 0a20  iltinicons>`__. 
+00008f80: 2020 2020 2020 2020 2020 2061 6e64 0a20             and. 
+00008f90: 2020 2020 2020 2020 2020 2060 6375 7374             `cust
+00008fa0: 6f6d 203c 6874 7470 733a 2f2f 6465 7665  om <https://deve
+00008fb0: 6c6f 7065 7273 2e67 6f6f 676c 652e 636f  lopers.google.co
+00008fc0: 6d2f 776f 726b 7370 6163 652f 6368 6174  m/workspace/chat
+00008fd0: 2f66 6f72 6d61 742d 6d65 7373 6167 6573  /format-messages
+00008fe0: 2363 7573 746f 6d69 636f 6e73 3e60 5f5f  #customicons>`__
+00008ff0: 0a20 2020 2020 2020 2020 2020 2069 636f  .            ico
+00009000: 6e73 2e0a 0a20 2020 2020 2020 2020 2020  ns...           
+00009010: 2054 6869 7320 6669 656c 6420 6973 2061   This field is a
+00009020: 206d 656d 6265 7220 6f66 2060 6f6e 656f   member of `oneo
+00009030: 6660 5f20 6060 636f 6e74 726f 6c60 602e  f`_ ``control``.
+00009040: 0a20 2020 2022 2222 0a0a 2020 2020 636c  .    """..    cl
+00009050: 6173 7320 5377 6974 6368 436f 6e74 726f  ass SwitchContro
+00009060: 6c28 7072 6f74 6f2e 4d65 7373 6167 6529  l(proto.Message)
+00009070: 3a0a 2020 2020 2020 2020 7222 2222 4569  :.        r"""Ei
+00009080: 7468 6572 2061 2074 6f67 676c 652d 7374  ther a toggle-st
+00009090: 796c 6520 7377 6974 6368 206f 7220 6120  yle switch or a 
+000090a0: 6368 6563 6b62 6f78 2069 6e73 6964 6520  checkbox inside 
+000090b0: 610a 2020 2020 2020 2020 6060 6465 636f  a.        ``deco
+000090c0: 7261 7465 6454 6578 7460 6020 7769 6467  ratedText`` widg
+000090d0: 6574 2e0a 0a20 2020 2020 2020 2060 476f  et...        `Go
+000090e0: 6f67 6c65 2057 6f72 6b73 7061 6365 2041  ogle Workspace A
+000090f0: 6464 2d6f 6e73 2061 6e64 2043 6861 740a  dd-ons and Chat.
+00009100: 2020 2020 2020 2020 6170 7073 203c 6874          apps <ht
+00009110: 7470 733a 2f2f 6465 7665 6c6f 7065 7273  tps://developers
+00009120: 2e67 6f6f 676c 652e 636f 6d2f 776f 726b  .google.com/work
+00009130: 7370 6163 652f 6578 7465 6e64 3e60 5f5f  space/extend>`__
+00009140: 3a0a 0a20 2020 2020 2020 204f 6e6c 7920  :..        Only 
+00009150: 7375 7070 6f72 7465 6420 696e 2074 6865  supported in the
+00009160: 2060 6064 6563 6f72 6174 6564 5465 7874   ``decoratedText
+00009170: 6060 2077 6964 6765 742e 0a0a 2020 2020  `` widget...    
+00009180: 2020 2020 4174 7472 6962 7574 6573 3a0a      Attributes:.
+00009190: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+000091a0: 2028 7374 7229 3a0a 2020 2020 2020 2020   (str):.        
+000091b0: 2020 2020 2020 2020 5468 6520 6e61 6d65          The name
+000091c0: 2062 7920 7768 6963 6820 7468 6520 7377   by which the sw
+000091d0: 6974 6368 2077 6964 6765 7420 6973 2069  itch widget is i
+000091e0: 6465 6e74 6966 6965 6420 696e 2061 2066  dentified in a f
+000091f0: 6f72 6d0a 2020 2020 2020 2020 2020 2020  orm.            
+00009200: 2020 2020 696e 7075 7420 6576 656e 742e      input event.
+00009210: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009220: 2020 466f 7220 6465 7461 696c 7320 6162    For details ab
+00009230: 6f75 7420 776f 726b 696e 6720 7769 7468  out working with
+00009240: 2066 6f72 6d20 696e 7075 7473 2c20 7365   form inputs, se
+00009250: 6520 6052 6563 6569 7665 0a20 2020 2020  e `Receive.     
+00009260: 2020 2020 2020 2020 2020 2066 6f72 6d0a             form.
+00009270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009280: 6461 7461 203c 6874 7470 733a 2f2f 6465  data <https://de
+00009290: 7665 6c6f 7065 7273 2e67 6f6f 676c 652e  velopers.google.
+000092a0: 636f 6d2f 776f 726b 7370 6163 652f 6368  com/workspace/ch
+000092b0: 6174 2f72 6561 642d 666f 726d 2d64 6174  at/read-form-dat
+000092c0: 613e 605f 5f2e 0a20 2020 2020 2020 2020  a>`__..         
+000092d0: 2020 2076 616c 7565 2028 7374 7229 3a0a     value (str):.
+000092e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000092f0: 5468 6520 7661 6c75 6520 656e 7465 7265  The value entere
+00009300: 6420 6279 2061 2075 7365 722c 2072 6574  d by a user, ret
+00009310: 7572 6e65 6420 6173 2070 6172 7420 6f66  urned as part of
+00009320: 2061 2066 6f72 6d0a 2020 2020 2020 2020   a form.        
+00009330: 2020 2020 2020 2020 696e 7075 7420 6576          input ev
+00009340: 656e 742e 0a0a 2020 2020 2020 2020 2020  ent...          
+00009350: 2020 2020 2020 466f 7220 6465 7461 696c        For detail
+00009360: 7320 6162 6f75 7420 776f 726b 696e 6720  s about working 
+00009370: 7769 7468 2066 6f72 6d20 696e 7075 7473  with form inputs
+00009380: 2c20 7365 6520 6052 6563 6569 7665 0a20  , see `Receive. 
+00009390: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000093a0: 6f72 6d0a 2020 2020 2020 2020 2020 2020  orm.            
+000093b0: 2020 2020 6461 7461 203c 6874 7470 733a      data <https:
+000093c0: 2f2f 6465 7665 6c6f 7065 7273 2e67 6f6f  //developers.goo
+000093d0: 676c 652e 636f 6d2f 776f 726b 7370 6163  gle.com/workspac
+000093e0: 652f 6368 6174 2f72 6561 642d 666f 726d  e/chat/read-form
+000093f0: 2d64 6174 613e 605f 5f2e 0a20 2020 2020  -data>`__..     
+00009400: 2020 2020 2020 2073 656c 6563 7465 6420         selected 
+00009410: 2862 6f6f 6c29 3a0a 2020 2020 2020 2020  (bool):.        
+00009420: 2020 2020 2020 2020 5768 656e 2060 6074          When ``t
+00009430: 7275 6560 602c 2074 6865 2073 7769 7463  rue``, the switc
+00009440: 6820 6973 2073 656c 6563 7465 642e 0a20  h is selected.. 
+00009450: 2020 2020 2020 2020 2020 206f 6e5f 6368             on_ch
+00009460: 616e 6765 5f61 6374 696f 6e20 2867 6f6f  ange_action (goo
+00009470: 676c 652e 6170 7073 2e63 6172 645f 7631  gle.apps.card_v1
+00009480: 2e74 7970 6573 2e41 6374 696f 6e29 3a0a  .types.Action):.
+00009490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000094a0: 5468 6520 6163 7469 6f6e 2074 6f20 7065  The action to pe
+000094b0: 7266 6f72 6d20 7768 656e 2074 6865 2073  rform when the s
+000094c0: 7769 7463 6820 7374 6174 650a 2020 2020  witch state.    
+000094d0: 2020 2020 2020 2020 2020 2020 6973 2063              is c
+000094e0: 6861 6e67 6564 2c20 7375 6368 2061 7320  hanged, such as 
+000094f0: 7768 6174 2020 6675 6e63 7469 6f6e 2074  what  function t
+00009500: 6f20 7275 6e2e 0a20 2020 2020 2020 2020  o run..         
+00009510: 2020 2063 6f6e 7472 6f6c 5f74 7970 6520     control_type 
+00009520: 2867 6f6f 676c 652e 6170 7073 2e63 6172  (google.apps.car
+00009530: 645f 7631 2e74 7970 6573 2e44 6563 6f72  d_v1.types.Decor
+00009540: 6174 6564 5465 7874 2e53 7769 7463 6843  atedText.SwitchC
+00009550: 6f6e 7472 6f6c 2e43 6f6e 7472 6f6c 5479  ontrol.ControlTy
+00009560: 7065 293a 0a20 2020 2020 2020 2020 2020  pe):.           
+00009570: 2020 2020 2048 6f77 2074 6865 2073 7769       How the swi
+00009580: 7463 6820 6170 7065 6172 7320 696e 2074  tch appears in t
+00009590: 6865 2075 7365 7220 696e 7465 7266 6163  he user interfac
+000095a0: 652e 0a0a 2020 2020 2020 2020 2020 2020  e...            
+000095b0: 2020 2020 6047 6f6f 676c 6520 576f 726b      `Google Work
+000095c0: 7370 6163 6520 4164 642d 6f6e 7320 616e  space Add-ons an
+000095d0: 6420 4368 6174 0a20 2020 2020 2020 2020  d Chat.         
+000095e0: 2020 2020 2020 2061 7070 7320 3c68 7474         apps <htt
+000095f0: 7073 3a2f 2f64 6576 656c 6f70 6572 732e  ps://developers.
+00009600: 676f 6f67 6c65 2e63 6f6d 2f77 6f72 6b73  google.com/works
+00009610: 7061 6365 2f65 7874 656e 643e 605f 5f3a  pace/extend>`__:
+00009620: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
+00009630: 2020 2020 2020 636c 6173 7320 436f 6e74        class Cont
+00009640: 726f 6c54 7970 6528 7072 6f74 6f2e 456e  rolType(proto.En
+00009650: 756d 293a 0a20 2020 2020 2020 2020 2020  um):.           
+00009660: 2072 2222 2248 6f77 2074 6865 2073 7769   r"""How the swi
+00009670: 7463 6820 6170 7065 6172 7320 696e 2074  tch appears in t
+00009680: 6865 2075 7365 7220 696e 7465 7266 6163  he user interfac
+00009690: 652e 0a0a 2020 2020 2020 2020 2020 2020  e...            
+000096a0: 6047 6f6f 676c 6520 576f 726b 7370 6163  `Google Workspac
+000096b0: 6520 4164 642d 6f6e 7320 616e 6420 4368  e Add-ons and Ch
+000096c0: 6174 0a20 2020 2020 2020 2020 2020 2061  at.            a
+000096d0: 7070 7320 3c68 7474 7073 3a2f 2f64 6576  pps <https://dev
+000096e0: 656c 6f70 6572 732e 676f 6f67 6c65 2e63  elopers.google.c
+000096f0: 6f6d 2f77 6f72 6b73 7061 6365 2f65 7874  om/workspace/ext
+00009700: 656e 643e 605f 5f3a 0a0a 2020 2020 2020  end>`__:..      
+00009710: 2020 2020 2020 5661 6c75 6573 3a0a 2020        Values:.  
+00009720: 2020 2020 2020 2020 2020 2020 2020 5357                SW
+00009730: 4954 4348 2028 3029 3a0a 2020 2020 2020  ITCH (0):.      
+00009740: 2020 2020 2020 2020 2020 2020 2020 4120                A 
+00009750: 746f 6767 6c65 2d73 7479 6c65 2073 7769  toggle-style swi
+00009760: 7463 682e 0a20 2020 2020 2020 2020 2020  tch..           
+00009770: 2020 2020 2043 4845 434b 424f 5820 2831       CHECKBOX (1
+00009780: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00009790: 2020 2020 2020 2044 6570 7265 6361 7465         Deprecate
+000097a0: 6420 696e 2066 6176 6f72 206f 6620 6060  d in favor of ``
+000097b0: 4348 4543 4b5f 424f 5860 602e 0a20 2020  CHECK_BOX``..   
+000097c0: 2020 2020 2020 2020 2020 2020 2043 4845               CHE
+000097d0: 434b 5f42 4f58 2028 3229 3a0a 2020 2020  CK_BOX (2):.    
+000097e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000097f0: 4120 6368 6563 6b62 6f78 2e0a 2020 2020  A checkbox..    
+00009800: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00009810: 2020 2020 2020 2020 5357 4954 4348 203d          SWITCH =
+00009820: 2030 0a20 2020 2020 2020 2020 2020 2043   0.            C
+00009830: 4845 434b 424f 5820 3d20 310a 2020 2020  HECKBOX = 1.    
+00009840: 2020 2020 2020 2020 4348 4543 4b5f 424f          CHECK_BO
+00009850: 5820 3d20 320a 0a20 2020 2020 2020 206e  X = 2..        n
+00009860: 616d 653a 2073 7472 203d 2070 726f 746f  ame: str = proto
+00009870: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
+00009880: 2020 2020 7072 6f74 6f2e 5354 5249 4e47      proto.STRING
+00009890: 2c0a 2020 2020 2020 2020 2020 2020 6e75  ,.            nu
+000098a0: 6d62 6572 3d31 2c0a 2020 2020 2020 2020  mber=1,.        
+000098b0: 290a 2020 2020 2020 2020 7661 6c75 653a  ).        value:
+000098c0: 2073 7472 203d 2070 726f 746f 2e46 6965   str = proto.Fie
+000098d0: 6c64 280a 2020 2020 2020 2020 2020 2020  ld(.            
+000098e0: 7072 6f74 6f2e 5354 5249 4e47 2c0a 2020  proto.STRING,.  
+000098f0: 2020 2020 2020 2020 2020 6e75 6d62 6572            number
+00009900: 3d32 2c0a 2020 2020 2020 2020 290a 2020  =2,.        ).  
+00009910: 2020 2020 2020 7365 6c65 6374 6564 3a20        selected: 
+00009920: 626f 6f6c 203d 2070 726f 746f 2e46 6965  bool = proto.Fie
+00009930: 6c64 280a 2020 2020 2020 2020 2020 2020  ld(.            
+00009940: 7072 6f74 6f2e 424f 4f4c 2c0a 2020 2020  proto.BOOL,.    
+00009950: 2020 2020 2020 2020 6e75 6d62 6572 3d33          number=3
+00009960: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+00009970: 2020 2020 6f6e 5f63 6861 6e67 655f 6163      on_change_ac
+00009980: 7469 6f6e 3a20 2241 6374 696f 6e22 203d  tion: "Action" =
+00009990: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
+000099a0: 2020 2020 2020 2020 2020 7072 6f74 6f2e            proto.
+000099b0: 4d45 5353 4147 452c 0a20 2020 2020 2020  MESSAGE,.       
+000099c0: 2020 2020 206e 756d 6265 723d 342c 0a20       number=4,. 
+000099d0: 2020 2020 2020 2020 2020 206d 6573 7361             messa
+000099e0: 6765 3d22 4163 7469 6f6e 222c 0a20 2020  ge="Action",.   
+000099f0: 2020 2020 2029 0a20 2020 2020 2020 2063       ).        c
+00009a00: 6f6e 7472 6f6c 5f74 7970 653a 2022 4465  ontrol_type: "De
+00009a10: 636f 7261 7465 6454 6578 742e 5377 6974  coratedText.Swit
+00009a20: 6368 436f 6e74 726f 6c2e 436f 6e74 726f  chControl.Contro
+00009a30: 6c54 7970 6522 203d 2070 726f 746f 2e46  lType" = proto.F
+00009a40: 6965 6c64 280a 2020 2020 2020 2020 2020  ield(.          
+00009a50: 2020 7072 6f74 6f2e 454e 554d 2c0a 2020    proto.ENUM,.  
+00009a60: 2020 2020 2020 2020 2020 6e75 6d62 6572            number
+00009a70: 3d35 2c0a 2020 2020 2020 2020 2020 2020  =5,.            
+00009a80: 656e 756d 3d22 4465 636f 7261 7465 6454  enum="DecoratedT
+00009a90: 6578 742e 5377 6974 6368 436f 6e74 726f  ext.SwitchContro
+00009aa0: 6c2e 436f 6e74 726f 6c54 7970 6522 2c0a  l.ControlType",.
+00009ab0: 2020 2020 2020 2020 290a 0a20 2020 2069          )..    i
+00009ac0: 636f 6e3a 2022 4963 6f6e 2220 3d20 7072  con: "Icon" = pr
+00009ad0: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
+00009ae0: 2020 2070 726f 746f 2e4d 4553 5341 4745     proto.MESSAGE
+00009af0: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
+00009b00: 3d31 2c0a 2020 2020 2020 2020 6d65 7373  =1,.        mess
+00009b10: 6167 653d 2249 636f 6e22 2c0a 2020 2020  age="Icon",.    
+00009b20: 290a 2020 2020 7374 6172 745f 6963 6f6e  ).    start_icon
+00009b30: 3a20 2249 636f 6e22 203d 2070 726f 746f  : "Icon" = proto
+00009b40: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
+00009b50: 7072 6f74 6f2e 4d45 5353 4147 452c 0a20  proto.MESSAGE,. 
+00009b60: 2020 2020 2020 206e 756d 6265 723d 3132         number=12
+00009b70: 2c0a 2020 2020 2020 2020 6d65 7373 6167  ,.        messag
+00009b80: 653d 2249 636f 6e22 2c0a 2020 2020 290a  e="Icon",.    ).
+00009b90: 2020 2020 746f 705f 6c61 6265 6c3a 2073      top_label: s
+00009ba0: 7472 203d 2070 726f 746f 2e46 6965 6c64  tr = proto.Field
+00009bb0: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
+00009bc0: 5354 5249 4e47 2c0a 2020 2020 2020 2020  STRING,.        
+00009bd0: 6e75 6d62 6572 3d33 2c0a 2020 2020 290a  number=3,.    ).
+00009be0: 2020 2020 7465 7874 3a20 7374 7220 3d20      text: str = 
+00009bf0: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
+00009c00: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
+00009c10: 472c 0a20 2020 2020 2020 206e 756d 6265  G,.        numbe
+00009c20: 723d 342c 0a20 2020 2029 0a20 2020 2077  r=4,.    ).    w
+00009c30: 7261 705f 7465 7874 3a20 626f 6f6c 203d  rap_text: bool =
+00009c40: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
+00009c50: 2020 2020 2020 7072 6f74 6f2e 424f 4f4c        proto.BOOL
+00009c60: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
+00009c70: 3d35 2c0a 2020 2020 290a 2020 2020 626f  =5,.    ).    bo
+00009c80: 7474 6f6d 5f6c 6162 656c 3a20 7374 7220  ttom_label: str 
+00009c90: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
+00009ca0: 2020 2020 2020 2070 726f 746f 2e53 5452         proto.STR
+00009cb0: 494e 472c 0a20 2020 2020 2020 206e 756d  ING,.        num
+00009cc0: 6265 723d 362c 0a20 2020 2029 0a20 2020  ber=6,.    ).   
+00009cd0: 206f 6e5f 636c 6963 6b3a 2022 4f6e 436c   on_click: "OnCl
+00009ce0: 6963 6b22 203d 2070 726f 746f 2e46 6965  ick" = proto.Fie
+00009cf0: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
+00009d00: 6f2e 4d45 5353 4147 452c 0a20 2020 2020  o.MESSAGE,.     
+00009d10: 2020 206e 756d 6265 723d 372c 0a20 2020     number=7,.   
+00009d20: 2020 2020 206d 6573 7361 6765 3d22 4f6e       message="On
+00009d30: 436c 6963 6b22 2c0a 2020 2020 290a 2020  Click",.    ).  
+00009d40: 2020 6275 7474 6f6e 3a20 2242 7574 746f    button: "Butto
+00009d50: 6e22 203d 2070 726f 746f 2e46 6965 6c64  n" = proto.Field
+00009d60: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
+00009d70: 4d45 5353 4147 452c 0a20 2020 2020 2020  MESSAGE,.       
+00009d80: 206e 756d 6265 723d 382c 0a20 2020 2020   number=8,.     
+00009d90: 2020 206f 6e65 6f66 3d22 636f 6e74 726f     oneof="contro
+00009da0: 6c22 2c0a 2020 2020 2020 2020 6d65 7373  l",.        mess
+00009db0: 6167 653d 2242 7574 746f 6e22 2c0a 2020  age="Button",.  
+00009dc0: 2020 290a 2020 2020 7377 6974 6368 5f63    ).    switch_c
+00009dd0: 6f6e 7472 6f6c 3a20 5377 6974 6368 436f  ontrol: SwitchCo
+00009de0: 6e74 726f 6c20 3d20 7072 6f74 6f2e 4669  ntrol = proto.Fi
+00009df0: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
+00009e00: 746f 2e4d 4553 5341 4745 2c0a 2020 2020  to.MESSAGE,.    
+00009e10: 2020 2020 6e75 6d62 6572 3d39 2c0a 2020      number=9,.  
+00009e20: 2020 2020 2020 6f6e 656f 663d 2263 6f6e        oneof="con
+00009e30: 7472 6f6c 222c 0a20 2020 2020 2020 206d  trol",.        m
+00009e40: 6573 7361 6765 3d53 7769 7463 6843 6f6e  essage=SwitchCon
+00009e50: 7472 6f6c 2c0a 2020 2020 290a 2020 2020  trol,.    ).    
+00009e60: 656e 645f 6963 6f6e 3a20 2249 636f 6e22  end_icon: "Icon"
+00009e70: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
+00009e80: 2020 2020 2020 2020 7072 6f74 6f2e 4d45          proto.ME
+00009e90: 5353 4147 452c 0a20 2020 2020 2020 206e  SSAGE,.        n
+00009ea0: 756d 6265 723d 3131 2c0a 2020 2020 2020  umber=11,.      
+00009eb0: 2020 6f6e 656f 663d 2263 6f6e 7472 6f6c    oneof="control
+00009ec0: 222c 0a20 2020 2020 2020 206d 6573 7361  ",.        messa
+00009ed0: 6765 3d22 4963 6f6e 222c 0a20 2020 2029  ge="Icon",.    )
+00009ee0: 0a0a 0a63 6c61 7373 2054 6578 7449 6e70  ...class TextInp
+00009ef0: 7574 2870 726f 746f 2e4d 6573 7361 6765  ut(proto.Message
+00009f00: 293a 0a20 2020 2072 2222 2241 2066 6965  ):.    r"""A fie
+00009f10: 6c64 2069 6e20 7768 6963 6820 7573 6572  ld in which user
+00009f20: 7320 6361 6e20 656e 7465 7220 7465 7874  s can enter text
+00009f30: 2e20 5375 7070 6f72 7473 2073 7567 6765  . Supports sugge
+00009f40: 7374 696f 6e73 2061 6e64 0a20 2020 206f  stions and.    o
+00009f50: 6e2d 6368 616e 6765 2061 6374 696f 6e73  n-change actions
+00009f60: 2e20 466f 7220 616e 2065 7861 6d70 6c65  . For an example
+00009f70: 2069 6e20 476f 6f67 6c65 2043 6861 7420   in Google Chat 
+00009f80: 6170 7073 2c20 7365 6520 6041 6464 2061  apps, see `Add a
+00009f90: 0a20 2020 2066 6965 6c64 2069 6e20 7768  .    field in wh
+00009fa0: 6963 6820 6120 7573 6572 2063 616e 2065  ich a user can e
+00009fb0: 6e74 6572 0a20 2020 2074 6578 7420 3c68  nter.    text <h
+00009fc0: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
+00009fd0: 732e 676f 6f67 6c65 2e63 6f6d 2f77 6f72  s.google.com/wor
+00009fe0: 6b73 7061 6365 2f63 6861 742f 6465 7369  kspace/chat/desi
+00009ff0: 676e 2d69 6e74 6572 6163 7469 7665 2d63  gn-interactive-c
+0000a000: 6172 642d 6469 616c 6f67 2361 6464 5f61  ard-dialog#add_a
+0000a010: 5f66 6965 6c64 5f69 6e5f 7768 6963 685f  _field_in_which_
+0000a020: 615f 7573 6572 5f63 616e 5f65 6e74 6572  a_user_can_enter
+0000a030: 5f74 6578 743e 605f 5f2e 0a0a 2020 2020  _text>`__...    
+0000a040: 4368 6174 2061 7070 7320 7265 6365 6976  Chat apps receiv
+0000a050: 6520 616e 6420 6361 6e20 7072 6f63 6573  e and can proces
+0000a060: 7320 7468 6520 7661 6c75 6520 6f66 2065  s the value of e
+0000a070: 6e74 6572 6564 2074 6578 7420 6475 7269  ntered text duri
+0000a080: 6e67 0a20 2020 2066 6f72 6d20 696e 7075  ng.    form inpu
+0000a090: 7420 6576 656e 7473 2e20 466f 7220 6465  t events. For de
+0000a0a0: 7461 696c 7320 6162 6f75 7420 776f 726b  tails about work
+0000a0b0: 696e 6720 7769 7468 2066 6f72 6d20 696e  ing with form in
+0000a0c0: 7075 7473 2c20 7365 650a 2020 2020 6052  puts, see.    `R
+0000a0d0: 6563 6569 7665 2066 6f72 6d0a 2020 2020  eceive form.    
+0000a0e0: 6461 7461 203c 6874 7470 733a 2f2f 6465  data <https://de
+0000a0f0: 7665 6c6f 7065 7273 2e67 6f6f 676c 652e  velopers.google.
+0000a100: 636f 6d2f 776f 726b 7370 6163 652f 6368  com/workspace/ch
+0000a110: 6174 2f72 6561 642d 666f 726d 2d64 6174  at/read-form-dat
+0000a120: 613e 605f 5f2e 0a0a 2020 2020 5768 656e  a>`__...    When
+0000a130: 2079 6f75 206e 6565 6420 746f 2063 6f6c   you need to col
+0000a140: 6c65 6374 2075 6e64 6566 696e 6564 206f  lect undefined o
+0000a150: 7220 6162 7374 7261 6374 2064 6174 6120  r abstract data 
+0000a160: 6672 6f6d 2075 7365 7273 2c20 7573 650a  from users, use.
+0000a170: 2020 2020 6120 7465 7874 2069 6e70 7574      a text input
+0000a180: 2e20 546f 2063 6f6c 6c65 6374 2064 6566  . To collect def
+0000a190: 696e 6564 206f 7220 656e 756d 6572 6174  ined or enumerat
+0000a1a0: 6564 2064 6174 6120 6672 6f6d 2075 7365  ed data from use
+0000a1b0: 7273 2c20 7573 650a 2020 2020 7468 6520  rs, use.    the 
+0000a1c0: 5b53 656c 6563 7469 6f6e 496e 7075 745d  [SelectionInput]
+0000a1d0: 5b67 6f6f 676c 652e 6170 7073 2e63 6172  [google.apps.car
+0000a1e0: 642e 7631 2e53 656c 6563 7469 6f6e 496e  d.v1.SelectionIn
+0000a1f0: 7075 745d 2077 6964 6765 742e 0a0a 2020  put] widget...  
+0000a200: 2020 6047 6f6f 676c 6520 576f 726b 7370    `Google Worksp
+0000a210: 6163 6520 4164 642d 6f6e 7320 616e 6420  ace Add-ons and 
+0000a220: 4368 6174 0a20 2020 2061 7070 7320 3c68  Chat.    apps <h
+0000a230: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
+0000a240: 732e 676f 6f67 6c65 2e63 6f6d 2f77 6f72  s.google.com/wor
+0000a250: 6b73 7061 6365 2f65 7874 656e 643e 605f  kspace/extend>`_
+0000a260: 5f3a 0a0a 2020 2020 4174 7472 6962 7574  _:..    Attribut
+0000a270: 6573 3a0a 2020 2020 2020 2020 6e61 6d65  es:.        name
+0000a280: 2028 7374 7229 3a0a 2020 2020 2020 2020   (str):.        
+0000a290: 2020 2020 5468 6520 6e61 6d65 2062 7920      The name by 
+0000a2a0: 7768 6963 6820 7468 6520 7465 7874 2069  which the text i
+0000a2b0: 6e70 7574 2069 7320 6964 656e 7469 6669  nput is identifi
+0000a2c0: 6564 2069 6e20 6120 666f 726d 0a20 2020  ed in a form.   
+0000a2d0: 2020 2020 2020 2020 2069 6e70 7574 2065           input e
+0000a2e0: 7665 6e74 2e0a 0a20 2020 2020 2020 2020  vent...         
+0000a2f0: 2020 2046 6f72 2064 6574 6169 6c73 2061     For details a
+0000a300: 626f 7574 2077 6f72 6b69 6e67 2077 6974  bout working wit
+0000a310: 6820 666f 726d 2069 6e70 7574 732c 2073  h form inputs, s
+0000a320: 6565 2060 5265 6365 6976 650a 2020 2020  ee `Receive.    
+0000a330: 2020 2020 2020 2020 666f 726d 0a20 2020          form.   
+0000a340: 2020 2020 2020 2020 2064 6174 6120 3c68           data <h
+0000a350: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
+0000a360: 732e 676f 6f67 6c65 2e63 6f6d 2f77 6f72  s.google.com/wor
+0000a370: 6b73 7061 6365 2f63 6861 742f 7265 6164  kspace/chat/read
+0000a380: 2d66 6f72 6d2d 6461 7461 3e60 5f5f 2e0a  -form-data>`__..
+0000a390: 2020 2020 2020 2020 6c61 6265 6c20 2873          label (s
+0000a3a0: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
+0000a3b0: 2054 6865 2074 6578 7420 7468 6174 2061   The text that a
+0000a3c0: 7070 6561 7273 2061 626f 7665 2074 6865  ppears above the
+0000a3d0: 2074 6578 7420 696e 7075 7420 6669 656c   text input fiel
+0000a3e0: 6420 696e 2074 6865 2075 7365 720a 2020  d in the user.  
+0000a3f0: 2020 2020 2020 2020 2020 696e 7465 7266            interf
+0000a400: 6163 652e 0a0a 2020 2020 2020 2020 2020  ace...          
+0000a410: 2020 5370 6563 6966 7920 7465 7874 2074    Specify text t
+0000a420: 6861 7420 6865 6c70 7320 7468 6520 7573  hat helps the us
+0000a430: 6572 2065 6e74 6572 2074 6865 2069 6e66  er enter the inf
+0000a440: 6f72 6d61 7469 6f6e 2079 6f75 720a 2020  ormation your.  
+0000a450: 2020 2020 2020 2020 2020 6170 7020 6e65            app ne
+0000a460: 6564 732e 2046 6f72 2065 7861 6d70 6c65  eds. For example
+0000a470: 2c20 6966 2079 6f75 2061 7265 2061 736b  , if you are ask
+0000a480: 696e 6720 736f 6d65 6f6e 6527 7320 6e61  ing someone's na
+0000a490: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
+0000a4a0: 6275 7420 7370 6563 6966 6963 616c 6c79  but specifically
+0000a4b0: 206e 6565 6420 7468 6569 7220 7375 726e   need their surn
+0000a4c0: 616d 652c 2077 7269 7465 2060 6073 7572  ame, write ``sur
+0000a4d0: 6e61 6d65 6060 0a20 2020 2020 2020 2020  name``.         
+0000a4e0: 2020 2069 6e73 7465 6164 206f 6620 6060     instead of ``
+0000a4f0: 6e61 6d65 6060 2e0a 0a20 2020 2020 2020  name``...       
+0000a500: 2020 2020 2052 6571 7569 7265 6420 6966       Required if
+0000a510: 2060 6068 696e 7454 6578 7460 6020 6973   ``hintText`` is
+0000a520: 2075 6e73 7065 6369 6669 6564 2e20 4f74   unspecified. Ot
+0000a530: 6865 7277 6973 652c 0a20 2020 2020 2020  herwise,.       
+0000a540: 2020 2020 206f 7074 696f 6e61 6c2e 0a20       optional.. 
+0000a550: 2020 2020 2020 2068 696e 745f 7465 7874         hint_text
+0000a560: 2028 7374 7229 3a0a 2020 2020 2020 2020   (str):.        
+0000a570: 2020 2020 5465 7874 2074 6861 7420 6170      Text that ap
+0000a580: 7065 6172 7320 6265 6c6f 7720 7468 6520  pears below the 
+0000a590: 7465 7874 2069 6e70 7574 2066 6965 6c64  text input field
+0000a5a0: 206d 6561 6e74 2074 6f20 6173 7369 7374   meant to assist
+0000a5b0: 0a20 2020 2020 2020 2020 2020 2075 7365  .            use
+0000a5c0: 7273 2062 7920 7072 6f6d 7074 696e 6720  rs by prompting 
+0000a5d0: 7468 656d 2074 6f20 656e 7465 7220 6120  them to enter a 
+0000a5e0: 6365 7274 6169 6e20 7661 6c75 652e 2054  certain value. T
+0000a5f0: 6869 7320 7465 7874 0a20 2020 2020 2020  his text.       
+0000a600: 2020 2020 2069 7320 616c 7761 7973 2076       is always v
+0000a610: 6973 6962 6c65 2e0a 0a20 2020 2020 2020  isible...       
+0000a620: 2020 2020 2052 6571 7569 7265 6420 6966       Required if
+0000a630: 2060 606c 6162 656c 6060 2069 7320 756e   ``label`` is un
+0000a640: 7370 6563 6966 6965 642e 204f 7468 6572  specified. Other
+0000a650: 7769 7365 2c20 6f70 7469 6f6e 616c 2e0a  wise, optional..
+0000a660: 2020 2020 2020 2020 7661 6c75 6520 2873          value (s
+0000a670: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
+0000a680: 2054 6865 2076 616c 7565 2065 6e74 6572   The value enter
+0000a690: 6564 2062 7920 6120 7573 6572 2c20 7265  ed by a user, re
+0000a6a0: 7475 726e 6564 2061 7320 7061 7274 206f  turned as part o
+0000a6b0: 6620 6120 666f 726d 0a20 2020 2020 2020  f a form.       
+0000a6c0: 2020 2020 2069 6e70 7574 2065 7665 6e74       input event
+0000a6d0: 2e0a 0a20 2020 2020 2020 2020 2020 2046  ...            F
+0000a6e0: 6f72 2064 6574 6169 6c73 2061 626f 7574  or details about
+0000a6f0: 2077 6f72 6b69 6e67 2077 6974 6820 666f   working with fo
+0000a700: 726d 2069 6e70 7574 732c 2073 6565 2060  rm inputs, see `
+0000a710: 5265 6365 6976 650a 2020 2020 2020 2020  Receive.        
+0000a720: 2020 2020 666f 726d 0a20 2020 2020 2020      form.       
+0000a730: 2020 2020 2064 6174 6120 3c68 7474 7073       data <https
+0000a740: 3a2f 2f64 6576 656c 6f70 6572 732e 676f  ://developers.go
+0000a750: 6f67 6c65 2e63 6f6d 2f77 6f72 6b73 7061  ogle.com/workspa
+0000a760: 6365 2f63 6861 742f 7265 6164 2d66 6f72  ce/chat/read-for
+0000a770: 6d2d 6461 7461 3e60 5f5f 2e0a 2020 2020  m-data>`__..    
+0000a780: 2020 2020 7479 7065 5f20 2867 6f6f 676c      type_ (googl
+0000a790: 652e 6170 7073 2e63 6172 645f 7631 2e74  e.apps.card_v1.t
+0000a7a0: 7970 6573 2e54 6578 7449 6e70 7574 2e54  ypes.TextInput.T
+0000a7b0: 7970 6529 3a0a 2020 2020 2020 2020 2020  ype):.          
+0000a7c0: 2020 486f 7720 6120 7465 7874 2069 6e70    How a text inp
+0000a7d0: 7574 2066 6965 6c64 2061 7070 6561 7273  ut field appears
+0000a7e0: 2069 6e20 7468 6520 7573 6572 0a20 2020   in the user.   
+0000a7f0: 2020 2020 2020 2020 2069 6e74 6572 6661           interfa
+0000a800: 6365 2e20 466f 7220 6578 616d 706c 652c  ce. For example,
+0000a810: 2077 6865 7468 6572 2074 6865 2066 6965   whether the fie
+0000a820: 6c64 2069 730a 2020 2020 2020 2020 2020  ld is.          
+0000a830: 2020 7369 6e67 6c65 206f 7220 6d75 6c74    single or mult
+0000a840: 692d 6c69 6e65 2e0a 2020 2020 2020 2020  i-line..        
+0000a850: 6f6e 5f63 6861 6e67 655f 6163 7469 6f6e  on_change_action
+0000a860: 2028 676f 6f67 6c65 2e61 7070 732e 6361   (google.apps.ca
+0000a870: 7264 5f76 312e 7479 7065 732e 4163 7469  rd_v1.types.Acti
+0000a880: 6f6e 293a 0a20 2020 2020 2020 2020 2020  on):.           
+0000a890: 2057 6861 7420 746f 2064 6f20 7768 656e   What to do when
+0000a8a0: 2061 2063 6861 6e67 6520 6f63 6375 7273   a change occurs
+0000a8b0: 2069 6e20 7468 6520 7465 7874 2069 6e70   in the text inp
+0000a8c0: 7574 2066 6965 6c64 2e20 466f 720a 2020  ut field. For.  
+0000a8d0: 2020 2020 2020 2020 2020 6578 616d 706c            exampl
+0000a8e0: 652c 2061 2075 7365 7220 6164 6469 6e67  e, a user adding
+0000a8f0: 2074 6f20 7468 6520 6669 656c 6420 6f72   to the field or
+0000a900: 2064 656c 6574 696e 6720 7465 7874 2e0a   deleting text..
+0000a910: 0a20 2020 2020 2020 2020 2020 2045 7861  .            Exa
+0000a920: 6d70 6c65 7320 6f66 2061 6374 696f 6e73  mples of actions
+0000a930: 2074 6f20 7461 6b65 2069 6e63 6c75 6465   to take include
+0000a940: 2072 756e 6e69 6e67 2061 2063 7573 746f   running a custo
+0000a950: 6d0a 2020 2020 2020 2020 2020 2020 6675  m.            fu
+0000a960: 6e63 7469 6f6e 206f 7220 6f70 656e 696e  nction or openin
+0000a970: 6720 610a 2020 2020 2020 2020 2020 2020  g a.            
+0000a980: 6064 6961 6c6f 6720 3c68 7474 7073 3a2f  `dialog <https:/
+0000a990: 2f64 6576 656c 6f70 6572 732e 676f 6f67  /developers.goog
+0000a9a0: 6c65 2e63 6f6d 2f77 6f72 6b73 7061 6365  le.com/workspace
+0000a9b0: 2f63 6861 742f 6469 616c 6f67 733e 605f  /chat/dialogs>`_
+0000a9c0: 5f0a 2020 2020 2020 2020 2020 2020 696e  _.            in
+0000a9d0: 2047 6f6f 676c 6520 4368 6174 2e0a 2020   Google Chat..  
+0000a9e0: 2020 2020 2020 696e 6974 6961 6c5f 7375        initial_su
+0000a9f0: 6767 6573 7469 6f6e 7320 2867 6f6f 676c  ggestions (googl
+0000aa00: 652e 6170 7073 2e63 6172 645f 7631 2e74  e.apps.card_v1.t
+0000aa10: 7970 6573 2e53 7567 6765 7374 696f 6e73  ypes.Suggestions
+0000aa20: 293a 0a20 2020 2020 2020 2020 2020 2053  ):.            S
+0000aa30: 7567 6765 7374 6564 2076 616c 7565 7320  uggested values 
+0000aa40: 7468 6174 2075 7365 7273 2063 616e 2065  that users can e
+0000aa50: 6e74 6572 2e20 5468 6573 6520 7661 6c75  nter. These valu
+0000aa60: 6573 2061 7070 6561 720a 2020 2020 2020  es appear.      
+0000aa70: 2020 2020 2020 7768 656e 2075 7365 7273        when users
+0000aa80: 2063 6c69 636b 2069 6e73 6964 6520 7468   click inside th
+0000aa90: 6520 7465 7874 2069 6e70 7574 2066 6965  e text input fie
+0000aaa0: 6c64 2e20 4173 2075 7365 7273 2074 7970  ld. As users typ
+0000aab0: 652c 0a20 2020 2020 2020 2020 2020 2074  e,.            t
+0000aac0: 6865 2073 7567 6765 7374 6564 2076 616c  he suggested val
+0000aad0: 7565 7320 6479 6e61 6d69 6361 6c6c 7920  ues dynamically 
+0000aae0: 6669 6c74 6572 2074 6f20 6d61 7463 6820  filter to match 
+0000aaf0: 7768 6174 2074 6865 0a20 2020 2020 2020  what the.       
+0000ab00: 2020 2020 2075 7365 7273 2068 6176 6520       users have 
+0000ab10: 7479 7065 642e 0a0a 2020 2020 2020 2020  typed...        
+0000ab20: 2020 2020 466f 7220 6578 616d 706c 652c      For example,
+0000ab30: 2061 2074 6578 7420 696e 7075 7420 6669   a text input fi
+0000ab40: 656c 6420 666f 7220 7072 6f67 7261 6d6d  eld for programm
+0000ab50: 696e 6720 6c61 6e67 7561 6765 0a20 2020  ing language.   
+0000ab60: 2020 2020 2020 2020 206d 6967 6874 2073           might s
+0000ab70: 7567 6765 7374 204a 6176 612c 204a 6176  uggest Java, Jav
+0000ab80: 6153 6372 6970 742c 2050 7974 686f 6e2c  aScript, Python,
+0000ab90: 2061 6e64 2043 2b2b 2e20 5768 656e 2075   and C++. When u
+0000aba0: 7365 7273 0a20 2020 2020 2020 2020 2020  sers.           
+0000abb0: 2073 7461 7274 2074 7970 696e 6720 6060   start typing ``
+0000abc0: 4a61 7660 602c 2074 6865 206c 6973 7420  Jav``, the list 
+0000abd0: 6f66 2073 7567 6765 7374 696f 6e73 2066  of suggestions f
+0000abe0: 696c 7465 7273 2074 6f0a 2020 2020 2020  ilters to.      
+0000abf0: 2020 2020 2020 7368 6f77 206a 7573 7420        show just 
+0000ac00: 6060 4a61 7661 6060 2061 6e64 2060 604a  ``Java`` and ``J
+0000ac10: 6176 6153 6372 6970 7460 602e 0a0a 2020  avaScript``...  
+0000ac20: 2020 2020 2020 2020 2020 5375 6767 6573            Sugges
+0000ac30: 7465 6420 7661 6c75 6573 2068 656c 7020  ted values help 
+0000ac40: 6775 6964 6520 7573 6572 7320 746f 2065  guide users to e
+0000ac50: 6e74 6572 2076 616c 7565 7320 7468 6174  nter values that
+0000ac60: 2079 6f75 720a 2020 2020 2020 2020 2020   your.          
+0000ac70: 2020 6170 7020 6361 6e20 6d61 6b65 2073    app can make s
+0000ac80: 656e 7365 206f 662e 2057 6865 6e20 7265  ense of. When re
+0000ac90: 6665 7272 696e 6720 746f 204a 6176 6153  ferring to JavaS
+0000aca0: 6372 6970 742c 2073 6f6d 650a 2020 2020  cript, some.    
+0000acb0: 2020 2020 2020 2020 7573 6572 7320 6d69          users mi
+0000acc0: 6768 7420 656e 7465 7220 6060 6a61 7661  ght enter ``java
+0000acd0: 7363 7269 7074 6060 2061 6e64 206f 7468  script`` and oth
+0000ace0: 6572 7320 6060 6a61 7661 2073 6372 6970  ers ``java scrip
+0000acf0: 7460 602e 0a20 2020 2020 2020 2020 2020  t``..           
+0000ad00: 2053 7567 6765 7374 696e 6720 6060 4a61   Suggesting ``Ja
+0000ad10: 7661 5363 7269 7074 6060 2063 616e 2073  vaScript`` can s
+0000ad20: 7461 6e64 6172 6469 7a65 2068 6f77 2075  tandardize how u
+0000ad30: 7365 7273 2069 6e74 6572 6163 740a 2020  sers interact.  
+0000ad40: 2020 2020 2020 2020 2020 7769 7468 2079            with y
+0000ad50: 6f75 7220 6170 702e 0a0a 2020 2020 2020  our app...      
+0000ad60: 2020 2020 2020 5768 656e 2073 7065 6369        When speci
+0000ad70: 6669 6564 2c20 6060 5465 7874 496e 7075  fied, ``TextInpu
+0000ad80: 742e 7479 7065 6060 2069 7320 616c 7761  t.type`` is alwa
+0000ad90: 7973 0a20 2020 2020 2020 2020 2020 2060  ys.            `
+0000ada0: 6053 494e 474c 455f 4c49 4e45 6060 2c20  `SINGLE_LINE``, 
+0000adb0: 6576 656e 2069 6620 6974 2773 2073 6574  even if it's set
+0000adc0: 2074 6f20 6060 4d55 4c54 4950 4c45 5f4c   to ``MULTIPLE_L
+0000add0: 494e 4560 602e 0a0a 2020 2020 2020 2020  INE``...        
+0000ade0: 2020 2020 6047 6f6f 676c 6520 576f 726b      `Google Work
+0000adf0: 7370 6163 6520 4164 642d 6f6e 7320 616e  space Add-ons an
+0000ae00: 6420 4368 6174 0a20 2020 2020 2020 2020  d Chat.         
+0000ae10: 2020 2061 7070 7320 3c68 7474 7073 3a2f     apps <https:/
+0000ae20: 2f64 6576 656c 6f70 6572 732e 676f 6f67  /developers.goog
+0000ae30: 6c65 2e63 6f6d 2f77 6f72 6b73 7061 6365  le.com/workspace
+0000ae40: 2f65 7874 656e 643e 605f 5f3a 0a20 2020  /extend>`__:.   
+0000ae50: 2020 2020 2061 7574 6f5f 636f 6d70 6c65       auto_comple
+0000ae60: 7465 5f61 6374 696f 6e20 2867 6f6f 676c  te_action (googl
+0000ae70: 652e 6170 7073 2e63 6172 645f 7631 2e74  e.apps.card_v1.t
+0000ae80: 7970 6573 2e41 6374 696f 6e29 3a0a 2020  ypes.Action):.  
+0000ae90: 2020 2020 2020 2020 2020 4f70 7469 6f6e            Option
+0000aea0: 616c 2e20 5370 6563 6966 7920 7768 6174  al. Specify what
+0000aeb0: 2061 6374 696f 6e20 746f 2074 616b 6520   action to take 
+0000aec0: 7768 656e 2074 6865 2074 6578 7420 696e  when the text in
+0000aed0: 7075 740a 2020 2020 2020 2020 2020 2020  put.            
+0000aee0: 6669 656c 6420 7072 6f76 6964 6573 2073  field provides s
+0000aef0: 7567 6765 7374 696f 6e73 2074 6f20 7573  uggestions to us
+0000af00: 6572 7320 7768 6f20 696e 7465 7261 6374  ers who interact
+0000af10: 2077 6974 6820 6974 2e0a 0a20 2020 2020   with it...     
+0000af20: 2020 2020 2020 2049 6620 756e 7370 6563         If unspec
+0000af30: 6966 6965 642c 2074 6865 2073 7567 6765  ified, the sugge
+0000af40: 7374 696f 6e73 2061 7265 2073 6574 2062  stions are set b
+0000af50: 790a 2020 2020 2020 2020 2020 2020 6060  y.            ``
+0000af60: 696e 6974 6961 6c53 7567 6765 7374 696f  initialSuggestio
+0000af70: 6e73 6060 2061 6e64 2061 7265 2070 726f  ns`` and are pro
+0000af80: 6365 7373 6564 2062 7920 7468 6520 636c  cessed by the cl
+0000af90: 6965 6e74 2e0a 0a20 2020 2020 2020 2020  ient...         
+0000afa0: 2020 2049 6620 7370 6563 6966 6965 642c     If specified,
+0000afb0: 2074 6865 2061 7070 2074 616b 6573 2074   the app takes t
+0000afc0: 6865 2061 6374 696f 6e20 7370 6563 6966  he action specif
+0000afd0: 6965 6420 6865 7265 2c20 7375 6368 0a20  ied here, such. 
+0000afe0: 2020 2020 2020 2020 2020 2061 7320 7275             as ru
+0000aff0: 6e6e 696e 6720 6120 6375 7374 6f6d 2066  nning a custom f
+0000b000: 756e 6374 696f 6e2e 0a0a 2020 2020 2020  unction...      
+0000b010: 2020 2020 2020 6047 6f6f 676c 6520 576f        `Google Wo
+0000b020: 726b 7370 6163 650a 2020 2020 2020 2020  rkspace.        
+0000b030: 2020 2020 4164 642d 6f6e 7320 3c68 7474      Add-ons <htt
+0000b040: 7073 3a2f 2f64 6576 656c 6f70 6572 732e  ps://developers.
+0000b050: 676f 6f67 6c65 2e63 6f6d 2f77 6f72 6b73  google.com/works
+0000b060: 7061 6365 2f61 6464 2d6f 6e73 3e60 5f5f  pace/add-ons>`__
+0000b070: 3a0a 2020 2020 2020 2020 706c 6163 6568  :.        placeh
+0000b080: 6f6c 6465 725f 7465 7874 2028 7374 7229  older_text (str)
+0000b090: 3a0a 2020 2020 2020 2020 2020 2020 5465  :.            Te
+0000b0a0: 7874 2074 6861 7420 6170 7065 6172 7320  xt that appears 
+0000b0b0: 696e 2074 6865 2074 6578 7420 696e 7075  in the text inpu
+0000b0c0: 7420 6669 656c 6420 7768 656e 2074 6865  t field when the
+0000b0d0: 2066 6965 6c64 2069 730a 2020 2020 2020   field is.      
+0000b0e0: 2020 2020 2020 656d 7074 792e 2055 7365        empty. Use
+0000b0f0: 2074 6869 7320 7465 7874 2074 6f20 7072   this text to pr
+0000b100: 6f6d 7074 2075 7365 7273 2074 6f20 656e  ompt users to en
+0000b110: 7465 7220 6120 7661 6c75 652e 2046 6f72  ter a value. For
+0000b120: 0a20 2020 2020 2020 2020 2020 2065 7861  .            exa
+0000b130: 6d70 6c65 2c20 6060 456e 7465 7220 6120  mple, ``Enter a 
+0000b140: 6e75 6d62 6572 2066 726f 6d20 3020 746f  number from 0 to
+0000b150: 2031 3030 6060 2e0a 0a20 2020 2020 2020   100``...       
+0000b160: 2020 2020 2060 476f 6f67 6c65 2043 6861       `Google Cha
+0000b170: 740a 2020 2020 2020 2020 2020 2020 6170  t.            ap
+0000b180: 7073 203c 6874 7470 733a 2f2f 6465 7665  ps <https://deve
+0000b190: 6c6f 7065 7273 2e67 6f6f 676c 652e 636f  lopers.google.co
+0000b1a0: 6d2f 776f 726b 7370 6163 652f 6368 6174  m/workspace/chat
+0000b1b0: 3e60 5f5f 3a0a 2020 2020 2222 220a 0a20  >`__:.    """.. 
+0000b1c0: 2020 2063 6c61 7373 2054 7970 6528 7072     class Type(pr
+0000b1d0: 6f74 6f2e 456e 756d 293a 0a20 2020 2020  oto.Enum):.     
+0000b1e0: 2020 2072 2222 2248 6f77 2061 2074 6578     r"""How a tex
+0000b1f0: 7420 696e 7075 7420 6669 656c 6420 6170  t input field ap
+0000b200: 7065 6172 7320 696e 2074 6865 2075 7365  pears in the use
+0000b210: 7220 696e 7465 7266 6163 652e 2046 6f72  r interface. For
+0000b220: 2065 7861 6d70 6c65 2c0a 2020 2020 2020   example,.      
+0000b230: 2020 7768 6574 6865 7220 6974 2773 2061    whether it's a
+0000b240: 2073 696e 676c 6520 6c69 6e65 2069 6e70   single line inp
+0000b250: 7574 2066 6965 6c64 2c20 6f72 2061 206d  ut field, or a m
+0000b260: 756c 7469 2d6c 696e 6520 696e 7075 742e  ulti-line input.
+0000b270: 2049 660a 2020 2020 2020 2020 6060 696e   If.        ``in
+0000b280: 6974 6961 6c53 7567 6765 7374 696f 6e73  itialSuggestions
+0000b290: 6060 2069 7320 7370 6563 6966 6965 642c  `` is specified,
+0000b2a0: 2060 6074 7970 6560 6020 6973 2061 6c77   ``type`` is alw
+0000b2b0: 6179 730a 2020 2020 2020 2020 6060 5349  ays.        ``SI
+0000b2c0: 4e47 4c45 5f4c 494e 4560 602c 2065 7665  NGLE_LINE``, eve
+0000b2d0: 6e20 6966 2069 7427 7320 7365 7420 746f  n if it's set to
+0000b2e0: 2060 604d 554c 5449 504c 455f 4c49 4e45   ``MULTIPLE_LINE
+0000b2f0: 6060 2e0a 0a20 2020 2020 2020 2060 476f  ``...        `Go
+0000b300: 6f67 6c65 2057 6f72 6b73 7061 6365 2041  ogle Workspace A
+0000b310: 6464 2d6f 6e73 2061 6e64 2043 6861 740a  dd-ons and Chat.
+0000b320: 2020 2020 2020 2020 6170 7073 203c 6874          apps <ht
+0000b330: 7470 733a 2f2f 6465 7665 6c6f 7065 7273  tps://developers
+0000b340: 2e67 6f6f 676c 652e 636f 6d2f 776f 726b  .google.com/work
+0000b350: 7370 6163 652f 6578 7465 6e64 3e60 5f5f  space/extend>`__
+0000b360: 3a0a 0a20 2020 2020 2020 2056 616c 7565  :..        Value
+0000b370: 733a 0a20 2020 2020 2020 2020 2020 2053  s:.            S
+0000b380: 494e 474c 455f 4c49 4e45 2028 3029 3a0a  INGLE_LINE (0):.
+0000b390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b3a0: 5468 6520 7465 7874 2069 6e70 7574 2066  The text input f
+0000b3b0: 6965 6c64 2068 6173 2061 2066 6978 6564  ield has a fixed
+0000b3c0: 2068 6569 6768 7420 6f66 0a20 2020 2020   height of.     
+0000b3d0: 2020 2020 2020 2020 2020 206f 6e65 206c             one l
+0000b3e0: 696e 652e 0a20 2020 2020 2020 2020 2020  ine..           
+0000b3f0: 204d 554c 5449 504c 455f 4c49 4e45 2028   MULTIPLE_LINE (
+0000b400: 3129 3a0a 2020 2020 2020 2020 2020 2020  1):.            
+0000b410: 2020 2020 5468 6520 7465 7874 2069 6e70      The text inp
+0000b420: 7574 2066 6965 6c64 2068 6173 2061 2066  ut field has a f
+0000b430: 6978 6564 2068 6569 6768 7420 6f66 0a20  ixed height of. 
+0000b440: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0000b450: 756c 7469 706c 6520 6c69 6e65 732e 0a20  ultiple lines.. 
+0000b460: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000b470: 2020 2053 494e 474c 455f 4c49 4e45 203d     SINGLE_LINE =
+0000b480: 2030 0a20 2020 2020 2020 204d 554c 5449   0.        MULTI
+0000b490: 504c 455f 4c49 4e45 203d 2031 0a0a 2020  PLE_LINE = 1..  
+0000b4a0: 2020 6e61 6d65 3a20 7374 7220 3d20 7072    name: str = pr
+0000b4b0: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
+0000b4c0: 2020 2070 726f 746f 2e53 5452 494e 472c     proto.STRING,
+0000b4d0: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
+0000b4e0: 312c 0a20 2020 2029 0a20 2020 206c 6162  1,.    ).    lab
+0000b4f0: 656c 3a20 7374 7220 3d20 7072 6f74 6f2e  el: str = proto.
+0000b500: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
+0000b510: 726f 746f 2e53 5452 494e 472c 0a20 2020  roto.STRING,.   
+0000b520: 2020 2020 206e 756d 6265 723d 322c 0a20       number=2,. 
+0000b530: 2020 2029 0a20 2020 2068 696e 745f 7465     ).    hint_te
+0000b540: 7874 3a20 7374 7220 3d20 7072 6f74 6f2e  xt: str = proto.
+0000b550: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
+0000b560: 726f 746f 2e53 5452 494e 472c 0a20 2020  roto.STRING,.   
+0000b570: 2020 2020 206e 756d 6265 723d 332c 0a20       number=3,. 
+0000b580: 2020 2029 0a20 2020 2076 616c 7565 3a20     ).    value: 
+0000b590: 7374 7220 3d20 7072 6f74 6f2e 4669 656c  str = proto.Fiel
+0000b5a0: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
+0000b5b0: 2e53 5452 494e 472c 0a20 2020 2020 2020  .STRING,.       
+0000b5c0: 206e 756d 6265 723d 342c 0a20 2020 2029   number=4,.    )
+0000b5d0: 0a20 2020 2074 7970 655f 3a20 5479 7065  .    type_: Type
+0000b5e0: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
+0000b5f0: 2020 2020 2020 2020 7072 6f74 6f2e 454e          proto.EN
+0000b600: 554d 2c0a 2020 2020 2020 2020 6e75 6d62  UM,.        numb
+0000b610: 6572 3d35 2c0a 2020 2020 2020 2020 656e  er=5,.        en
+0000b620: 756d 3d54 7970 652c 0a20 2020 2029 0a20  um=Type,.    ). 
+0000b630: 2020 206f 6e5f 6368 616e 6765 5f61 6374     on_change_act
+0000b640: 696f 6e3a 2022 4163 7469 6f6e 2220 3d20  ion: "Action" = 
+0000b650: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
+0000b660: 2020 2020 2070 726f 746f 2e4d 4553 5341       proto.MESSA
+0000b670: 4745 2c0a 2020 2020 2020 2020 6e75 6d62  GE,.        numb
+0000b680: 6572 3d36 2c0a 2020 2020 2020 2020 6d65  er=6,.        me
+0000b690: 7373 6167 653d 2241 6374 696f 6e22 2c0a  ssage="Action",.
+0000b6a0: 2020 2020 290a 2020 2020 696e 6974 6961      ).    initia
+0000b6b0: 6c5f 7375 6767 6573 7469 6f6e 733a 2022  l_suggestions: "
+0000b6c0: 5375 6767 6573 7469 6f6e 7322 203d 2070  Suggestions" = p
+0000b6d0: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
+0000b6e0: 2020 2020 7072 6f74 6f2e 4d45 5353 4147      proto.MESSAG
+0000b6f0: 452c 0a20 2020 2020 2020 206e 756d 6265  E,.        numbe
+0000b700: 723d 372c 0a20 2020 2020 2020 206d 6573  r=7,.        mes
+0000b710: 7361 6765 3d22 5375 6767 6573 7469 6f6e  sage="Suggestion
+0000b720: 7322 2c0a 2020 2020 290a 2020 2020 6175  s",.    ).    au
+0000b730: 746f 5f63 6f6d 706c 6574 655f 6163 7469  to_complete_acti
+0000b740: 6f6e 3a20 2241 6374 696f 6e22 203d 2070  on: "Action" = p
+0000b750: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
+0000b760: 2020 2020 7072 6f74 6f2e 4d45 5353 4147      proto.MESSAG
+0000b770: 452c 0a20 2020 2020 2020 206e 756d 6265  E,.        numbe
+0000b780: 723d 382c 0a20 2020 2020 2020 206d 6573  r=8,.        mes
+0000b790: 7361 6765 3d22 4163 7469 6f6e 222c 0a20  sage="Action",. 
+0000b7a0: 2020 2029 0a20 2020 2070 6c61 6365 686f     ).    placeho
+0000b7b0: 6c64 6572 5f74 6578 743a 2073 7472 203d  lder_text: str =
+0000b7c0: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
+0000b7d0: 2020 2020 2020 7072 6f74 6f2e 5354 5249        proto.STRI
+0000b7e0: 4e47 2c0a 2020 2020 2020 2020 6e75 6d62  NG,.        numb
+0000b7f0: 6572 3d31 322c 0a20 2020 2029 0a0a 0a63  er=12,.    )...c
+0000b800: 6c61 7373 2053 7567 6765 7374 696f 6e73  lass Suggestions
+0000b810: 2870 726f 746f 2e4d 6573 7361 6765 293a  (proto.Message):
+0000b820: 0a20 2020 2072 2222 2253 7567 6765 7374  .    r"""Suggest
+0000b830: 6564 2076 616c 7565 7320 7468 6174 2075  ed values that u
+0000b840: 7365 7273 2063 616e 2065 6e74 6572 2e20  sers can enter. 
+0000b850: 5468 6573 6520 7661 6c75 6573 2061 7070  These values app
+0000b860: 6561 7220 7768 656e 0a20 2020 2075 7365  ear when.    use
+0000b870: 7273 2063 6c69 636b 2069 6e73 6964 6520  rs click inside 
+0000b880: 7468 6520 7465 7874 2069 6e70 7574 2066  the text input f
+0000b890: 6965 6c64 2e20 4173 2075 7365 7273 2074  ield. As users t
+0000b8a0: 7970 652c 2074 6865 0a20 2020 2073 7567  ype, the.    sug
+0000b8b0: 6765 7374 6564 2076 616c 7565 7320 6479  gested values dy
+0000b8c0: 6e61 6d69 6361 6c6c 7920 6669 6c74 6572  namically filter
+0000b8d0: 2074 6f20 6d61 7463 6820 7768 6174 2074   to match what t
+0000b8e0: 6865 2075 7365 7273 2068 6176 650a 2020  he users have.  
+0000b8f0: 2020 7479 7065 642e 0a0a 2020 2020 466f    typed...    Fo
+0000b900: 7220 6578 616d 706c 652c 2061 2074 6578  r example, a tex
+0000b910: 7420 696e 7075 7420 6669 656c 6420 666f  t input field fo
+0000b920: 7220 7072 6f67 7261 6d6d 696e 6720 6c61  r programming la
+0000b930: 6e67 7561 6765 206d 6967 6874 0a20 2020  nguage might.   
+0000b940: 2073 7567 6765 7374 204a 6176 612c 204a   suggest Java, J
+0000b950: 6176 6153 6372 6970 742c 2050 7974 686f  avaScript, Pytho
+0000b960: 6e2c 2061 6e64 2043 2b2b 2e20 5768 656e  n, and C++. When
+0000b970: 2075 7365 7273 2073 7461 7274 2074 7970   users start typ
+0000b980: 696e 670a 2020 2020 6060 4a61 7660 602c  ing.    ``Jav``,
+0000b990: 2074 6865 206c 6973 7420 6f66 2073 7567   the list of sug
+0000b9a0: 6765 7374 696f 6e73 2066 696c 7465 7273  gestions filters
+0000b9b0: 2074 6f20 7368 6f77 2060 604a 6176 6160   to show ``Java`
+0000b9c0: 6020 616e 640a 2020 2020 6060 4a61 7661  ` and.    ``Java
+0000b9d0: 5363 7269 7074 6060 2e0a 0a20 2020 2053  Script``...    S
+0000b9e0: 7567 6765 7374 6564 2076 616c 7565 7320  uggested values 
+0000b9f0: 6865 6c70 2067 7569 6465 2075 7365 7273  help guide users
+0000ba00: 2074 6f20 656e 7465 7220 7661 6c75 6573   to enter values
+0000ba10: 2074 6861 7420 796f 7572 2061 7070 2063   that your app c
+0000ba20: 616e 0a20 2020 206d 616b 6520 7365 6e73  an.    make sens
+0000ba30: 6520 6f66 2e20 5768 656e 2072 6566 6572  e of. When refer
+0000ba40: 7269 6e67 2074 6f20 4a61 7661 5363 7269  ring to JavaScri
+0000ba50: 7074 2c20 736f 6d65 2075 7365 7273 206d  pt, some users m
+0000ba60: 6967 6874 2065 6e74 6572 0a20 2020 2060  ight enter.    `
+0000ba70: 606a 6176 6173 6372 6970 7460 6020 616e  `javascript`` an
+0000ba80: 6420 6f74 6865 7273 2060 606a 6176 6120  d others ``java 
+0000ba90: 7363 7269 7074 6060 2e20 5375 6767 6573  script``. Sugges
+0000baa0: 7469 6e67 2060 604a 6176 6153 6372 6970  ting ``JavaScrip
+0000bab0: 7460 600a 2020 2020 6361 6e20 7374 616e  t``.    can stan
+0000bac0: 6461 7264 697a 6520 686f 7720 7573 6572  dardize how user
+0000bad0: 7320 696e 7465 7261 6374 2077 6974 6820  s interact with 
+0000bae0: 796f 7572 2061 7070 2e0a 0a20 2020 2057  your app...    W
+0000baf0: 6865 6e20 7370 6563 6966 6965 642c 2060  hen specified, `
+0000bb00: 6054 6578 7449 6e70 7574 2e74 7970 6560  `TextInput.type`
+0000bb10: 6020 6973 2061 6c77 6179 7320 6060 5349  ` is always ``SI
+0000bb20: 4e47 4c45 5f4c 494e 4560 602c 2065 7665  NGLE_LINE``, eve
+0000bb30: 6e0a 2020 2020 6966 2069 7427 7320 7365  n.    if it's se
+0000bb40: 7420 746f 2060 604d 554c 5449 504c 455f  t to ``MULTIPLE_
+0000bb50: 4c49 4e45 6060 2e0a 0a20 2020 2060 476f  LINE``...    `Go
+0000bb60: 6f67 6c65 2057 6f72 6b73 7061 6365 2041  ogle Workspace A
+0000bb70: 6464 2d6f 6e73 2061 6e64 2043 6861 740a  dd-ons and Chat.
+0000bb80: 2020 2020 6170 7073 203c 6874 7470 733a      apps <https:
+0000bb90: 2f2f 6465 7665 6c6f 7065 7273 2e67 6f6f  //developers.goo
+0000bba0: 676c 652e 636f 6d2f 776f 726b 7370 6163  gle.com/workspac
+0000bbb0: 652f 6578 7465 6e64 3e60 5f5f 3a0a 0a20  e/extend>`__:.. 
+0000bbc0: 2020 2041 7474 7269 6275 7465 733a 0a20     Attributes:. 
+0000bbd0: 2020 2020 2020 2069 7465 6d73 2028 4d75         items (Mu
+0000bbe0: 7461 626c 6553 6571 7565 6e63 655b 676f  tableSequence[go
+0000bbf0: 6f67 6c65 2e61 7070 732e 6361 7264 5f76  ogle.apps.card_v
+0000bc00: 312e 7479 7065 732e 5375 6767 6573 7469  1.types.Suggesti
+0000bc10: 6f6e 732e 5375 6767 6573 7469 6f6e 4974  ons.SuggestionIt
+0000bc20: 656d 5d29 3a0a 2020 2020 2020 2020 2020  em]):.          
+0000bc30: 2020 4120 6c69 7374 206f 6620 7375 6767    A list of sugg
+0000bc40: 6573 7469 6f6e 7320 7573 6564 2066 6f72  estions used for
+0000bc50: 2061 7574 6f63 6f6d 706c 6574 650a 2020   autocomplete.  
+0000bc60: 2020 2020 2020 2020 2020 7265 636f 6d6d            recomm
+0000bc70: 656e 6461 7469 6f6e 7320 696e 2074 6578  endations in tex
+0000bc80: 7420 696e 7075 7420 6669 656c 6473 2e0a  t input fields..
+0000bc90: 2020 2020 2222 220a 0a20 2020 2063 6c61      """..    cla
+0000bca0: 7373 2053 7567 6765 7374 696f 6e49 7465  ss SuggestionIte
+0000bcb0: 6d28 7072 6f74 6f2e 4d65 7373 6167 6529  m(proto.Message)
+0000bcc0: 3a0a 2020 2020 2020 2020 7222 2222 4f6e  :.        r"""On
+0000bcd0: 6520 7375 6767 6573 7465 6420 7661 6c75  e suggested valu
+0000bce0: 6520 7468 6174 2075 7365 7273 2063 616e  e that users can
+0000bcf0: 2065 6e74 6572 2069 6e20 6120 7465 7874   enter in a text
+0000bd00: 2069 6e70 7574 2066 6965 6c64 2e0a 0a20   input field... 
+0000bd10: 2020 2020 2020 2060 476f 6f67 6c65 2057         `Google W
+0000bd20: 6f72 6b73 7061 6365 2041 6464 2d6f 6e73  orkspace Add-ons
+0000bd30: 2061 6e64 2043 6861 740a 2020 2020 2020   and Chat.      
+0000bd40: 2020 6170 7073 203c 6874 7470 733a 2f2f    apps <https://
+0000bd50: 6465 7665 6c6f 7065 7273 2e67 6f6f 676c  developers.googl
+0000bd60: 652e 636f 6d2f 776f 726b 7370 6163 652f  e.com/workspace/
+0000bd70: 6578 7465 6e64 3e60 5f5f 3a0a 0a0a 2020  extend>`__:...  
+0000bd80: 2020 2020 2020 2e2e 205f 6f6e 656f 663a        .. _oneof:
+0000bd90: 2068 7474 7073 3a2f 2f70 726f 746f 2d70   https://proto-p
+0000bda0: 6c75 732d 7079 7468 6f6e 2e72 6561 6474  lus-python.readt
+0000bdb0: 6865 646f 6373 2e69 6f2f 656e 2f73 7461  hedocs.io/en/sta
+0000bdc0: 626c 652f 6669 656c 6473 2e68 746d 6c23  ble/fields.html#
+0000bdd0: 6f6e 656f 6673 2d6d 7574 7561 6c6c 792d  oneofs-mutually-
+0000bde0: 6578 636c 7573 6976 652d 6669 656c 6473  exclusive-fields
+0000bdf0: 0a0a 2020 2020 2020 2020 4174 7472 6962  ..        Attrib
+0000be00: 7574 6573 3a0a 2020 2020 2020 2020 2020  utes:.          
+0000be10: 2020 7465 7874 2028 7374 7229 3a0a 2020    text (str):.  
+0000be20: 2020 2020 2020 2020 2020 2020 2020 5468                Th
+0000be30: 6520 7661 6c75 6520 6f66 2061 2073 7567  e value of a sug
+0000be40: 6765 7374 6564 2069 6e70 7574 2074 6f20  gested input to 
+0000be50: 6120 7465 7874 0a20 2020 2020 2020 2020  a text.         
+0000be60: 2020 2020 2020 2069 6e70 7574 2066 6965         input fie
+0000be70: 6c64 2e20 5468 6973 2069 7320 6571 7569  ld. This is equi
+0000be80: 7661 6c65 6e74 2074 6f20 7768 6174 2075  valent to what u
+0000be90: 7365 7273 0a20 2020 2020 2020 2020 2020  sers.           
+0000bea0: 2020 2020 2065 6e74 6572 2074 6865 6d73       enter thems
+0000beb0: 656c 7665 732e 0a0a 2020 2020 2020 2020  elves...        
+0000bec0: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
+0000bed0: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
+0000bee0: 6620 606f 6e65 6f66 605f 2060 6063 6f6e  f `oneof`_ ``con
+0000bef0: 7465 6e74 6060 2e0a 2020 2020 2020 2020  tent``..        
+0000bf00: 2222 220a 0a20 2020 2020 2020 2074 6578  """..        tex
+0000bf10: 743a 2073 7472 203d 2070 726f 746f 2e46  t: str = proto.F
+0000bf20: 6965 6c64 280a 2020 2020 2020 2020 2020  ield(.          
+0000bf30: 2020 7072 6f74 6f2e 5354 5249 4e47 2c0a    proto.STRING,.
+0000bf40: 2020 2020 2020 2020 2020 2020 6e75 6d62              numb
+0000bf50: 6572 3d31 2c0a 2020 2020 2020 2020 2020  er=1,.          
+0000bf60: 2020 6f6e 656f 663d 2263 6f6e 7465 6e74    oneof="content
+0000bf70: 222c 0a20 2020 2020 2020 2029 0a0a 2020  ",.        )..  
+0000bf80: 2020 6974 656d 733a 204d 7574 6162 6c65    items: Mutable
+0000bf90: 5365 7175 656e 6365 5b53 7567 6765 7374  Sequence[Suggest
+0000bfa0: 696f 6e49 7465 6d5d 203d 2070 726f 746f  ionItem] = proto
+0000bfb0: 2e52 6570 6561 7465 6446 6965 6c64 280a  .RepeatedField(.
+0000bfc0: 2020 2020 2020 2020 7072 6f74 6f2e 4d45          proto.ME
+0000bfd0: 5353 4147 452c 0a20 2020 2020 2020 206e  SSAGE,.        n
+0000bfe0: 756d 6265 723d 312c 0a20 2020 2020 2020  umber=1,.       
+0000bff0: 206d 6573 7361 6765 3d53 7567 6765 7374   message=Suggest
+0000c000: 696f 6e49 7465 6d2c 0a20 2020 2029 0a0a  ionItem,.    )..
+0000c010: 0a63 6c61 7373 2042 7574 746f 6e4c 6973  .class ButtonLis
+0000c020: 7428 7072 6f74 6f2e 4d65 7373 6167 6529  t(proto.Message)
+0000c030: 3a0a 2020 2020 7222 2222 4120 6c69 7374  :.    r"""A list
+0000c040: 206f 6620 6275 7474 6f6e 7320 6c61 7965   of buttons laye
+0000c050: 6420 6f75 7420 686f 7269 7a6f 6e74 616c  d out horizontal
+0000c060: 6c79 2e20 466f 7220 616e 2065 7861 6d70  ly. For an examp
+0000c070: 6c65 2069 6e20 476f 6f67 6c65 0a20 2020  le in Google.   
+0000c080: 2043 6861 7420 6170 7073 2c20 7365 6520   Chat apps, see 
+0000c090: 6041 6464 2061 0a20 2020 2062 7574 746f  `Add a.    butto
+0000c0a0: 6e20 3c68 7474 7073 3a2f 2f64 6576 656c  n <https://devel
+0000c0b0: 6f70 6572 732e 676f 6f67 6c65 2e63 6f6d  opers.google.com
+0000c0c0: 2f77 6f72 6b73 7061 6365 2f63 6861 742f  /workspace/chat/
+0000c0d0: 6465 7369 676e 2d69 6e74 6572 6163 7469  design-interacti
+0000c0e0: 7665 2d63 6172 642d 6469 616c 6f67 2361  ve-card-dialog#a
+0000c0f0: 6464 5f61 5f62 7574 746f 6e3e 605f 5f2e  dd_a_button>`__.
+0000c100: 0a0a 2020 2020 6047 6f6f 676c 6520 576f  ..    `Google Wo
+0000c110: 726b 7370 6163 6520 4164 642d 6f6e 7320  rkspace Add-ons 
+0000c120: 616e 6420 4368 6174 0a20 2020 2061 7070  and Chat.    app
+0000c130: 7320 3c68 7474 7073 3a2f 2f64 6576 656c  s <https://devel
+0000c140: 6f70 6572 732e 676f 6f67 6c65 2e63 6f6d  opers.google.com
+0000c150: 2f77 6f72 6b73 7061 6365 2f65 7874 656e  /workspace/exten
+0000c160: 643e 605f 5f3a 0a0a 2020 2020 4174 7472  d>`__:..    Attr
+0000c170: 6962 7574 6573 3a0a 2020 2020 2020 2020  ibutes:.        
+0000c180: 6275 7474 6f6e 7320 284d 7574 6162 6c65  buttons (Mutable
+0000c190: 5365 7175 656e 6365 5b67 6f6f 676c 652e  Sequence[google.
+0000c1a0: 6170 7073 2e63 6172 645f 7631 2e74 7970  apps.card_v1.typ
+0000c1b0: 6573 2e42 7574 746f 6e5d 293a 0a20 2020  es.Button]):.   
+0000c1c0: 2020 2020 2020 2020 2041 6e20 6172 7261           An arra
+0000c1d0: 7920 6f66 2062 7574 746f 6e73 2e0a 2020  y of buttons..  
+0000c1e0: 2020 2222 220a 0a20 2020 2062 7574 746f    """..    butto
+0000c1f0: 6e73 3a20 4d75 7461 626c 6553 6571 7565  ns: MutableSeque
+0000c200: 6e63 655b 2242 7574 746f 6e22 5d20 3d20  nce["Button"] = 
+0000c210: 7072 6f74 6f2e 5265 7065 6174 6564 4669  proto.RepeatedFi
+0000c220: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
+0000c230: 746f 2e4d 4553 5341 4745 2c0a 2020 2020  to.MESSAGE,.    
+0000c240: 2020 2020 6e75 6d62 6572 3d31 2c0a 2020      number=1,.  
+0000c250: 2020 2020 2020 6d65 7373 6167 653d 2242        message="B
+0000c260: 7574 746f 6e22 2c0a 2020 2020 290a 0a0a  utton",.    )...
+0000c270: 636c 6173 7320 5365 6c65 6374 696f 6e49  class SelectionI
+0000c280: 6e70 7574 2870 726f 746f 2e4d 6573 7361  nput(proto.Messa
+0000c290: 6765 293a 0a20 2020 2072 2222 2241 2077  ge):.    r"""A w
+0000c2a0: 6964 6765 7420 7468 6174 2063 7265 6174  idget that creat
+0000c2b0: 6573 206f 6e65 206f 7220 6d6f 7265 2055  es one or more U
+0000c2c0: 4920 6974 656d 7320 7468 6174 2075 7365  I items that use
+0000c2d0: 7273 2063 616e 2073 656c 6563 742e 0a20  rs can select.. 
+0000c2e0: 2020 2046 6f72 2065 7861 6d70 6c65 2c20     For example, 
+0000c2f0: 6120 6472 6f70 646f 776e 206d 656e 7520  a dropdown menu 
+0000c300: 6f72 2063 6865 636b 626f 7865 732e 2059  or checkboxes. Y
+0000c310: 6f75 2063 616e 2075 7365 2074 6869 7320  ou can use this 
+0000c320: 7769 6467 6574 0a20 2020 2074 6f20 636f  widget.    to co
+0000c330: 6c6c 6563 7420 6461 7461 2074 6861 7420  llect data that 
+0000c340: 6361 6e20 6265 2070 7265 6469 6374 6564  can be predicted
+0000c350: 206f 7220 656e 756d 6572 6174 6564 2e20   or enumerated. 
+0000c360: 466f 7220 616e 2065 7861 6d70 6c65 0a20  For an example. 
+0000c370: 2020 2069 6e20 476f 6f67 6c65 2043 6861     in Google Cha
+0000c380: 7420 6170 7073 2c20 7365 6520 6041 6464  t apps, see `Add
+0000c390: 2073 656c 6563 7461 626c 6520 5549 0a20   selectable UI. 
+0000c3a0: 2020 2065 6c65 6d65 6e74 7320 3c2f 776f     elements </wo
+0000c3b0: 726b 7370 6163 652f 6368 6174 2f64 6573  rkspace/chat/des
+0000c3c0: 6967 6e2d 696e 7465 7261 6374 6976 652d  ign-interactive-
+0000c3d0: 6361 7264 2d64 6961 6c6f 6723 6164 645f  card-dialog#add_
+0000c3e0: 7365 6c65 6374 6162 6c65 5f75 695f 656c  selectable_ui_el
+0000c3f0: 656d 656e 7473 3e60 5f5f 2e0a 0a20 2020  ements>`__...   
+0000c400: 2043 6861 7420 6170 7073 2063 616e 2070   Chat apps can p
+0000c410: 726f 6365 7373 2074 6865 2076 616c 7565  rocess the value
+0000c420: 206f 6620 6974 656d 7320 7468 6174 2075   of items that u
+0000c430: 7365 7273 2073 656c 6563 7420 6f72 2069  sers select or i
+0000c440: 6e70 7574 2e0a 2020 2020 466f 7220 6465  nput..    For de
+0000c450: 7461 696c 7320 6162 6f75 7420 776f 726b  tails about work
+0000c460: 696e 6720 7769 7468 2066 6f72 6d20 696e  ing with form in
+0000c470: 7075 7473 2c20 7365 6520 6052 6563 6569  puts, see `Recei
+0000c480: 7665 2066 6f72 6d0a 2020 2020 6461 7461  ve form.    data
+0000c490: 203c 6874 7470 733a 2f2f 6465 7665 6c6f   <https://develo
+0000c4a0: 7065 7273 2e67 6f6f 676c 652e 636f 6d2f  pers.google.com/
+0000c4b0: 776f 726b 7370 6163 652f 6368 6174 2f72  workspace/chat/r
+0000c4c0: 6561 642d 666f 726d 2d64 6174 613e 605f  ead-form-data>`_
+0000c4d0: 5f2e 0a0a 2020 2020 546f 2063 6f6c 6c65  _...    To colle
+0000c4e0: 6374 2075 6e64 6566 696e 6564 206f 7220  ct undefined or 
+0000c4f0: 6162 7374 7261 6374 2064 6174 6120 6672  abstract data fr
+0000c500: 6f6d 2075 7365 7273 2c20 7573 6520 7468  om users, use th
+0000c510: 650a 2020 2020 5b54 6578 7449 6e70 7574  e.    [TextInput
+0000c520: 5d5b 676f 6f67 6c65 2e61 7070 732e 6361  ][google.apps.ca
+0000c530: 7264 2e76 312e 5465 7874 496e 7075 745d  rd.v1.TextInput]
+0000c540: 2077 6964 6765 742e 0a0a 2020 2020 6047   widget...    `G
+0000c550: 6f6f 676c 6520 576f 726b 7370 6163 6520  oogle Workspace 
+0000c560: 4164 642d 6f6e 7320 616e 6420 4368 6174  Add-ons and Chat
+0000c570: 0a20 2020 2061 7070 7320 3c68 7474 7073  .    apps <https
+0000c580: 3a2f 2f64 6576 656c 6f70 6572 732e 676f  ://developers.go
+0000c590: 6f67 6c65 2e63 6f6d 2f77 6f72 6b73 7061  ogle.com/workspa
+0000c5a0: 6365 2f65 7874 656e 643e 605f 5f3a 0a0a  ce/extend>`__:..
+0000c5b0: 2020 2020 5468 6973 206d 6573 7361 6765      This message
+0000c5c0: 2068 6173 2060 6f6e 656f 6660 5f20 6669   has `oneof`_ fi
+0000c5d0: 656c 6473 2028 6d75 7475 616c 6c79 2065  elds (mutually e
+0000c5e0: 7863 6c75 7369 7665 2066 6965 6c64 7329  xclusive fields)
+0000c5f0: 2e0a 2020 2020 466f 7220 6561 6368 206f  ..    For each o
+0000c600: 6e65 6f66 2c20 6174 206d 6f73 7420 6f6e  neof, at most on
+0000c610: 6520 6d65 6d62 6572 2066 6965 6c64 2063  e member field c
+0000c620: 616e 2062 6520 7365 7420 6174 2074 6865  an be set at the
+0000c630: 2073 616d 6520 7469 6d65 2e0a 2020 2020   same time..    
+0000c640: 5365 7474 696e 6720 616e 7920 6d65 6d62  Setting any memb
+0000c650: 6572 206f 6620 7468 6520 6f6e 656f 6620  er of the oneof 
+0000c660: 6175 746f 6d61 7469 6361 6c6c 7920 636c  automatically cl
+0000c670: 6561 7273 2061 6c6c 206f 7468 6572 0a20  ears all other. 
+0000c680: 2020 206d 656d 6265 7273 2e0a 0a20 2020     members...   
+0000c690: 202e 2e20 5f6f 6e65 6f66 3a20 6874 7470   .. _oneof: http
+0000c6a0: 733a 2f2f 7072 6f74 6f2d 706c 7573 2d70  s://proto-plus-p
+0000c6b0: 7974 686f 6e2e 7265 6164 7468 6564 6f63  ython.readthedoc
+0000c6c0: 732e 696f 2f65 6e2f 7374 6162 6c65 2f66  s.io/en/stable/f
+0000c6d0: 6965 6c64 732e 6874 6d6c 236f 6e65 6f66  ields.html#oneof
+0000c6e0: 732d 6d75 7475 616c 6c79 2d65 7863 6c75  s-mutually-exclu
+0000c6f0: 7369 7665 2d66 6965 6c64 730a 0a20 2020  sive-fields..   
+0000c700: 2041 7474 7269 6275 7465 733a 0a20 2020   Attributes:.   
+0000c710: 2020 2020 206e 616d 6520 2873 7472 293a       name (str):
+0000c720: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
+0000c730: 206e 616d 6520 7468 6174 2069 6465 6e74   name that ident
+0000c740: 6966 6965 7320 7468 6520 7365 6c65 6374  ifies the select
+0000c750: 696f 6e20 696e 7075 7420 696e 2061 2066  ion input in a f
+0000c760: 6f72 6d20 696e 7075 740a 2020 2020 2020  orm input.      
+0000c770: 2020 2020 2020 6576 656e 742e 0a0a 2020        event...  
+0000c780: 2020 2020 2020 2020 2020 466f 7220 6465            For de
+0000c790: 7461 696c 7320 6162 6f75 7420 776f 726b  tails about work
+0000c7a0: 696e 6720 7769 7468 2066 6f72 6d20 696e  ing with form in
+0000c7b0: 7075 7473 2c20 7365 6520 6052 6563 6569  puts, see `Recei
+0000c7c0: 7665 0a20 2020 2020 2020 2020 2020 2066  ve.            f
+0000c7d0: 6f72 6d0a 2020 2020 2020 2020 2020 2020  orm.            
+0000c7e0: 6461 7461 203c 6874 7470 733a 2f2f 6465  data <https://de
+0000c7f0: 7665 6c6f 7065 7273 2e67 6f6f 676c 652e  velopers.google.
+0000c800: 636f 6d2f 776f 726b 7370 6163 652f 6368  com/workspace/ch
+0000c810: 6174 2f72 6561 642d 666f 726d 2d64 6174  at/read-form-dat
+0000c820: 613e 605f 5f2e 0a20 2020 2020 2020 206c  a>`__..        l
+0000c830: 6162 656c 2028 7374 7229 3a0a 2020 2020  abel (str):.    
+0000c840: 2020 2020 2020 2020 5468 6520 7465 7874          The text
+0000c850: 2074 6861 7420 6170 7065 6172 7320 6162   that appears ab
+0000c860: 6f76 6520 7468 6520 7365 6c65 6374 696f  ove the selectio
+0000c870: 6e0a 2020 2020 2020 2020 2020 2020 696e  n.            in
+0000c880: 7075 7420 6669 656c 6420 696e 2074 6865  put field in the
+0000c890: 2075 7365 7220 696e 7465 7266 6163 652e   user interface.
+0000c8a0: 0a0a 2020 2020 2020 2020 2020 2020 5370  ..            Sp
+0000c8b0: 6563 6966 7920 7465 7874 2074 6861 7420  ecify text that 
+0000c8c0: 6865 6c70 7320 7468 6520 7573 6572 2065  helps the user e
+0000c8d0: 6e74 6572 2074 6865 0a20 2020 2020 2020  nter the.       
+0000c8e0: 2020 2020 2069 6e66 6f72 6d61 7469 6f6e       information
+0000c8f0: 2079 6f75 7220 6170 7020 6e65 6564 732e   your app needs.
+0000c900: 2046 6f72 2065 7861 6d70 6c65 2c20 6966   For example, if
+0000c910: 0a20 2020 2020 2020 2020 2020 2075 7365  .            use
+0000c920: 7273 2061 7265 2073 656c 6563 7469 6e67  rs are selecting
+0000c930: 2074 6865 2075 7267 656e 6379 206f 6620   the urgency of 
+0000c940: 6120 776f 726b 2074 6963 6b65 740a 2020  a work ticket.  
+0000c950: 2020 2020 2020 2020 2020 6672 6f6d 2061            from a
+0000c960: 2064 726f 702d 646f 776e 206d 656e 752c   drop-down menu,
+0000c970: 2074 6865 206c 6162 656c 206d 6967 6874   the label might
+0000c980: 2062 650a 2020 2020 2020 2020 2020 2020   be.            
+0000c990: 2255 7267 656e 6379 2220 6f72 2022 5365  "Urgency" or "Se
+0000c9a0: 6c65 6374 2075 7267 656e 6379 222e 0a20  lect urgency".. 
+0000c9b0: 2020 2020 2020 2074 7970 655f 2028 676f         type_ (go
+0000c9c0: 6f67 6c65 2e61 7070 732e 6361 7264 5f76  ogle.apps.card_v
+0000c9d0: 312e 7479 7065 732e 5365 6c65 6374 696f  1.types.Selectio
+0000c9e0: 6e49 6e70 7574 2e53 656c 6563 7469 6f6e  nInput.Selection
+0000c9f0: 5479 7065 293a 0a20 2020 2020 2020 2020  Type):.         
+0000ca00: 2020 2054 6865 2074 7970 6520 6f66 2069     The type of i
+0000ca10: 7465 6d73 2074 6861 7420 6172 6520 6469  tems that are di
+0000ca20: 7370 6c61 7965 6420 746f 2075 7365 7273  splayed to users
+0000ca30: 2069 6e20 610a 2020 2020 2020 2020 2020   in a.          
+0000ca40: 2020 6060 5365 6c65 6374 696f 6e49 6e70    ``SelectionInp
+0000ca50: 7574 6060 2077 6964 6765 742e 2053 656c  ut`` widget. Sel
+0000ca60: 6563 7469 6f6e 2074 7970 6573 2073 7570  ection types sup
+0000ca70: 706f 7274 2064 6966 6665 7265 6e74 0a20  port different. 
+0000ca80: 2020 2020 2020 2020 2020 2074 7970 6573             types
+0000ca90: 206f 6620 696e 7465 7261 6374 696f 6e73   of interactions
+0000caa0: 2e20 466f 7220 6578 616d 706c 652c 2075  . For example, u
+0000cab0: 7365 7273 2063 616e 2073 656c 6563 7420  sers can select 
+0000cac0: 6f6e 6520 6f72 0a20 2020 2020 2020 2020  one or.         
+0000cad0: 2020 206d 6f72 6520 6368 6563 6b62 6f78     more checkbox
+0000cae0: 6573 2c20 6275 7420 7468 6579 2063 616e  es, but they can
+0000caf0: 206f 6e6c 7920 7365 6c65 6374 206f 6e65   only select one
+0000cb00: 2076 616c 7565 2066 726f 6d20 610a 2020   value from a.  
+0000cb10: 2020 2020 2020 2020 2020 6472 6f70 646f            dropdo
+0000cb20: 776e 206d 656e 752e 0a20 2020 2020 2020  wn menu..       
+0000cb30: 2069 7465 6d73 2028 4d75 7461 626c 6553   items (MutableS
+0000cb40: 6571 7565 6e63 655b 676f 6f67 6c65 2e61  equence[google.a
+0000cb50: 7070 732e 6361 7264 5f76 312e 7479 7065  pps.card_v1.type
+0000cb60: 732e 5365 6c65 6374 696f 6e49 6e70 7574  s.SelectionInput
+0000cb70: 2e53 656c 6563 7469 6f6e 4974 656d 5d29  .SelectionItem])
+0000cb80: 3a0a 2020 2020 2020 2020 2020 2020 416e  :.            An
+0000cb90: 2061 7272 6179 206f 6620 7365 6c65 6374   array of select
+0000cba0: 6162 6c65 2069 7465 6d73 2e20 466f 7220  able items. For 
+0000cbb0: 6578 616d 706c 652c 2061 6e0a 2020 2020  example, an.    
+0000cbc0: 2020 2020 2020 2020 6172 7261 7920 6f66          array of
+0000cbd0: 2072 6164 696f 2062 7574 746f 6e73 206f   radio buttons o
+0000cbe0: 7220 6368 6563 6b62 6f78 6573 2e20 5375  r checkboxes. Su
+0000cbf0: 7070 6f72 7473 0a20 2020 2020 2020 2020  pports.         
+0000cc00: 2020 2075 7020 746f 2031 3030 2069 7465     up to 100 ite
+0000cc10: 6d73 2e0a 2020 2020 2020 2020 6f6e 5f63  ms..        on_c
+0000cc20: 6861 6e67 655f 6163 7469 6f6e 2028 676f  hange_action (go
+0000cc30: 6f67 6c65 2e61 7070 732e 6361 7264 5f76  ogle.apps.card_v
+0000cc40: 312e 7479 7065 732e 4163 7469 6f6e 293a  1.types.Action):
+0000cc50: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
+0000cc60: 7370 6563 6966 6965 642c 2074 6865 2066  specified, the f
+0000cc70: 6f72 6d20 6973 2073 7562 6d69 7474 6564  orm is submitted
+0000cc80: 2077 6865 6e20 7468 6520 7365 6c65 6374   when the select
+0000cc90: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
+0000cca0: 6368 616e 6765 732e 2049 6620 6e6f 7420  changes. If not 
+0000ccb0: 7370 6563 6966 6965 642c 2079 6f75 206d  specified, you m
+0000ccc0: 7573 7420 7370 6563 6966 7920 6120 7365  ust specify a se
+0000ccd0: 7061 7261 7465 0a20 2020 2020 2020 2020  parate.         
+0000cce0: 2020 2062 7574 746f 6e20 7468 6174 2073     button that s
+0000ccf0: 7562 6d69 7473 2074 6865 2066 6f72 6d2e  ubmits the form.
+0000cd00: 0a0a 2020 2020 2020 2020 2020 2020 466f  ..            Fo
+0000cd10: 7220 6465 7461 696c 7320 6162 6f75 7420  r details about 
+0000cd20: 776f 726b 696e 6720 7769 7468 2066 6f72  working with for
+0000cd30: 6d20 696e 7075 7473 2c20 7365 6520 6052  m inputs, see `R
+0000cd40: 6563 6569 7665 0a20 2020 2020 2020 2020  eceive.         
+0000cd50: 2020 2066 6f72 6d0a 2020 2020 2020 2020     form.        
+0000cd60: 2020 2020 6461 7461 203c 6874 7470 733a      data <https:
+0000cd70: 2f2f 6465 7665 6c6f 7065 7273 2e67 6f6f  //developers.goo
+0000cd80: 676c 652e 636f 6d2f 776f 726b 7370 6163  gle.com/workspac
+0000cd90: 652f 6368 6174 2f72 6561 642d 666f 726d  e/chat/read-form
+0000cda0: 2d64 6174 613e 605f 5f2e 0a20 2020 2020  -data>`__..     
+0000cdb0: 2020 206d 756c 7469 5f73 656c 6563 745f     multi_select_
+0000cdc0: 6d61 785f 7365 6c65 6374 6564 5f69 7465  max_selected_ite
+0000cdd0: 6d73 2028 696e 7429 3a0a 2020 2020 2020  ms (int):.      
+0000cde0: 2020 2020 2020 466f 7220 6d75 6c74 6973        For multis
+0000cdf0: 656c 6563 7420 6d65 6e75 732c 2074 6865  elect menus, the
+0000ce00: 206d 6178 696d 756d 206e 756d 6265 7220   maximum number 
+0000ce10: 6f66 0a20 2020 2020 2020 2020 2020 2069  of.            i
+0000ce20: 7465 6d73 2074 6861 7420 6120 7573 6572  tems that a user
+0000ce30: 2063 616e 2073 656c 6563 742e 204d 696e   can select. Min
+0000ce40: 696d 756d 2076 616c 7565 2069 7320 310a  imum value is 1.
+0000ce50: 2020 2020 2020 2020 2020 2020 6974 656d              item
+0000ce60: 2e20 4966 2075 6e73 7065 6369 6669 6564  . If unspecified
+0000ce70: 2c20 6465 6661 756c 7473 2074 6f20 3320  , defaults to 3 
+0000ce80: 6974 656d 732e 0a20 2020 2020 2020 206d  items..        m
+0000ce90: 756c 7469 5f73 656c 6563 745f 6d69 6e5f  ulti_select_min_
+0000cea0: 7175 6572 795f 6c65 6e67 7468 2028 696e  query_length (in
+0000ceb0: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+0000cec0: 466f 7220 6d75 6c74 6973 656c 6563 7420  For multiselect 
+0000ced0: 6d65 6e75 732c 2074 6865 206e 756d 6265  menus, the numbe
+0000cee0: 7220 6f66 2074 6578 740a 2020 2020 2020  r of text.      
+0000cef0: 2020 2020 2020 6368 6172 6163 7465 7273        characters
+0000cf00: 2074 6861 7420 6120 7573 6572 2069 6e70   that a user inp
+0000cf10: 7574 7320 6265 666f 7265 2074 6865 2061  uts before the a
+0000cf20: 7070 0a20 2020 2020 2020 2020 2020 2071  pp.            q
+0000cf30: 7565 7269 6573 2061 7574 6f63 6f6d 706c  ueries autocompl
+0000cf40: 6574 6520 616e 6420 6469 7370 6c61 7973  ete and displays
+0000cf50: 2073 7567 6765 7374 6564 0a20 2020 2020   suggested.     
+0000cf60: 2020 2020 2020 2069 7465 6d73 2069 6e20         items in 
+0000cf70: 7468 6520 6d65 6e75 2e0a 0a20 2020 2020  the menu...     
+0000cf80: 2020 2020 2020 2049 6620 756e 7370 6563         If unspec
+0000cf90: 6966 6965 642c 2064 6566 6175 6c74 7320  ified, defaults 
+0000cfa0: 746f 2030 2063 6861 7261 6374 6572 7320  to 0 characters 
+0000cfb0: 666f 720a 2020 2020 2020 2020 2020 2020  for.            
+0000cfc0: 7374 6174 6963 2064 6174 6120 736f 7572  static data sour
+0000cfd0: 6365 7320 616e 6420 3320 6368 6172 6163  ces and 3 charac
+0000cfe0: 7465 7273 2066 6f72 0a20 2020 2020 2020  ters for.       
+0000cff0: 2020 2020 2065 7874 6572 6e61 6c20 6461       external da
+0000d000: 7461 2073 6f75 7263 6573 2e0a 2020 2020  ta sources..    
+0000d010: 2020 2020 6578 7465 726e 616c 5f64 6174      external_dat
+0000d020: 615f 736f 7572 6365 2028 676f 6f67 6c65  a_source (google
+0000d030: 2e61 7070 732e 6361 7264 5f76 312e 7479  .apps.card_v1.ty
+0000d040: 7065 732e 4163 7469 6f6e 293a 0a20 2020  pes.Action):.   
+0000d050: 2020 2020 2020 2020 2041 6e20 6578 7465           An exte
+0000d060: 726e 616c 2064 6174 6120 736f 7572 6365  rnal data source
+0000d070: 2c20 7375 6368 2061 7320 6120 7265 6c61  , such as a rela
+0000d080: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
+0000d090: 2020 2064 6174 6120 6261 7365 2e0a 0a20     data base... 
+0000d0a0: 2020 2020 2020 2020 2020 2054 6869 7320             This 
+0000d0b0: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
+0000d0c0: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
+0000d0d0: 6d75 6c74 695f 7365 6c65 6374 5f64 6174  multi_select_dat
+0000d0e0: 615f 736f 7572 6365 6060 2e0a 2020 2020  a_source``..    
+0000d0f0: 2020 2020 706c 6174 666f 726d 5f64 6174      platform_dat
+0000d100: 615f 736f 7572 6365 2028 676f 6f67 6c65  a_source (google
+0000d110: 2e61 7070 732e 6361 7264 5f76 312e 7479  .apps.card_v1.ty
+0000d120: 7065 732e 5365 6c65 6374 696f 6e49 6e70  pes.SelectionInp
+0000d130: 7574 2e50 6c61 7466 6f72 6d44 6174 6153  ut.PlatformDataS
+0000d140: 6f75 7263 6529 3a0a 2020 2020 2020 2020  ource):.        
+0000d150: 2020 2020 4120 6461 7461 2073 6f75 7263      A data sourc
+0000d160: 6520 6672 6f6d 2047 6f6f 676c 6520 576f  e from Google Wo
+0000d170: 726b 7370 6163 652e 0a0a 2020 2020 2020  rkspace...      
+0000d180: 2020 2020 2020 5468 6973 2066 6965 6c64        This field
+0000d190: 2069 7320 6120 6d65 6d62 6572 206f 6620   is a member of 
+0000d1a0: 606f 6e65 6f66 605f 2060 606d 756c 7469  `oneof`_ ``multi
+0000d1b0: 5f73 656c 6563 745f 6461 7461 5f73 6f75  _select_data_sou
+0000d1c0: 7263 6560 602e 0a20 2020 2022 2222 0a0a  rce``..    """..
+0000d1d0: 2020 2020 636c 6173 7320 5365 6c65 6374      class Select
+0000d1e0: 696f 6e54 7970 6528 7072 6f74 6f2e 456e  ionType(proto.En
+0000d1f0: 756d 293a 0a20 2020 2020 2020 2072 2222  um):.        r""
+0000d200: 2254 6865 2066 6f72 6d61 7420 666f 7220  "The format for 
+0000d210: 7468 6520 6974 656d 7320 7468 6174 2075  the items that u
+0000d220: 7365 7273 2063 616e 2073 656c 6563 742e  sers can select.
+0000d230: 2044 6966 6665 7265 6e74 206f 7074 696f   Different optio
+0000d240: 6e73 0a20 2020 2020 2020 2073 7570 706f  ns.        suppo
+0000d250: 7274 2064 6966 6665 7265 6e74 2074 7970  rt different typ
+0000d260: 6573 206f 6620 696e 7465 7261 6374 696f  es of interactio
+0000d270: 6e73 2e20 466f 7220 6578 616d 706c 652c  ns. For example,
+0000d280: 2075 7365 7273 2063 616e 0a20 2020 2020   users can.     
+0000d290: 2020 2073 656c 6563 7420 6d75 6c74 6970     select multip
+0000d2a0: 6c65 2063 6865 636b 626f 7865 732c 2062  le checkboxes, b
+0000d2b0: 7574 2063 616e 206f 6e6c 7920 7365 6c65  ut can only sele
+0000d2c0: 6374 206f 6e65 2069 7465 6d20 6672 6f6d  ct one item from
+0000d2d0: 2061 0a20 2020 2020 2020 2064 726f 7064   a.        dropd
+0000d2e0: 6f77 6e20 6d65 6e75 2e0a 0a20 2020 2020  own menu...     
+0000d2f0: 2020 2045 6163 6820 7365 6c65 6374 696f     Each selectio
+0000d300: 6e20 696e 7075 7420 7375 7070 6f72 7473  n input supports
+0000d310: 206f 6e65 2074 7970 6520 6f66 2073 656c   one type of sel
+0000d320: 6563 7469 6f6e 2e20 4d69 7869 6e67 0a20  ection. Mixing. 
+0000d330: 2020 2020 2020 2063 6865 636b 626f 7865         checkboxe
+0000d340: 7320 616e 6420 7377 6974 6368 6573 2c20  s and switches, 
+0000d350: 666f 7220 6578 616d 706c 652c 2069 736e  for example, isn
+0000d360: 2774 2073 7570 706f 7274 6564 2e0a 0a20  't supported... 
+0000d370: 2020 2020 2020 2060 476f 6f67 6c65 2057         `Google W
+0000d380: 6f72 6b73 7061 6365 2041 6464 2d6f 6e73  orkspace Add-ons
+0000d390: 2061 6e64 2043 6861 740a 2020 2020 2020   and Chat.      
+0000d3a0: 2020 6170 7073 203c 6874 7470 733a 2f2f    apps <https://
+0000d3b0: 6465 7665 6c6f 7065 7273 2e67 6f6f 676c  developers.googl
+0000d3c0: 652e 636f 6d2f 776f 726b 7370 6163 652f  e.com/workspace/
+0000d3d0: 6578 7465 6e64 3e60 5f5f 3a0a 0a20 2020  extend>`__:..   
+0000d3e0: 2020 2020 2056 616c 7565 733a 0a20 2020       Values:.   
+0000d3f0: 2020 2020 2020 2020 2043 4845 434b 5f42           CHECK_B
+0000d400: 4f58 2028 3029 3a0a 2020 2020 2020 2020  OX (0):.        
+0000d410: 2020 2020 2020 2020 4120 7365 7420 6f66          A set of
+0000d420: 2063 6865 636b 626f 7865 732e 2055 7365   checkboxes. Use
+0000d430: 7273 2063 616e 2073 656c 6563 7420 6f6e  rs can select on
+0000d440: 6520 6f72 0a20 2020 2020 2020 2020 2020  e or.           
+0000d450: 2020 2020 206d 6f72 6520 6368 6563 6b62       more checkb
+0000d460: 6f78 6573 2e0a 2020 2020 2020 2020 2020  oxes..          
+0000d470: 2020 5241 4449 4f5f 4255 5454 4f4e 2028    RADIO_BUTTON (
+0000d480: 3129 3a0a 2020 2020 2020 2020 2020 2020  1):.            
+0000d490: 2020 2020 4120 7365 7420 6f66 2072 6164      A set of rad
+0000d4a0: 696f 2062 7574 746f 6e73 2e20 5573 6572  io buttons. User
+0000d4b0: 7320 6361 6e20 7365 6c65 6374 206f 6e65  s can select one
+0000d4c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d4d0: 2072 6164 696f 2062 7574 746f 6e2e 0a20   radio button.. 
+0000d4e0: 2020 2020 2020 2020 2020 2053 5749 5443             SWITC
+0000d4f0: 4820 2832 293a 0a20 2020 2020 2020 2020  H (2):.         
+0000d500: 2020 2020 2020 2041 2073 6574 206f 6620         A set of 
+0000d510: 7377 6974 6368 6573 2e20 5573 6572 7320  switches. Users 
+0000d520: 6361 6e20 7475 726e 206f 6e20 6f6e 6520  can turn on one 
+0000d530: 6f72 0a20 2020 2020 2020 2020 2020 2020  or.             
+0000d540: 2020 206d 6f72 6520 7377 6974 6368 6573     more switches
+0000d550: 2e0a 2020 2020 2020 2020 2020 2020 4452  ..            DR
+0000d560: 4f50 444f 574e 2028 3329 3a0a 2020 2020  OPDOWN (3):.    
+0000d570: 2020 2020 2020 2020 2020 2020 4120 6472              A dr
+0000d580: 6f70 646f 776e 206d 656e 752e 2055 7365  opdown menu. Use
+0000d590: 7273 2063 616e 2073 656c 6563 7420 6f6e  rs can select on
+0000d5a0: 6520 6974 656d 0a20 2020 2020 2020 2020  e item.         
+0000d5b0: 2020 2020 2020 2066 726f 6d20 7468 6520         from the 
+0000d5c0: 6d65 6e75 2e0a 2020 2020 2020 2020 2020  menu..          
+0000d5d0: 2020 4d55 4c54 495f 5345 4c45 4354 2028    MULTI_SELECT (
+0000d5e0: 3429 3a0a 2020 2020 2020 2020 2020 2020  4):.            
+0000d5f0: 2020 2020 4120 6d75 6c74 6973 656c 6563      A multiselec
+0000d600: 7420 6d65 6e75 2066 6f72 2073 7461 7469  t menu for stati
+0000d610: 6320 6f72 2064 796e 616d 6963 2064 6174  c or dynamic dat
+0000d620: 612e 2046 726f 6d20 7468 6520 6d65 6e75  a. From the menu
+0000d630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d640: 2062 6172 2c20 7573 6572 7320 7365 6c65   bar, users sele
+0000d650: 6374 206f 6e65 206f 7220 6d6f 7265 2069  ct one or more i
+0000d660: 7465 6d73 2e20 5573 6572 7320 6361 6e20  tems. Users can 
+0000d670: 616c 736f 2069 6e70 7574 0a20 2020 2020  also input.     
+0000d680: 2020 2020 2020 2020 2020 2076 616c 7565             value
+0000d690: 7320 746f 2070 6f70 756c 6174 6520 6479  s to populate dy
+0000d6a0: 6e61 6d69 6320 6461 7461 2e20 466f 7220  namic data. For 
+0000d6b0: 6578 616d 706c 652c 2075 7365 7273 2063  example, users c
+0000d6c0: 616e 0a20 2020 2020 2020 2020 2020 2020  an.             
+0000d6d0: 2020 2073 7461 7274 2074 7970 696e 6720     start typing 
+0000d6e0: 7468 6520 6e61 6d65 206f 6620 6120 476f  the name of a Go
+0000d6f0: 6f67 6c65 2043 6861 7420 7370 6163 6520  ogle Chat space 
+0000d700: 616e 6420 7468 6520 7769 6467 6574 0a20  and the widget. 
+0000d710: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0000d720: 7574 6f73 7567 6765 7374 7320 7468 6520  utosuggests the 
+0000d730: 7370 6163 652e 0a0a 2020 2020 2020 2020  space...        
+0000d740: 2020 2020 2020 2020 546f 2070 6f70 756c          To popul
+0000d750: 6174 6520 6974 656d 7320 666f 7220 6120  ate items for a 
+0000d760: 6d75 6c74 6973 656c 6563 7420 6d65 6e75  multiselect menu
+0000d770: 2c20 796f 7520 6361 6e20 7573 6520 6f6e  , you can use on
+0000d780: 6520 6f66 0a20 2020 2020 2020 2020 2020  e of.           
+0000d790: 2020 2020 2074 6865 2066 6f6c 6c6f 7769       the followi
+0000d7a0: 6e67 2074 7970 6573 206f 6620 6461 7461  ng types of data
+0000d7b0: 2073 6f75 7263 6573 3a0a 0a20 2020 2020   sources:..     
+0000d7c0: 2020 2020 2020 2020 2020 202d 2020 5374             -  St
+0000d7d0: 6174 6963 2064 6174 613a 2049 7465 6d73  atic data: Items
+0000d7e0: 2061 7265 2073 7065 6369 6669 6564 2061   are specified a
+0000d7f0: 7320 6060 5365 6c65 6374 696f 6e49 7465  s ``SelectionIte
+0000d800: 6d60 600a 2020 2020 2020 2020 2020 2020  m``.            
+0000d810: 2020 2020 2020 206f 626a 6563 7473 2069         objects i
+0000d820: 6e20 7468 6520 7769 6467 6574 2e20 5570  n the widget. Up
+0000d830: 2074 6f20 3130 3020 6974 656d 732e 0a20   to 100 items.. 
+0000d840: 2020 2020 2020 2020 2020 2020 2020 202d                 -
+0000d850: 2020 476f 6f67 6c65 2057 6f72 6b73 7061    Google Workspa
+0000d860: 6365 2064 6174 613a 2049 7465 6d73 2061  ce data: Items a
+0000d870: 7265 2070 6f70 756c 6174 6564 2075 7369  re populated usi
+0000d880: 6e67 2064 6174 610a 2020 2020 2020 2020  ng data.        
+0000d890: 2020 2020 2020 2020 2020 2066 726f 6d20             from 
+0000d8a0: 476f 6f67 6c65 2057 6f72 6b73 7061 6365  Google Workspace
+0000d8b0: 2c20 7375 6368 2061 7320 476f 6f67 6c65  , such as Google
+0000d8c0: 2057 6f72 6b73 7061 6365 2075 7365 7273   Workspace users
+0000d8d0: 206f 720a 2020 2020 2020 2020 2020 2020   or.            
+0000d8e0: 2020 2020 2020 2047 6f6f 676c 6520 4368         Google Ch
+0000d8f0: 6174 2073 7061 6365 732e 0a20 2020 2020  at spaces..     
+0000d900: 2020 2020 2020 2020 2020 202d 2020 4578             -  Ex
+0000d910: 7465 726e 616c 2064 6174 613a 2049 7465  ternal data: Ite
+0000d920: 6d73 2061 7265 2070 6f70 756c 6174 6564  ms are populated
+0000d930: 2066 726f 6d20 616e 2065 7874 6572 6e61   from an externa
+0000d940: 6c20 6461 7461 0a20 2020 2020 2020 2020  l data.         
+0000d950: 2020 2020 2020 2020 2020 736f 7572 6365            source
+0000d960: 206f 7574 7369 6465 206f 6620 476f 6f67   outside of Goog
+0000d970: 6c65 2057 6f72 6b73 7061 6365 2e0a 0a20  le Workspace... 
+0000d980: 2020 2020 2020 2020 2020 2020 2020 2046                 F
+0000d990: 6f72 2065 7861 6d70 6c65 7320 6f66 2068  or examples of h
+0000d9a0: 6f77 2074 6f20 696d 706c 656d 656e 7420  ow to implement 
+0000d9b0: 6d75 6c74 6973 656c 6563 7420 6d65 6e75  multiselect menu
+0000d9c0: 732c 2073 6565 2060 4164 640a 2020 2020  s, see `Add.    
+0000d9d0: 2020 2020 2020 2020 2020 2020 6120 6d75              a mu
+0000d9e0: 6c74 6973 656c 6563 740a 2020 2020 2020  ltiselect.      
+0000d9f0: 2020 2020 2020 2020 2020 6d65 6e75 203c            menu <
+0000da00: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
+0000da10: 7273 2e67 6f6f 676c 652e 636f 6d2f 776f  rs.google.com/wo
+0000da20: 726b 7370 6163 652f 6368 6174 2f64 6573  rkspace/chat/des
+0000da30: 6967 6e2d 696e 7465 7261 6374 6976 652d  ign-interactive-
+0000da40: 6361 7264 2d64 6961 6c6f 6723 6d75 6c74  card-dialog#mult
+0000da50: 6973 656c 6563 742d 6d65 6e75 3e60 5f5f  iselect-menu>`__
+0000da60: 2e0a 0a20 2020 2020 2020 2020 2020 2020  ...             
+0000da70: 2020 2060 476f 6f67 6c65 2057 6f72 6b73     `Google Works
+0000da80: 7061 6365 2041 6464 2d6f 6e73 2061 6e64  pace Add-ons and
+0000da90: 2043 6861 740a 2020 2020 2020 2020 2020   Chat.          
+0000daa0: 2020 2020 2020 6170 7073 203c 6874 7470        apps <http
+0000dab0: 733a 2f2f 6465 7665 6c6f 7065 7273 2e67  s://developers.g
+0000dac0: 6f6f 676c 652e 636f 6d2f 776f 726b 7370  oogle.com/worksp
+0000dad0: 6163 652f 6578 7465 6e64 3e60 5f5f 3a0a  ace/extend>`__:.
+0000dae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000daf0: 4d75 6c74 6973 656c 6563 7420 666f 7220  Multiselect for 
+0000db00: 476f 6f67 6c65 2057 6f72 6b73 7061 6365  Google Workspace
+0000db10: 2041 6464 2d6f 6e73 2061 7265 2069 6e20   Add-ons are in 
+0000db20: 4465 7665 6c6f 7065 720a 2020 2020 2020  Developer.      
+0000db30: 2020 2020 2020 2020 2020 5072 6576 6965            Previe
+0000db40: 772e 0a20 2020 2020 2020 2022 2222 0a20  w..        """. 
+0000db50: 2020 2020 2020 2043 4845 434b 5f42 4f58         CHECK_BOX
+0000db60: 203d 2030 0a20 2020 2020 2020 2052 4144   = 0.        RAD
+0000db70: 494f 5f42 5554 544f 4e20 3d20 310a 2020  IO_BUTTON = 1.  
+0000db80: 2020 2020 2020 5357 4954 4348 203d 2032        SWITCH = 2
+0000db90: 0a20 2020 2020 2020 2044 524f 5044 4f57  .        DROPDOW
+0000dba0: 4e20 3d20 330a 2020 2020 2020 2020 4d55  N = 3.        MU
+0000dbb0: 4c54 495f 5345 4c45 4354 203d 2034 0a0a  LTI_SELECT = 4..
+0000dbc0: 2020 2020 636c 6173 7320 5365 6c65 6374      class Select
+0000dbd0: 696f 6e49 7465 6d28 7072 6f74 6f2e 4d65  ionItem(proto.Me
+0000dbe0: 7373 6167 6529 3a0a 2020 2020 2020 2020  ssage):.        
+0000dbf0: 7222 2222 416e 2069 7465 6d20 7468 6174  r"""An item that
+0000dc00: 2075 7365 7273 2063 616e 2073 656c 6563   users can selec
+0000dc10: 7420 696e 2061 2073 656c 6563 7469 6f6e  t in a selection
+0000dc20: 2069 6e70 7574 2c20 7375 6368 2061 7320   input, such as 
+0000dc30: 610a 2020 2020 2020 2020 6368 6563 6b62  a.        checkb
+0000dc40: 6f78 206f 7220 7377 6974 6368 2e0a 0a20  ox or switch... 
+0000dc50: 2020 2020 2020 2060 476f 6f67 6c65 2057         `Google W
+0000dc60: 6f72 6b73 7061 6365 2041 6464 2d6f 6e73  orkspace Add-ons
+0000dc70: 2061 6e64 2043 6861 740a 2020 2020 2020   and Chat.      
+0000dc80: 2020 6170 7073 203c 6874 7470 733a 2f2f    apps <https://
+0000dc90: 6465 7665 6c6f 7065 7273 2e67 6f6f 676c  developers.googl
+0000dca0: 652e 636f 6d2f 776f 726b 7370 6163 652f  e.com/workspace/
+0000dcb0: 6578 7465 6e64 3e60 5f5f 3a0a 0a20 2020  extend>`__:..   
+0000dcc0: 2020 2020 2041 7474 7269 6275 7465 733a       Attributes:
+0000dcd0: 0a20 2020 2020 2020 2020 2020 2074 6578  .            tex
+0000dce0: 7420 2873 7472 293a 0a20 2020 2020 2020  t (str):.       
+0000dcf0: 2020 2020 2020 2020 2054 6865 2074 6578           The tex
+0000dd00: 7420 7468 6174 2069 6465 6e74 6966 6965  t that identifie
+0000dd10: 7320 6f72 2064 6573 6372 6962 6573 2074  s or describes t
+0000dd20: 6865 0a20 2020 2020 2020 2020 2020 2020  he.             
+0000dd30: 2020 2069 7465 6d20 746f 2075 7365 7273     item to users
+0000dd40: 2e0a 2020 2020 2020 2020 2020 2020 7661  ..            va
+0000dd50: 6c75 6520 2873 7472 293a 0a20 2020 2020  lue (str):.     
+0000dd60: 2020 2020 2020 2020 2020 2054 6865 2076             The v
+0000dd70: 616c 7565 2061 7373 6f63 6961 7465 6420  alue associated 
+0000dd80: 7769 7468 2074 6869 7320 6974 656d 2e20  with this item. 
+0000dd90: 5468 6520 636c 6965 6e74 2073 686f 756c  The client shoul
+0000dda0: 6420 7573 650a 2020 2020 2020 2020 2020  d use.          
+0000ddb0: 2020 2020 2020 7468 6973 2061 7320 6120        this as a 
+0000ddc0: 666f 726d 2069 6e70 7574 2076 616c 7565  form input value
+0000ddd0: 2e0a 0a20 2020 2020 2020 2020 2020 2020  ...             
+0000dde0: 2020 2046 6f72 2064 6574 6169 6c73 2061     For details a
+0000ddf0: 626f 7574 2077 6f72 6b69 6e67 2077 6974  bout working wit
+0000de00: 6820 666f 726d 2069 6e70 7574 732c 2073  h form inputs, s
+0000de10: 6565 2060 5265 6365 6976 650a 2020 2020  ee `Receive.    
+0000de20: 2020 2020 2020 2020 2020 2020 666f 726d              form
+0000de30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000de40: 2064 6174 6120 3c68 7474 7073 3a2f 2f64   data <https://d
+0000de50: 6576 656c 6f70 6572 732e 676f 6f67 6c65  evelopers.google
+0000de60: 2e63 6f6d 2f77 6f72 6b73 7061 6365 2f63  .com/workspace/c
+0000de70: 6861 742f 7265 6164 2d66 6f72 6d2d 6461  hat/read-form-da
+0000de80: 7461 3e60 5f5f 2e0a 2020 2020 2020 2020  ta>`__..        
+0000de90: 2020 2020 7365 6c65 6374 6564 2028 626f      selected (bo
+0000dea0: 6f6c 293a 0a20 2020 2020 2020 2020 2020  ol):.           
+0000deb0: 2020 2020 2057 6865 7468 6572 2074 6865       Whether the
+0000dec0: 2069 7465 6d20 6973 2073 656c 6563 7465   item is selecte
+0000ded0: 6420 6279 2064 6566 6175 6c74 2e20 4966  d by default. If
+0000dee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000def0: 2074 6865 2073 656c 6563 7469 6f6e 2069   the selection i
+0000df00: 6e70 7574 206f 6e6c 7920 6163 6365 7074  nput only accept
+0000df10: 7320 6f6e 6520 7661 6c75 6520 2873 7563  s one value (suc
+0000df20: 680a 2020 2020 2020 2020 2020 2020 2020  h.              
+0000df30: 2020 6173 2066 6f72 2072 6164 696f 2062    as for radio b
+0000df40: 7574 746f 6e73 206f 7220 6120 6472 6f70  uttons or a drop
+0000df50: 646f 776e 206d 656e 7529 2c20 6f6e 6c79  down menu), only
+0000df60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000df70: 2073 6574 2074 6869 7320 6669 656c 6420   set this field 
+0000df80: 666f 7220 6f6e 6520 6974 656d 2e0a 2020  for one item..  
+0000df90: 2020 2020 2020 2020 2020 7374 6172 745f            start_
+0000dfa0: 6963 6f6e 5f75 7269 2028 7374 7229 3a0a  icon_uri (str):.
+0000dfb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dfc0: 466f 7220 6d75 6c74 6973 656c 6563 7420  For multiselect 
+0000dfd0: 6d65 6e75 732c 2074 6865 2055 524c 2066  menus, the URL f
+0000dfe0: 6f72 2074 6865 2069 636f 6e20 6469 7370  or the icon disp
+0000dff0: 6c61 7965 6420 6e65 7874 0a20 2020 2020  layed next.     
+0000e000: 2020 2020 2020 2020 2020 2074 6f20 7468             to th
+0000e010: 6520 6974 656d 2773 2060 6074 6578 7460  e item's ``text`
+0000e020: 6020 6669 656c 642e 2053 7570 706f 7274  ` field. Support
+0000e030: 7320 504e 4720 616e 6420 4a50 4547 2066  s PNG and JPEG f
+0000e040: 696c 6573 2e0a 2020 2020 2020 2020 2020  iles..          
+0000e050: 2020 2020 2020 4d75 7374 2062 6520 616e        Must be an
+0000e060: 2060 6048 5454 5053 6060 2055 524c 2e20   ``HTTPS`` URL. 
+0000e070: 466f 7220 6578 616d 706c 652c 0a20 2020  For example,.   
+0000e080: 2020 2020 2020 2020 2020 2020 2060 6068               ``h
+0000e090: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
+0000e0a0: 732e 676f 6f67 6c65 2e63 6f6d 2f77 6f72  s.google.com/wor
+0000e0b0: 6b73 7061 6365 2f63 6861 742f 696d 6167  kspace/chat/imag
+0000e0c0: 6573 2f71 7569 636b 7374 6172 742d 6170  es/quickstart-ap
+0000e0d0: 702d 6176 6174 6172 2e70 6e67 6060 2e0a  p-avatar.png``..
+0000e0e0: 2020 2020 2020 2020 2020 2020 626f 7474              bott
+0000e0f0: 6f6d 5f74 6578 7420 2873 7472 293a 0a20  om_text (str):. 
+0000e100: 2020 2020 2020 2020 2020 2020 2020 2046                 F
+0000e110: 6f72 206d 756c 7469 7365 6c65 6374 206d  or multiselect m
+0000e120: 656e 7573 2c20 6120 7465 7874 2064 6573  enus, a text des
+0000e130: 6372 6970 7469 6f6e 206f 7220 6c61 6265  cription or labe
+0000e140: 6c20 7468 6174 2773 0a20 2020 2020 2020  l that's.       
+0000e150: 2020 2020 2020 2020 2064 6973 706c 6179           display
+0000e160: 6564 2062 656c 6f77 2074 6865 2069 7465  ed below the ite
+0000e170: 6d27 7320 6060 7465 7874 6060 2066 6965  m's ``text`` fie
+0000e180: 6c64 2e0a 2020 2020 2020 2020 2222 220a  ld..        """.
+0000e190: 0a20 2020 2020 2020 2074 6578 743a 2073  .        text: s
+0000e1a0: 7472 203d 2070 726f 746f 2e46 6965 6c64  tr = proto.Field
+0000e1b0: 280a 2020 2020 2020 2020 2020 2020 7072  (.            pr
+0000e1c0: 6f74 6f2e 5354 5249 4e47 2c0a 2020 2020  oto.STRING,.    
+0000e1d0: 2020 2020 2020 2020 6e75 6d62 6572 3d31          number=1
+0000e1e0: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+0000e1f0: 2020 2020 7661 6c75 653a 2073 7472 203d      value: str =
+0000e200: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
+0000e210: 2020 2020 2020 2020 2020 7072 6f74 6f2e            proto.
+0000e220: 5354 5249 4e47 2c0a 2020 2020 2020 2020  STRING,.        
+0000e230: 2020 2020 6e75 6d62 6572 3d32 2c0a 2020      number=2,.  
+0000e240: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000e250: 7365 6c65 6374 6564 3a20 626f 6f6c 203d  selected: bool =
+0000e260: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
+0000e270: 2020 2020 2020 2020 2020 7072 6f74 6f2e            proto.
+0000e280: 424f 4f4c 2c0a 2020 2020 2020 2020 2020  BOOL,.          
+0000e290: 2020 6e75 6d62 6572 3d33 2c0a 2020 2020    number=3,.    
+0000e2a0: 2020 2020 290a 2020 2020 2020 2020 7374      ).        st
+0000e2b0: 6172 745f 6963 6f6e 5f75 7269 3a20 7374  art_icon_uri: st
+0000e2c0: 7220 3d20 7072 6f74 6f2e 4669 656c 6428  r = proto.Field(
+0000e2d0: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
+0000e2e0: 746f 2e53 5452 494e 472c 0a20 2020 2020  to.STRING,.     
+0000e2f0: 2020 2020 2020 206e 756d 6265 723d 342c         number=4,
+0000e300: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+0000e310: 2020 2062 6f74 746f 6d5f 7465 7874 3a20     bottom_text: 
+0000e320: 7374 7220 3d20 7072 6f74 6f2e 4669 656c  str = proto.Fiel
+0000e330: 6428 0a20 2020 2020 2020 2020 2020 2070  d(.            p
+0000e340: 726f 746f 2e53 5452 494e 472c 0a20 2020  roto.STRING,.   
+0000e350: 2020 2020 2020 2020 206e 756d 6265 723d           number=
+0000e360: 352c 0a20 2020 2020 2020 2029 0a0a 2020  5,.        )..  
+0000e370: 2020 636c 6173 7320 506c 6174 666f 726d    class Platform
+0000e380: 4461 7461 536f 7572 6365 2870 726f 746f  DataSource(proto
+0000e390: 2e4d 6573 7361 6765 293a 0a20 2020 2020  .Message):.     
+0000e3a0: 2020 2072 2222 2246 6f72 2061 205b 6060     r"""For a [``
+0000e3b0: 5365 6c65 6374 696f 6e49 6e70 7574 6060  SelectionInput``
+0000e3c0: 5d5b 676f 6f67 6c65 2e61 7070 732e 6361  ][google.apps.ca
+0000e3d0: 7264 2e76 312e 5365 6c65 6374 696f 6e49  rd.v1.SelectionI
+0000e3e0: 6e70 7574 5d0a 2020 2020 2020 2020 7769  nput].        wi
+0000e3f0: 6467 6574 2074 6861 7420 7573 6573 2061  dget that uses a
+0000e400: 206d 756c 7469 7365 6c65 6374 206d 656e   multiselect men
+0000e410: 752c 2061 2064 6174 6120 736f 7572 6365  u, a data source
+0000e420: 2066 726f 6d20 476f 6f67 6c65 0a20 2020   from Google.   
+0000e430: 2020 2020 2057 6f72 6b73 7061 6365 2e20       Workspace. 
+0000e440: 5573 6564 2074 6f20 706f 7075 6c61 7465  Used to populate
+0000e450: 2069 7465 6d73 2069 6e20 6120 6d75 6c74   items in a mult
+0000e460: 6973 656c 6563 7420 6d65 6e75 2e0a 0a20  iselect menu... 
+0000e470: 2020 2020 2020 2060 476f 6f67 6c65 2043         `Google C
+0000e480: 6861 7420 6170 7073 203c 6874 7470 733a  hat apps <https:
+0000e490: 2f2f 6465 7665 6c6f 7065 7273 2e67 6f6f  //developers.goo
+0000e4a0: 676c 652e 636f 6d2f 776f 726b 7370 6163  gle.com/workspac
+0000e4b0: 652f 6368 6174 3e60 5f5f 3a0a 0a0a 2020  e/chat>`__:...  
+0000e4c0: 2020 2020 2020 2e2e 205f 6f6e 656f 663a        .. _oneof:
+0000e4d0: 2068 7474 7073 3a2f 2f70 726f 746f 2d70   https://proto-p
+0000e4e0: 6c75 732d 7079 7468 6f6e 2e72 6561 6474  lus-python.readt
+0000e4f0: 6865 646f 6373 2e69 6f2f 656e 2f73 7461  hedocs.io/en/sta
+0000e500: 626c 652f 6669 656c 6473 2e68 746d 6c23  ble/fields.html#
+0000e510: 6f6e 656f 6673 2d6d 7574 7561 6c6c 792d  oneofs-mutually-
+0000e520: 6578 636c 7573 6976 652d 6669 656c 6473  exclusive-fields
+0000e530: 0a0a 2020 2020 2020 2020 4174 7472 6962  ..        Attrib
+0000e540: 7574 6573 3a0a 2020 2020 2020 2020 2020  utes:.          
+0000e550: 2020 636f 6d6d 6f6e 5f64 6174 615f 736f    common_data_so
+0000e560: 7572 6365 2028 676f 6f67 6c65 2e61 7070  urce (google.app
+0000e570: 732e 6361 7264 5f76 312e 7479 7065 732e  s.card_v1.types.
+0000e580: 5365 6c65 6374 696f 6e49 6e70 7574 2e50  SelectionInput.P
+0000e590: 6c61 7466 6f72 6d44 6174 6153 6f75 7263  latformDataSourc
+0000e5a0: 652e 436f 6d6d 6f6e 4461 7461 536f 7572  e.CommonDataSour
+0000e5b0: 6365 293a 0a20 2020 2020 2020 2020 2020  ce):.           
+0000e5c0: 2020 2020 2041 2064 6174 6120 736f 7572       A data sour
+0000e5d0: 6365 2073 6861 7265 6420 6279 2061 6c6c  ce shared by all
+0000e5e0: 2047 6f6f 676c 6520 576f 726b 7370 6163   Google Workspac
+0000e5f0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0000e600: 2020 6170 706c 6963 6174 696f 6e73 2c20    applications, 
+0000e610: 7375 6368 2061 7320 7573 6572 7320 696e  such as users in
+0000e620: 2061 2047 6f6f 676c 650a 2020 2020 2020   a Google.      
+0000e630: 2020 2020 2020 2020 2020 576f 726b 7370            Worksp
+0000e640: 6163 6520 6f72 6761 6e69 7a61 7469 6f6e  ace organization
+0000e650: 2e0a 0a20 2020 2020 2020 2020 2020 2020  ...             
+0000e660: 2020 2054 6869 7320 6669 656c 6420 6973     This field is
+0000e670: 2061 206d 656d 6265 7220 6f66 2060 6f6e   a member of `on
+0000e680: 656f 6660 5f20 6060 6461 7461 5f73 6f75  eof`_ ``data_sou
+0000e690: 7263 6560 602e 0a20 2020 2020 2020 2022  rce``..        "
+0000e6a0: 2222 0a0a 2020 2020 2020 2020 636c 6173  ""..        clas
+0000e6b0: 7320 436f 6d6d 6f6e 4461 7461 536f 7572  s CommonDataSour
+0000e6c0: 6365 2870 726f 746f 2e45 6e75 6d29 3a0a  ce(proto.Enum):.
+0000e6d0: 2020 2020 2020 2020 2020 2020 7222 2222              r"""
+0000e6e0: 4120 6461 7461 2073 6f75 7263 6520 7368  A data source sh
+0000e6f0: 6172 6564 2062 7920 616c 6c20 5b47 6f6f  ared by all [Goo
+0000e700: 676c 6520 576f 726b 7370 6163 6520 6170  gle Workspace ap
+0000e710: 706c 6963 6174 696f 6e73 5d0a 2020 2020  plications].    
+0000e720: 2020 2020 2020 2020 2868 7474 7073 3a2f          (https:/
+0000e730: 2f64 6576 656c 6f70 6572 732e 676f 6f67  /developers.goog
+0000e740: 6c65 2e63 6f6d 2f77 6f72 6b73 7061 6365  le.com/workspace
+0000e750: 2f63 6861 742f 6170 692f 7265 6665 7265  /chat/api/refere
+0000e760: 6e63 652f 7265 7374 2f76 312f 486f 7374  nce/rest/v1/Host
+0000e770: 4170 7029 2e0a 0a20 2020 2020 2020 2020  App)...         
+0000e780: 2020 2060 476f 6f67 6c65 2043 6861 7420     `Google Chat 
+0000e790: 6170 7073 203c 6874 7470 733a 2f2f 6465  apps <https://de
+0000e7a0: 7665 6c6f 7065 7273 2e67 6f6f 676c 652e  velopers.google.
+0000e7b0: 636f 6d2f 776f 726b 7370 6163 652f 6368  com/workspace/ch
+0000e7c0: 6174 3e60 5f5f 3a0a 0a20 2020 2020 2020  at>`__:..       
+0000e7d0: 2020 2020 2056 616c 7565 733a 0a20 2020       Values:.   
+0000e7e0: 2020 2020 2020 2020 2020 2020 2055 4e4b               UNK
+0000e7f0: 4e4f 574e 2028 3029 3a0a 2020 2020 2020  NOWN (0):.      
+0000e800: 2020 2020 2020 2020 2020 2020 2020 4465                De
+0000e810: 6661 756c 7420 7661 6c75 652e 2044 6f6e  fault value. Don
+0000e820: 2774 2075 7365 2e0a 2020 2020 2020 2020  't use..        
+0000e830: 2020 2020 2020 2020 5553 4552 2028 3129          USER (1)
+0000e840: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000e850: 2020 2020 2020 476f 6f67 6c65 2057 6f72        Google Wor
+0000e860: 6b73 7061 6365 2075 7365 7273 2e20 5468  kspace users. Th
+0000e870: 6520 7573 6572 2063 616e 206f 6e6c 790a  e user can only.
+0000e880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e890: 2020 2020 7669 6577 2061 6e64 2073 656c      view and sel
+0000e8a0: 6563 7420 7573 6572 7320 6672 6f6d 2074  ect users from t
+0000e8b0: 6865 6972 2047 6f6f 676c 650a 2020 2020  heir Google.    
+0000e8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e8d0: 576f 726b 7370 6163 6520 6f72 6761 6e69  Workspace organi
+0000e8e0: 7a61 7469 6f6e 2e0a 2020 2020 2020 2020  zation..        
+0000e8f0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000e900: 2020 2020 554e 4b4e 4f57 4e20 3d20 300a      UNKNOWN = 0.
+0000e910: 2020 2020 2020 2020 2020 2020 5553 4552              USER
+0000e920: 203d 2031 0a0a 2020 2020 2020 2020 636f   = 1..        co
+0000e930: 6d6d 6f6e 5f64 6174 615f 736f 7572 6365  mmon_data_source
+0000e940: 3a20 2253 656c 6563 7469 6f6e 496e 7075  : "SelectionInpu
+0000e950: 742e 506c 6174 666f 726d 4461 7461 536f  t.PlatformDataSo
+0000e960: 7572 6365 2e43 6f6d 6d6f 6e44 6174 6153  urce.CommonDataS
+0000e970: 6f75 7263 6522 203d 2028 0a20 2020 2020  ource" = (.     
+0000e980: 2020 2020 2020 2070 726f 746f 2e46 6965         proto.Fie
+0000e990: 6c64 280a 2020 2020 2020 2020 2020 2020  ld(.            
+0000e9a0: 2020 2020 7072 6f74 6f2e 454e 554d 2c0a      proto.ENUM,.
+0000e9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e9c0: 6e75 6d62 6572 3d31 2c0a 2020 2020 2020  number=1,.      
+0000e9d0: 2020 2020 2020 2020 2020 6f6e 656f 663d            oneof=
+0000e9e0: 2264 6174 615f 736f 7572 6365 222c 0a20  "data_source",. 
+0000e9f0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000ea00: 6e75 6d3d 2253 656c 6563 7469 6f6e 496e  num="SelectionIn
+0000ea10: 7075 742e 506c 6174 666f 726d 4461 7461  put.PlatformData
+0000ea20: 536f 7572 6365 2e43 6f6d 6d6f 6e44 6174  Source.CommonDat
+0000ea30: 6153 6f75 7263 6522 2c0a 2020 2020 2020  aSource",.      
+0000ea40: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000ea50: 290a 0a20 2020 206e 616d 653a 2073 7472  )..    name: str
+0000ea60: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
+0000ea70: 2020 2020 2020 2020 7072 6f74 6f2e 5354          proto.ST
+0000ea80: 5249 4e47 2c0a 2020 2020 2020 2020 6e75  RING,.        nu
+0000ea90: 6d62 6572 3d31 2c0a 2020 2020 290a 2020  mber=1,.    ).  
+0000eaa0: 2020 6c61 6265 6c3a 2073 7472 203d 2070    label: str = p
+0000eab0: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
+0000eac0: 2020 2020 7072 6f74 6f2e 5354 5249 4e47      proto.STRING
+0000ead0: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
+0000eae0: 3d32 2c0a 2020 2020 290a 2020 2020 7479  =2,.    ).    ty
+0000eaf0: 7065 5f3a 2053 656c 6563 7469 6f6e 5479  pe_: SelectionTy
+0000eb00: 7065 203d 2070 726f 746f 2e46 6965 6c64  pe = proto.Field
+0000eb10: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
+0000eb20: 454e 554d 2c0a 2020 2020 2020 2020 6e75  ENUM,.        nu
+0000eb30: 6d62 6572 3d33 2c0a 2020 2020 2020 2020  mber=3,.        
+0000eb40: 656e 756d 3d53 656c 6563 7469 6f6e 5479  enum=SelectionTy
+0000eb50: 7065 2c0a 2020 2020 290a 2020 2020 6974  pe,.    ).    it
+0000eb60: 656d 733a 204d 7574 6162 6c65 5365 7175  ems: MutableSequ
+0000eb70: 656e 6365 5b53 656c 6563 7469 6f6e 4974  ence[SelectionIt
+0000eb80: 656d 5d20 3d20 7072 6f74 6f2e 5265 7065  em] = proto.Repe
+0000eb90: 6174 6564 4669 656c 6428 0a20 2020 2020  atedField(.     
+0000eba0: 2020 2070 726f 746f 2e4d 4553 5341 4745     proto.MESSAGE
+0000ebb0: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
+0000ebc0: 3d34 2c0a 2020 2020 2020 2020 6d65 7373  =4,.        mess
+0000ebd0: 6167 653d 5365 6c65 6374 696f 6e49 7465  age=SelectionIte
+0000ebe0: 6d2c 0a20 2020 2029 0a20 2020 206f 6e5f  m,.    ).    on_
+0000ebf0: 6368 616e 6765 5f61 6374 696f 6e3a 2022  change_action: "
+0000ec00: 4163 7469 6f6e 2220 3d20 7072 6f74 6f2e  Action" = proto.
+0000ec10: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
+0000ec20: 726f 746f 2e4d 4553 5341 4745 2c0a 2020  roto.MESSAGE,.  
+0000ec30: 2020 2020 2020 6e75 6d62 6572 3d35 2c0a        number=5,.
+0000ec40: 2020 2020 2020 2020 6d65 7373 6167 653d          message=
+0000ec50: 2241 6374 696f 6e22 2c0a 2020 2020 290a  "Action",.    ).
+0000ec60: 2020 2020 6d75 6c74 695f 7365 6c65 6374      multi_select
+0000ec70: 5f6d 6178 5f73 656c 6563 7465 645f 6974  _max_selected_it
+0000ec80: 656d 733a 2069 6e74 203d 2070 726f 746f  ems: int = proto
+0000ec90: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
+0000eca0: 7072 6f74 6f2e 494e 5433 322c 0a20 2020  proto.INT32,.   
+0000ecb0: 2020 2020 206e 756d 6265 723d 362c 0a20       number=6,. 
+0000ecc0: 2020 2029 0a20 2020 206d 756c 7469 5f73     ).    multi_s
+0000ecd0: 656c 6563 745f 6d69 6e5f 7175 6572 795f  elect_min_query_
+0000ece0: 6c65 6e67 7468 3a20 696e 7420 3d20 7072  length: int = pr
+0000ecf0: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
+0000ed00: 2020 2070 726f 746f 2e49 4e54 3332 2c0a     proto.INT32,.
+0000ed10: 2020 2020 2020 2020 6e75 6d62 6572 3d37          number=7
+0000ed20: 2c0a 2020 2020 290a 2020 2020 6578 7465  ,.    ).    exte
+0000ed30: 726e 616c 5f64 6174 615f 736f 7572 6365  rnal_data_source
+0000ed40: 3a20 2241 6374 696f 6e22 203d 2070 726f  : "Action" = pro
+0000ed50: 746f 2e46 6965 6c64 280a 2020 2020 2020  to.Field(.      
+0000ed60: 2020 7072 6f74 6f2e 4d45 5353 4147 452c    proto.MESSAGE,
+0000ed70: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
+0000ed80: 382c 0a20 2020 2020 2020 206f 6e65 6f66  8,.        oneof
+0000ed90: 3d22 6d75 6c74 695f 7365 6c65 6374 5f64  ="multi_select_d
+0000eda0: 6174 615f 736f 7572 6365 222c 0a20 2020  ata_source",.   
+0000edb0: 2020 2020 206d 6573 7361 6765 3d22 4163       message="Ac
+0000edc0: 7469 6f6e 222c 0a20 2020 2029 0a20 2020  tion",.    ).   
+0000edd0: 2070 6c61 7466 6f72 6d5f 6461 7461 5f73   platform_data_s
+0000ede0: 6f75 7263 653a 2050 6c61 7466 6f72 6d44  ource: PlatformD
+0000edf0: 6174 6153 6f75 7263 6520 3d20 7072 6f74  ataSource = prot
+0000ee00: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+0000ee10: 2070 726f 746f 2e4d 4553 5341 4745 2c0a   proto.MESSAGE,.
+0000ee20: 2020 2020 2020 2020 6e75 6d62 6572 3d39          number=9
+0000ee30: 2c0a 2020 2020 2020 2020 6f6e 656f 663d  ,.        oneof=
+0000ee40: 226d 756c 7469 5f73 656c 6563 745f 6461  "multi_select_da
+0000ee50: 7461 5f73 6f75 7263 6522 2c0a 2020 2020  ta_source",.    
+0000ee60: 2020 2020 6d65 7373 6167 653d 506c 6174      message=Plat
+0000ee70: 666f 726d 4461 7461 536f 7572 6365 2c0a  formDataSource,.
+0000ee80: 2020 2020 290a 0a0a 636c 6173 7320 4461      )...class Da
+0000ee90: 7465 5469 6d65 5069 636b 6572 2870 726f  teTimePicker(pro
+0000eea0: 746f 2e4d 6573 7361 6765 293a 0a20 2020  to.Message):.   
+0000eeb0: 2072 2222 224c 6574 7320 7573 6572 7320   r"""Lets users 
+0000eec0: 696e 7075 7420 6120 6461 7465 2c20 6120  input a date, a 
+0000eed0: 7469 6d65 2c20 6f72 2062 6f74 6820 6120  time, or both a 
+0000eee0: 6461 7465 2061 6e64 2061 2074 696d 652e  date and a time.
+0000eef0: 2046 6f72 2061 6e0a 2020 2020 6578 616d   For an.    exam
+0000ef00: 706c 6520 696e 2047 6f6f 676c 6520 4368  ple in Google Ch
+0000ef10: 6174 2061 7070 732c 2073 6565 2060 4c65  at apps, see `Le
+0000ef20: 7420 6120 7573 6572 2070 6963 6b20 6120  t a user pick a 
+0000ef30: 6461 7465 2061 6e64 0a20 2020 2074 696d  date and.    tim
+0000ef40: 6520 3c68 7474 7073 3a2f 2f64 6576 656c  e <https://devel
+0000ef50: 6f70 6572 732e 676f 6f67 6c65 2e63 6f6d  opers.google.com
+0000ef60: 2f77 6f72 6b73 7061 6365 2f63 6861 742f  /workspace/chat/
+0000ef70: 6465 7369 676e 2d69 6e74 6572 6163 7469  design-interacti
+0000ef80: 7665 2d63 6172 642d 6469 616c 6f67 236c  ve-card-dialog#l
+0000ef90: 6574 5f61 5f75 7365 725f 7069 636b 5f61  et_a_user_pick_a
+0000efa0: 5f64 6174 655f 616e 645f 7469 6d65 3e60  _date_and_time>`
+0000efb0: 5f5f 2e0a 0a20 2020 2055 7365 7273 2063  __...    Users c
+0000efc0: 616e 2069 6e70 7574 2074 6578 7420 6f72  an input text or
+0000efd0: 2075 7365 2074 6865 2070 6963 6b65 7220   use the picker 
+0000efe0: 746f 2073 656c 6563 7420 6461 7465 7320  to select dates 
+0000eff0: 616e 6420 7469 6d65 732e 2049 660a 2020  and times. If.  
+0000f000: 2020 7573 6572 7320 696e 7075 7420 616e    users input an
+0000f010: 2069 6e76 616c 6964 2064 6174 6520 6f72   invalid date or
+0000f020: 2074 696d 652c 2074 6865 2070 6963 6b65   time, the picke
+0000f030: 7220 7368 6f77 7320 616e 2065 7272 6f72  r shows an error
+0000f040: 2074 6861 740a 2020 2020 7072 6f6d 7074   that.    prompt
+0000f050: 7320 7573 6572 7320 746f 2069 6e70 7574  s users to input
+0000f060: 2074 6865 2069 6e66 6f72 6d61 7469 6f6e   the information
+0000f070: 2063 6f72 7265 6374 6c79 2e0a 0a20 2020   correctly...   
+0000f080: 2060 476f 6f67 6c65 2057 6f72 6b73 7061   `Google Workspa
+0000f090: 6365 2041 6464 2d6f 6e73 2061 6e64 2043  ce Add-ons and C
+0000f0a0: 6861 740a 2020 2020 6170 7073 203c 6874  hat.    apps <ht
+0000f0b0: 7470 733a 2f2f 6465 7665 6c6f 7065 7273  tps://developers
+0000f0c0: 2e67 6f6f 676c 652e 636f 6d2f 776f 726b  .google.com/work
+0000f0d0: 7370 6163 652f 6578 7465 6e64 3e60 5f5f  space/extend>`__
+0000f0e0: 3a0a 0a20 2020 2041 7474 7269 6275 7465  :..    Attribute
+0000f0f0: 733a 0a20 2020 2020 2020 206e 616d 6520  s:.        name 
+0000f100: 2873 7472 293a 0a20 2020 2020 2020 2020  (str):.         
+0000f110: 2020 2054 6865 206e 616d 6520 6279 2077     The name by w
+0000f120: 6869 6368 2074 6865 2060 6044 6174 6554  hich the ``DateT
+0000f130: 696d 6550 6963 6b65 7260 6020 6973 2069  imePicker`` is i
+0000f140: 6465 6e74 6966 6965 6420 696e 2061 0a20  dentified in a. 
+0000f150: 2020 2020 2020 2020 2020 2066 6f72 6d20             form 
+0000f160: 696e 7075 7420 6576 656e 742e 0a0a 2020  input event...  
+0000f170: 2020 2020 2020 2020 2020 466f 7220 6465            For de
+0000f180: 7461 696c 7320 6162 6f75 7420 776f 726b  tails about work
+0000f190: 696e 6720 7769 7468 2066 6f72 6d20 696e  ing with form in
+0000f1a0: 7075 7473 2c20 7365 6520 6052 6563 6569  puts, see `Recei
+0000f1b0: 7665 0a20 2020 2020 2020 2020 2020 2066  ve.            f
+0000f1c0: 6f72 6d0a 2020 2020 2020 2020 2020 2020  orm.            
+0000f1d0: 6461 7461 203c 6874 7470 733a 2f2f 6465  data <https://de
+0000f1e0: 7665 6c6f 7065 7273 2e67 6f6f 676c 652e  velopers.google.
+0000f1f0: 636f 6d2f 776f 726b 7370 6163 652f 6368  com/workspace/ch
+0000f200: 6174 2f72 6561 642d 666f 726d 2d64 6174  at/read-form-dat
+0000f210: 613e 605f 5f2e 0a20 2020 2020 2020 206c  a>`__..        l
+0000f220: 6162 656c 2028 7374 7229 3a0a 2020 2020  abel (str):.    
+0000f230: 2020 2020 2020 2020 5468 6520 7465 7874          The text
+0000f240: 2074 6861 7420 7072 6f6d 7074 7320 7573   that prompts us
+0000f250: 6572 7320 746f 2069 6e70 7574 2061 2064  ers to input a d
+0000f260: 6174 652c 2061 2074 696d 652c 206f 7220  ate, a time, or 
+0000f270: 610a 2020 2020 2020 2020 2020 2020 6461  a.            da
+0000f280: 7465 2061 6e64 2074 696d 652e 2046 6f72  te and time. For
+0000f290: 2065 7861 6d70 6c65 2c20 6966 2075 7365   example, if use
+0000f2a0: 7273 2061 7265 2073 6368 6564 756c 696e  rs are schedulin
+0000f2b0: 6720 616e 0a20 2020 2020 2020 2020 2020  g an.           
+0000f2c0: 2061 7070 6f69 6e74 6d65 6e74 2c20 7573   appointment, us
+0000f2d0: 6520 6120 6c61 6265 6c20 7375 6368 2061  e a label such a
+0000f2e0: 7320 6060 4170 706f 696e 746d 656e 7420  s ``Appointment 
+0000f2f0: 6461 7465 6060 206f 720a 2020 2020 2020  date`` or.      
+0000f300: 2020 2020 2020 6060 4170 706f 696e 746d        ``Appointm
+0000f310: 656e 7420 6461 7465 2061 6e64 2074 696d  ent date and tim
+0000f320: 6560 602e 0a20 2020 2020 2020 2074 7970  e``..        typ
+0000f330: 655f 2028 676f 6f67 6c65 2e61 7070 732e  e_ (google.apps.
+0000f340: 6361 7264 5f76 312e 7479 7065 732e 4461  card_v1.types.Da
+0000f350: 7465 5469 6d65 5069 636b 6572 2e44 6174  teTimePicker.Dat
+0000f360: 6554 696d 6550 6963 6b65 7254 7970 6529  eTimePickerType)
+0000f370: 3a0a 2020 2020 2020 2020 2020 2020 5768  :.            Wh
+0000f380: 6574 6865 7220 7468 6520 7769 6467 6574  ether the widget
+0000f390: 2073 7570 706f 7274 7320 696e 7075 7474   supports inputt
+0000f3a0: 696e 6720 6120 6461 7465 2c0a 2020 2020  ing a date,.    
+0000f3b0: 2020 2020 2020 2020 6120 7469 6d65 2c20          a time, 
+0000f3c0: 6f72 2074 6865 2064 6174 6520 616e 6420  or the date and 
+0000f3d0: 7469 6d65 2e0a 2020 2020 2020 2020 7661  time..        va
+0000f3e0: 6c75 655f 6d73 5f65 706f 6368 2028 696e  lue_ms_epoch (in
+0000f3f0: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+0000f400: 5468 6520 6465 6661 756c 7420 7661 6c75  The default valu
+0000f410: 6520 6469 7370 6c61 7965 6420 696e 2074  e displayed in t
+0000f420: 6865 2077 6964 6765 742c 2069 6e20 6d69  he widget, in mi
+0000f430: 6c6c 6973 6563 6f6e 6473 0a20 2020 2020  lliseconds.     
+0000f440: 2020 2020 2020 2073 696e 6365 2060 556e         since `Un
+0000f450: 6978 2065 706f 6368 0a20 2020 2020 2020  ix epoch.       
+0000f460: 2020 2020 2074 696d 6520 3c68 7474 7073       time <https
+0000f470: 3a2f 2f65 6e2e 7769 6b69 7065 6469 612e  ://en.wikipedia.
+0000f480: 6f72 672f 7769 6b69 2f55 6e69 785f 7469  org/wiki/Unix_ti
+0000f490: 6d65 3e60 5f5f 2e0a 0a20 2020 2020 2020  me>`__...       
+0000f4a0: 2020 2020 2053 7065 6369 6679 2074 6865       Specify the
+0000f4b0: 2076 616c 7565 2062 6173 6564 206f 6e20   value based on 
+0000f4c0: 7468 6520 7479 7065 206f 6620 7069 636b  the type of pick
+0000f4d0: 6572 0a20 2020 2020 2020 2020 2020 2028  er.            (
+0000f4e0: 6060 4461 7465 5469 6d65 5069 636b 6572  ``DateTimePicker
+0000f4f0: 5479 7065 6060 293a 0a0a 2020 2020 2020  Type``):..      
+0000f500: 2020 2020 2020 2d20 2060 6044 4154 455f        -  ``DATE_
+0000f510: 414e 445f 5449 4d45 6060 3a20 6120 6361  AND_TIME``: a ca
+0000f520: 6c65 6e64 6172 2064 6174 6520 616e 6420  lendar date and 
+0000f530: 7469 6d65 2069 6e20 5554 432e 2046 6f72  time in UTC. For
+0000f540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f550: 6578 616d 706c 652c 2074 6f20 7265 7072  example, to repr
+0000f560: 6573 656e 7420 4a61 6e75 6172 7920 312c  esent January 1,
+0000f570: 2032 3032 3320 6174 2031 323a 3030 2050   2023 at 12:00 P
+0000f580: 4d20 5554 432c 0a20 2020 2020 2020 2020  M UTC,.         
+0000f590: 2020 2020 2020 7573 6520 6060 3136 3732        use ``1672
+0000f5a0: 3537 3434 3030 3030 3060 602e 0a20 2020  574400000``..   
+0000f5b0: 2020 2020 2020 2020 202d 2020 6060 4441           -  ``DA
+0000f5c0: 5445 5f4f 4e4c 5960 603a 2061 2063 616c  TE_ONLY``: a cal
+0000f5d0: 656e 6461 7220 6461 7465 2061 7420 3030  endar date at 00
+0000f5e0: 3a30 303a 3030 2055 5443 2e20 466f 720a  :00:00 UTC. For.
+0000f5f0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000f600: 7861 6d70 6c65 2c20 746f 2072 6570 7265  xample, to repre
+0000f610: 7365 6e74 204a 616e 7561 7279 2031 2c20  sent January 1, 
+0000f620: 3230 3233 2c20 7573 650a 2020 2020 2020  2023, use.      
+0000f630: 2020 2020 2020 2020 2060 6031 3637 3235           ``16725
+0000f640: 3331 3230 3030 3030 6060 2e0a 2020 2020  31200000``..    
+0000f650: 2020 2020 2020 2020 2d20 2060 6054 494d          -  ``TIM
+0000f660: 455f 4f4e 4c59 6060 3a20 6120 7469 6d65  E_ONLY``: a time
+0000f670: 2069 6e20 5554 432e 2046 6f72 2065 7861   in UTC. For exa
+0000f680: 6d70 6c65 2c20 746f 2072 6570 7265 7365  mple, to represe
+0000f690: 6e74 0a20 2020 2020 2020 2020 2020 2020  nt.             
+0000f6a0: 2020 3132 3a30 3020 504d 2c20 7573 6520    12:00 PM, use 
+0000f6b0: 6060 3433 3230 3030 3030 6060 2028 6f72  ``43200000`` (or
+0000f6c0: 2060 6031 3220 2a20 3630 202a 2036 3020   ``12 * 60 * 60 
+0000f6d0: 2a20 3130 3030 6060 292e 0a20 2020 2020  * 1000``)..     
+0000f6e0: 2020 2074 696d 657a 6f6e 655f 6f66 6673     timezone_offs
+0000f6f0: 6574 5f64 6174 6520 2869 6e74 293a 0a20  et_date (int):. 
+0000f700: 2020 2020 2020 2020 2020 2054 6865 206e             The n
+0000f710: 756d 6265 7220 7265 7072 6573 656e 7469  umber representi
+0000f720: 6e67 2074 6865 2074 696d 6520 7a6f 6e65  ng the time zone
+0000f730: 206f 6666 7365 7420 6672 6f6d 2055 5443   offset from UTC
+0000f740: 2c20 696e 0a20 2020 2020 2020 2020 2020  , in.           
+0000f750: 206d 696e 7574 6573 2e20 4966 2073 6574   minutes. If set
+0000f760: 2c20 7468 6520 6060 7661 6c75 655f 6d73  , the ``value_ms
+0000f770: 5f65 706f 6368 6060 2069 7320 6469 7370  _epoch`` is disp
+0000f780: 6c61 7965 6420 696e 2074 6865 0a20 2020  layed in the.   
+0000f790: 2020 2020 2020 2020 2073 7065 6369 6669           specifi
+0000f7a0: 6564 2074 696d 6520 7a6f 6e65 2e20 4966  ed time zone. If
+0000f7b0: 2075 6e73 6574 2c20 7468 6520 7661 6c75   unset, the valu
+0000f7c0: 6520 6465 6661 756c 7473 2074 6f20 7468  e defaults to th
+0000f7d0: 650a 2020 2020 2020 2020 2020 2020 7573  e.            us
+0000f7e0: 6572 2773 2074 696d 6520 7a6f 6e65 2073  er's time zone s
+0000f7f0: 6574 7469 6e67 2e0a 2020 2020 2020 2020  etting..        
+0000f800: 6f6e 5f63 6861 6e67 655f 6163 7469 6f6e  on_change_action
+0000f810: 2028 676f 6f67 6c65 2e61 7070 732e 6361   (google.apps.ca
+0000f820: 7264 5f76 312e 7479 7065 732e 4163 7469  rd_v1.types.Acti
+0000f830: 6f6e 293a 0a20 2020 2020 2020 2020 2020  on):.           
+0000f840: 2054 7269 6767 6572 6564 2077 6865 6e20   Triggered when 
+0000f850: 7468 6520 7573 6572 2063 6c69 636b 7320  the user clicks 
+0000f860: 2a2a 5361 7665 2a2a 206f 7220 2a2a 436c  **Save** or **Cl
+0000f870: 6561 722a 2a20 6672 6f6d 0a20 2020 2020  ear** from.     
+0000f880: 2020 2020 2020 2074 6865 2060 6044 6174         the ``Dat
+0000f890: 6554 696d 6550 6963 6b65 7260 6020 696e  eTimePicker`` in
+0000f8a0: 7465 7266 6163 652e 0a20 2020 2022 2222  terface..    """
+0000f8b0: 0a0a 2020 2020 636c 6173 7320 4461 7465  ..    class Date
+0000f8c0: 5469 6d65 5069 636b 6572 5479 7065 2870  TimePickerType(p
+0000f8d0: 726f 746f 2e45 6e75 6d29 3a0a 2020 2020  roto.Enum):.    
+0000f8e0: 2020 2020 7222 2222 5468 6520 666f 726d      r"""The form
+0000f8f0: 6174 2066 6f72 2074 6865 2064 6174 6520  at for the date 
+0000f900: 616e 6420 7469 6d65 2069 6e20 7468 6520  and time in the 
+0000f910: 6060 4461 7465 5469 6d65 5069 636b 6572  ``DateTimePicker
+0000f920: 6060 2077 6964 6765 742e 0a20 2020 2020  `` widget..     
+0000f930: 2020 2044 6574 6572 6d69 6e65 7320 7768     Determines wh
+0000f940: 6574 6865 7220 7573 6572 7320 6361 6e20  ether users can 
+0000f950: 696e 7075 7420 6120 6461 7465 2c20 6120  input a date, a 
+0000f960: 7469 6d65 2c20 6f72 2062 6f74 6820 6120  time, or both a 
+0000f970: 6461 7465 0a20 2020 2020 2020 2061 6e64  date.        and
+0000f980: 2074 696d 652e 0a0a 2020 2020 2020 2020   time...        
+0000f990: 6047 6f6f 676c 6520 576f 726b 7370 6163  `Google Workspac
+0000f9a0: 6520 4164 642d 6f6e 7320 616e 6420 4368  e Add-ons and Ch
+0000f9b0: 6174 0a20 2020 2020 2020 2061 7070 7320  at.        apps 
+0000f9c0: 3c68 7474 7073 3a2f 2f64 6576 656c 6f70  <https://develop
+0000f9d0: 6572 732e 676f 6f67 6c65 2e63 6f6d 2f77  ers.google.com/w
+0000f9e0: 6f72 6b73 7061 6365 2f65 7874 656e 643e  orkspace/extend>
+0000f9f0: 605f 5f3a 0a0a 2020 2020 2020 2020 5661  `__:..        Va
+0000fa00: 6c75 6573 3a0a 2020 2020 2020 2020 2020  lues:.          
+0000fa10: 2020 4441 5445 5f41 4e44 5f54 494d 4520    DATE_AND_TIME 
+0000fa20: 2830 293a 0a20 2020 2020 2020 2020 2020  (0):.           
+0000fa30: 2020 2020 2055 7365 7273 2069 6e70 7574       Users input
+0000fa40: 2061 2064 6174 6520 616e 6420 7469 6d65   a date and time
+0000fa50: 2e0a 2020 2020 2020 2020 2020 2020 4441  ..            DA
+0000fa60: 5445 5f4f 4e4c 5920 2831 293a 0a20 2020  TE_ONLY (1):.   
+0000fa70: 2020 2020 2020 2020 2020 2020 2055 7365               Use
+0000fa80: 7273 2069 6e70 7574 2061 2064 6174 652e  rs input a date.
+0000fa90: 0a20 2020 2020 2020 2020 2020 2054 494d  .            TIM
+0000faa0: 455f 4f4e 4c59 2028 3229 3a0a 2020 2020  E_ONLY (2):.    
+0000fab0: 2020 2020 2020 2020 2020 2020 5573 6572              User
+0000fac0: 7320 696e 7075 7420 6120 7469 6d65 2e0a  s input a time..
+0000fad0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000fae0: 2020 2020 4441 5445 5f41 4e44 5f54 494d      DATE_AND_TIM
+0000faf0: 4520 3d20 300a 2020 2020 2020 2020 4441  E = 0.        DA
+0000fb00: 5445 5f4f 4e4c 5920 3d20 310a 2020 2020  TE_ONLY = 1.    
+0000fb10: 2020 2020 5449 4d45 5f4f 4e4c 5920 3d20      TIME_ONLY = 
+0000fb20: 320a 0a20 2020 206e 616d 653a 2073 7472  2..    name: str
+0000fb30: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
+0000fb40: 2020 2020 2020 2020 7072 6f74 6f2e 5354          proto.ST
+0000fb50: 5249 4e47 2c0a 2020 2020 2020 2020 6e75  RING,.        nu
+0000fb60: 6d62 6572 3d31 2c0a 2020 2020 290a 2020  mber=1,.    ).  
+0000fb70: 2020 6c61 6265 6c3a 2073 7472 203d 2070    label: str = p
+0000fb80: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
+0000fb90: 2020 2020 7072 6f74 6f2e 5354 5249 4e47      proto.STRING
+0000fba0: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
+0000fbb0: 3d32 2c0a 2020 2020 290a 2020 2020 7479  =2,.    ).    ty
+0000fbc0: 7065 5f3a 2044 6174 6554 696d 6550 6963  pe_: DateTimePic
+0000fbd0: 6b65 7254 7970 6520 3d20 7072 6f74 6f2e  kerType = proto.
+0000fbe0: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
+0000fbf0: 726f 746f 2e45 4e55 4d2c 0a20 2020 2020  roto.ENUM,.     
+0000fc00: 2020 206e 756d 6265 723d 332c 0a20 2020     number=3,.   
+0000fc10: 2020 2020 2065 6e75 6d3d 4461 7465 5469       enum=DateTi
+0000fc20: 6d65 5069 636b 6572 5479 7065 2c0a 2020  mePickerType,.  
+0000fc30: 2020 290a 2020 2020 7661 6c75 655f 6d73    ).    value_ms
+0000fc40: 5f65 706f 6368 3a20 696e 7420 3d20 7072  _epoch: int = pr
+0000fc50: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
+0000fc60: 2020 2070 726f 746f 2e49 4e54 3634 2c0a     proto.INT64,.
+0000fc70: 2020 2020 2020 2020 6e75 6d62 6572 3d34          number=4
+0000fc80: 2c0a 2020 2020 290a 2020 2020 7469 6d65  ,.    ).    time
+0000fc90: 7a6f 6e65 5f6f 6666 7365 745f 6461 7465  zone_offset_date
+0000fca0: 3a20 696e 7420 3d20 7072 6f74 6f2e 4669  : int = proto.Fi
+0000fcb0: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
+0000fcc0: 746f 2e49 4e54 3332 2c0a 2020 2020 2020  to.INT32,.      
+0000fcd0: 2020 6e75 6d62 6572 3d35 2c0a 2020 2020    number=5,.    
+0000fce0: 290a 2020 2020 6f6e 5f63 6861 6e67 655f  ).    on_change_
+0000fcf0: 6163 7469 6f6e 3a20 2241 6374 696f 6e22  action: "Action"
+0000fd00: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
+0000fd10: 2020 2020 2020 2020 7072 6f74 6f2e 4d45          proto.ME
+0000fd20: 5353 4147 452c 0a20 2020 2020 2020 206e  SSAGE,.        n
+0000fd30: 756d 6265 723d 362c 0a20 2020 2020 2020  umber=6,.       
+0000fd40: 206d 6573 7361 6765 3d22 4163 7469 6f6e   message="Action
+0000fd50: 222c 0a20 2020 2029 0a0a 0a63 6c61 7373  ",.    )...class
+0000fd60: 2042 7574 746f 6e28 7072 6f74 6f2e 4d65   Button(proto.Me
+0000fd70: 7373 6167 6529 3a0a 2020 2020 7222 2222  ssage):.    r"""
+0000fd80: 4120 7465 7874 2c20 6963 6f6e 2c20 6f72  A text, icon, or
+0000fd90: 2074 6578 7420 616e 6420 6963 6f6e 2062   text and icon b
+0000fda0: 7574 746f 6e20 7468 6174 2075 7365 7273  utton that users
+0000fdb0: 2063 616e 2063 6c69 636b 2e20 466f 7220   can click. For 
+0000fdc0: 616e 0a20 2020 2065 7861 6d70 6c65 2069  an.    example i
+0000fdd0: 6e20 476f 6f67 6c65 2043 6861 7420 6170  n Google Chat ap
+0000fde0: 7073 2c20 7365 6520 6041 6464 2061 0a20  ps, see `Add a. 
+0000fdf0: 2020 2062 7574 746f 6e20 3c68 7474 7073     button <https
+0000fe00: 3a2f 2f64 6576 656c 6f70 6572 732e 676f  ://developers.go
+0000fe10: 6f67 6c65 2e63 6f6d 2f77 6f72 6b73 7061  ogle.com/workspa
+0000fe20: 6365 2f63 6861 742f 6465 7369 676e 2d69  ce/chat/design-i
+0000fe30: 6e74 6572 6163 7469 7665 2d63 6172 642d  nteractive-card-
+0000fe40: 6469 616c 6f67 2361 6464 5f61 5f62 7574  dialog#add_a_but
+0000fe50: 746f 6e3e 605f 5f2e 0a0a 2020 2020 546f  ton>`__...    To
+0000fe60: 206d 616b 6520 616e 2069 6d61 6765 2061   make an image a
+0000fe70: 2063 6c69 636b 6162 6c65 2062 7574 746f   clickable butto
+0000fe80: 6e2c 2073 7065 6369 6679 2061 6e0a 2020  n, specify an.  
+0000fe90: 2020 5b60 6049 6d61 6765 6060 5d5b 676f    [``Image``][go
+0000fea0: 6f67 6c65 2e61 7070 732e 6361 7264 2e76  ogle.apps.card.v
+0000feb0: 312e 496d 6167 655d 2028 6e6f 7420 616e  1.Image] (not an
+0000fec0: 0a20 2020 205b 6060 496d 6167 6543 6f6d  .    [``ImageCom
+0000fed0: 706f 6e65 6e74 6060 5d5b 676f 6f67 6c65  ponent``][google
+0000fee0: 2e61 7070 732e 6361 7264 2e76 312e 496d  .apps.card.v1.Im
+0000fef0: 6167 6543 6f6d 706f 6e65 6e74 5d29 2061  ageComponent]) a
+0000ff00: 6e64 2073 6574 2061 6e0a 2020 2020 6060  nd set an.    ``
+0000ff10: 6f6e 436c 6963 6b60 6020 6163 7469 6f6e  onClick`` action
+0000ff20: 2e0a 0a20 2020 2060 476f 6f67 6c65 2057  ...    `Google W
+0000ff30: 6f72 6b73 7061 6365 2041 6464 2d6f 6e73  orkspace Add-ons
+0000ff40: 2061 6e64 2043 6861 740a 2020 2020 6170   and Chat.    ap
+0000ff50: 7073 203c 6874 7470 733a 2f2f 6465 7665  ps <https://deve
+0000ff60: 6c6f 7065 7273 2e67 6f6f 676c 652e 636f  lopers.google.co
+0000ff70: 6d2f 776f 726b 7370 6163 652f 6578 7465  m/workspace/exte
+0000ff80: 6e64 3e60 5f5f 3a0a 0a20 2020 2041 7474  nd>`__:..    Att
+0000ff90: 7269 6275 7465 733a 0a20 2020 2020 2020  ributes:.       
+0000ffa0: 2074 6578 7420 2873 7472 293a 0a20 2020   text (str):.   
+0000ffb0: 2020 2020 2020 2020 2054 6865 2074 6578           The tex
+0000ffc0: 7420 6469 7370 6c61 7965 6420 696e 7369  t displayed insi
+0000ffd0: 6465 2074 6865 2062 7574 746f 6e2e 0a20  de the button.. 
+0000ffe0: 2020 2020 2020 2069 636f 6e20 2867 6f6f         icon (goo
+0000fff0: 676c 652e 6170 7073 2e63 6172 645f 7631  gle.apps.card_v1
+00010000: 2e74 7970 6573 2e49 636f 6e29 3a0a 2020  .types.Icon):.  
+00010010: 2020 2020 2020 2020 2020 5468 6520 6963            The ic
+00010020: 6f6e 2069 6d61 6765 2e20 4966 2062 6f74  on image. If bot
+00010030: 6820 6060 6963 6f6e 6060 2061 6e64 2060  h ``icon`` and `
+00010040: 6074 6578 7460 6020 6172 6520 7365 742c  `text`` are set,
+00010050: 2074 6865 6e0a 2020 2020 2020 2020 2020   then.          
+00010060: 2020 7468 6520 6963 6f6e 2061 7070 6561    the icon appea
+00010070: 7273 2062 6566 6f72 6520 7468 6520 7465  rs before the te
+00010080: 7874 2e0a 2020 2020 2020 2020 636f 6c6f  xt..        colo
+00010090: 7220 2867 6f6f 676c 652e 7479 7065 2e63  r (google.type.c
+000100a0: 6f6c 6f72 5f70 6232 2e43 6f6c 6f72 293a  olor_pb2.Color):
+000100b0: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
+000100c0: 7365 742c 2074 6865 2062 7574 746f 6e20  set, the button 
+000100d0: 6973 2066 696c 6c65 6420 7769 7468 2061  is filled with a
+000100e0: 2073 6f6c 6964 2062 6163 6b67 726f 756e   solid backgroun
+000100f0: 6420 636f 6c6f 720a 2020 2020 2020 2020  d color.        
+00010100: 2020 2020 616e 6420 7468 6520 666f 6e74      and the font
+00010110: 2063 6f6c 6f72 2063 6861 6e67 6573 2074   color changes t
+00010120: 6f20 6d61 696e 7461 696e 2063 6f6e 7472  o maintain contr
+00010130: 6173 7420 7769 7468 2074 6865 0a20 2020  ast with the.   
+00010140: 2020 2020 2020 2020 2062 6163 6b67 726f           backgro
+00010150: 756e 6420 636f 6c6f 722e 2046 6f72 2065  und color. For e
+00010160: 7861 6d70 6c65 2c20 7365 7474 696e 6720  xample, setting 
+00010170: 6120 626c 7565 2062 6163 6b67 726f 756e  a blue backgroun
+00010180: 640a 2020 2020 2020 2020 2020 2020 6c69  d.            li
+00010190: 6b65 6c79 2072 6573 756c 7473 2069 6e20  kely results in 
+000101a0: 7768 6974 6520 7465 7874 2e0a 0a20 2020  white text...   
+000101b0: 2020 2020 2020 2020 2049 6620 756e 7365           If unse
+000101c0: 742c 2074 6865 2069 6d61 6765 2062 6163  t, the image bac
+000101d0: 6b67 726f 756e 6420 6973 2077 6869 7465  kground is white
+000101e0: 2061 6e64 2074 6865 2066 6f6e 7420 636f   and the font co
+000101f0: 6c6f 720a 2020 2020 2020 2020 2020 2020  lor.            
+00010200: 6973 2062 6c75 652e 0a0a 2020 2020 2020  is blue...      
+00010210: 2020 2020 2020 466f 7220 7265 642c 2067        For red, g
+00010220: 7265 656e 2c20 616e 6420 626c 7565 2c20  reen, and blue, 
+00010230: 7468 6520 7661 6c75 6520 6f66 2065 6163  the value of eac
+00010240: 6820 6669 656c 6420 6973 2061 0a20 2020  h field is a.   
+00010250: 2020 2020 2020 2020 2060 6066 6c6f 6174           ``float
+00010260: 6060 206e 756d 6265 7220 7468 6174 2079  `` number that y
+00010270: 6f75 2063 616e 2065 7870 7265 7373 2069  ou can express i
+00010280: 6e20 6569 7468 6572 206f 6620 7477 6f20  n either of two 
+00010290: 7761 7973 3a0a 2020 2020 2020 2020 2020  ways:.          
+000102a0: 2020 6173 2061 206e 756d 6265 7220 6265    as a number be
+000102b0: 7477 6565 6e20 3020 616e 6420 3235 3520  tween 0 and 255 
+000102c0: 6469 7669 6465 6420 6279 2032 3535 2028  divided by 255 (
+000102d0: 3135 332f 3235 3529 2c20 6f72 0a20 2020  153/255), or.   
+000102e0: 2020 2020 2020 2020 2061 7320 6120 7661           as a va
+000102f0: 6c75 6520 6265 7477 6565 6e20 3020 616e  lue between 0 an
+00010300: 6420 3120 2830 2e36 292e 2030 2072 6570  d 1 (0.6). 0 rep
+00010310: 7265 7365 6e74 7320 7468 6520 6162 7365  resents the abse
+00010320: 6e63 650a 2020 2020 2020 2020 2020 2020  nce.            
+00010330: 6f66 2061 2063 6f6c 6f72 2061 6e64 2031  of a color and 1
+00010340: 206f 7220 3235 352f 3235 3520 7265 7072   or 255/255 repr
+00010350: 6573 656e 7420 7468 6520 6675 6c6c 2070  esent the full p
+00010360: 7265 7365 6e63 6520 6f66 0a20 2020 2020  resence of.     
+00010370: 2020 2020 2020 2074 6861 7420 636f 6c6f         that colo
+00010380: 7220 6f6e 2074 6865 2052 4742 2073 6361  r on the RGB sca
+00010390: 6c65 2e0a 0a20 2020 2020 2020 2020 2020  le...           
+000103a0: 204f 7074 696f 6e61 6c6c 7920 7365 7420   Optionally set 
+000103b0: 6060 616c 7068 6160 602c 2077 6869 6368  ``alpha``, which
+000103c0: 2073 6574 7320 6120 6c65 7665 6c20 6f66   sets a level of
+000103d0: 2074 7261 6e73 7061 7265 6e63 790a 2020   transparency.  
+000103e0: 2020 2020 2020 2020 2020 7573 696e 6720            using 
+000103f0: 7468 6973 2065 7175 6174 696f 6e3a 0a0a  this equation:..
+00010400: 2020 2020 2020 2020 2020 2020 3a3a 0a0a              ::..
+00010410: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00010420: 6978 656c 2063 6f6c 6f72 203d 2061 6c70  ixel color = alp
+00010430: 6861 202a 2028 7468 6973 2063 6f6c 6f72  ha * (this color
+00010440: 2920 2b20 2831 2e30 202d 2061 6c70 6861  ) + (1.0 - alpha
+00010450: 2920 2a20 2862 6163 6b67 726f 756e 6420  ) * (background 
+00010460: 636f 6c6f 7229 0a0a 2020 2020 2020 2020  color)..        
+00010470: 2020 2020 466f 7220 6060 616c 7068 6160      For ``alpha`
+00010480: 602c 2061 2076 616c 7565 206f 6620 6060  `, a value of ``
+00010490: 3160 6020 636f 7272 6573 706f 6e64 7320  1`` corresponds 
+000104a0: 7769 7468 2061 2073 6f6c 6964 0a20 2020  with a solid.   
+000104b0: 2020 2020 2020 2020 2063 6f6c 6f72 2c20           color, 
+000104c0: 616e 6420 6120 7661 6c75 6520 6f66 2060  and a value of `
+000104d0: 6030 6060 2063 6f72 7265 7370 6f6e 6473  `0`` corresponds
+000104e0: 2077 6974 6820 6120 636f 6d70 6c65 7465   with a complete
+000104f0: 6c79 0a20 2020 2020 2020 2020 2020 2074  ly.            t
+00010500: 7261 6e73 7061 7265 6e74 2063 6f6c 6f72  ransparent color
+00010510: 2e0a 0a20 2020 2020 2020 2020 2020 2046  ...            F
+00010520: 6f72 2065 7861 6d70 6c65 2c20 7468 6520  or example, the 
+00010530: 666f 6c6c 6f77 696e 6720 636f 6c6f 7220  following color 
+00010540: 7265 7072 6573 656e 7473 2061 2068 616c  represents a hal
+00010550: 660a 2020 2020 2020 2020 2020 2020 7472  f.            tr
+00010560: 616e 7370 6172 656e 7420 7265 643a 0a0a  ansparent red:..
+00010570: 2020 2020 2020 2020 2020 2020 3a3a 0a0a              ::..
+00010580: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00010590: 636f 6c6f 7222 3a20 7b0a 2020 2020 2020  color": {.      
+000105a0: 2020 2020 2020 2020 2020 2020 2272 6564              "red
+000105b0: 223a 2031 2c0a 2020 2020 2020 2020 2020  ": 1,.          
+000105c0: 2020 2020 2020 2020 2267 7265 656e 223a          "green":
+000105d0: 2030 2c0a 2020 2020 2020 2020 2020 2020   0,.            
+000105e0: 2020 2020 2020 2262 6c75 6522 3a20 302c        "blue": 0,
+000105f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010600: 2020 2022 616c 7068 6122 3a20 302e 350a     "alpha": 0.5.
+00010610: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00010620: 0a20 2020 2020 2020 206f 6e5f 636c 6963  .        on_clic
+00010630: 6b20 2867 6f6f 676c 652e 6170 7073 2e63  k (google.apps.c
+00010640: 6172 645f 7631 2e74 7970 6573 2e4f 6e43  ard_v1.types.OnC
+00010650: 6c69 636b 293a 0a20 2020 2020 2020 2020  lick):.         
+00010660: 2020 2052 6571 7569 7265 642e 2054 6865     Required. The
+00010670: 2061 6374 696f 6e20 746f 2070 6572 666f   action to perfo
+00010680: 726d 2077 6865 6e20 6120 7573 6572 0a20  rm when a user. 
+00010690: 2020 2020 2020 2020 2020 2063 6c69 636b             click
+000106a0: 7320 7468 6520 6275 7474 6f6e 2c20 7375  s the button, su
+000106b0: 6368 2061 7320 6f70 656e 696e 6720 6120  ch as opening a 
+000106c0: 6879 7065 726c 696e 6b0a 2020 2020 2020  hyperlink.      
+000106d0: 2020 2020 2020 6f72 2072 756e 6e69 6e67        or running
+000106e0: 2061 2063 7573 746f 6d20 6675 6e63 7469   a custom functi
+000106f0: 6f6e 2e0a 2020 2020 2020 2020 6469 7361  on..        disa
+00010700: 626c 6564 2028 626f 6f6c 293a 0a20 2020  bled (bool):.   
+00010710: 2020 2020 2020 2020 2049 6620 6060 7472           If ``tr
+00010720: 7565 6060 2c20 7468 6520 6275 7474 6f6e  ue``, the button
+00010730: 2069 7320 6469 7370 6c61 7965 6420 696e   is displayed in
+00010740: 2061 6e20 696e 6163 7469 7665 2073 7461   an inactive sta
+00010750: 7465 0a20 2020 2020 2020 2020 2020 2061  te.            a
+00010760: 6e64 2064 6f65 736e 2774 2072 6573 706f  nd doesn't respo
+00010770: 6e64 2074 6f20 7573 6572 2061 6374 696f  nd to user actio
+00010780: 6e73 2e0a 2020 2020 2020 2020 616c 745f  ns..        alt_
+00010790: 7465 7874 2028 7374 7229 3a0a 2020 2020  text (str):.    
+000107a0: 2020 2020 2020 2020 5468 6520 616c 7465          The alte
+000107b0: 726e 6174 6976 6520 7465 7874 2074 6861  rnative text tha
+000107c0: 7427 7320 7573 6564 2066 6f72 0a20 2020  t's used for.   
+000107d0: 2020 2020 2020 2020 2061 6363 6573 7369           accessi
+000107e0: 6269 6c69 7479 2e0a 2020 2020 2020 2020  bility..        
+000107f0: 2020 2020 5365 7420 6465 7363 7269 7074      Set descript
+00010800: 6976 6520 7465 7874 2074 6861 7420 6c65  ive text that le
+00010810: 7473 2075 7365 7273 206b 6e6f 7720 7768  ts users know wh
+00010820: 6174 0a20 2020 2020 2020 2020 2020 2074  at.            t
+00010830: 6865 2062 7574 746f 6e20 646f 6573 2e20  he button does. 
+00010840: 466f 7220 6578 616d 706c 652c 2069 6620  For example, if 
+00010850: 6120 6275 7474 6f6e 206f 7065 6e73 0a20  a button opens. 
+00010860: 2020 2020 2020 2020 2020 2061 2068 7970             a hyp
+00010870: 6572 6c69 6e6b 2c20 796f 7520 6d69 6768  erlink, you migh
+00010880: 7420 7772 6974 653a 2022 4f70 656e 7320  t write: "Opens 
+00010890: 6120 6e65 770a 2020 2020 2020 2020 2020  a new.          
+000108a0: 2020 6272 6f77 7365 7220 7461 6220 616e    browser tab an
+000108b0: 6420 6e61 7669 6761 7465 7320 746f 2074  d navigates to t
+000108c0: 6865 2047 6f6f 676c 6520 4368 6174 0a20  he Google Chat. 
+000108d0: 2020 2020 2020 2020 2020 2064 6576 656c             devel
+000108e0: 6f70 6572 2064 6f63 756d 656e 7461 7469  oper documentati
+000108f0: 6f6e 2061 740a 2020 2020 2020 2020 2020  on at.          
+00010900: 2020 6874 7470 733a 2f2f 6465 7665 6c6f    https://develo
+00010910: 7065 7273 2e67 6f6f 676c 652e 636f 6d2f  pers.google.com/
+00010920: 776f 726b 7370 6163 652f 6368 6174 222e  workspace/chat".
+00010930: 0a20 2020 2022 2222 0a0a 2020 2020 7465  .    """..    te
+00010940: 7874 3a20 7374 7220 3d20 7072 6f74 6f2e  xt: str = proto.
+00010950: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
+00010960: 726f 746f 2e53 5452 494e 472c 0a20 2020  roto.STRING,.   
+00010970: 2020 2020 206e 756d 6265 723d 312c 0a20       number=1,. 
+00010980: 2020 2029 0a20 2020 2069 636f 6e3a 2022     ).    icon: "
+00010990: 4963 6f6e 2220 3d20 7072 6f74 6f2e 4669  Icon" = proto.Fi
+000109a0: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
+000109b0: 746f 2e4d 4553 5341 4745 2c0a 2020 2020  to.MESSAGE,.    
+000109c0: 2020 2020 6e75 6d62 6572 3d32 2c0a 2020      number=2,.  
+000109d0: 2020 2020 2020 6d65 7373 6167 653d 2249        message="I
+000109e0: 636f 6e22 2c0a 2020 2020 290a 2020 2020  con",.    ).    
+000109f0: 636f 6c6f 723a 2063 6f6c 6f72 5f70 6232  color: color_pb2
+00010a00: 2e43 6f6c 6f72 203d 2070 726f 746f 2e46  .Color = proto.F
+00010a10: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
+00010a20: 6f74 6f2e 4d45 5353 4147 452c 0a20 2020  oto.MESSAGE,.   
+00010a30: 2020 2020 206e 756d 6265 723d 332c 0a20       number=3,. 
+00010a40: 2020 2020 2020 206d 6573 7361 6765 3d63         message=c
+00010a50: 6f6c 6f72 5f70 6232 2e43 6f6c 6f72 2c0a  olor_pb2.Color,.
+00010a60: 2020 2020 290a 2020 2020 6f6e 5f63 6c69      ).    on_cli
+00010a70: 636b 3a20 224f 6e43 6c69 636b 2220 3d20  ck: "OnClick" = 
+00010a80: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
+00010a90: 2020 2020 2070 726f 746f 2e4d 4553 5341       proto.MESSA
+00010aa0: 4745 2c0a 2020 2020 2020 2020 6e75 6d62  GE,.        numb
+00010ab0: 6572 3d34 2c0a 2020 2020 2020 2020 6d65  er=4,.        me
+00010ac0: 7373 6167 653d 224f 6e43 6c69 636b 222c  ssage="OnClick",
+00010ad0: 0a20 2020 2029 0a20 2020 2064 6973 6162  .    ).    disab
+00010ae0: 6c65 643a 2062 6f6f 6c20 3d20 7072 6f74  led: bool = prot
+00010af0: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+00010b00: 2070 726f 746f 2e42 4f4f 4c2c 0a20 2020   proto.BOOL,.   
+00010b10: 2020 2020 206e 756d 6265 723d 352c 0a20       number=5,. 
+00010b20: 2020 2029 0a20 2020 2061 6c74 5f74 6578     ).    alt_tex
+00010b30: 743a 2073 7472 203d 2070 726f 746f 2e46  t: str = proto.F
+00010b40: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
+00010b50: 6f74 6f2e 5354 5249 4e47 2c0a 2020 2020  oto.STRING,.    
+00010b60: 2020 2020 6e75 6d62 6572 3d36 2c0a 2020      number=6,.  
+00010b70: 2020 290a 0a0a 636c 6173 7320 4963 6f6e    )...class Icon
+00010b80: 2870 726f 746f 2e4d 6573 7361 6765 293a  (proto.Message):
+00010b90: 0a20 2020 2072 2222 2241 6e20 6963 6f6e  .    r"""An icon
+00010ba0: 2064 6973 706c 6179 6564 2069 6e20 6120   displayed in a 
+00010bb0: 7769 6467 6574 206f 6e20 6120 6361 7264  widget on a card
+00010bc0: 2e20 466f 7220 616e 2065 7861 6d70 6c65  . For an example
+00010bd0: 2069 6e20 476f 6f67 6c65 0a20 2020 2043   in Google.    C
+00010be0: 6861 7420 6170 7073 2c20 7365 6520 6041  hat apps, see `A
+00010bf0: 6464 2061 6e0a 2020 2020 6963 6f6e 203c  dd an.    icon <
+00010c00: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
+00010c10: 7273 2e67 6f6f 676c 652e 636f 6d2f 776f  rs.google.com/wo
+00010c20: 726b 7370 6163 652f 6368 6174 2f61 6464  rkspace/chat/add
+00010c30: 2d74 6578 742d 696d 6167 652d 6361 7264  -text-image-card
+00010c40: 2d64 6961 6c6f 6723 6164 645f 616e 5f69  -dialog#add_an_i
+00010c50: 636f 6e3e 605f 5f2e 0a0a 2020 2020 5375  con>`__...    Su
+00010c60: 7070 6f72 7473 0a20 2020 2060 6275 696c  pports.    `buil
+00010c70: 742d 696e 203c 6874 7470 733a 2f2f 6465  t-in <https://de
+00010c80: 7665 6c6f 7065 7273 2e67 6f6f 676c 652e  velopers.google.
+00010c90: 636f 6d2f 776f 726b 7370 6163 652f 6368  com/workspace/ch
+00010ca0: 6174 2f66 6f72 6d61 742d 6d65 7373 6167  at/format-messag
+00010cb0: 6573 2362 7569 6c74 696e 6963 6f6e 733e  es#builtinicons>
+00010cc0: 605f 5f0a 2020 2020 616e 640a 2020 2020  `__.    and.    
+00010cd0: 6063 7573 746f 6d20 3c68 7474 7073 3a2f  `custom <https:/
+00010ce0: 2f64 6576 656c 6f70 6572 732e 676f 6f67  /developers.goog
+00010cf0: 6c65 2e63 6f6d 2f77 6f72 6b73 7061 6365  le.com/workspace
+00010d00: 2f63 6861 742f 666f 726d 6174 2d6d 6573  /chat/format-mes
+00010d10: 7361 6765 7323 6375 7374 6f6d 6963 6f6e  sages#customicon
+00010d20: 733e 605f 5f0a 2020 2020 6963 6f6e 732e  s>`__.    icons.
+00010d30: 0a0a 2020 2020 6047 6f6f 676c 6520 576f  ..    `Google Wo
+00010d40: 726b 7370 6163 6520 4164 642d 6f6e 7320  rkspace Add-ons 
+00010d50: 616e 6420 4368 6174 0a20 2020 2061 7070  and Chat.    app
+00010d60: 7320 3c68 7474 7073 3a2f 2f64 6576 656c  s <https://devel
+00010d70: 6f70 6572 732e 676f 6f67 6c65 2e63 6f6d  opers.google.com
+00010d80: 2f77 6f72 6b73 7061 6365 2f65 7874 656e  /workspace/exten
+00010d90: 643e 605f 5f3a 0a0a 2020 2020 5468 6973  d>`__:..    This
+00010da0: 206d 6573 7361 6765 2068 6173 2060 6f6e   message has `on
+00010db0: 656f 6660 5f20 6669 656c 6473 2028 6d75  eof`_ fields (mu
+00010dc0: 7475 616c 6c79 2065 7863 6c75 7369 7665  tually exclusive
+00010dd0: 2066 6965 6c64 7329 2e0a 2020 2020 466f   fields)..    Fo
+00010de0: 7220 6561 6368 206f 6e65 6f66 2c20 6174  r each oneof, at
+00010df0: 206d 6f73 7420 6f6e 6520 6d65 6d62 6572   most one member
+00010e00: 2066 6965 6c64 2063 616e 2062 6520 7365   field can be se
+00010e10: 7420 6174 2074 6865 2073 616d 6520 7469  t at the same ti
+00010e20: 6d65 2e0a 2020 2020 5365 7474 696e 6720  me..    Setting 
+00010e30: 616e 7920 6d65 6d62 6572 206f 6620 7468  any member of th
+00010e40: 6520 6f6e 656f 6620 6175 746f 6d61 7469  e oneof automati
+00010e50: 6361 6c6c 7920 636c 6561 7273 2061 6c6c  cally clears all
+00010e60: 206f 7468 6572 0a20 2020 206d 656d 6265   other.    membe
+00010e70: 7273 2e0a 0a20 2020 202e 2e20 5f6f 6e65  rs...    .. _one
+00010e80: 6f66 3a20 6874 7470 733a 2f2f 7072 6f74  of: https://prot
+00010e90: 6f2d 706c 7573 2d70 7974 686f 6e2e 7265  o-plus-python.re
+00010ea0: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+00010eb0: 7374 6162 6c65 2f66 6965 6c64 732e 6874  stable/fields.ht
+00010ec0: 6d6c 236f 6e65 6f66 732d 6d75 7475 616c  ml#oneofs-mutual
+00010ed0: 6c79 2d65 7863 6c75 7369 7665 2d66 6965  ly-exclusive-fie
+00010ee0: 6c64 730a 0a20 2020 2041 7474 7269 6275  lds..    Attribu
+00010ef0: 7465 733a 0a20 2020 2020 2020 206b 6e6f  tes:.        kno
+00010f00: 776e 5f69 636f 6e20 2873 7472 293a 0a20  wn_icon (str):. 
+00010f10: 2020 2020 2020 2020 2020 2044 6973 706c             Displ
+00010f20: 6179 206f 6e65 206f 6620 7468 6520 6275  ay one of the bu
+00010f30: 696c 742d 696e 2069 636f 6e73 2070 726f  ilt-in icons pro
+00010f40: 7669 6465 6420 6279 2047 6f6f 676c 650a  vided by Google.
+00010f50: 2020 2020 2020 2020 2020 2020 576f 726b              Work
+00010f60: 7370 6163 652e 0a0a 2020 2020 2020 2020  space...        
+00010f70: 2020 2020 466f 7220 6578 616d 706c 652c      For example,
+00010f80: 2074 6f20 6469 7370 6c61 7920 616e 2061   to display an a
+00010f90: 6972 706c 616e 6520 6963 6f6e 2c20 7370  irplane icon, sp
+00010fa0: 6563 6966 790a 2020 2020 2020 2020 2020  ecify.          
+00010fb0: 2020 6060 4149 5250 4c41 4e45 6060 2e20    ``AIRPLANE``. 
+00010fc0: 466f 7220 6120 6275 732c 2073 7065 6369  For a bus, speci
+00010fd0: 6679 2060 6042 5553 6060 2e0a 0a20 2020  fy ``BUS``...   
+00010fe0: 2020 2020 2020 2020 2046 6f72 2061 2066           For a f
+00010ff0: 756c 6c20 6c69 7374 206f 6620 7375 7070  ull list of supp
+00011000: 6f72 7465 6420 6963 6f6e 732c 2073 6565  orted icons, see
+00011010: 2060 6275 696c 742d 696e 0a20 2020 2020   `built-in.     
+00011020: 2020 2020 2020 2069 636f 6e73 203c 6874         icons <ht
+00011030: 7470 733a 2f2f 6465 7665 6c6f 7065 7273  tps://developers
+00011040: 2e67 6f6f 676c 652e 636f 6d2f 776f 726b  .google.com/work
+00011050: 7370 6163 652f 6368 6174 2f66 6f72 6d61  space/chat/forma
+00011060: 742d 6d65 7373 6167 6573 2362 7569 6c74  t-messages#built
+00011070: 696e 6963 6f6e 733e 605f 5f2e 0a0a 2020  inicons>`__...  
+00011080: 2020 2020 2020 2020 2020 5468 6973 2066            This f
+00011090: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
+000110a0: 206f 6620 606f 6e65 6f66 605f 2060 6069   of `oneof`_ ``i
+000110b0: 636f 6e73 6060 2e0a 2020 2020 2020 2020  cons``..        
+000110c0: 6963 6f6e 5f75 726c 2028 7374 7229 3a0a  icon_url (str):.
+000110d0: 2020 2020 2020 2020 2020 2020 4469 7370              Disp
+000110e0: 6c61 7920 6120 6375 7374 6f6d 2069 636f  lay a custom ico
+000110f0: 6e20 686f 7374 6564 2061 7420 616e 2048  n hosted at an H
+00011100: 5454 5053 2055 524c 2e0a 0a20 2020 2020  TTPS URL...     
+00011110: 2020 2020 2020 2046 6f72 2065 7861 6d70         For examp
+00011120: 6c65 3a0a 0a20 2020 2020 2020 2020 2020  le:..           
+00011130: 203a 3a0a 0a20 2020 2020 2020 2020 2020   ::..           
+00011140: 2020 2020 2269 636f 6e55 726c 223a 0a20      "iconUrl":. 
+00011150: 2020 2020 2020 2020 2020 2020 2020 2268                "h
+00011160: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
+00011170: 732e 676f 6f67 6c65 2e63 6f6d 2f77 6f72  s.google.com/wor
+00011180: 6b73 7061 6365 2f63 6861 742f 696d 6167  kspace/chat/imag
+00011190: 6573 2f71 7569 636b 7374 6172 742d 6170  es/quickstart-ap
+000111a0: 702d 6176 6174 6172 2e70 6e67 220a 0a20  p-avatar.png".. 
+000111b0: 2020 2020 2020 2020 2020 2053 7570 706f             Suppo
+000111c0: 7274 6564 2066 696c 6520 7479 7065 7320  rted file types 
+000111d0: 696e 636c 7564 6520 6060 2e70 6e67 6060  include ``.png``
+000111e0: 2061 6e64 2060 602e 6a70 6760 602e 0a0a   and ``.jpg``...
+000111f0: 2020 2020 2020 2020 2020 2020 5468 6973              This
+00011200: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
+00011210: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
+00011220: 6069 636f 6e73 6060 2e0a 2020 2020 2020  `icons``..      
+00011230: 2020 6d61 7465 7269 616c 5f69 636f 6e20    material_icon 
+00011240: 2867 6f6f 676c 652e 6170 7073 2e63 6172  (google.apps.car
+00011250: 645f 7631 2e74 7970 6573 2e4d 6174 6572  d_v1.types.Mater
+00011260: 6961 6c49 636f 6e29 3a0a 2020 2020 2020  ialIcon):.      
+00011270: 2020 2020 2020 4469 7370 6c61 7920 6f6e        Display on
+00011280: 6520 6f66 2074 6865 2060 476f 6f67 6c65  e of the `Google
+00011290: 204d 6174 6572 6961 6c0a 2020 2020 2020   Material.      
+000112a0: 2020 2020 2020 4963 6f6e 7320 3c68 7474        Icons <htt
+000112b0: 7073 3a2f 2f66 6f6e 7473 2e67 6f6f 676c  ps://fonts.googl
+000112c0: 652e 636f 6d2f 6963 6f6e 733e 605f 5f2e  e.com/icons>`__.
+000112d0: 0a0a 2020 2020 2020 2020 2020 2020 466f  ..            Fo
+000112e0: 7220 6578 616d 706c 652c 2074 6f20 6469  r example, to di
+000112f0: 7370 6c61 7920 6120 6063 6865 636b 626f  splay a `checkbo
+00011300: 780a 2020 2020 2020 2020 2020 2020 6963  x.            ic
+00011310: 6f6e 203c 6874 7470 733a 2f2f 666f 6e74  on <https://font
+00011320: 732e 676f 6f67 6c65 2e63 6f6d 2f69 636f  s.google.com/ico
+00011330: 6e73 3f73 656c 6563 7465 643d 4d61 7465  ns?selected=Mate
+00011340: 7269 616c 2532 3053 796d 626f 6c73 2532  rial%20Symbols%2
+00011350: 304f 7574 6c69 6e65 6425 3341 6368 6563  0Outlined%3Achec
+00011360: 6b5f 626f 7825 3341 4649 4c4c 2534 3030  k_box%3AFILL%400
+00011370: 2533 4277 6768 7425 3430 3430 3025 3342  %3Bwght%40400%3B
+00011380: 4752 4144 2534 3030 2533 426f 7073 7a25  GRAD%400%3Bopsz%
+00011390: 3430 3438 3e60 5f5f 2c0a 2020 2020 2020  4048>`__,.      
+000113a0: 2020 2020 2020 7573 650a 0a20 2020 2020        use..     
+000113b0: 2020 2020 2020 203a 3a0a 0a20 2020 2020         ::..     
+000113c0: 2020 2020 2020 2020 2020 226d 6174 6572            "mater
+000113d0: 6961 6c5f 6963 6f6e 223a 207b 0a20 2020  ial_icon": {.   
+000113e0: 2020 2020 2020 2020 2020 2020 2020 226e                "n
+000113f0: 616d 6522 3a20 2263 6865 636b 5f62 6f78  ame": "check_box
+00011400: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00011410: 207d 0a0a 2020 2020 2020 2020 2020 2020   }..            
+00011420: 6047 6f6f 676c 6520 4368 6174 0a20 2020  `Google Chat.   
+00011430: 2020 2020 2020 2020 2061 7070 7320 3c68           apps <h
+00011440: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
+00011450: 732e 676f 6f67 6c65 2e63 6f6d 2f77 6f72  s.google.com/wor
+00011460: 6b73 7061 6365 2f63 6861 743e 605f 5f3a  kspace/chat>`__:
+00011470: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
+00011480: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
+00011490: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
+000114a0: 2060 6069 636f 6e73 6060 2e0a 2020 2020   ``icons``..    
+000114b0: 2020 2020 616c 745f 7465 7874 2028 7374      alt_text (st
+000114c0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+000114d0: 4f70 7469 6f6e 616c 2e20 4120 6465 7363  Optional. A desc
+000114e0: 7269 7074 696f 6e20 6f66 2074 6865 2069  ription of the i
+000114f0: 636f 6e20 7573 6564 2066 6f72 2061 6363  con used for acc
+00011500: 6573 7369 6269 6c69 7479 2e0a 2020 2020  essibility..    
+00011510: 2020 2020 2020 2020 4966 2075 6e73 7065          If unspe
+00011520: 6369 6669 6564 2c20 7468 6520 6465 6661  cified, the defa
+00011530: 756c 7420 7661 6c75 6520 6060 4275 7474  ult value ``Butt
+00011540: 6f6e 6060 2069 7320 7072 6f76 6964 6564  on`` is provided
+00011550: 2e20 4173 0a20 2020 2020 2020 2020 2020  . As.           
+00011560: 2061 2062 6573 7420 7072 6163 7469 6365   a best practice
+00011570: 2c20 796f 7520 7368 6f75 6c64 2073 6574  , you should set
+00011580: 2061 2068 656c 7066 756c 2064 6573 6372   a helpful descr
+00011590: 6970 7469 6f6e 2066 6f72 0a20 2020 2020  iption for.     
+000115a0: 2020 2020 2020 2077 6861 7420 7468 6520         what the 
+000115b0: 6963 6f6e 2064 6973 706c 6179 732c 2061  icon displays, a
+000115c0: 6e64 2069 6620 6170 706c 6963 6162 6c65  nd if applicable
+000115d0: 2c20 7768 6174 2069 7420 646f 6573 2e20  , what it does. 
+000115e0: 466f 720a 2020 2020 2020 2020 2020 2020  For.            
+000115f0: 6578 616d 706c 652c 2060 6041 2075 7365  example, ``A use
+00011600: 7227 7320 6163 636f 756e 7420 706f 7274  r's account port
+00011610: 7261 6974 6060 2c20 6f72 0a20 2020 2020  rait``, or.     
+00011620: 2020 2020 2020 2060 604f 7065 6e73 2061         ``Opens a
+00011630: 206e 6577 2062 726f 7773 6572 2074 6162   new browser tab
+00011640: 2061 6e64 206e 6176 6967 6174 6573 2074   and navigates t
+00011650: 6f20 7468 6520 476f 6f67 6c65 2043 6861  o the Google Cha
+00011660: 7420 6465 7665 6c6f 7065 7220 646f 6375  t developer docu
+00011670: 6d65 6e74 6174 696f 6e20 6174 2068 7474  mentation at htt
+00011680: 7073 3a2f 2f64 6576 656c 6f70 6572 732e  ps://developers.
+00011690: 676f 6f67 6c65 2e63 6f6d 2f77 6f72 6b73  google.com/works
+000116a0: 7061 6365 2f63 6861 7460 602e 0a0a 2020  pace/chat``...  
+000116b0: 2020 2020 2020 2020 2020 4966 2074 6865            If the
+000116c0: 2069 636f 6e20 6973 2073 6574 2069 6e20   icon is set in 
+000116d0: 610a 2020 2020 2020 2020 2020 2020 5b60  a.            [`
+000116e0: 6042 7574 746f 6e60 605d 5b67 6f6f 676c  `Button``][googl
+000116f0: 652e 6170 7073 2e63 6172 642e 7631 2e42  e.apps.card.v1.B
+00011700: 7574 746f 6e5d 2c20 7468 6520 6060 616c  utton], the ``al
+00011710: 7454 6578 7460 600a 2020 2020 2020 2020  tText``.        
+00011720: 2020 2020 6170 7065 6172 7320 6173 2068      appears as h
+00011730: 656c 7065 7220 7465 7874 2077 6865 6e20  elper text when 
+00011740: 7468 6520 7573 6572 2068 6f76 6572 7320  the user hovers 
+00011750: 6f76 6572 2074 6865 2062 7574 746f 6e2e  over the button.
+00011760: 0a20 2020 2020 2020 2020 2020 2048 6f77  .            How
+00011770: 6576 6572 2c20 6966 2074 6865 2062 7574  ever, if the but
+00011780: 746f 6e20 616c 736f 2073 6574 7320 6060  ton also sets ``
+00011790: 7465 7874 6060 2c20 7468 6520 6963 6f6e  text``, the icon
+000117a0: 2773 0a20 2020 2020 2020 2020 2020 2060  's.            `
+000117b0: 6061 6c74 5465 7874 6060 2069 7320 6967  `altText`` is ig
+000117c0: 6e6f 7265 642e 0a20 2020 2020 2020 2069  nored..        i
+000117d0: 6d61 6765 5f74 7970 6520 2867 6f6f 676c  mage_type (googl
+000117e0: 652e 6170 7073 2e63 6172 645f 7631 2e74  e.apps.card_v1.t
+000117f0: 7970 6573 2e57 6964 6765 742e 496d 6167  ypes.Widget.Imag
+00011800: 6554 7970 6529 3a0a 2020 2020 2020 2020  eType):.        
+00011810: 2020 2020 5468 6520 6372 6f70 2073 7479      The crop sty
+00011820: 6c65 2061 7070 6c69 6564 2074 6f20 7468  le applied to th
+00011830: 6520 696d 6167 652e 2049 6e20 736f 6d65  e image. In some
+00011840: 2063 6173 6573 2c20 6170 706c 7969 6e67   cases, applying
+00011850: 0a20 2020 2020 2020 2020 2020 2061 2060  .            a `
+00011860: 6043 4952 434c 4560 6020 6372 6f70 2063  `CIRCLE`` crop c
+00011870: 6175 7365 7320 7468 6520 696d 6167 6520  auses the image 
+00011880: 746f 2062 6520 6472 6177 6e20 6c61 7267  to be drawn larg
+00011890: 6572 2074 6861 6e20 610a 2020 2020 2020  er than a.      
+000118a0: 2020 2020 2020 6275 696c 742d 696e 2069        built-in i
+000118b0: 636f 6e2e 0a20 2020 2022 2222 0a0a 2020  con..    """..  
+000118c0: 2020 6b6e 6f77 6e5f 6963 6f6e 3a20 7374    known_icon: st
+000118d0: 7220 3d20 7072 6f74 6f2e 4669 656c 6428  r = proto.Field(
+000118e0: 0a20 2020 2020 2020 2070 726f 746f 2e53  .        proto.S
+000118f0: 5452 494e 472c 0a20 2020 2020 2020 206e  TRING,.        n
+00011900: 756d 6265 723d 312c 0a20 2020 2020 2020  umber=1,.       
+00011910: 206f 6e65 6f66 3d22 6963 6f6e 7322 2c0a   oneof="icons",.
+00011920: 2020 2020 290a 2020 2020 6963 6f6e 5f75      ).    icon_u
+00011930: 726c 3a20 7374 7220 3d20 7072 6f74 6f2e  rl: str = proto.
+00011940: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
+00011950: 726f 746f 2e53 5452 494e 472c 0a20 2020  roto.STRING,.   
+00011960: 2020 2020 206e 756d 6265 723d 322c 0a20       number=2,. 
+00011970: 2020 2020 2020 206f 6e65 6f66 3d22 6963         oneof="ic
+00011980: 6f6e 7322 2c0a 2020 2020 290a 2020 2020  ons",.    ).    
+00011990: 6d61 7465 7269 616c 5f69 636f 6e3a 2022  material_icon: "
+000119a0: 4d61 7465 7269 616c 4963 6f6e 2220 3d20  MaterialIcon" = 
+000119b0: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
+000119c0: 2020 2020 2070 726f 746f 2e4d 4553 5341       proto.MESSA
+000119d0: 4745 2c0a 2020 2020 2020 2020 6e75 6d62  GE,.        numb
+000119e0: 6572 3d35 2c0a 2020 2020 2020 2020 6f6e  er=5,.        on
+000119f0: 656f 663d 2269 636f 6e73 222c 0a20 2020  eof="icons",.   
+00011a00: 2020 2020 206d 6573 7361 6765 3d22 4d61       message="Ma
+00011a10: 7465 7269 616c 4963 6f6e 222c 0a20 2020  terialIcon",.   
+00011a20: 2029 0a20 2020 2061 6c74 5f74 6578 743a   ).    alt_text:
+00011a30: 2073 7472 203d 2070 726f 746f 2e46 6965   str = proto.Fie
+00011a40: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
+00011a50: 6f2e 5354 5249 4e47 2c0a 2020 2020 2020  o.STRING,.      
+00011a60: 2020 6e75 6d62 6572 3d33 2c0a 2020 2020    number=3,.    
+00011a70: 290a 2020 2020 696d 6167 655f 7479 7065  ).    image_type
+00011a80: 3a20 2257 6964 6765 742e 496d 6167 6554  : "Widget.ImageT
+00011a90: 7970 6522 203d 2070 726f 746f 2e46 6965  ype" = proto.Fie
+00011aa0: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
+00011ab0: 6f2e 454e 554d 2c0a 2020 2020 2020 2020  o.ENUM,.        
+00011ac0: 6e75 6d62 6572 3d34 2c0a 2020 2020 2020  number=4,.      
+00011ad0: 2020 656e 756d 3d22 5769 6467 6574 2e49    enum="Widget.I
+00011ae0: 6d61 6765 5479 7065 222c 0a20 2020 2029  mageType",.    )
+00011af0: 0a0a 0a63 6c61 7373 204d 6174 6572 6961  ...class Materia
+00011b00: 6c49 636f 6e28 7072 6f74 6f2e 4d65 7373  lIcon(proto.Mess
+00011b10: 6167 6529 3a0a 2020 2020 7222 2222 4120  age):.    r"""A 
+00011b20: 6047 6f6f 676c 6520 4d61 7465 7269 616c  `Google Material
+00011b30: 2049 636f 6e20 3c68 7474 7073 3a2f 2f66   Icon <https://f
+00011b40: 6f6e 7473 2e67 6f6f 676c 652e 636f 6d2f  onts.google.com/
+00011b50: 6963 6f6e 733e 605f 5f2c 2077 6869 6368  icons>`__, which
+00011b60: 0a20 2020 2069 6e63 6c75 6465 7320 6f76  .    includes ov
+00011b70: 6572 2032 3530 302b 206f 7074 696f 6e73  er 2500+ options
+00011b80: 2e0a 0a20 2020 2046 6f72 2065 7861 6d70  ...    For examp
+00011b90: 6c65 2c20 746f 2064 6973 706c 6179 2061  le, to display a
+00011ba0: 2060 6368 6563 6b62 6f78 0a20 2020 2069   `checkbox.    i
+00011bb0: 636f 6e20 3c68 7474 7073 3a2f 2f66 6f6e  con <https://fon
+00011bc0: 7473 2e67 6f6f 676c 652e 636f 6d2f 6963  ts.google.com/ic
+00011bd0: 6f6e 733f 7365 6c65 6374 6564 3d4d 6174  ons?selected=Mat
+00011be0: 6572 6961 6c25 3230 5379 6d62 6f6c 7325  erial%20Symbols%
+00011bf0: 3230 4f75 746c 696e 6564 2533 4163 6865  20Outlined%3Ache
+00011c00: 636b 5f62 6f78 2533 4146 494c 4c25 3430  ck_box%3AFILL%40
+00011c10: 3025 3342 7767 6874 2534 3034 3030 2533  0%3Bwght%40400%3
+00011c20: 4247 5241 4425 3430 3025 3342 6f70 737a  BGRAD%400%3Bopsz
+00011c30: 2534 3034 383e 605f 5f0a 2020 2020 7769  %4048>`__.    wi
+00011c40: 7468 2063 7573 746f 6d69 7a65 6420 7765  th customized we
+00011c50: 6967 6874 2061 6e64 2067 7261 6465 2c20  ight and grade, 
+00011c60: 7772 6974 6520 7468 6520 666f 6c6c 6f77  write the follow
+00011c70: 696e 673a 0a0a 2020 2020 3a3a 0a0a 2020  ing:..    ::..  
+00011c80: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00011c90: 226e 616d 6522 3a20 2263 6865 636b 5f62  "name": "check_b
+00011ca0: 6f78 222c 0a20 2020 2020 2020 2020 2266  ox",.         "f
+00011cb0: 696c 6c22 3a20 7472 7565 2c0a 2020 2020  ill": true,.    
+00011cc0: 2020 2020 2022 7765 6967 6874 223a 2033       "weight": 3
+00011cd0: 3030 2c0a 2020 2020 2020 2020 2022 6772  00,.         "gr
+00011ce0: 6164 6522 3a20 2d32 350a 2020 2020 2020  ade": -25.      
+00011cf0: 207d 0a0a 2020 2020 6047 6f6f 676c 6520   }..    `Google 
+00011d00: 4368 6174 2061 7070 7320 3c68 7474 7073  Chat apps <https
+00011d10: 3a2f 2f64 6576 656c 6f70 6572 732e 676f  ://developers.go
+00011d20: 6f67 6c65 2e63 6f6d 2f77 6f72 6b73 7061  ogle.com/workspa
+00011d30: 6365 2f63 6861 743e 605f 5f3a 0a0a 2020  ce/chat>`__:..  
+00011d40: 2020 4174 7472 6962 7574 6573 3a0a 2020    Attributes:.  
+00011d50: 2020 2020 2020 6e61 6d65 2028 7374 7229        name (str)
+00011d60: 3a0a 2020 2020 2020 2020 2020 2020 5468  :.            Th
+00011d70: 6520 6963 6f6e 206e 616d 6520 6465 6669  e icon name defi
+00011d80: 6e65 6420 696e 2074 6865 2060 476f 6f67  ned in the `Goog
+00011d90: 6c65 204d 6174 6572 6961 6c0a 2020 2020  le Material.    
+00011da0: 2020 2020 2020 2020 4963 6f6e 203c 6874          Icon <ht
+00011db0: 7470 733a 2f2f 666f 6e74 732e 676f 6f67  tps://fonts.goog
+00011dc0: 6c65 2e63 6f6d 2f69 636f 6e73 3e60 5f5f  le.com/icons>`__
+00011dd0: 2c20 666f 7220 6578 616d 706c 652c 0a20  , for example,. 
+00011de0: 2020 2020 2020 2020 2020 2060 6063 6865             ``che
+00011df0: 636b 5f62 6f78 6060 2e20 416e 7920 696e  ck_box``. Any in
+00011e00: 7661 6c69 6420 6e61 6d65 7320 6172 6520  valid names are 
+00011e10: 6162 616e 646f 6e65 6420 616e 6420 7265  abandoned and re
+00011e20: 706c 6163 6564 0a20 2020 2020 2020 2020  placed.         
+00011e30: 2020 2077 6974 6820 656d 7074 7920 7374     with empty st
+00011e40: 7269 6e67 2061 6e64 2072 6573 756c 7473  ring and results
+00011e50: 2069 6e20 7468 6520 6963 6f6e 2066 6169   in the icon fai
+00011e60: 6c69 6e67 2074 6f20 7265 6e64 6572 2e0a  ling to render..
+00011e70: 2020 2020 2020 2020 6669 6c6c 2028 626f          fill (bo
+00011e80: 6f6c 293a 0a20 2020 2020 2020 2020 2020  ol):.           
+00011e90: 2057 6865 7468 6572 2074 6865 2069 636f   Whether the ico
+00011ea0: 6e20 7265 6e64 6572 7320 6173 2066 696c  n renders as fil
+00011eb0: 6c65 642e 2044 6566 6175 6c74 2076 616c  led. Default val
+00011ec0: 7565 2069 7320 6661 6c73 652e 0a0a 2020  ue is false...  
+00011ed0: 2020 2020 2020 2020 2020 546f 2070 7265            To pre
+00011ee0: 7669 6577 2064 6966 6665 7265 6e74 2069  view different i
+00011ef0: 636f 6e20 7365 7474 696e 6773 2c20 676f  con settings, go
+00011f00: 2074 6f20 6047 6f6f 676c 6520 466f 6e74   to `Google Font
+00011f10: 0a20 2020 2020 2020 2020 2020 2049 636f  .            Ico
+00011f20: 6e73 203c 6874 7470 733a 2f2f 666f 6e74  ns <https://font
+00011f30: 732e 676f 6f67 6c65 2e63 6f6d 2f69 636f  s.google.com/ico
+00011f40: 6e73 3e60 5f5f 2061 6e64 2061 646a 7573  ns>`__ and adjus
+00011f50: 7420 7468 650a 2020 2020 2020 2020 2020  t the.          
+00011f60: 2020 7365 7474 696e 6773 2075 6e64 6572    settings under
+00011f70: 202a 2a43 7573 746f 6d69 7a65 2a2a 2e0a   **Customize**..
+00011f80: 2020 2020 2020 2020 7765 6967 6874 2028          weight (
+00011f90: 696e 7429 3a0a 2020 2020 2020 2020 2020  int):.          
+00011fa0: 2020 5468 6520 7374 726f 6b65 2077 6569    The stroke wei
+00011fb0: 6768 7420 6f66 2074 6865 2069 636f 6e2e  ght of the icon.
+00011fc0: 2043 686f 6f73 6520 6672 6f6d 207b 3130   Choose from {10
+00011fd0: 302c 2032 3030 2c20 3330 302c 0a20 2020  0, 200, 300,.   
+00011fe0: 2020 2020 2020 2020 2034 3030 2c20 3530           400, 50
+00011ff0: 302c 2036 3030 2c20 3730 307d 2e20 4966  0, 600, 700}. If
+00012000: 2061 6273 656e 742c 2064 6566 6175 6c74   absent, default
+00012010: 2076 616c 7565 2069 7320 3430 302e 2049   value is 400. I
+00012020: 6620 616e 790a 2020 2020 2020 2020 2020  f any.          
+00012030: 2020 6f74 6865 7220 7661 6c75 6520 6973    other value is
+00012040: 2073 7065 6369 6669 6564 2c20 7468 6520   specified, the 
+00012050: 6465 6661 756c 7420 7661 6c75 6520 6973  default value is
+00012060: 2075 7365 642e 0a0a 2020 2020 2020 2020   used...        
+00012070: 2020 2020 546f 2070 7265 7669 6577 2064      To preview d
+00012080: 6966 6665 7265 6e74 2069 636f 6e20 7365  ifferent icon se
+00012090: 7474 696e 6773 2c20 676f 2074 6f20 6047  ttings, go to `G
+000120a0: 6f6f 676c 6520 466f 6e74 0a20 2020 2020  oogle Font.     
+000120b0: 2020 2020 2020 2049 636f 6e73 203c 6874         Icons <ht
+000120c0: 7470 733a 2f2f 666f 6e74 732e 676f 6f67  tps://fonts.goog
+000120d0: 6c65 2e63 6f6d 2f69 636f 6e73 3e60 5f5f  le.com/icons>`__
+000120e0: 2061 6e64 2061 646a 7573 7420 7468 650a   and adjust the.
+000120f0: 2020 2020 2020 2020 2020 2020 7365 7474              sett
+00012100: 696e 6773 2075 6e64 6572 202a 2a43 7573  ings under **Cus
+00012110: 746f 6d69 7a65 2a2a 2e0a 2020 2020 2020  tomize**..      
+00012120: 2020 6772 6164 6520 2869 6e74 293a 0a20    grade (int):. 
+00012130: 2020 2020 2020 2020 2020 2057 6569 6768             Weigh
+00012140: 7420 616e 6420 6772 6164 6520 6166 6665  t and grade affe
+00012150: 6374 2061 2073 796d 626f 6ce2 8099 7320  ct a symbol...s 
+00012160: 7468 6963 6b6e 6573 732e 2041 646a 7573  thickness. Adjus
+00012170: 746d 656e 7473 2074 6f0a 2020 2020 2020  tments to.      
+00012180: 2020 2020 2020 6772 6164 6520 6172 6520        grade are 
+00012190: 6d6f 7265 2067 7261 6e75 6c61 7220 7468  more granular th
+000121a0: 616e 2061 646a 7573 746d 656e 7473 2074  an adjustments t
+000121b0: 6f20 7765 6967 6874 2061 6e64 2068 6176  o weight and hav
+000121c0: 650a 2020 2020 2020 2020 2020 2020 6120  e.            a 
+000121d0: 736d 616c 6c20 696d 7061 6374 206f 6e20  small impact on 
+000121e0: 7468 6520 7369 7a65 206f 6620 7468 6520  the size of the 
+000121f0: 7379 6d62 6f6c 2e20 4368 6f6f 7365 2066  symbol. Choose f
+00012200: 726f 6d20 7b2d 3235 2c0a 2020 2020 2020  rom {-25,.      
+00012210: 2020 2020 2020 302c 2032 3030 7d2e 2049        0, 200}. I
+00012220: 6620 6162 7365 6e74 2c20 6465 6661 756c  f absent, defaul
+00012230: 7420 7661 6c75 6520 6973 2030 2e20 4966  t value is 0. If
+00012240: 2061 6e79 206f 7468 6572 2076 616c 7565   any other value
+00012250: 0a20 2020 2020 2020 2020 2020 2069 7320  .            is 
+00012260: 7370 6563 6966 6965 642c 2074 6865 2064  specified, the d
+00012270: 6566 6175 6c74 2076 616c 7565 2069 7320  efault value is 
+00012280: 7573 6564 2e0a 0a20 2020 2020 2020 2020  used...         
+00012290: 2020 2054 6f20 7072 6576 6965 7720 6469     To preview di
+000122a0: 6666 6572 656e 7420 6963 6f6e 2073 6574  fferent icon set
+000122b0: 7469 6e67 732c 2067 6f20 746f 2060 476f  tings, go to `Go
+000122c0: 6f67 6c65 2046 6f6e 740a 2020 2020 2020  ogle Font.      
+000122d0: 2020 2020 2020 4963 6f6e 7320 3c68 7474        Icons <htt
+000122e0: 7073 3a2f 2f66 6f6e 7473 2e67 6f6f 676c  ps://fonts.googl
+000122f0: 652e 636f 6d2f 6963 6f6e 733e 605f 5f20  e.com/icons>`__ 
+00012300: 616e 6420 6164 6a75 7374 2074 6865 0a20  and adjust the. 
+00012310: 2020 2020 2020 2020 2020 2073 6574 7469             setti
+00012320: 6e67 7320 756e 6465 7220 2a2a 4375 7374  ngs under **Cust
+00012330: 6f6d 697a 652a 2a2e 0a20 2020 2022 2222  omize**..    """
+00012340: 0a0a 2020 2020 6e61 6d65 3a20 7374 7220  ..    name: str 
+00012350: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
+00012360: 2020 2020 2020 2070 726f 746f 2e53 5452         proto.STR
+00012370: 494e 472c 0a20 2020 2020 2020 206e 756d  ING,.        num
+00012380: 6265 723d 312c 0a20 2020 2029 0a20 2020  ber=1,.    ).   
+00012390: 2066 696c 6c3a 2062 6f6f 6c20 3d20 7072   fill: bool = pr
+000123a0: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
+000123b0: 2020 2070 726f 746f 2e42 4f4f 4c2c 0a20     proto.BOOL,. 
+000123c0: 2020 2020 2020 206e 756d 6265 723d 322c         number=2,
+000123d0: 0a20 2020 2029 0a20 2020 2077 6569 6768  .    ).    weigh
+000123e0: 743a 2069 6e74 203d 2070 726f 746f 2e46  t: int = proto.F
+000123f0: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
+00012400: 6f74 6f2e 494e 5433 322c 0a20 2020 2020  oto.INT32,.     
+00012410: 2020 206e 756d 6265 723d 332c 0a20 2020     number=3,.   
+00012420: 2029 0a20 2020 2067 7261 6465 3a20 696e   ).    grade: in
+00012430: 7420 3d20 7072 6f74 6f2e 4669 656c 6428  t = proto.Field(
+00012440: 0a20 2020 2020 2020 2070 726f 746f 2e49  .        proto.I
+00012450: 4e54 3332 2c0a 2020 2020 2020 2020 6e75  NT32,.        nu
+00012460: 6d62 6572 3d34 2c0a 2020 2020 290a 0a0a  mber=4,.    )...
+00012470: 636c 6173 7320 496d 6167 6543 726f 7053  class ImageCropS
+00012480: 7479 6c65 2870 726f 746f 2e4d 6573 7361  tyle(proto.Messa
+00012490: 6765 293a 0a20 2020 2072 2222 2252 6570  ge):.    r"""Rep
+000124a0: 7265 7365 6e74 7320 7468 6520 6372 6f70  resents the crop
+000124b0: 2073 7479 6c65 2061 7070 6c69 6564 2074   style applied t
+000124c0: 6f20 616e 2069 6d61 6765 2e0a 0a20 2020  o an image...   
+000124d0: 2060 476f 6f67 6c65 2057 6f72 6b73 7061   `Google Workspa
+000124e0: 6365 2041 6464 2d6f 6e73 2061 6e64 2043  ce Add-ons and C
+000124f0: 6861 740a 2020 2020 6170 7073 203c 6874  hat.    apps <ht
+00012500: 7470 733a 2f2f 6465 7665 6c6f 7065 7273  tps://developers
+00012510: 2e67 6f6f 676c 652e 636f 6d2f 776f 726b  .google.com/work
+00012520: 7370 6163 652f 6578 7465 6e64 3e60 5f5f  space/extend>`__
+00012530: 3a0a 0a20 2020 2046 6f72 2065 7861 6d70  :..    For examp
+00012540: 6c65 2c20 6865 7265 2773 2068 6f77 2074  le, here's how t
+00012550: 6f20 6170 706c 7920 6120 3136 3a39 2061  o apply a 16:9 a
+00012560: 7370 6563 7420 7261 7469 6f3a 0a0a 2020  spect ratio:..  
+00012570: 2020 3a3a 0a0a 2020 2020 2020 2063 726f    ::..       cro
+00012580: 7053 7479 6c65 207b 0a20 2020 2020 2020  pStyle {.       
+00012590: 2022 7479 7065 223a 2022 5245 4354 414e   "type": "RECTAN
+000125a0: 474c 455f 4355 5354 4f4d 222c 0a20 2020  GLE_CUSTOM",.   
+000125b0: 2020 2020 2022 6173 7065 6374 5261 7469       "aspectRati
+000125c0: 6f22 3a20 3136 2f39 0a20 2020 2020 2020  o": 16/9.       
+000125d0: 7d0a 0a20 2020 2041 7474 7269 6275 7465  }..    Attribute
+000125e0: 733a 0a20 2020 2020 2020 2074 7970 655f  s:.        type_
+000125f0: 2028 676f 6f67 6c65 2e61 7070 732e 6361   (google.apps.ca
+00012600: 7264 5f76 312e 7479 7065 732e 496d 6167  rd_v1.types.Imag
+00012610: 6543 726f 7053 7479 6c65 2e49 6d61 6765  eCropStyle.Image
+00012620: 4372 6f70 5479 7065 293a 0a20 2020 2020  CropType):.     
+00012630: 2020 2020 2020 2054 6865 2063 726f 7020         The crop 
+00012640: 7479 7065 2e0a 2020 2020 2020 2020 6173  type..        as
+00012650: 7065 6374 5f72 6174 696f 2028 666c 6f61  pect_ratio (floa
+00012660: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+00012670: 5468 6520 6173 7065 6374 2072 6174 696f  The aspect ratio
+00012680: 2074 6f20 7573 6520 6966 2074 6865 2063   to use if the c
+00012690: 726f 7020 7479 7065 2069 730a 2020 2020  rop type is.    
+000126a0: 2020 2020 2020 2020 6060 5245 4354 414e          ``RECTAN
+000126b0: 474c 455f 4355 5354 4f4d 6060 2e0a 0a20  GLE_CUSTOM``... 
+000126c0: 2020 2020 2020 2020 2020 2046 6f72 2065             For e
+000126d0: 7861 6d70 6c65 2c20 6865 7265 2773 2068  xample, here's h
+000126e0: 6f77 2074 6f20 6170 706c 7920 6120 3136  ow to apply a 16
+000126f0: 3a39 2061 7370 6563 7420 7261 7469 6f3a  :9 aspect ratio:
+00012700: 0a0a 2020 2020 2020 2020 2020 2020 3a3a  ..            ::
+00012710: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012720: 2063 726f 7053 7479 6c65 207b 0a20 2020   cropStyle {.   
+00012730: 2020 2020 2020 2020 2020 2020 2022 7479               "ty
+00012740: 7065 223a 2022 5245 4354 414e 474c 455f  pe": "RECTANGLE_
+00012750: 4355 5354 4f4d 222c 0a20 2020 2020 2020  CUSTOM",.       
+00012760: 2020 2020 2020 2020 2022 6173 7065 6374           "aspect
+00012770: 5261 7469 6f22 3a20 3136 2f39 0a20 2020  Ratio": 16/9.   
+00012780: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00012790: 2020 2222 220a 0a20 2020 2063 6c61 7373    """..    class
+000127a0: 2049 6d61 6765 4372 6f70 5479 7065 2870   ImageCropType(p
+000127b0: 726f 746f 2e45 6e75 6d29 3a0a 2020 2020  roto.Enum):.    
+000127c0: 2020 2020 7222 2222 5265 7072 6573 656e      r"""Represen
+000127d0: 7473 2074 6865 2063 726f 7020 7374 796c  ts the crop styl
+000127e0: 6520 6170 706c 6965 6420 746f 2061 6e20  e applied to an 
+000127f0: 696d 6167 652e 0a0a 2020 2020 2020 2020  image...        
+00012800: 6047 6f6f 676c 6520 576f 726b 7370 6163  `Google Workspac
+00012810: 6520 4164 642d 6f6e 7320 616e 6420 4368  e Add-ons and Ch
+00012820: 6174 0a20 2020 2020 2020 2061 7070 7320  at.        apps 
+00012830: 3c68 7474 7073 3a2f 2f64 6576 656c 6f70  <https://develop
+00012840: 6572 732e 676f 6f67 6c65 2e63 6f6d 2f77  ers.google.com/w
+00012850: 6f72 6b73 7061 6365 2f65 7874 656e 643e  orkspace/extend>
+00012860: 605f 5f3a 0a0a 2020 2020 2020 2020 5661  `__:..        Va
+00012870: 6c75 6573 3a0a 2020 2020 2020 2020 2020  lues:.          
+00012880: 2020 494d 4147 455f 4352 4f50 5f54 5950    IMAGE_CROP_TYP
+00012890: 455f 554e 5350 4543 4946 4945 4420 2830  E_UNSPECIFIED (0
+000128a0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000128b0: 2020 2044 6f6e 2774 2075 7365 2e20 556e     Don't use. Un
+000128c0: 7370 6563 6966 6965 642e 0a20 2020 2020  specified..     
+000128d0: 2020 2020 2020 2053 5155 4152 4520 2831         SQUARE (1
+000128e0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000128f0: 2020 2044 6566 6175 6c74 2076 616c 7565     Default value
+00012900: 2e20 4170 706c 6965 7320 6120 7371 7561  . Applies a squa
+00012910: 7265 2063 726f 702e 0a20 2020 2020 2020  re crop..       
+00012920: 2020 2020 2043 4952 434c 4520 2832 293a       CIRCLE (2):
+00012930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012940: 2041 7070 6c69 6573 2061 2063 6972 6375   Applies a circu
+00012950: 6c61 7220 6372 6f70 2e0a 2020 2020 2020  lar crop..      
+00012960: 2020 2020 2020 5245 4354 414e 474c 455f        RECTANGLE_
+00012970: 4355 5354 4f4d 2028 3329 3a0a 2020 2020  CUSTOM (3):.    
+00012980: 2020 2020 2020 2020 2020 2020 4170 706c              Appl
+00012990: 6965 7320 6120 7265 6374 616e 6775 6c61  ies a rectangula
+000129a0: 7220 6372 6f70 2077 6974 6820 6120 6375  r crop with a cu
+000129b0: 7374 6f6d 2061 7370 6563 7420 7261 7469  stom aspect rati
+000129c0: 6f2e 2053 6574 0a20 2020 2020 2020 2020  o. Set.         
+000129d0: 2020 2020 2020 2074 6865 2063 7573 746f         the custo
+000129e0: 6d20 6173 7065 6374 2072 6174 696f 2077  m aspect ratio w
+000129f0: 6974 6820 6060 6173 7065 6374 5261 7469  ith ``aspectRati
+00012a00: 6f60 602e 0a20 2020 2020 2020 2020 2020  o``..           
+00012a10: 2052 4543 5441 4e47 4c45 5f34 5f33 2028   RECTANGLE_4_3 (
+00012a20: 3429 3a0a 2020 2020 2020 2020 2020 2020  4):.            
+00012a30: 2020 2020 4170 706c 6965 7320 6120 7265      Applies a re
+00012a40: 6374 616e 6775 6c61 7220 6372 6f70 2077  ctangular crop w
+00012a50: 6974 6820 6120 343a 3320 6173 7065 6374  ith a 4:3 aspect
+00012a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012a70: 2072 6174 696f 2e0a 2020 2020 2020 2020   ratio..        
+00012a80: 2222 220a 2020 2020 2020 2020 494d 4147  """.        IMAG
+00012a90: 455f 4352 4f50 5f54 5950 455f 554e 5350  E_CROP_TYPE_UNSP
+00012aa0: 4543 4946 4945 4420 3d20 300a 2020 2020  ECIFIED = 0.    
+00012ab0: 2020 2020 5351 5541 5245 203d 2031 0a20      SQUARE = 1. 
+00012ac0: 2020 2020 2020 2043 4952 434c 4520 3d20         CIRCLE = 
+00012ad0: 320a 2020 2020 2020 2020 5245 4354 414e  2.        RECTAN
+00012ae0: 474c 455f 4355 5354 4f4d 203d 2033 0a20  GLE_CUSTOM = 3. 
+00012af0: 2020 2020 2020 2052 4543 5441 4e47 4c45         RECTANGLE
+00012b00: 5f34 5f33 203d 2034 0a0a 2020 2020 7479  _4_3 = 4..    ty
+00012b10: 7065 5f3a 2049 6d61 6765 4372 6f70 5479  pe_: ImageCropTy
+00012b20: 7065 203d 2070 726f 746f 2e46 6965 6c64  pe = proto.Field
+00012b30: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
+00012b40: 454e 554d 2c0a 2020 2020 2020 2020 6e75  ENUM,.        nu
+00012b50: 6d62 6572 3d31 2c0a 2020 2020 2020 2020  mber=1,.        
+00012b60: 656e 756d 3d49 6d61 6765 4372 6f70 5479  enum=ImageCropTy
+00012b70: 7065 2c0a 2020 2020 290a 2020 2020 6173  pe,.    ).    as
+00012b80: 7065 6374 5f72 6174 696f 3a20 666c 6f61  pect_ratio: floa
+00012b90: 7420 3d20 7072 6f74 6f2e 4669 656c 6428  t = proto.Field(
+00012ba0: 0a20 2020 2020 2020 2070 726f 746f 2e44  .        proto.D
+00012bb0: 4f55 424c 452c 0a20 2020 2020 2020 206e  OUBLE,.        n
+00012bc0: 756d 6265 723d 322c 0a20 2020 2029 0a0a  umber=2,.    )..
+00012bd0: 0a63 6c61 7373 2042 6f72 6465 7253 7479  .class BorderSty
+00012be0: 6c65 2870 726f 746f 2e4d 6573 7361 6765  le(proto.Message
+00012bf0: 293a 0a20 2020 2072 2222 2254 6865 2073  ):.    r"""The s
+00012c00: 7479 6c65 206f 7074 696f 6e73 2066 6f72  tyle options for
+00012c10: 2074 6865 2062 6f72 6465 7220 6f66 2061   the border of a
+00012c20: 2063 6172 6420 6f72 2077 6964 6765 742c   card or widget,
+00012c30: 2069 6e63 6c75 6469 6e67 2074 6865 0a20   including the. 
+00012c40: 2020 2062 6f72 6465 7220 7479 7065 2061     border type a
+00012c50: 6e64 2063 6f6c 6f72 2e0a 0a20 2020 2060  nd color...    `
+00012c60: 476f 6f67 6c65 2057 6f72 6b73 7061 6365  Google Workspace
+00012c70: 2041 6464 2d6f 6e73 2061 6e64 2043 6861   Add-ons and Cha
+00012c80: 740a 2020 2020 6170 7073 203c 6874 7470  t.    apps <http
+00012c90: 733a 2f2f 6465 7665 6c6f 7065 7273 2e67  s://developers.g
+00012ca0: 6f6f 676c 652e 636f 6d2f 776f 726b 7370  oogle.com/worksp
+00012cb0: 6163 652f 6578 7465 6e64 3e60 5f5f 3a0a  ace/extend>`__:.
+00012cc0: 0a20 2020 2041 7474 7269 6275 7465 733a  .    Attributes:
+00012cd0: 0a20 2020 2020 2020 2074 7970 655f 2028  .        type_ (
+00012ce0: 676f 6f67 6c65 2e61 7070 732e 6361 7264  google.apps.card
+00012cf0: 5f76 312e 7479 7065 732e 426f 7264 6572  _v1.types.Border
+00012d00: 5374 796c 652e 426f 7264 6572 5479 7065  Style.BorderType
+00012d10: 293a 0a20 2020 2020 2020 2020 2020 2054  ):.            T
+00012d20: 6865 2062 6f72 6465 7220 7479 7065 2e0a  he border type..
+00012d30: 2020 2020 2020 2020 7374 726f 6b65 5f63          stroke_c
+00012d40: 6f6c 6f72 2028 676f 6f67 6c65 2e74 7970  olor (google.typ
+00012d50: 652e 636f 6c6f 725f 7062 322e 436f 6c6f  e.color_pb2.Colo
+00012d60: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00012d70: 5468 6520 636f 6c6f 7273 2074 6f20 7573  The colors to us
+00012d80: 6520 7768 656e 2074 6865 2074 7970 6520  e when the type 
+00012d90: 6973 2060 6042 4f52 4445 525f 5459 5045  is ``BORDER_TYPE
+00012da0: 5f53 5452 4f4b 4560 602e 0a20 2020 2020  _STROKE``..     
+00012db0: 2020 2063 6f72 6e65 725f 7261 6469 7573     corner_radius
+00012dc0: 2028 696e 7429 3a0a 2020 2020 2020 2020   (int):.        
+00012dd0: 2020 2020 5468 6520 636f 726e 6572 2072      The corner r
+00012de0: 6164 6975 7320 666f 7220 7468 6520 626f  adius for the bo
+00012df0: 7264 6572 2e0a 2020 2020 2222 220a 0a20  rder..    """.. 
+00012e00: 2020 2063 6c61 7373 2042 6f72 6465 7254     class BorderT
+00012e10: 7970 6528 7072 6f74 6f2e 456e 756d 293a  ype(proto.Enum):
+00012e20: 0a20 2020 2020 2020 2072 2222 2252 6570  .        r"""Rep
+00012e30: 7265 7365 6e74 7320 7468 6520 626f 7264  resents the bord
+00012e40: 6572 2074 7970 6573 2061 7070 6c69 6564  er types applied
+00012e50: 2074 6f20 7769 6467 6574 732e 0a0a 2020   to widgets...  
+00012e60: 2020 2020 2020 6047 6f6f 676c 6520 576f        `Google Wo
+00012e70: 726b 7370 6163 6520 4164 642d 6f6e 7320  rkspace Add-ons 
+00012e80: 616e 6420 4368 6174 0a20 2020 2020 2020  and Chat.       
+00012e90: 2061 7070 7320 3c68 7474 7073 3a2f 2f64   apps <https://d
+00012ea0: 6576 656c 6f70 6572 732e 676f 6f67 6c65  evelopers.google
+00012eb0: 2e63 6f6d 2f77 6f72 6b73 7061 6365 2f65  .com/workspace/e
+00012ec0: 7874 656e 643e 605f 5f3a 0a0a 2020 2020  xtend>`__:..    
+00012ed0: 2020 2020 5661 6c75 6573 3a0a 2020 2020      Values:.    
+00012ee0: 2020 2020 2020 2020 424f 5244 4552 5f54          BORDER_T
+00012ef0: 5950 455f 554e 5350 4543 4946 4945 4420  YPE_UNSPECIFIED 
+00012f00: 2830 293a 0a20 2020 2020 2020 2020 2020  (0):.           
+00012f10: 2020 2020 2044 6f6e 2774 2075 7365 2e20       Don't use. 
+00012f20: 556e 7370 6563 6966 6965 642e 0a20 2020  Unspecified..   
+00012f30: 2020 2020 2020 2020 204e 4f5f 424f 5244           NO_BORD
+00012f40: 4552 2028 3129 3a0a 2020 2020 2020 2020  ER (1):.        
+00012f50: 2020 2020 2020 2020 4465 6661 756c 7420          Default 
+00012f60: 7661 6c75 652e 204e 6f20 626f 7264 6572  value. No border
+00012f70: 2e0a 2020 2020 2020 2020 2020 2020 5354  ..            ST
+00012f80: 524f 4b45 2028 3229 3a0a 2020 2020 2020  ROKE (2):.      
+00012f90: 2020 2020 2020 2020 2020 4f75 746c 696e            Outlin
+00012fa0: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
+00012fb0: 2020 2020 2020 2042 4f52 4445 525f 5459         BORDER_TY
+00012fc0: 5045 5f55 4e53 5045 4349 4649 4544 203d  PE_UNSPECIFIED =
+00012fd0: 2030 0a20 2020 2020 2020 204e 4f5f 424f   0.        NO_BO
+00012fe0: 5244 4552 203d 2031 0a20 2020 2020 2020  RDER = 1.       
+00012ff0: 2053 5452 4f4b 4520 3d20 320a 0a20 2020   STROKE = 2..   
+00013000: 2074 7970 655f 3a20 426f 7264 6572 5479   type_: BorderTy
+00013010: 7065 203d 2070 726f 746f 2e46 6965 6c64  pe = proto.Field
+00013020: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
+00013030: 454e 554d 2c0a 2020 2020 2020 2020 6e75  ENUM,.        nu
+00013040: 6d62 6572 3d31 2c0a 2020 2020 2020 2020  mber=1,.        
+00013050: 656e 756d 3d42 6f72 6465 7254 7970 652c  enum=BorderType,
+00013060: 0a20 2020 2029 0a20 2020 2073 7472 6f6b  .    ).    strok
+00013070: 655f 636f 6c6f 723a 2063 6f6c 6f72 5f70  e_color: color_p
+00013080: 6232 2e43 6f6c 6f72 203d 2070 726f 746f  b2.Color = proto
+00013090: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
+000130a0: 7072 6f74 6f2e 4d45 5353 4147 452c 0a20  proto.MESSAGE,. 
+000130b0: 2020 2020 2020 206e 756d 6265 723d 322c         number=2,
+000130c0: 0a20 2020 2020 2020 206d 6573 7361 6765  .        message
+000130d0: 3d63 6f6c 6f72 5f70 6232 2e43 6f6c 6f72  =color_pb2.Color
+000130e0: 2c0a 2020 2020 290a 2020 2020 636f 726e  ,.    ).    corn
+000130f0: 6572 5f72 6164 6975 733a 2069 6e74 203d  er_radius: int =
+00013100: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
+00013110: 2020 2020 2020 7072 6f74 6f2e 494e 5433        proto.INT3
+00013120: 322c 0a20 2020 2020 2020 206e 756d 6265  2,.        numbe
+00013130: 723d 332c 0a20 2020 2029 0a0a 0a63 6c61  r=3,.    )...cla
+00013140: 7373 2049 6d61 6765 436f 6d70 6f6e 656e  ss ImageComponen
+00013150: 7428 7072 6f74 6f2e 4d65 7373 6167 6529  t(proto.Message)
+00013160: 3a0a 2020 2020 7222 2222 5265 7072 6573  :.    r"""Repres
+00013170: 656e 7473 2061 6e20 696d 6167 652e 0a0a  ents an image...
+00013180: 2020 2020 6047 6f6f 676c 6520 576f 726b      `Google Work
+00013190: 7370 6163 6520 4164 642d 6f6e 7320 616e  space Add-ons an
+000131a0: 6420 4368 6174 0a20 2020 2061 7070 7320  d Chat.    apps 
+000131b0: 3c68 7474 7073 3a2f 2f64 6576 656c 6f70  <https://develop
+000131c0: 6572 732e 676f 6f67 6c65 2e63 6f6d 2f77  ers.google.com/w
+000131d0: 6f72 6b73 7061 6365 2f65 7874 656e 643e  orkspace/extend>
+000131e0: 605f 5f3a 0a0a 2020 2020 4174 7472 6962  `__:..    Attrib
+000131f0: 7574 6573 3a0a 2020 2020 2020 2020 696d  utes:.        im
+00013200: 6167 655f 7572 6920 2873 7472 293a 0a20  age_uri (str):. 
+00013210: 2020 2020 2020 2020 2020 2054 6865 2069             The i
+00013220: 6d61 6765 2055 524c 2e0a 2020 2020 2020  mage URL..      
+00013230: 2020 616c 745f 7465 7874 2028 7374 7229    alt_text (str)
+00013240: 3a0a 2020 2020 2020 2020 2020 2020 5468  :.            Th
+00013250: 6520 6163 6365 7373 6962 696c 6974 7920  e accessibility 
+00013260: 6c61 6265 6c20 666f 7220 7468 6520 696d  label for the im
+00013270: 6167 652e 0a20 2020 2020 2020 2063 726f  age..        cro
+00013280: 705f 7374 796c 6520 2867 6f6f 676c 652e  p_style (google.
+00013290: 6170 7073 2e63 6172 645f 7631 2e74 7970  apps.card_v1.typ
+000132a0: 6573 2e49 6d61 6765 4372 6f70 5374 796c  es.ImageCropStyl
+000132b0: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+000132c0: 5468 6520 6372 6f70 2073 7479 6c65 2074  The crop style t
+000132d0: 6f20 6170 706c 7920 746f 2074 6865 2069  o apply to the i
+000132e0: 6d61 6765 2e0a 2020 2020 2020 2020 626f  mage..        bo
+000132f0: 7264 6572 5f73 7479 6c65 2028 676f 6f67  rder_style (goog
+00013300: 6c65 2e61 7070 732e 6361 7264 5f76 312e  le.apps.card_v1.
+00013310: 7479 7065 732e 426f 7264 6572 5374 796c  types.BorderStyl
+00013320: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+00013330: 5468 6520 626f 7264 6572 2073 7479 6c65  The border style
+00013340: 2074 6f20 6170 706c 7920 746f 2074 6865   to apply to the
+00013350: 2069 6d61 6765 2e0a 2020 2020 2222 220a   image..    """.
+00013360: 0a20 2020 2069 6d61 6765 5f75 7269 3a20  .    image_uri: 
+00013370: 7374 7220 3d20 7072 6f74 6f2e 4669 656c  str = proto.Fiel
+00013380: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
+00013390: 2e53 5452 494e 472c 0a20 2020 2020 2020  .STRING,.       
+000133a0: 206e 756d 6265 723d 312c 0a20 2020 2029   number=1,.    )
+000133b0: 0a20 2020 2061 6c74 5f74 6578 743a 2073  .    alt_text: s
+000133c0: 7472 203d 2070 726f 746f 2e46 6965 6c64  tr = proto.Field
+000133d0: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
+000133e0: 5354 5249 4e47 2c0a 2020 2020 2020 2020  STRING,.        
+000133f0: 6e75 6d62 6572 3d32 2c0a 2020 2020 290a  number=2,.    ).
+00013400: 2020 2020 6372 6f70 5f73 7479 6c65 3a20      crop_style: 
+00013410: 2249 6d61 6765 4372 6f70 5374 796c 6522  "ImageCropStyle"
+00013420: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
+00013430: 2020 2020 2020 2020 7072 6f74 6f2e 4d45          proto.ME
+00013440: 5353 4147 452c 0a20 2020 2020 2020 206e  SSAGE,.        n
+00013450: 756d 6265 723d 332c 0a20 2020 2020 2020  umber=3,.       
+00013460: 206d 6573 7361 6765 3d22 496d 6167 6543   message="ImageC
+00013470: 726f 7053 7479 6c65 222c 0a20 2020 2029  ropStyle",.    )
+00013480: 0a20 2020 2062 6f72 6465 725f 7374 796c  .    border_styl
+00013490: 653a 2022 426f 7264 6572 5374 796c 6522  e: "BorderStyle"
+000134a0: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
+000134b0: 2020 2020 2020 2020 7072 6f74 6f2e 4d45          proto.ME
+000134c0: 5353 4147 452c 0a20 2020 2020 2020 206e  SSAGE,.        n
+000134d0: 756d 6265 723d 342c 0a20 2020 2020 2020  umber=4,.       
+000134e0: 206d 6573 7361 6765 3d22 426f 7264 6572   message="Border
+000134f0: 5374 796c 6522 2c0a 2020 2020 290a 0a0a  Style",.    )...
+00013500: 636c 6173 7320 4772 6964 2870 726f 746f  class Grid(proto
+00013510: 2e4d 6573 7361 6765 293a 0a20 2020 2072  .Message):.    r
+00013520: 2222 2244 6973 706c 6179 7320 6120 6772  """Displays a gr
+00013530: 6964 2077 6974 6820 6120 636f 6c6c 6563  id with a collec
+00013540: 7469 6f6e 206f 6620 6974 656d 732e 2049  tion of items. I
+00013550: 7465 6d73 2063 616e 206f 6e6c 7920 696e  tems can only in
+00013560: 636c 7564 650a 2020 2020 7465 7874 206f  clude.    text o
+00013570: 7220 696d 6167 6573 2e20 466f 7220 7265  r images. For re
+00013580: 7370 6f6e 7369 7665 2063 6f6c 756d 6e73  sponsive columns
+00013590: 2c20 6f72 2074 6f20 696e 636c 7564 6520  , or to include 
+000135a0: 6d6f 7265 2074 6861 6e20 7465 7874 0a20  more than text. 
+000135b0: 2020 206f 7220 696d 6167 6573 2c20 7573     or images, us
+000135c0: 6520 5b60 6043 6f6c 756d 6e73 6060 5d5b  e [``Columns``][
+000135d0: 676f 6f67 6c65 2e61 7070 732e 6361 7264  google.apps.card
+000135e0: 2e76 312e 436f 6c75 6d6e 735d 2e20 466f  .v1.Columns]. Fo
+000135f0: 7220 616e 0a20 2020 2065 7861 6d70 6c65  r an.    example
+00013600: 2069 6e20 476f 6f67 6c65 2043 6861 7420   in Google Chat 
+00013610: 6170 7073 2c20 7365 6520 6044 6973 706c  apps, see `Displ
+00013620: 6179 2061 2047 7269 6420 7769 7468 2061  ay a Grid with a
+00013630: 2063 6f6c 6c65 6374 696f 6e0a 2020 2020   collection.    
+00013640: 6f66 0a20 2020 2069 7465 6d73 203c 6874  of.    items <ht
+00013650: 7470 733a 2f2f 6465 7665 6c6f 7065 7273  tps://developers
+00013660: 2e67 6f6f 676c 652e 636f 6d2f 776f 726b  .google.com/work
+00013670: 7370 6163 652f 6368 6174 2f66 6f72 6d61  space/chat/forma
+00013680: 742d 7374 7275 6374 7572 652d 6361 7264  t-structure-card
+00013690: 2d64 6961 6c6f 6723 6469 7370 6c61 795f  -dialog#display_
+000136a0: 615f 6772 6964 5f77 6974 685f 615f 636f  a_grid_with_a_co
+000136b0: 6c6c 6563 7469 6f6e 5f6f 665f 6974 656d  llection_of_item
+000136c0: 733e 605f 5f2e 0a0a 2020 2020 4120 6772  s>`__...    A gr
+000136d0: 6964 2073 7570 706f 7274 7320 616e 7920  id supports any 
+000136e0: 6e75 6d62 6572 206f 6620 636f 6c75 6d6e  number of column
+000136f0: 7320 616e 6420 6974 656d 732e 2054 6865  s and items. The
+00013700: 206e 756d 6265 7220 6f66 2072 6f77 730a   number of rows.
+00013710: 2020 2020 6973 2064 6574 6572 6d69 6e65      is determine
+00013720: 6420 6279 2069 7465 6d73 2064 6976 6964  d by items divid
+00013730: 6564 2062 7920 636f 6c75 6d6e 732e 2041  ed by columns. A
+00013740: 2067 7269 6420 7769 7468 2031 3020 6974   grid with 10 it
+00013750: 656d 7320 616e 640a 2020 2020 3220 636f  ems and.    2 co
+00013760: 6c75 6d6e 7320 6861 7320 3520 726f 7773  lumns has 5 rows
+00013770: 2e20 4120 6772 6964 2077 6974 6820 3131  . A grid with 11
+00013780: 2069 7465 6d73 2061 6e64 2032 2063 6f6c   items and 2 col
+00013790: 756d 6e73 2068 6173 2036 2072 6f77 732e  umns has 6 rows.
+000137a0: 0a0a 2020 2020 6047 6f6f 676c 6520 576f  ..    `Google Wo
+000137b0: 726b 7370 6163 6520 4164 642d 6f6e 7320  rkspace Add-ons 
+000137c0: 616e 6420 4368 6174 0a20 2020 2061 7070  and Chat.    app
+000137d0: 7320 3c68 7474 7073 3a2f 2f64 6576 656c  s <https://devel
+000137e0: 6f70 6572 732e 676f 6f67 6c65 2e63 6f6d  opers.google.com
+000137f0: 2f77 6f72 6b73 7061 6365 2f65 7874 656e  /workspace/exten
+00013800: 643e 605f 5f3a 0a0a 2020 2020 466f 7220  d>`__:..    For 
+00013810: 6578 616d 706c 652c 2074 6865 2066 6f6c  example, the fol
+00013820: 6c6f 7769 6e67 204a 534f 4e20 6372 6561  lowing JSON crea
+00013830: 7465 7320 6120 3220 636f 6c75 6d6e 2067  tes a 2 column g
+00013840: 7269 6420 7769 7468 2061 0a20 2020 2073  rid with a.    s
+00013850: 696e 676c 6520 6974 656d 3a0a 0a20 2020  ingle item:..   
+00013860: 203a 3a0a 0a20 2020 2020 2020 2267 7269   ::..       "gri
+00013870: 6422 3a20 7b0a 2020 2020 2020 2020 2022  d": {.         "
+00013880: 7469 746c 6522 3a20 2241 2066 696e 6520  title": "A fine 
+00013890: 636f 6c6c 6563 7469 6f6e 206f 6620 6974  collection of it
+000138a0: 656d 7322 2c0a 2020 2020 2020 2020 2022  ems",.         "
+000138b0: 636f 6c75 6d6e 436f 756e 7422 3a20 322c  columnCount": 2,
+000138c0: 0a20 2020 2020 2020 2020 2262 6f72 6465  .         "borde
+000138d0: 7253 7479 6c65 223a 207b 0a20 2020 2020  rStyle": {.     
+000138e0: 2020 2020 2020 2274 7970 6522 3a20 2253        "type": "S
+000138f0: 5452 4f4b 4522 2c0a 2020 2020 2020 2020  TROKE",.        
+00013900: 2020 2022 636f 726e 6572 5261 6469 7573     "cornerRadius
+00013910: 223a 2034 0a20 2020 2020 2020 2020 7d2c  ": 4.         },
+00013920: 0a20 2020 2020 2020 2020 2269 7465 6d73  .         "items
+00013930: 223a 205b 0a20 2020 2020 2020 2020 2020  ": [.           
+00013940: 7b0a 2020 2020 2020 2020 2020 2020 2022  {.             "
+00013950: 696d 6167 6522 3a20 7b0a 2020 2020 2020  image": {.      
+00013960: 2020 2020 2020 2020 2022 696d 6167 6555           "imageU
+00013970: 7269 223a 2022 6874 7470 733a 2f2f 7777  ri": "https://ww
+00013980: 772e 6578 616d 706c 652e 636f 6d2f 696d  w.example.com/im
+00013990: 6167 652e 706e 6722 2c0a 2020 2020 2020  age.png",.      
+000139a0: 2020 2020 2020 2020 2022 6372 6f70 5374           "cropSt
+000139b0: 796c 6522 3a20 7b0a 2020 2020 2020 2020  yle": {.        
+000139c0: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
+000139d0: 2022 5351 5541 5245 220a 2020 2020 2020   "SQUARE".      
+000139e0: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+000139f0: 2020 2020 2020 2020 2020 2022 626f 7264             "bord
+00013a00: 6572 5374 796c 6522 3a20 7b0a 2020 2020  erStyle": {.    
+00013a10: 2020 2020 2020 2020 2020 2020 2022 7479               "ty
+00013a20: 7065 223a 2022 5354 524f 4b45 220a 2020  pe": "STROKE".  
+00013a30: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
+00013a40: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+00013a50: 2020 2020 2020 2020 2020 2020 2274 6974              "tit
+00013a60: 6c65 223a 2022 416e 2069 7465 6d22 2c0a  le": "An item",.
+00013a70: 2020 2020 2020 2020 2020 2020 2022 7465               "te
+00013a80: 7874 416c 6967 6e6d 656e 7422 3a20 2243  xtAlignment": "C
+00013a90: 454e 5445 5222 0a20 2020 2020 2020 2020  ENTER".         
+00013aa0: 2020 7d0a 2020 2020 2020 2020 205d 2c0a    }.         ],.
+00013ab0: 2020 2020 2020 2020 2022 6f6e 436c 6963           "onClic
+00013ac0: 6b22 3a20 7b0a 2020 2020 2020 2020 2020  k": {.          
+00013ad0: 2022 6f70 656e 4c69 6e6b 223a 207b 0a20   "openLink": {. 
+00013ae0: 2020 2020 2020 2020 2020 2020 2275 726c              "url
+00013af0: 223a 2022 6874 7470 733a 2f2f 7777 772e  ": "https://www.
+00013b00: 6578 616d 706c 652e 636f 6d22 0a20 2020  example.com".   
+00013b10: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00013b20: 2020 207d 0a20 2020 2020 2020 7d0a 0a20     }.       }.. 
+00013b30: 2020 2041 7474 7269 6275 7465 733a 0a20     Attributes:. 
+00013b40: 2020 2020 2020 2074 6974 6c65 2028 7374         title (st
+00013b50: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00013b60: 5468 6520 7465 7874 2074 6861 7420 6469  The text that di
+00013b70: 7370 6c61 7973 2069 6e20 7468 6520 6772  splays in the gr
+00013b80: 6964 2068 6561 6465 722e 0a20 2020 2020  id header..     
+00013b90: 2020 2069 7465 6d73 2028 4d75 7461 626c     items (Mutabl
+00013ba0: 6553 6571 7565 6e63 655b 676f 6f67 6c65  eSequence[google
+00013bb0: 2e61 7070 732e 6361 7264 5f76 312e 7479  .apps.card_v1.ty
+00013bc0: 7065 732e 4772 6964 2e47 7269 6449 7465  pes.Grid.GridIte
+00013bd0: 6d5d 293a 0a20 2020 2020 2020 2020 2020  m]):.           
+00013be0: 2054 6865 2069 7465 6d73 2074 6f20 6469   The items to di
+00013bf0: 7370 6c61 7920 696e 2074 6865 2067 7269  splay in the gri
+00013c00: 642e 0a20 2020 2020 2020 2062 6f72 6465  d..        borde
+00013c10: 725f 7374 796c 6520 2867 6f6f 676c 652e  r_style (google.
+00013c20: 6170 7073 2e63 6172 645f 7631 2e74 7970  apps.card_v1.typ
+00013c30: 6573 2e42 6f72 6465 7253 7479 6c65 293a  es.BorderStyle):
+00013c40: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
+00013c50: 2062 6f72 6465 7220 7374 796c 6520 746f   border style to
+00013c60: 2061 7070 6c79 2074 6f20 6561 6368 2067   apply to each g
+00013c70: 7269 6420 6974 656d 2e0a 2020 2020 2020  rid item..      
+00013c80: 2020 636f 6c75 6d6e 5f63 6f75 6e74 2028    column_count (
+00013c90: 696e 7429 3a0a 2020 2020 2020 2020 2020  int):.          
+00013ca0: 2020 5468 6520 6e75 6d62 6572 206f 6620    The number of 
+00013cb0: 636f 6c75 6d6e 7320 746f 2064 6973 706c  columns to displ
+00013cc0: 6179 2069 6e20 7468 6520 6772 6964 2e0a  ay in the grid..
+00013cd0: 2020 2020 2020 2020 2020 2020 4120 6465              A de
+00013ce0: 6661 756c 7420 7661 6c75 6520 6973 2075  fault value is u
+00013cf0: 7365 6420 6966 2074 6869 7320 6669 656c  sed if this fiel
+00013d00: 6420 6973 6e27 740a 2020 2020 2020 2020  d isn't.        
+00013d10: 2020 2020 7370 6563 6966 6965 642c 2061      specified, a
+00013d20: 6e64 2074 6861 7420 6465 6661 756c 7420  nd that default 
+00013d30: 7661 6c75 6520 6973 2064 6966 6665 7265  value is differe
+00013d40: 6e74 0a20 2020 2020 2020 2020 2020 2064  nt.            d
+00013d50: 6570 656e 6469 6e67 206f 6e20 7768 6572  epending on wher
+00013d60: 6520 7468 6520 6772 6964 2069 7320 7368  e the grid is sh
+00013d70: 6f77 6e20 2864 6961 6c6f 670a 2020 2020  own (dialog.    
+00013d80: 2020 2020 2020 2020 7665 7273 7573 2063          versus c
+00013d90: 6f6d 7061 6e69 6f6e 292e 0a20 2020 2020  ompanion)..     
+00013da0: 2020 206f 6e5f 636c 6963 6b20 2867 6f6f     on_click (goo
+00013db0: 676c 652e 6170 7073 2e63 6172 645f 7631  gle.apps.card_v1
+00013dc0: 2e74 7970 6573 2e4f 6e43 6c69 636b 293a  .types.OnClick):
+00013dd0: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
+00013de0: 7320 6361 6c6c 6261 636b 2069 7320 7265  s callback is re
+00013df0: 7573 6564 2062 7920 6561 6368 2069 6e64  used by each ind
+00013e00: 6976 6964 7561 6c0a 2020 2020 2020 2020  ividual.        
+00013e10: 2020 2020 6772 6964 2069 7465 6d2c 2062      grid item, b
+00013e20: 7574 2077 6974 6820 7468 6520 6974 656d  ut with the item
+00013e30: 2773 2069 6465 6e74 6966 6965 7220 616e  's identifier an
+00013e40: 640a 2020 2020 2020 2020 2020 2020 696e  d.            in
+00013e50: 6465 7820 696e 2074 6865 2069 7465 6d73  dex in the items
+00013e60: 206c 6973 7420 6164 6465 6420 746f 2074   list added to t
+00013e70: 6865 2063 616c 6c62 6163 6b27 730a 2020  he callback's.  
+00013e80: 2020 2020 2020 2020 2020 7061 7261 6d65            parame
+00013e90: 7465 7273 2e0a 2020 2020 2222 220a 0a20  ters..    """.. 
+00013ea0: 2020 2063 6c61 7373 2047 7269 6449 7465     class GridIte
+00013eb0: 6d28 7072 6f74 6f2e 4d65 7373 6167 6529  m(proto.Message)
+00013ec0: 3a0a 2020 2020 2020 2020 7222 2222 5265  :.        r"""Re
+00013ed0: 7072 6573 656e 7473 2061 6e20 6974 656d  presents an item
+00013ee0: 2069 6e20 6120 6772 6964 206c 6179 6f75   in a grid layou
+00013ef0: 742e 2049 7465 6d73 2063 616e 2063 6f6e  t. Items can con
+00013f00: 7461 696e 2074 6578 742c 2061 6e0a 2020  tain text, an.  
+00013f10: 2020 2020 2020 696d 6167 652c 206f 7220        image, or 
+00013f20: 626f 7468 2074 6578 7420 616e 6420 616e  both text and an
+00013f30: 2069 6d61 6765 2e0a 0a20 2020 2020 2020   image...       
+00013f40: 2060 476f 6f67 6c65 2057 6f72 6b73 7061   `Google Workspa
+00013f50: 6365 2041 6464 2d6f 6e73 2061 6e64 2043  ce Add-ons and C
+00013f60: 6861 740a 2020 2020 2020 2020 6170 7073  hat.        apps
+00013f70: 203c 6874 7470 733a 2f2f 6465 7665 6c6f   <https://develo
+00013f80: 7065 7273 2e67 6f6f 676c 652e 636f 6d2f  pers.google.com/
+00013f90: 776f 726b 7370 6163 652f 6578 7465 6e64  workspace/extend
+00013fa0: 3e60 5f5f 3a0a 0a20 2020 2020 2020 2041  >`__:..        A
+00013fb0: 7474 7269 6275 7465 733a 0a20 2020 2020  ttributes:.     
+00013fc0: 2020 2020 2020 2069 6420 2873 7472 293a         id (str):
+00013fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013fe0: 2041 2075 7365 722d 7370 6563 6966 6965   A user-specifie
+00013ff0: 6420 6964 656e 7469 6669 6572 2066 6f72  d identifier for
+00014000: 2074 6869 7320 6772 6964 2069 7465 6d2e   this grid item.
+00014010: 2054 6869 730a 2020 2020 2020 2020 2020   This.          
+00014020: 2020 2020 2020 6964 656e 7469 6669 6572        identifier
+00014030: 2069 7320 7265 7475 726e 6564 2069 6e20   is returned in 
+00014040: 7468 6520 7061 7265 6e74 2067 7269 6427  the parent grid'
+00014050: 7320 6060 6f6e 436c 6963 6b60 600a 2020  s ``onClick``.  
+00014060: 2020 2020 2020 2020 2020 2020 2020 6361                ca
+00014070: 6c6c 6261 636b 2070 6172 616d 6574 6572  llback parameter
+00014080: 732e 0a20 2020 2020 2020 2020 2020 2069  s..            i
+00014090: 6d61 6765 2028 676f 6f67 6c65 2e61 7070  mage (google.app
+000140a0: 732e 6361 7264 5f76 312e 7479 7065 732e  s.card_v1.types.
+000140b0: 496d 6167 6543 6f6d 706f 6e65 6e74 293a  ImageComponent):
+000140c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000140d0: 2054 6865 2069 6d61 6765 2074 6861 7420   The image that 
+000140e0: 6469 7370 6c61 7973 2069 6e20 7468 6520  displays in the 
+000140f0: 6772 6964 2069 7465 6d2e 0a20 2020 2020  grid item..     
+00014100: 2020 2020 2020 2074 6974 6c65 2028 7374         title (st
+00014110: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00014120: 2020 2020 5468 6520 6772 6964 2069 7465      The grid ite
+00014130: 6d27 7320 7469 746c 652e 0a20 2020 2020  m's title..     
+00014140: 2020 2020 2020 2073 7562 7469 746c 6520         subtitle 
+00014150: 2873 7472 293a 0a20 2020 2020 2020 2020  (str):.         
+00014160: 2020 2020 2020 2054 6865 2067 7269 6420         The grid 
+00014170: 6974 656d 2773 2073 7562 7469 746c 652e  item's subtitle.
+00014180: 0a20 2020 2020 2020 2020 2020 206c 6179  .            lay
+00014190: 6f75 7420 2867 6f6f 676c 652e 6170 7073  out (google.apps
+000141a0: 2e63 6172 645f 7631 2e74 7970 6573 2e47  .card_v1.types.G
+000141b0: 7269 642e 4772 6964 4974 656d 2e47 7269  rid.GridItem.Gri
+000141c0: 6449 7465 6d4c 6179 6f75 7429 3a0a 2020  dItemLayout):.  
+000141d0: 2020 2020 2020 2020 2020 2020 2020 5468                Th
+000141e0: 6520 6c61 796f 7574 2074 6f20 7573 6520  e layout to use 
+000141f0: 666f 7220 7468 6520 6772 6964 2069 7465  for the grid ite
+00014200: 6d2e 0a20 2020 2020 2020 2022 2222 0a0a  m..        """..
+00014210: 2020 2020 2020 2020 636c 6173 7320 4772          class Gr
+00014220: 6964 4974 656d 4c61 796f 7574 2870 726f  idItemLayout(pro
+00014230: 746f 2e45 6e75 6d29 3a0a 2020 2020 2020  to.Enum):.      
+00014240: 2020 2020 2020 7222 2222 5265 7072 6573        r"""Repres
+00014250: 656e 7473 2074 6865 2076 6172 696f 7573  ents the various
+00014260: 206c 6179 6f75 7420 6f70 7469 6f6e 7320   layout options 
+00014270: 6176 6169 6c61 626c 6520 666f 7220 6120  available for a 
+00014280: 6772 6964 2069 7465 6d2e 0a0a 2020 2020  grid item...    
+00014290: 2020 2020 2020 2020 6047 6f6f 676c 6520          `Google 
+000142a0: 576f 726b 7370 6163 6520 4164 642d 6f6e  Workspace Add-on
+000142b0: 7320 616e 6420 4368 6174 0a20 2020 2020  s and Chat.     
+000142c0: 2020 2020 2020 2061 7070 7320 3c68 7474         apps <htt
+000142d0: 7073 3a2f 2f64 6576 656c 6f70 6572 732e  ps://developers.
+000142e0: 676f 6f67 6c65 2e63 6f6d 2f77 6f72 6b73  google.com/works
+000142f0: 7061 6365 2f65 7874 656e 643e 605f 5f3a  pace/extend>`__:
+00014300: 0a0a 2020 2020 2020 2020 2020 2020 5661  ..            Va
+00014310: 6c75 6573 3a0a 2020 2020 2020 2020 2020  lues:.          
+00014320: 2020 2020 2020 4752 4944 5f49 5445 4d5f        GRID_ITEM_
+00014330: 4c41 594f 5554 5f55 4e53 5045 4349 4649  LAYOUT_UNSPECIFI
+00014340: 4544 2028 3029 3a0a 2020 2020 2020 2020  ED (0):.        
+00014350: 2020 2020 2020 2020 2020 2020 446f 6e27              Don'
+00014360: 7420 7573 652e 2055 6e73 7065 6369 6669  t use. Unspecifi
+00014370: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
+00014380: 2020 2020 5445 5854 5f42 454c 4f57 2028      TEXT_BELOW (
+00014390: 3129 3a0a 2020 2020 2020 2020 2020 2020  1):.            
+000143a0: 2020 2020 2020 2020 5468 6520 7469 746c          The titl
+000143b0: 6520 616e 6420 7375 6274 6974 6c65 2061  e and subtitle a
+000143c0: 7265 2073 686f 776e 2062 656c 6f77 2074  re shown below t
+000143d0: 6865 0a20 2020 2020 2020 2020 2020 2020  he.             
+000143e0: 2020 2020 2020 2067 7269 6420 6974 656d         grid item
+000143f0: 2773 2069 6d61 6765 2e0a 2020 2020 2020  's image..      
+00014400: 2020 2020 2020 2020 2020 5445 5854 5f41            TEXT_A
+00014410: 424f 5645 2028 3229 3a0a 2020 2020 2020  BOVE (2):.      
+00014420: 2020 2020 2020 2020 2020 2020 2020 5468                Th
+00014430: 6520 7469 746c 6520 616e 6420 7375 6274  e title and subt
+00014440: 6974 6c65 2061 7265 2073 686f 776e 2061  itle are shown a
+00014450: 626f 7665 2074 6865 0a20 2020 2020 2020  bove the.       
+00014460: 2020 2020 2020 2020 2020 2020 2067 7269               gri
+00014470: 6420 6974 656d 2773 2069 6d61 6765 2e0a  d item's image..
+00014480: 2020 2020 2020 2020 2020 2020 2222 220a              """.
+00014490: 2020 2020 2020 2020 2020 2020 4752 4944              GRID
+000144a0: 5f49 5445 4d5f 4c41 594f 5554 5f55 4e53  _ITEM_LAYOUT_UNS
+000144b0: 5045 4349 4649 4544 203d 2030 0a20 2020  PECIFIED = 0.   
+000144c0: 2020 2020 2020 2020 2054 4558 545f 4245           TEXT_BE
+000144d0: 4c4f 5720 3d20 310a 2020 2020 2020 2020  LOW = 1.        
+000144e0: 2020 2020 5445 5854 5f41 424f 5645 203d      TEXT_ABOVE =
+000144f0: 2032 0a0a 2020 2020 2020 2020 6964 3a20   2..        id: 
+00014500: 7374 7220 3d20 7072 6f74 6f2e 4669 656c  str = proto.Fiel
+00014510: 6428 0a20 2020 2020 2020 2020 2020 2070  d(.            p
+00014520: 726f 746f 2e53 5452 494e 472c 0a20 2020  roto.STRING,.   
+00014530: 2020 2020 2020 2020 206e 756d 6265 723d           number=
+00014540: 312c 0a20 2020 2020 2020 2029 0a20 2020  1,.        ).   
+00014550: 2020 2020 2069 6d61 6765 3a20 2249 6d61       image: "Ima
+00014560: 6765 436f 6d70 6f6e 656e 7422 203d 2070  geComponent" = p
+00014570: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
+00014580: 2020 2020 2020 2020 7072 6f74 6f2e 4d45          proto.ME
+00014590: 5353 4147 452c 0a20 2020 2020 2020 2020  SSAGE,.         
+000145a0: 2020 206e 756d 6265 723d 322c 0a20 2020     number=2,.   
+000145b0: 2020 2020 2020 2020 206d 6573 7361 6765           message
+000145c0: 3d22 496d 6167 6543 6f6d 706f 6e65 6e74  ="ImageComponent
+000145d0: 222c 0a20 2020 2020 2020 2029 0a20 2020  ",.        ).   
+000145e0: 2020 2020 2074 6974 6c65 3a20 7374 7220       title: str 
+000145f0: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
+00014600: 2020 2020 2020 2020 2020 2070 726f 746f             proto
+00014610: 2e53 5452 494e 472c 0a20 2020 2020 2020  .STRING,.       
+00014620: 2020 2020 206e 756d 6265 723d 332c 0a20       number=3,. 
+00014630: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00014640: 2073 7562 7469 746c 653a 2073 7472 203d   subtitle: str =
+00014650: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
+00014660: 2020 2020 2020 2020 2020 7072 6f74 6f2e            proto.
+00014670: 5354 5249 4e47 2c0a 2020 2020 2020 2020  STRING,.        
+00014680: 2020 2020 6e75 6d62 6572 3d34 2c0a 2020      number=4,.  
+00014690: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+000146a0: 6c61 796f 7574 3a20 2247 7269 642e 4772  layout: "Grid.Gr
+000146b0: 6964 4974 656d 2e47 7269 6449 7465 6d4c  idItem.GridItemL
+000146c0: 6179 6f75 7422 203d 2070 726f 746f 2e46  ayout" = proto.F
+000146d0: 6965 6c64 280a 2020 2020 2020 2020 2020  ield(.          
+000146e0: 2020 7072 6f74 6f2e 454e 554d 2c0a 2020    proto.ENUM,.  
+000146f0: 2020 2020 2020 2020 2020 6e75 6d62 6572            number
+00014700: 3d39 2c0a 2020 2020 2020 2020 2020 2020  =9,.            
+00014710: 656e 756d 3d22 4772 6964 2e47 7269 6449  enum="Grid.GridI
+00014720: 7465 6d2e 4772 6964 4974 656d 4c61 796f  tem.GridItemLayo
+00014730: 7574 222c 0a20 2020 2020 2020 2029 0a0a  ut",.        )..
+00014740: 2020 2020 7469 746c 653a 2073 7472 203d      title: str =
+00014750: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
+00014760: 2020 2020 2020 7072 6f74 6f2e 5354 5249        proto.STRI
+00014770: 4e47 2c0a 2020 2020 2020 2020 6e75 6d62  NG,.        numb
+00014780: 6572 3d31 2c0a 2020 2020 290a 2020 2020  er=1,.    ).    
+00014790: 6974 656d 733a 204d 7574 6162 6c65 5365  items: MutableSe
+000147a0: 7175 656e 6365 5b47 7269 6449 7465 6d5d  quence[GridItem]
+000147b0: 203d 2070 726f 746f 2e52 6570 6561 7465   = proto.Repeate
+000147c0: 6446 6965 6c64 280a 2020 2020 2020 2020  dField(.        
+000147d0: 7072 6f74 6f2e 4d45 5353 4147 452c 0a20  proto.MESSAGE,. 
+000147e0: 2020 2020 2020 206e 756d 6265 723d 322c         number=2,
+000147f0: 0a20 2020 2020 2020 206d 6573 7361 6765  .        message
+00014800: 3d47 7269 6449 7465 6d2c 0a20 2020 2029  =GridItem,.    )
+00014810: 0a20 2020 2062 6f72 6465 725f 7374 796c  .    border_styl
+00014820: 653a 2022 426f 7264 6572 5374 796c 6522  e: "BorderStyle"
+00014830: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
+00014840: 2020 2020 2020 2020 7072 6f74 6f2e 4d45          proto.ME
+00014850: 5353 4147 452c 0a20 2020 2020 2020 206e  SSAGE,.        n
+00014860: 756d 6265 723d 332c 0a20 2020 2020 2020  umber=3,.       
+00014870: 206d 6573 7361 6765 3d22 426f 7264 6572   message="Border
+00014880: 5374 796c 6522 2c0a 2020 2020 290a 2020  Style",.    ).  
+00014890: 2020 636f 6c75 6d6e 5f63 6f75 6e74 3a20    column_count: 
+000148a0: 696e 7420 3d20 7072 6f74 6f2e 4669 656c  int = proto.Fiel
+000148b0: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
+000148c0: 2e49 4e54 3332 2c0a 2020 2020 2020 2020  .INT32,.        
+000148d0: 6e75 6d62 6572 3d34 2c0a 2020 2020 290a  number=4,.    ).
+000148e0: 2020 2020 6f6e 5f63 6c69 636b 3a20 224f      on_click: "O
+000148f0: 6e43 6c69 636b 2220 3d20 7072 6f74 6f2e  nClick" = proto.
+00014900: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
+00014910: 726f 746f 2e4d 4553 5341 4745 2c0a 2020  roto.MESSAGE,.  
+00014920: 2020 2020 2020 6e75 6d62 6572 3d35 2c0a        number=5,.
+00014930: 2020 2020 2020 2020 6d65 7373 6167 653d          message=
+00014940: 224f 6e43 6c69 636b 222c 0a20 2020 2029  "OnClick",.    )
+00014950: 0a0a 0a63 6c61 7373 2043 6f6c 756d 6e73  ...class Columns
+00014960: 2870 726f 746f 2e4d 6573 7361 6765 293a  (proto.Message):
+00014970: 0a20 2020 2072 2222 2254 6865 2060 6043  .    r"""The ``C
+00014980: 6f6c 756d 6e73 6060 2077 6964 6765 7420  olumns`` widget 
+00014990: 6469 7370 6c61 7973 2075 7020 746f 2032  displays up to 2
+000149a0: 2063 6f6c 756d 6e73 2069 6e20 6120 6361   columns in a ca
+000149b0: 7264 206f 7220 6469 616c 6f67 2e0a 2020  rd or dialog..  
+000149c0: 2020 596f 7520 6361 6e20 6164 6420 7769    You can add wi
+000149d0: 6467 6574 7320 746f 2065 6163 6820 636f  dgets to each co
+000149e0: 6c75 6d6e 3b20 7468 6520 7769 6467 6574  lumn; the widget
+000149f0: 7320 6170 7065 6172 2069 6e20 7468 6520  s appear in the 
+00014a00: 6f72 6465 720a 2020 2020 7468 6174 2074  order.    that t
+00014a10: 6865 7920 6172 6520 7370 6563 6966 6965  hey are specifie
+00014a20: 642e 2046 6f72 2061 6e20 6578 616d 706c  d. For an exampl
+00014a30: 6520 696e 2047 6f6f 676c 6520 4368 6174  e in Google Chat
+00014a40: 2061 7070 732c 2073 6565 0a20 2020 2060   apps, see.    `
+00014a50: 4469 7370 6c61 7920 6361 7264 7320 616e  Display cards an
+00014a60: 6420 6469 616c 6f67 7320 696e 0a20 2020  d dialogs in.   
+00014a70: 2063 6f6c 756d 6e73 203c 6874 7470 733a   columns <https:
+00014a80: 2f2f 6465 7665 6c6f 7065 7273 2e67 6f6f  //developers.goo
+00014a90: 676c 652e 636f 6d2f 776f 726b 7370 6163  gle.com/workspac
+00014aa0: 652f 6368 6174 2f66 6f72 6d61 742d 7374  e/chat/format-st
+00014ab0: 7275 6374 7572 652d 6361 7264 2d64 6961  ructure-card-dia
+00014ac0: 6c6f 6723 6469 7370 6c61 795f 6361 7264  log#display_card
+00014ad0: 735f 616e 645f 6469 616c 6f67 735f 696e  s_and_dialogs_in
+00014ae0: 5f63 6f6c 756d 6e73 3e60 5f5f 2e0a 0a20  _columns>`__... 
+00014af0: 2020 2054 6865 2068 6569 6768 7420 6f66     The height of
+00014b00: 2065 6163 6820 636f 6c75 6d6e 2069 7320   each column is 
+00014b10: 6465 7465 726d 696e 6564 2062 7920 7468  determined by th
+00014b20: 6520 7461 6c6c 6572 2063 6f6c 756d 6e2e  e taller column.
+00014b30: 2046 6f72 0a20 2020 2065 7861 6d70 6c65   For.    example
+00014b40: 2c20 6966 2074 6865 2066 6972 7374 2063  , if the first c
+00014b50: 6f6c 756d 6e20 6973 2074 616c 6c65 7220  olumn is taller 
+00014b60: 7468 616e 2074 6865 2073 6563 6f6e 6420  than the second 
+00014b70: 636f 6c75 6d6e 2c20 626f 7468 0a20 2020  column, both.   
+00014b80: 2063 6f6c 756d 6e73 2068 6176 6520 7468   columns have th
+00014b90: 6520 6865 6967 6874 206f 6620 7468 6520  e height of the 
+00014ba0: 6669 7273 7420 636f 6c75 6d6e 2e20 4265  first column. Be
+00014bb0: 6361 7573 6520 6561 6368 2063 6f6c 756d  cause each colum
+00014bc0: 6e20 6361 6e0a 2020 2020 636f 6e74 6169  n can.    contai
+00014bd0: 6e20 6120 6469 6666 6572 656e 7420 6e75  n a different nu
+00014be0: 6d62 6572 206f 6620 7769 6467 6574 732c  mber of widgets,
+00014bf0: 2079 6f75 2063 616e 2774 2064 6566 696e   you can't defin
+00014c00: 6520 726f 7773 206f 720a 2020 2020 616c  e rows or.    al
+00014c10: 6967 6e20 7769 6467 6574 7320 6265 7477  ign widgets betw
+00014c20: 6565 6e20 7468 6520 636f 6c75 6d6e 732e  een the columns.
+00014c30: 0a0a 2020 2020 436f 6c75 6d6e 7320 6172  ..    Columns ar
+00014c40: 6520 6469 7370 6c61 7965 6420 7369 6465  e displayed side
+00014c50: 2d62 792d 7369 6465 2e20 596f 7520 6361  -by-side. You ca
+00014c60: 6e20 6375 7374 6f6d 697a 6520 7468 6520  n customize the 
+00014c70: 7769 6474 6820 6f66 0a20 2020 2065 6163  width of.    eac
+00014c80: 6820 636f 6c75 6d6e 2075 7369 6e67 2074  h column using t
+00014c90: 6865 2060 6048 6f72 697a 6f6e 7461 6c53  he ``HorizontalS
+00014ca0: 697a 6553 7479 6c65 6060 2066 6965 6c64  izeStyle`` field
+00014cb0: 2e20 4966 2074 6865 2075 7365 7227 730a  . If the user's.
+00014cc0: 2020 2020 7363 7265 656e 2077 6964 7468      screen width
+00014cd0: 2069 7320 746f 6f20 6e61 7272 6f77 2c20   is too narrow, 
+00014ce0: 7468 6520 7365 636f 6e64 2063 6f6c 756d  the second colum
+00014cf0: 6e20 7772 6170 7320 6265 6c6f 7720 7468  n wraps below th
+00014d00: 6520 6669 7273 743a 0a0a 2020 2020 2d20  e first:..    - 
+00014d10: 204f 6e20 7765 622c 2074 6865 2073 6563   On web, the sec
+00014d20: 6f6e 6420 636f 6c75 6d6e 2077 7261 7073  ond column wraps
+00014d30: 2069 6620 7468 6520 7363 7265 656e 2077   if the screen w
+00014d40: 6964 7468 2069 7320 6c65 7373 2074 6861  idth is less tha
+00014d50: 6e0a 2020 2020 2020 206f 7220 6571 7561  n.       or equa
+00014d60: 6c20 746f 2034 3830 2070 6978 656c 732e  l to 480 pixels.
+00014d70: 0a20 2020 202d 2020 4f6e 2069 4f53 2064  .    -  On iOS d
+00014d80: 6576 6963 6573 2c20 7468 6520 7365 636f  evices, the seco
+00014d90: 6e64 2063 6f6c 756d 6e20 7772 6170 7320  nd column wraps 
+00014da0: 6966 2074 6865 2073 6372 6565 6e20 7769  if the screen wi
+00014db0: 6474 6820 6973 0a20 2020 2020 2020 6c65  dth is.       le
+00014dc0: 7373 2074 6861 6e20 6f72 2065 7175 616c  ss than or equal
+00014dd0: 2074 6f20 3330 3020 7074 2e0a 2020 2020   to 300 pt..    
+00014de0: 2d20 204f 6e20 416e 6472 6f69 6420 6465  -  On Android de
+00014df0: 7669 6365 732c 2074 6865 2073 6563 6f6e  vices, the secon
+00014e00: 6420 636f 6c75 6d6e 2077 7261 7073 2069  d column wraps i
+00014e10: 6620 7468 6520 7363 7265 656e 2077 6964  f the screen wid
+00014e20: 7468 0a20 2020 2020 2020 6973 206c 6573  th.       is les
+00014e30: 7320 7468 616e 206f 7220 6571 7561 6c20  s than or equal 
+00014e40: 746f 2033 3230 2064 702e 0a0a 2020 2020  to 320 dp...    
+00014e50: 546f 2069 6e63 6c75 6465 206d 6f72 6520  To include more 
+00014e60: 7468 616e 2032 2063 6f6c 756d 6e73 2c20  than 2 columns, 
+00014e70: 6f72 2074 6f20 7573 6520 726f 7773 2c20  or to use rows, 
+00014e80: 7573 6520 7468 650a 2020 2020 5b60 6047  use the.    [``G
+00014e90: 7269 6460 605d 5b67 6f6f 676c 652e 6170  rid``][google.ap
+00014ea0: 7073 2e63 6172 642e 7631 2e47 7269 645d  ps.card.v1.Grid]
+00014eb0: 2077 6964 6765 742e 0a0a 2020 2020 6047   widget...    `G
+00014ec0: 6f6f 676c 6520 576f 726b 7370 6163 6520  oogle Workspace 
+00014ed0: 4164 642d 6f6e 7320 616e 6420 4368 6174  Add-ons and Chat
+00014ee0: 0a20 2020 2061 7070 7320 3c68 7474 7073  .    apps <https
+00014ef0: 3a2f 2f64 6576 656c 6f70 6572 732e 676f  ://developers.go
+00014f00: 6f67 6c65 2e63 6f6d 2f77 6f72 6b73 7061  ogle.com/workspa
+00014f10: 6365 2f65 7874 656e 643e 605f 5f3a 2043  ce/extend>`__: C
+00014f20: 6f6c 756d 6e73 0a20 2020 2066 6f72 2047  olumns.    for G
+00014f30: 6f6f 676c 6520 576f 726b 7370 6163 6520  oogle Workspace 
+00014f40: 4164 642d 6f6e 7320 6172 6520 696e 2044  Add-ons are in D
+00014f50: 6576 656c 6f70 6572 2050 7265 7669 6577  eveloper Preview
+00014f60: 2e0a 0a20 2020 2041 7474 7269 6275 7465  ...    Attribute
+00014f70: 733a 0a20 2020 2020 2020 2063 6f6c 756d  s:.        colum
+00014f80: 6e5f 6974 656d 7320 284d 7574 6162 6c65  n_items (Mutable
+00014f90: 5365 7175 656e 6365 5b67 6f6f 676c 652e  Sequence[google.
+00014fa0: 6170 7073 2e63 6172 645f 7631 2e74 7970  apps.card_v1.typ
+00014fb0: 6573 2e43 6f6c 756d 6e73 2e43 6f6c 756d  es.Columns.Colum
+00014fc0: 6e5d 293a 0a20 2020 2020 2020 2020 2020  n]):.           
+00014fd0: 2041 6e20 6172 7261 7920 6f66 2063 6f6c   An array of col
+00014fe0: 756d 6e73 2e20 596f 7520 6361 6e20 696e  umns. You can in
+00014ff0: 636c 7564 6520 7570 2074 6f20 320a 2020  clude up to 2.  
+00015000: 2020 2020 2020 2020 2020 636f 6c75 6d6e            column
+00015010: 7320 696e 2061 2063 6172 6420 6f72 2064  s in a card or d
+00015020: 6961 6c6f 672e 0a20 2020 2022 2222 0a0a  ialog..    """..
+00015030: 2020 2020 636c 6173 7320 436f 6c75 6d6e      class Column
+00015040: 2870 726f 746f 2e4d 6573 7361 6765 293a  (proto.Message):
+00015050: 0a20 2020 2020 2020 2072 2222 2241 2063  .        r"""A c
+00015060: 6f6c 756d 6e2e 0a0a 2020 2020 2020 2020  olumn...        
+00015070: 6047 6f6f 676c 6520 576f 726b 7370 6163  `Google Workspac
+00015080: 6520 4164 642d 6f6e 7320 616e 6420 4368  e Add-ons and Ch
+00015090: 6174 0a20 2020 2020 2020 2061 7070 7320  at.        apps 
+000150a0: 3c68 7474 7073 3a2f 2f64 6576 656c 6f70  <https://develop
+000150b0: 6572 732e 676f 6f67 6c65 2e63 6f6d 2f77  ers.google.com/w
+000150c0: 6f72 6b73 7061 6365 2f65 7874 656e 643e  orkspace/extend>
+000150d0: 605f 5f3a 2043 6f6c 756d 6e73 0a20 2020  `__: Columns.   
+000150e0: 2020 2020 2066 6f72 2047 6f6f 676c 6520       for Google 
+000150f0: 576f 726b 7370 6163 6520 4164 642d 6f6e  Workspace Add-on
+00015100: 7320 6172 6520 696e 2044 6576 656c 6f70  s are in Develop
+00015110: 6572 2050 7265 7669 6577 2e0a 0a20 2020  er Preview...   
+00015120: 2020 2020 2041 7474 7269 6275 7465 733a       Attributes:
+00015130: 0a20 2020 2020 2020 2020 2020 2068 6f72  .            hor
+00015140: 697a 6f6e 7461 6c5f 7369 7a65 5f73 7479  izontal_size_sty
+00015150: 6c65 2028 676f 6f67 6c65 2e61 7070 732e  le (google.apps.
+00015160: 6361 7264 5f76 312e 7479 7065 732e 436f  card_v1.types.Co
+00015170: 6c75 6d6e 732e 436f 6c75 6d6e 2e48 6f72  lumns.Column.Hor
+00015180: 697a 6f6e 7461 6c53 697a 6553 7479 6c65  izontalSizeStyle
+00015190: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000151a0: 2020 2053 7065 6369 6669 6573 2068 6f77     Specifies how
+000151b0: 2061 2063 6f6c 756d 6e20 6669 6c6c 7320   a column fills 
+000151c0: 7468 6520 7769 6474 6820 6f66 2074 6865  the width of the
+000151d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000151e0: 2063 6172 642e 0a20 2020 2020 2020 2020   card..         
+000151f0: 2020 2068 6f72 697a 6f6e 7461 6c5f 616c     horizontal_al
+00015200: 6967 6e6d 656e 7420 2867 6f6f 676c 652e  ignment (google.
+00015210: 6170 7073 2e63 6172 645f 7631 2e74 7970  apps.card_v1.typ
+00015220: 6573 2e57 6964 6765 742e 486f 7269 7a6f  es.Widget.Horizo
+00015230: 6e74 616c 416c 6967 6e6d 656e 7429 3a0a  ntalAlignment):.
+00015240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015250: 5370 6563 6966 6965 7320 7768 6574 6865  Specifies whethe
+00015260: 7220 7769 6467 6574 7320 616c 6967 6e20  r widgets align 
+00015270: 746f 2074 6865 206c 6566 742c 0a20 2020  to the left,.   
+00015280: 2020 2020 2020 2020 2020 2020 2072 6967               rig
+00015290: 6874 2c20 6f72 2063 656e 7465 7220 6f66  ht, or center of
+000152a0: 2061 2063 6f6c 756d 6e2e 0a20 2020 2020   a column..     
+000152b0: 2020 2020 2020 2076 6572 7469 6361 6c5f         vertical_
+000152c0: 616c 6967 6e6d 656e 7420 2867 6f6f 676c  alignment (googl
+000152d0: 652e 6170 7073 2e63 6172 645f 7631 2e74  e.apps.card_v1.t
+000152e0: 7970 6573 2e43 6f6c 756d 6e73 2e43 6f6c  ypes.Columns.Col
+000152f0: 756d 6e2e 5665 7274 6963 616c 416c 6967  umn.VerticalAlig
+00015300: 6e6d 656e 7429 3a0a 2020 2020 2020 2020  nment):.        
+00015310: 2020 2020 2020 2020 5370 6563 6966 6965          Specifie
+00015320: 7320 7768 6574 6865 7220 7769 6467 6574  s whether widget
+00015330: 7320 616c 6967 6e20 746f 2074 6865 2074  s align to the t
+00015340: 6f70 2c0a 2020 2020 2020 2020 2020 2020  op,.            
+00015350: 2020 2020 626f 7474 6f6d 2c20 6f72 2063      bottom, or c
+00015360: 656e 7465 7220 6f66 2061 2063 6f6c 756d  enter of a colum
+00015370: 6e2e 0a20 2020 2020 2020 2020 2020 2077  n..            w
+00015380: 6964 6765 7473 2028 4d75 7461 626c 6553  idgets (MutableS
+00015390: 6571 7565 6e63 655b 676f 6f67 6c65 2e61  equence[google.a
+000153a0: 7070 732e 6361 7264 5f76 312e 7479 7065  pps.card_v1.type
+000153b0: 732e 436f 6c75 6d6e 732e 436f 6c75 6d6e  s.Columns.Column
+000153c0: 2e57 6964 6765 7473 5d29 3a0a 2020 2020  .Widgets]):.    
+000153d0: 2020 2020 2020 2020 2020 2020 416e 2061              An a
+000153e0: 7272 6179 206f 6620 7769 6467 6574 7320  rray of widgets 
+000153f0: 696e 636c 7564 6564 2069 6e20 6120 636f  included in a co
+00015400: 6c75 6d6e 2e0a 2020 2020 2020 2020 2020  lumn..          
+00015410: 2020 2020 2020 5769 6467 6574 7320 6170        Widgets ap
+00015420: 7065 6172 2069 6e20 7468 6520 6f72 6465  pear in the orde
+00015430: 7220 7468 6174 2074 6865 7920 6172 650a  r that they are.
+00015440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015450: 7370 6563 6966 6965 642e 0a20 2020 2020  specified..     
+00015460: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+00015470: 636c 6173 7320 486f 7269 7a6f 6e74 616c  class Horizontal
+00015480: 5369 7a65 5374 796c 6528 7072 6f74 6f2e  SizeStyle(proto.
+00015490: 456e 756d 293a 0a20 2020 2020 2020 2020  Enum):.         
+000154a0: 2020 2072 2222 2253 7065 6369 6669 6573     r"""Specifies
+000154b0: 2068 6f77 2061 2063 6f6c 756d 6e20 6669   how a column fi
+000154c0: 6c6c 7320 7468 6520 7769 6474 6820 6f66  lls the width of
+000154d0: 2074 6865 2063 6172 642e 2054 6865 2077   the card. The w
+000154e0: 6964 7468 206f 660a 2020 2020 2020 2020  idth of.        
+000154f0: 2020 2020 6561 6368 2063 6f6c 756d 6e20      each column 
+00015500: 6465 7065 6e64 7320 6f6e 2062 6f74 6820  depends on both 
+00015510: 7468 6520 6060 486f 7269 7a6f 6e74 616c  the ``Horizontal
+00015520: 5369 7a65 5374 796c 6560 6020 616e 6420  SizeStyle`` and 
+00015530: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
+00015540: 7769 6474 6820 6f66 2074 6865 2077 6964  width of the wid
+00015550: 6765 7473 2077 6974 6869 6e20 7468 6520  gets within the 
+00015560: 636f 6c75 6d6e 2e0a 0a20 2020 2020 2020  column...       
+00015570: 2020 2020 2060 476f 6f67 6c65 2057 6f72       `Google Wor
+00015580: 6b73 7061 6365 2041 6464 2d6f 6e73 2061  kspace Add-ons a
+00015590: 6e64 2043 6861 740a 2020 2020 2020 2020  nd Chat.        
+000155a0: 2020 2020 6170 7073 203c 6874 7470 733a      apps <https:
+000155b0: 2f2f 6465 7665 6c6f 7065 7273 2e67 6f6f  //developers.goo
+000155c0: 676c 652e 636f 6d2f 776f 726b 7370 6163  gle.com/workspac
+000155d0: 652f 6578 7465 6e64 3e60 5f5f 3a20 436f  e/extend>`__: Co
+000155e0: 6c75 6d6e 730a 2020 2020 2020 2020 2020  lumns.          
+000155f0: 2020 666f 7220 476f 6f67 6c65 2057 6f72    for Google Wor
+00015600: 6b73 7061 6365 2041 6464 2d6f 6e73 2061  kspace Add-ons a
+00015610: 7265 2069 6e20 4465 7665 6c6f 7065 7220  re in Developer 
+00015620: 5072 6576 6965 772e 0a0a 2020 2020 2020  Preview...      
+00015630: 2020 2020 2020 5661 6c75 6573 3a0a 2020        Values:.  
+00015640: 2020 2020 2020 2020 2020 2020 2020 484f                HO
+00015650: 5249 5a4f 4e54 414c 5f53 495a 455f 5354  RIZONTAL_SIZE_ST
+00015660: 594c 455f 554e 5350 4543 4946 4945 4420  YLE_UNSPECIFIED 
+00015670: 2830 293a 0a20 2020 2020 2020 2020 2020  (0):.           
+00015680: 2020 2020 2020 2020 2044 6f6e 2774 2075           Don't u
+00015690: 7365 2e20 556e 7370 6563 6966 6965 642e  se. Unspecified.
+000156a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000156b0: 2046 494c 4c5f 4156 4149 4c41 424c 455f   FILL_AVAILABLE_
+000156c0: 5350 4143 4520 2831 293a 0a20 2020 2020  SPACE (1):.     
+000156d0: 2020 2020 2020 2020 2020 2020 2020 2044                 D
+000156e0: 6566 6175 6c74 2076 616c 7565 2e20 436f  efault value. Co
+000156f0: 6c75 6d6e 2066 696c 6c73 2074 6865 2061  lumn fills the a
+00015700: 7661 696c 6162 6c65 2073 7061 6365 2c20  vailable space, 
+00015710: 7570 2074 6f20 3730 250a 2020 2020 2020  up to 70%.      
+00015720: 2020 2020 2020 2020 2020 2020 2020 6f66                of
+00015730: 2074 6865 2063 6172 6427 7320 7769 6474   the card's widt
+00015740: 682e 2049 6620 626f 7468 2063 6f6c 756d  h. If both colum
+00015750: 6e73 2061 7265 2073 6574 2074 6f0a 2020  ns are set to.  
+00015760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015770: 2020 6060 4649 4c4c 5f41 5641 494c 4142    ``FILL_AVAILAB
+00015780: 4c45 5f53 5041 4345 6060 2c20 6561 6368  LE_SPACE``, each
+00015790: 2063 6f6c 756d 6e20 6669 6c6c 7320 3530   column fills 50
+000157a0: 2520 6f66 2074 6865 0a20 2020 2020 2020  % of the.       
+000157b0: 2020 2020 2020 2020 2020 2020 2073 7061               spa
+000157c0: 6365 2e0a 2020 2020 2020 2020 2020 2020  ce..            
+000157d0: 2020 2020 4649 4c4c 5f4d 494e 494d 554d      FILL_MINIMUM
+000157e0: 5f53 5041 4345 2028 3229 3a0a 2020 2020  _SPACE (2):.    
+000157f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015800: 436f 6c75 6d6e 2066 696c 6c73 2074 6865  Column fills the
+00015810: 206c 6561 7374 2061 6d6f 756e 7420 6f66   least amount of
+00015820: 2073 7061 6365 0a20 2020 2020 2020 2020   space.         
+00015830: 2020 2020 2020 2020 2020 2070 6f73 7369             possi
+00015840: 626c 6520 616e 6420 6e6f 206d 6f72 6520  ble and no more 
+00015850: 7468 616e 2033 3025 206f 6620 7468 6520  than 30% of the 
+00015860: 6361 7264 2773 0a20 2020 2020 2020 2020  card's.         
+00015870: 2020 2020 2020 2020 2020 2077 6964 7468             width
+00015880: 2e0a 2020 2020 2020 2020 2020 2020 2222  ..            ""
+00015890: 220a 2020 2020 2020 2020 2020 2020 484f  ".            HO
+000158a0: 5249 5a4f 4e54 414c 5f53 495a 455f 5354  RIZONTAL_SIZE_ST
+000158b0: 594c 455f 554e 5350 4543 4946 4945 4420  YLE_UNSPECIFIED 
+000158c0: 3d20 300a 2020 2020 2020 2020 2020 2020  = 0.            
+000158d0: 4649 4c4c 5f41 5641 494c 4142 4c45 5f53  FILL_AVAILABLE_S
+000158e0: 5041 4345 203d 2031 0a20 2020 2020 2020  PACE = 1.       
+000158f0: 2020 2020 2046 494c 4c5f 4d49 4e49 4d55       FILL_MINIMU
+00015900: 4d5f 5350 4143 4520 3d20 320a 0a20 2020  M_SPACE = 2..   
+00015910: 2020 2020 2063 6c61 7373 2056 6572 7469       class Verti
+00015920: 6361 6c41 6c69 676e 6d65 6e74 2870 726f  calAlignment(pro
+00015930: 746f 2e45 6e75 6d29 3a0a 2020 2020 2020  to.Enum):.      
+00015940: 2020 2020 2020 7222 2222 5370 6563 6966        r"""Specif
+00015950: 6965 7320 7768 6574 6865 7220 7769 6467  ies whether widg
+00015960: 6574 7320 616c 6967 6e20 746f 2074 6865  ets align to the
+00015970: 2074 6f70 2c20 626f 7474 6f6d 2c20 6f72   top, bottom, or
+00015980: 2063 656e 7465 7220 6f66 2061 0a20 2020   center of a.   
+00015990: 2020 2020 2020 2020 2063 6f6c 756d 6e2e           column.
+000159a0: 0a0a 2020 2020 2020 2020 2020 2020 6047  ..            `G
+000159b0: 6f6f 676c 6520 576f 726b 7370 6163 6520  oogle Workspace 
+000159c0: 4164 642d 6f6e 7320 616e 6420 4368 6174  Add-ons and Chat
+000159d0: 0a20 2020 2020 2020 2020 2020 2061 7070  .            app
+000159e0: 7320 3c68 7474 7073 3a2f 2f64 6576 656c  s <https://devel
+000159f0: 6f70 6572 732e 676f 6f67 6c65 2e63 6f6d  opers.google.com
+00015a00: 2f77 6f72 6b73 7061 6365 2f65 7874 656e  /workspace/exten
+00015a10: 643e 605f 5f3a 2043 6f6c 756d 6e73 0a20  d>`__: Columns. 
+00015a20: 2020 2020 2020 2020 2020 2066 6f72 2047             for G
+00015a30: 6f6f 676c 6520 576f 726b 7370 6163 6520  oogle Workspace 
+00015a40: 4164 642d 6f6e 7320 6172 6520 696e 2044  Add-ons are in D
+00015a50: 6576 656c 6f70 6572 2050 7265 7669 6577  eveloper Preview
+00015a60: 2e0a 0a20 2020 2020 2020 2020 2020 2056  ...            V
+00015a70: 616c 7565 733a 0a20 2020 2020 2020 2020  alues:.         
+00015a80: 2020 2020 2020 2056 4552 5449 4341 4c5f         VERTICAL_
+00015a90: 414c 4947 4e4d 454e 545f 554e 5350 4543  ALIGNMENT_UNSPEC
+00015aa0: 4946 4945 4420 2830 293a 0a20 2020 2020  IFIED (0):.     
+00015ab0: 2020 2020 2020 2020 2020 2020 2020 2044                 D
+00015ac0: 6f6e 2774 2075 7365 2e20 556e 7370 6563  on't use. Unspec
+00015ad0: 6966 6965 642e 0a20 2020 2020 2020 2020  ified..         
+00015ae0: 2020 2020 2020 2043 454e 5445 5220 2831         CENTER (1
+00015af0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00015b00: 2020 2020 2020 2044 6566 6175 6c74 2076         Default v
+00015b10: 616c 7565 2e20 416c 6967 6e73 2077 6964  alue. Aligns wid
+00015b20: 6765 7473 2074 6f20 7468 6520 6365 6e74  gets to the cent
+00015b30: 6572 0a20 2020 2020 2020 2020 2020 2020  er.             
+00015b40: 2020 2020 2020 206f 6620 6120 636f 6c75         of a colu
+00015b50: 6d6e 2e0a 2020 2020 2020 2020 2020 2020  mn..            
+00015b60: 2020 2020 544f 5020 2832 293a 0a20 2020      TOP (2):.   
+00015b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015b80: 2041 6c69 676e 7320 7769 6467 6574 7320   Aligns widgets 
+00015b90: 746f 2074 6865 2074 6f70 206f 6620 6120  to the top of a 
+00015ba0: 636f 6c75 6d6e 2e0a 2020 2020 2020 2020  column..        
+00015bb0: 2020 2020 2020 2020 424f 5454 4f4d 2028          BOTTOM (
+00015bc0: 3329 3a0a 2020 2020 2020 2020 2020 2020  3):.            
+00015bd0: 2020 2020 2020 2020 416c 6967 6e73 2077          Aligns w
+00015be0: 6964 6765 7473 2074 6f20 7468 6520 626f  idgets to the bo
+00015bf0: 7474 6f6d 206f 6620 6120 636f 6c75 6d6e  ttom of a column
+00015c00: 2e0a 2020 2020 2020 2020 2020 2020 2222  ..            ""
+00015c10: 220a 2020 2020 2020 2020 2020 2020 5645  ".            VE
+00015c20: 5254 4943 414c 5f41 4c49 474e 4d45 4e54  RTICAL_ALIGNMENT
+00015c30: 5f55 4e53 5045 4349 4649 4544 203d 2030  _UNSPECIFIED = 0
+00015c40: 0a20 2020 2020 2020 2020 2020 2043 454e  .            CEN
+00015c50: 5445 5220 3d20 310a 2020 2020 2020 2020  TER = 1.        
+00015c60: 2020 2020 544f 5020 3d20 320a 2020 2020      TOP = 2.    
+00015c70: 2020 2020 2020 2020 424f 5454 4f4d 203d          BOTTOM =
+00015c80: 2033 0a0a 2020 2020 2020 2020 636c 6173   3..        clas
+00015c90: 7320 5769 6467 6574 7328 7072 6f74 6f2e  s Widgets(proto.
+00015ca0: 4d65 7373 6167 6529 3a0a 2020 2020 2020  Message):.      
+00015cb0: 2020 2020 2020 7222 2222 5468 6520 7375        r"""The su
+00015cc0: 7070 6f72 7465 6420 7769 6467 6574 7320  pported widgets 
+00015cd0: 7468 6174 2079 6f75 2063 616e 2069 6e63  that you can inc
+00015ce0: 6c75 6465 2069 6e20 6120 636f 6c75 6d6e  lude in a column
+00015cf0: 2e0a 0a20 2020 2020 2020 2020 2020 2060  ...            `
+00015d00: 476f 6f67 6c65 2057 6f72 6b73 7061 6365  Google Workspace
+00015d10: 2041 6464 2d6f 6e73 2061 6e64 2043 6861   Add-ons and Cha
+00015d20: 740a 2020 2020 2020 2020 2020 2020 6170  t.            ap
+00015d30: 7073 203c 6874 7470 733a 2f2f 6465 7665  ps <https://deve
+00015d40: 6c6f 7065 7273 2e67 6f6f 676c 652e 636f  lopers.google.co
+00015d50: 6d2f 776f 726b 7370 6163 652f 6578 7465  m/workspace/exte
+00015d60: 6e64 3e60 5f5f 3a20 436f 6c75 6d6e 730a  nd>`__: Columns.
+00015d70: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00015d80: 476f 6f67 6c65 2057 6f72 6b73 7061 6365  Google Workspace
+00015d90: 2041 6464 2d6f 6e73 2061 7265 2069 6e20   Add-ons are in 
+00015da0: 4465 7665 6c6f 7065 7220 5072 6576 6965  Developer Previe
+00015db0: 772e 0a0a 2020 2020 2020 2020 2020 2020  w...            
+00015dc0: 5468 6973 206d 6573 7361 6765 2068 6173  This message has
+00015dd0: 2060 6f6e 656f 6660 5f20 6669 656c 6473   `oneof`_ fields
+00015de0: 2028 6d75 7475 616c 6c79 2065 7863 6c75   (mutually exclu
+00015df0: 7369 7665 2066 6965 6c64 7329 2e0a 2020  sive fields)..  
+00015e00: 2020 2020 2020 2020 2020 466f 7220 6561            For ea
+00015e10: 6368 206f 6e65 6f66 2c20 6174 206d 6f73  ch oneof, at mos
+00015e20: 7420 6f6e 6520 6d65 6d62 6572 2066 6965  t one member fie
+00015e30: 6c64 2063 616e 2062 6520 7365 7420 6174  ld can be set at
+00015e40: 2074 6865 2073 616d 6520 7469 6d65 2e0a   the same time..
+00015e50: 2020 2020 2020 2020 2020 2020 5365 7474              Sett
+00015e60: 696e 6720 616e 7920 6d65 6d62 6572 206f  ing any member o
+00015e70: 6620 7468 6520 6f6e 656f 6620 6175 746f  f the oneof auto
+00015e80: 6d61 7469 6361 6c6c 7920 636c 6561 7273  matically clears
+00015e90: 2061 6c6c 206f 7468 6572 0a20 2020 2020   all other.     
+00015ea0: 2020 2020 2020 206d 656d 6265 7273 2e0a         members..
+00015eb0: 0a20 2020 2020 2020 2020 2020 202e 2e20  .            .. 
+00015ec0: 5f6f 6e65 6f66 3a20 6874 7470 733a 2f2f  _oneof: https://
+00015ed0: 7072 6f74 6f2d 706c 7573 2d70 7974 686f  proto-plus-pytho
+00015ee0: 6e2e 7265 6164 7468 6564 6f63 732e 696f  n.readthedocs.io
+00015ef0: 2f65 6e2f 7374 6162 6c65 2f66 6965 6c64  /en/stable/field
+00015f00: 732e 6874 6d6c 236f 6e65 6f66 732d 6d75  s.html#oneofs-mu
+00015f10: 7475 616c 6c79 2d65 7863 6c75 7369 7665  tually-exclusive
+00015f20: 2d66 6965 6c64 730a 0a20 2020 2020 2020  -fields..       
+00015f30: 2020 2020 2041 7474 7269 6275 7465 733a       Attributes:
+00015f40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015f50: 2074 6578 745f 7061 7261 6772 6170 6820   text_paragraph 
+00015f60: 2867 6f6f 676c 652e 6170 7073 2e63 6172  (google.apps.car
+00015f70: 645f 7631 2e74 7970 6573 2e54 6578 7450  d_v1.types.TextP
+00015f80: 6172 6167 7261 7068 293a 0a20 2020 2020  aragraph):.     
+00015f90: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+00015fa0: 5465 7874 5061 7261 6772 6170 685d 5b67  TextParagraph][g
+00015fb0: 6f6f 676c 652e 6170 7073 2e63 6172 642e  oogle.apps.card.
+00015fc0: 7631 2e54 6578 7450 6172 6167 7261 7068  v1.TextParagraph
+00015fd0: 5d20 7769 6467 6574 2e0a 0a20 2020 2020  ] widget...     
+00015fe0: 2020 2020 2020 2020 2020 2020 2020 2054                 T
+00015ff0: 6869 7320 6669 656c 6420 6973 2061 206d  his field is a m
+00016000: 656d 6265 7220 6f66 2060 6f6e 656f 6660  ember of `oneof`
+00016010: 5f20 6060 6461 7461 6060 2e0a 2020 2020  _ ``data``..    
+00016020: 2020 2020 2020 2020 2020 2020 696d 6167              imag
+00016030: 6520 2867 6f6f 676c 652e 6170 7073 2e63  e (google.apps.c
+00016040: 6172 645f 7631 2e74 7970 6573 2e49 6d61  ard_v1.types.Ima
+00016050: 6765 293a 0a20 2020 2020 2020 2020 2020  ge):.           
+00016060: 2020 2020 2020 2020 205b 496d 6167 655d           [Image]
+00016070: 5b67 6f6f 676c 652e 6170 7073 2e63 6172  [google.apps.car
+00016080: 642e 7631 2e49 6d61 6765 5d20 7769 6467  d.v1.Image] widg
+00016090: 6574 2e0a 0a20 2020 2020 2020 2020 2020  et...           
+000160a0: 2020 2020 2020 2020 2054 6869 7320 6669           This fi
+000160b0: 656c 6420 6973 2061 206d 656d 6265 7220  eld is a member 
+000160c0: 6f66 2060 6f6e 656f 6660 5f20 6060 6461  of `oneof`_ ``da
+000160d0: 7461 6060 2e0a 2020 2020 2020 2020 2020  ta``..          
+000160e0: 2020 2020 2020 6465 636f 7261 7465 645f        decorated_
+000160f0: 7465 7874 2028 676f 6f67 6c65 2e61 7070  text (google.app
+00016100: 732e 6361 7264 5f76 312e 7479 7065 732e  s.card_v1.types.
+00016110: 4465 636f 7261 7465 6454 6578 7429 3a0a  DecoratedText):.
+00016120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016130: 2020 2020 5b44 6563 6f72 6174 6564 5465      [DecoratedTe
+00016140: 7874 5d5b 676f 6f67 6c65 2e61 7070 732e  xt][google.apps.
+00016150: 6361 7264 2e76 312e 4465 636f 7261 7465  card.v1.Decorate
+00016160: 6454 6578 745d 2077 6964 6765 742e 0a0a  dText] widget...
+00016170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016180: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
+00016190: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
+000161a0: 6e65 6f66 605f 2060 6064 6174 6160 602e  neof`_ ``data``.
+000161b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000161c0: 2062 7574 746f 6e5f 6c69 7374 2028 676f   button_list (go
+000161d0: 6f67 6c65 2e61 7070 732e 6361 7264 5f76  ogle.apps.card_v
+000161e0: 312e 7479 7065 732e 4275 7474 6f6e 4c69  1.types.ButtonLi
+000161f0: 7374 293a 0a20 2020 2020 2020 2020 2020  st):.           
+00016200: 2020 2020 2020 2020 205b 4275 7474 6f6e           [Button
+00016210: 4c69 7374 5d5b 676f 6f67 6c65 2e61 7070  List][google.app
+00016220: 732e 6361 7264 2e76 312e 4275 7474 6f6e  s.card.v1.Button
+00016230: 4c69 7374 5d20 7769 6467 6574 2e0a 0a20  List] widget... 
+00016240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016250: 2020 2054 6869 7320 6669 656c 6420 6973     This field is
+00016260: 2061 206d 656d 6265 7220 6f66 2060 6f6e   a member of `on
+00016270: 656f 6660 5f20 6060 6461 7461 6060 2e0a  eof`_ ``data``..
+00016280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016290: 7465 7874 5f69 6e70 7574 2028 676f 6f67  text_input (goog
+000162a0: 6c65 2e61 7070 732e 6361 7264 5f76 312e  le.apps.card_v1.
+000162b0: 7479 7065 732e 5465 7874 496e 7075 7429  types.TextInput)
+000162c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000162d0: 2020 2020 2020 5b54 6578 7449 6e70 7574        [TextInput
+000162e0: 5d5b 676f 6f67 6c65 2e61 7070 732e 6361  ][google.apps.ca
+000162f0: 7264 2e76 312e 5465 7874 496e 7075 745d  rd.v1.TextInput]
+00016300: 2077 6964 6765 742e 0a0a 2020 2020 2020   widget...      
+00016310: 2020 2020 2020 2020 2020 2020 2020 5468                Th
+00016320: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
+00016330: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
+00016340: 2060 6064 6174 6160 602e 0a20 2020 2020   ``data``..     
+00016350: 2020 2020 2020 2020 2020 2073 656c 6563             selec
+00016360: 7469 6f6e 5f69 6e70 7574 2028 676f 6f67  tion_input (goog
+00016370: 6c65 2e61 7070 732e 6361 7264 5f76 312e  le.apps.card_v1.
+00016380: 7479 7065 732e 5365 6c65 6374 696f 6e49  types.SelectionI
+00016390: 6e70 7574 293a 0a20 2020 2020 2020 2020  nput):.         
+000163a0: 2020 2020 2020 2020 2020 205b 5365 6c65             [Sele
+000163b0: 6374 696f 6e49 6e70 7574 5d5b 676f 6f67  ctionInput][goog
+000163c0: 6c65 2e61 7070 732e 6361 7264 2e76 312e  le.apps.card.v1.
+000163d0: 5365 6c65 6374 696f 6e49 6e70 7574 5d20  SelectionInput] 
+000163e0: 7769 6467 6574 2e0a 0a20 2020 2020 2020  widget...       
+000163f0: 2020 2020 2020 2020 2020 2020 2054 6869               Thi
+00016400: 7320 6669 656c 6420 6973 2061 206d 656d  s field is a mem
+00016410: 6265 7220 6f66 2060 6f6e 656f 6660 5f20  ber of `oneof`_ 
+00016420: 6060 6461 7461 6060 2e0a 2020 2020 2020  ``data``..      
+00016430: 2020 2020 2020 2020 2020 6461 7465 5f74            date_t
+00016440: 696d 655f 7069 636b 6572 2028 676f 6f67  ime_picker (goog
+00016450: 6c65 2e61 7070 732e 6361 7264 5f76 312e  le.apps.card_v1.
+00016460: 7479 7065 732e 4461 7465 5469 6d65 5069  types.DateTimePi
+00016470: 636b 6572 293a 0a20 2020 2020 2020 2020  cker):.         
+00016480: 2020 2020 2020 2020 2020 205b 4461 7465             [Date
+00016490: 5469 6d65 5069 636b 6572 5d5b 676f 6f67  TimePicker][goog
+000164a0: 6c65 2e61 7070 732e 6361 7264 2e76 312e  le.apps.card.v1.
+000164b0: 4461 7465 5469 6d65 5069 636b 6572 5d20  DateTimePicker] 
+000164c0: 7769 6467 6574 2e0a 0a20 2020 2020 2020  widget...       
+000164d0: 2020 2020 2020 2020 2020 2020 2054 6869               Thi
+000164e0: 7320 6669 656c 6420 6973 2061 206d 656d  s field is a mem
+000164f0: 6265 7220 6f66 2060 6f6e 656f 6660 5f20  ber of `oneof`_ 
+00016500: 6060 6461 7461 6060 2e0a 2020 2020 2020  ``data``..      
+00016510: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+00016520: 2020 2020 2020 2074 6578 745f 7061 7261         text_para
+00016530: 6772 6170 683a 2022 5465 7874 5061 7261  graph: "TextPara
+00016540: 6772 6170 6822 203d 2070 726f 746f 2e46  graph" = proto.F
+00016550: 6965 6c64 280a 2020 2020 2020 2020 2020  ield(.          
+00016560: 2020 2020 2020 7072 6f74 6f2e 4d45 5353        proto.MESS
+00016570: 4147 452c 0a20 2020 2020 2020 2020 2020  AGE,.           
+00016580: 2020 2020 206e 756d 6265 723d 312c 0a20       number=1,. 
+00016590: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+000165a0: 6e65 6f66 3d22 6461 7461 222c 0a20 2020  neof="data",.   
+000165b0: 2020 2020 2020 2020 2020 2020 206d 6573               mes
+000165c0: 7361 6765 3d22 5465 7874 5061 7261 6772  sage="TextParagr
+000165d0: 6170 6822 2c0a 2020 2020 2020 2020 2020  aph",.          
+000165e0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+000165f0: 696d 6167 653a 2022 496d 6167 6522 203d  image: "Image" =
+00016600: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
+00016610: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00016620: 6f74 6f2e 4d45 5353 4147 452c 0a20 2020  oto.MESSAGE,.   
+00016630: 2020 2020 2020 2020 2020 2020 206e 756d               num
+00016640: 6265 723d 322c 0a20 2020 2020 2020 2020  ber=2,.         
+00016650: 2020 2020 2020 206f 6e65 6f66 3d22 6461         oneof="da
+00016660: 7461 222c 0a20 2020 2020 2020 2020 2020  ta",.           
+00016670: 2020 2020 206d 6573 7361 6765 3d22 496d       message="Im
+00016680: 6167 6522 2c0a 2020 2020 2020 2020 2020  age",.          
+00016690: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+000166a0: 6465 636f 7261 7465 645f 7465 7874 3a20  decorated_text: 
+000166b0: 2244 6563 6f72 6174 6564 5465 7874 2220  "DecoratedText" 
+000166c0: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
+000166d0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000166e0: 726f 746f 2e4d 4553 5341 4745 2c0a 2020  roto.MESSAGE,.  
+000166f0: 2020 2020 2020 2020 2020 2020 2020 6e75                nu
+00016700: 6d62 6572 3d33 2c0a 2020 2020 2020 2020  mber=3,.        
+00016710: 2020 2020 2020 2020 6f6e 656f 663d 2264          oneof="d
+00016720: 6174 6122 2c0a 2020 2020 2020 2020 2020  ata",.          
+00016730: 2020 2020 2020 6d65 7373 6167 653d 2244        message="D
+00016740: 6563 6f72 6174 6564 5465 7874 222c 0a20  ecoratedText",. 
+00016750: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00016760: 2020 2020 2020 2020 2062 7574 746f 6e5f           button_
+00016770: 6c69 7374 3a20 2242 7574 746f 6e4c 6973  list: "ButtonLis
+00016780: 7422 203d 2070 726f 746f 2e46 6965 6c64  t" = proto.Field
+00016790: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000167a0: 2020 7072 6f74 6f2e 4d45 5353 4147 452c    proto.MESSAGE,
+000167b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000167c0: 206e 756d 6265 723d 342c 0a20 2020 2020   number=4,.     
+000167d0: 2020 2020 2020 2020 2020 206f 6e65 6f66             oneof
+000167e0: 3d22 6461 7461 222c 0a20 2020 2020 2020  ="data",.       
+000167f0: 2020 2020 2020 2020 206d 6573 7361 6765           message
+00016800: 3d22 4275 7474 6f6e 4c69 7374 222c 0a20  ="ButtonList",. 
+00016810: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00016820: 2020 2020 2020 2020 2074 6578 745f 696e           text_in
+00016830: 7075 743a 2022 5465 7874 496e 7075 7422  put: "TextInput"
+00016840: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
+00016850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016860: 7072 6f74 6f2e 4d45 5353 4147 452c 0a20  proto.MESSAGE,. 
+00016870: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00016880: 756d 6265 723d 352c 0a20 2020 2020 2020  umber=5,.       
+00016890: 2020 2020 2020 2020 206f 6e65 6f66 3d22           oneof="
+000168a0: 6461 7461 222c 0a20 2020 2020 2020 2020  data",.         
+000168b0: 2020 2020 2020 206d 6573 7361 6765 3d22         message="
+000168c0: 5465 7874 496e 7075 7422 2c0a 2020 2020  TextInput",.    
+000168d0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000168e0: 2020 2020 2020 7365 6c65 6374 696f 6e5f        selection_
+000168f0: 696e 7075 743a 2022 5365 6c65 6374 696f  input: "Selectio
+00016900: 6e49 6e70 7574 2220 3d20 7072 6f74 6f2e  nInput" = proto.
+00016910: 4669 656c 6428 0a20 2020 2020 2020 2020  Field(.         
+00016920: 2020 2020 2020 2070 726f 746f 2e4d 4553         proto.MES
+00016930: 5341 4745 2c0a 2020 2020 2020 2020 2020  SAGE,.          
+00016940: 2020 2020 2020 6e75 6d62 6572 3d36 2c0a        number=6,.
+00016950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016960: 6f6e 656f 663d 2264 6174 6122 2c0a 2020  oneof="data",.  
+00016970: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+00016980: 7373 6167 653d 2253 656c 6563 7469 6f6e  ssage="Selection
+00016990: 496e 7075 7422 2c0a 2020 2020 2020 2020  Input",.        
+000169a0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+000169b0: 2020 6461 7465 5f74 696d 655f 7069 636b    date_time_pick
+000169c0: 6572 3a20 2244 6174 6554 696d 6550 6963  er: "DateTimePic
+000169d0: 6b65 7222 203d 2070 726f 746f 2e46 6965  ker" = proto.Fie
+000169e0: 6c64 280a 2020 2020 2020 2020 2020 2020  ld(.            
+000169f0: 2020 2020 7072 6f74 6f2e 4d45 5353 4147      proto.MESSAG
+00016a00: 452c 0a20 2020 2020 2020 2020 2020 2020  E,.             
+00016a10: 2020 206e 756d 6265 723d 372c 0a20 2020     number=7,.   
+00016a20: 2020 2020 2020 2020 2020 2020 206f 6e65               one
+00016a30: 6f66 3d22 6461 7461 222c 0a20 2020 2020  of="data",.     
+00016a40: 2020 2020 2020 2020 2020 206d 6573 7361             messa
+00016a50: 6765 3d22 4461 7465 5469 6d65 5069 636b  ge="DateTimePick
+00016a60: 6572 222c 0a20 2020 2020 2020 2020 2020  er",.           
+00016a70: 2029 0a0a 2020 2020 2020 2020 686f 7269   )..        hori
+00016a80: 7a6f 6e74 616c 5f73 697a 655f 7374 796c  zontal_size_styl
+00016a90: 653a 2022 436f 6c75 6d6e 732e 436f 6c75  e: "Columns.Colu
+00016aa0: 6d6e 2e48 6f72 697a 6f6e 7461 6c53 697a  mn.HorizontalSiz
+00016ab0: 6553 7479 6c65 2220 3d20 7072 6f74 6f2e  eStyle" = proto.
+00016ac0: 4669 656c 6428 0a20 2020 2020 2020 2020  Field(.         
+00016ad0: 2020 2070 726f 746f 2e45 4e55 4d2c 0a20     proto.ENUM,. 
+00016ae0: 2020 2020 2020 2020 2020 206e 756d 6265             numbe
+00016af0: 723d 312c 0a20 2020 2020 2020 2020 2020  r=1,.           
+00016b00: 2065 6e75 6d3d 2243 6f6c 756d 6e73 2e43   enum="Columns.C
+00016b10: 6f6c 756d 6e2e 486f 7269 7a6f 6e74 616c  olumn.Horizontal
+00016b20: 5369 7a65 5374 796c 6522 2c0a 2020 2020  SizeStyle",.    
+00016b30: 2020 2020 290a 2020 2020 2020 2020 686f      ).        ho
+00016b40: 7269 7a6f 6e74 616c 5f61 6c69 676e 6d65  rizontal_alignme
+00016b50: 6e74 3a20 2257 6964 6765 742e 486f 7269  nt: "Widget.Hori
+00016b60: 7a6f 6e74 616c 416c 6967 6e6d 656e 7422  zontalAlignment"
+00016b70: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
+00016b80: 2020 2020 2020 2020 2020 2020 7072 6f74              prot
+00016b90: 6f2e 454e 554d 2c0a 2020 2020 2020 2020  o.ENUM,.        
+00016ba0: 2020 2020 6e75 6d62 6572 3d32 2c0a 2020      number=2,.  
+00016bb0: 2020 2020 2020 2020 2020 656e 756d 3d22            enum="
+00016bc0: 5769 6467 6574 2e48 6f72 697a 6f6e 7461  Widget.Horizonta
+00016bd0: 6c41 6c69 676e 6d65 6e74 222c 0a20 2020  lAlignment",.   
+00016be0: 2020 2020 2029 0a20 2020 2020 2020 2076       ).        v
+00016bf0: 6572 7469 6361 6c5f 616c 6967 6e6d 656e  ertical_alignmen
+00016c00: 743a 2022 436f 6c75 6d6e 732e 436f 6c75  t: "Columns.Colu
+00016c10: 6d6e 2e56 6572 7469 6361 6c41 6c69 676e  mn.VerticalAlign
+00016c20: 6d65 6e74 2220 3d20 7072 6f74 6f2e 4669  ment" = proto.Fi
+00016c30: 656c 6428 0a20 2020 2020 2020 2020 2020  eld(.           
+00016c40: 2070 726f 746f 2e45 4e55 4d2c 0a20 2020   proto.ENUM,.   
+00016c50: 2020 2020 2020 2020 206e 756d 6265 723d           number=
+00016c60: 332c 0a20 2020 2020 2020 2020 2020 2065  3,.            e
+00016c70: 6e75 6d3d 2243 6f6c 756d 6e73 2e43 6f6c  num="Columns.Col
+00016c80: 756d 6e2e 5665 7274 6963 616c 416c 6967  umn.VerticalAlig
+00016c90: 6e6d 656e 7422 2c0a 2020 2020 2020 2020  nment",.        
+00016ca0: 290a 2020 2020 2020 2020 7769 6467 6574  ).        widget
+00016cb0: 733a 204d 7574 6162 6c65 5365 7175 656e  s: MutableSequen
+00016cc0: 6365 5b22 436f 6c75 6d6e 732e 436f 6c75  ce["Columns.Colu
+00016cd0: 6d6e 2e57 6964 6765 7473 225d 203d 2070  mn.Widgets"] = p
+00016ce0: 726f 746f 2e52 6570 6561 7465 6446 6965  roto.RepeatedFie
+00016cf0: 6c64 280a 2020 2020 2020 2020 2020 2020  ld(.            
+00016d00: 7072 6f74 6f2e 4d45 5353 4147 452c 0a20  proto.MESSAGE,. 
+00016d10: 2020 2020 2020 2020 2020 206e 756d 6265             numbe
+00016d20: 723d 342c 0a20 2020 2020 2020 2020 2020  r=4,.           
+00016d30: 206d 6573 7361 6765 3d22 436f 6c75 6d6e   message="Column
+00016d40: 732e 436f 6c75 6d6e 2e57 6964 6765 7473  s.Column.Widgets
+00016d50: 222c 0a20 2020 2020 2020 2029 0a0a 2020  ",.        )..  
+00016d60: 2020 636f 6c75 6d6e 5f69 7465 6d73 3a20    column_items: 
+00016d70: 4d75 7461 626c 6553 6571 7565 6e63 655b  MutableSequence[
+00016d80: 436f 6c75 6d6e 5d20 3d20 7072 6f74 6f2e  Column] = proto.
+00016d90: 5265 7065 6174 6564 4669 656c 6428 0a20  RepeatedField(. 
+00016da0: 2020 2020 2020 2070 726f 746f 2e4d 4553         proto.MES
+00016db0: 5341 4745 2c0a 2020 2020 2020 2020 6e75  SAGE,.        nu
+00016dc0: 6d62 6572 3d32 2c0a 2020 2020 2020 2020  mber=2,.        
+00016dd0: 6d65 7373 6167 653d 436f 6c75 6d6e 2c0a  message=Column,.
+00016de0: 2020 2020 290a 0a0a 636c 6173 7320 4f6e      )...class On
+00016df0: 436c 6963 6b28 7072 6f74 6f2e 4d65 7373  Click(proto.Mess
+00016e00: 6167 6529 3a0a 2020 2020 7222 2222 5265  age):.    r"""Re
+00016e10: 7072 6573 656e 7473 2068 6f77 2074 6f20  presents how to 
+00016e20: 7265 7370 6f6e 6420 7768 656e 2075 7365  respond when use
+00016e30: 7273 2063 6c69 636b 2061 6e20 696e 7465  rs click an inte
+00016e40: 7261 6374 6976 6520 656c 656d 656e 7420  ractive element 
+00016e50: 6f6e 0a20 2020 2061 2063 6172 642c 2073  on.    a card, s
+00016e60: 7563 6820 6173 2061 2062 7574 746f 6e2e  uch as a button.
+00016e70: 0a0a 2020 2020 6047 6f6f 676c 6520 576f  ..    `Google Wo
+00016e80: 726b 7370 6163 6520 4164 642d 6f6e 7320  rkspace Add-ons 
+00016e90: 616e 6420 4368 6174 0a20 2020 2061 7070  and Chat.    app
+00016ea0: 7320 3c68 7474 7073 3a2f 2f64 6576 656c  s <https://devel
+00016eb0: 6f70 6572 732e 676f 6f67 6c65 2e63 6f6d  opers.google.com
+00016ec0: 2f77 6f72 6b73 7061 6365 2f65 7874 656e  /workspace/exten
+00016ed0: 643e 605f 5f3a 0a0a 2020 2020 5468 6973  d>`__:..    This
+00016ee0: 206d 6573 7361 6765 2068 6173 2060 6f6e   message has `on
+00016ef0: 656f 6660 5f20 6669 656c 6473 2028 6d75  eof`_ fields (mu
+00016f00: 7475 616c 6c79 2065 7863 6c75 7369 7665  tually exclusive
+00016f10: 2066 6965 6c64 7329 2e0a 2020 2020 466f   fields)..    Fo
+00016f20: 7220 6561 6368 206f 6e65 6f66 2c20 6174  r each oneof, at
+00016f30: 206d 6f73 7420 6f6e 6520 6d65 6d62 6572   most one member
+00016f40: 2066 6965 6c64 2063 616e 2062 6520 7365   field can be se
+00016f50: 7420 6174 2074 6865 2073 616d 6520 7469  t at the same ti
+00016f60: 6d65 2e0a 2020 2020 5365 7474 696e 6720  me..    Setting 
+00016f70: 616e 7920 6d65 6d62 6572 206f 6620 7468  any member of th
+00016f80: 6520 6f6e 656f 6620 6175 746f 6d61 7469  e oneof automati
+00016f90: 6361 6c6c 7920 636c 6561 7273 2061 6c6c  cally clears all
+00016fa0: 206f 7468 6572 0a20 2020 206d 656d 6265   other.    membe
+00016fb0: 7273 2e0a 0a20 2020 202e 2e20 5f6f 6e65  rs...    .. _one
+00016fc0: 6f66 3a20 6874 7470 733a 2f2f 7072 6f74  of: https://prot
+00016fd0: 6f2d 706c 7573 2d70 7974 686f 6e2e 7265  o-plus-python.re
+00016fe0: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+00016ff0: 7374 6162 6c65 2f66 6965 6c64 732e 6874  stable/fields.ht
+00017000: 6d6c 236f 6e65 6f66 732d 6d75 7475 616c  ml#oneofs-mutual
+00017010: 6c79 2d65 7863 6c75 7369 7665 2d66 6965  ly-exclusive-fie
+00017020: 6c64 730a 0a20 2020 2041 7474 7269 6275  lds..    Attribu
+00017030: 7465 733a 0a20 2020 2020 2020 2061 6374  tes:.        act
+00017040: 696f 6e20 2867 6f6f 676c 652e 6170 7073  ion (google.apps
+00017050: 2e63 6172 645f 7631 2e74 7970 6573 2e41  .card_v1.types.A
+00017060: 6374 696f 6e29 3a0a 2020 2020 2020 2020  ction):.        
+00017070: 2020 2020 4966 2073 7065 6369 6669 6564      If specified
+00017080: 2c20 616e 2061 6374 696f 6e20 6973 2074  , an action is t
+00017090: 7269 6767 6572 6564 2062 7920 7468 6973  riggered by this
+000170a0: 2060 606f 6e43 6c69 636b 6060 2e0a 0a20   ``onClick``... 
+000170b0: 2020 2020 2020 2020 2020 2054 6869 7320             This 
+000170c0: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
+000170d0: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
+000170e0: 6461 7461 6060 2e0a 2020 2020 2020 2020  data``..        
+000170f0: 6f70 656e 5f6c 696e 6b20 2867 6f6f 676c  open_link (googl
+00017100: 652e 6170 7073 2e63 6172 645f 7631 2e74  e.apps.card_v1.t
+00017110: 7970 6573 2e4f 7065 6e4c 696e 6b29 3a0a  ypes.OpenLink):.
+00017120: 2020 2020 2020 2020 2020 2020 4966 2073              If s
+00017130: 7065 6369 6669 6564 2c20 7468 6973 2060  pecified, this `
+00017140: 606f 6e43 6c69 636b 6060 2074 7269 6767  `onClick`` trigg
+00017150: 6572 7320 616e 206f 7065 6e20 6c69 6e6b  ers an open link
+00017160: 2061 6374 696f 6e2e 0a0a 2020 2020 2020   action...      
+00017170: 2020 2020 2020 5468 6973 2066 6965 6c64        This field
+00017180: 2069 7320 6120 6d65 6d62 6572 206f 6620   is a member of 
+00017190: 606f 6e65 6f66 605f 2060 6064 6174 6160  `oneof`_ ``data`
+000171a0: 602e 0a20 2020 2020 2020 206f 7065 6e5f  `..        open_
+000171b0: 6479 6e61 6d69 635f 6c69 6e6b 5f61 6374  dynamic_link_act
+000171c0: 696f 6e20 2867 6f6f 676c 652e 6170 7073  ion (google.apps
+000171d0: 2e63 6172 645f 7631 2e74 7970 6573 2e41  .card_v1.types.A
+000171e0: 6374 696f 6e29 3a0a 2020 2020 2020 2020  ction):.        
+000171f0: 2020 2020 416e 2061 6464 2d6f 6e20 7472      An add-on tr
+00017200: 6967 6765 7273 2074 6869 7320 6163 7469  iggers this acti
+00017210: 6f6e 2077 6865 6e20 7468 6520 6163 7469  on when the acti
+00017220: 6f6e 206e 6565 6473 2074 6f20 6f70 656e  on needs to open
+00017230: 0a20 2020 2020 2020 2020 2020 2061 206c  .            a l
+00017240: 696e 6b2e 2054 6869 7320 6469 6666 6572  ink. This differ
+00017250: 7320 6672 6f6d 2074 6865 2060 606f 7065  s from the ``ope
+00017260: 6e5f 6c69 6e6b 6060 2061 626f 7665 2069  n_link`` above i
+00017270: 6e20 7468 6174 0a20 2020 2020 2020 2020  n that.         
+00017280: 2020 2074 6869 7320 6e65 6564 7320 746f     this needs to
+00017290: 2074 616c 6b20 746f 2073 6572 7665 7220   talk to server 
+000172a0: 746f 2067 6574 2074 6865 206c 696e 6b2e  to get the link.
+000172b0: 2054 6875 7320 736f 6d65 0a20 2020 2020   Thus some.     
+000172c0: 2020 2020 2020 2070 7265 7061 7261 7469         preparati
+000172d0: 6f6e 2077 6f72 6b20 6973 2072 6571 7569  on work is requi
+000172e0: 7265 6420 666f 7220 7765 6220 636c 6965  red for web clie
+000172f0: 6e74 2074 6f20 646f 2062 6566 6f72 6520  nt to do before 
+00017300: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
+00017310: 6f70 656e 206c 696e 6b20 6163 7469 6f6e  open link action
+00017320: 2072 6573 706f 6e73 6520 636f 6d65 7320   response comes 
+00017330: 6261 636b 2e0a 0a20 2020 2020 2020 2020  back...         
+00017340: 2020 2060 476f 6f67 6c65 2057 6f72 6b73     `Google Works
+00017350: 7061 6365 0a20 2020 2020 2020 2020 2020  pace.           
+00017360: 2041 6464 2d6f 6e73 203c 6874 7470 733a   Add-ons <https:
+00017370: 2f2f 6465 7665 6c6f 7065 7273 2e67 6f6f  //developers.goo
+00017380: 676c 652e 636f 6d2f 776f 726b 7370 6163  gle.com/workspac
+00017390: 652f 6164 642d 6f6e 733e 605f 5f3a 0a0a  e/add-ons>`__:..
+000173a0: 2020 2020 2020 2020 2020 2020 5468 6973              This
+000173b0: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
+000173c0: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
+000173d0: 6064 6174 6160 602e 0a20 2020 2020 2020  `data``..       
+000173e0: 2063 6172 6420 2867 6f6f 676c 652e 6170   card (google.ap
+000173f0: 7073 2e63 6172 645f 7631 2e74 7970 6573  ps.card_v1.types
+00017400: 2e43 6172 6429 3a0a 2020 2020 2020 2020  .Card):.        
+00017410: 2020 2020 4120 6e65 7720 6361 7264 2069      A new card i
+00017420: 7320 7075 7368 6564 2074 6f20 7468 6520  s pushed to the 
+00017430: 6361 7264 2073 7461 636b 2061 6674 6572  card stack after
+00017440: 2063 6c69 636b 696e 6720 6966 0a20 2020   clicking if.   
+00017450: 2020 2020 2020 2020 2073 7065 6369 6669           specifi
+00017460: 6564 2e0a 0a20 2020 2020 2020 2020 2020  ed...           
+00017470: 2060 476f 6f67 6c65 2057 6f72 6b73 7061   `Google Workspa
+00017480: 6365 0a20 2020 2020 2020 2020 2020 2041  ce.            A
+00017490: 6464 2d6f 6e73 203c 6874 7470 733a 2f2f  dd-ons <https://
+000174a0: 6465 7665 6c6f 7065 7273 2e67 6f6f 676c  developers.googl
+000174b0: 652e 636f 6d2f 776f 726b 7370 6163 652f  e.com/workspace/
+000174c0: 6164 642d 6f6e 733e 605f 5f3a 0a0a 2020  add-ons>`__:..  
+000174d0: 2020 2020 2020 2020 2020 5468 6973 2066            This f
+000174e0: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
+000174f0: 206f 6620 606f 6e65 6f66 605f 2060 6064   of `oneof`_ ``d
+00017500: 6174 6160 602e 0a20 2020 2022 2222 0a0a  ata``..    """..
+00017510: 2020 2020 6163 7469 6f6e 3a20 2241 6374      action: "Act
+00017520: 696f 6e22 203d 2070 726f 746f 2e46 6965  ion" = proto.Fie
+00017530: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
+00017540: 6f2e 4d45 5353 4147 452c 0a20 2020 2020  o.MESSAGE,.     
+00017550: 2020 206e 756d 6265 723d 312c 0a20 2020     number=1,.   
+00017560: 2020 2020 206f 6e65 6f66 3d22 6461 7461       oneof="data
+00017570: 222c 0a20 2020 2020 2020 206d 6573 7361  ",.        messa
+00017580: 6765 3d22 4163 7469 6f6e 222c 0a20 2020  ge="Action",.   
+00017590: 2029 0a20 2020 206f 7065 6e5f 6c69 6e6b   ).    open_link
+000175a0: 3a20 224f 7065 6e4c 696e 6b22 203d 2070  : "OpenLink" = p
+000175b0: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
+000175c0: 2020 2020 7072 6f74 6f2e 4d45 5353 4147      proto.MESSAG
+000175d0: 452c 0a20 2020 2020 2020 206e 756d 6265  E,.        numbe
+000175e0: 723d 322c 0a20 2020 2020 2020 206f 6e65  r=2,.        one
+000175f0: 6f66 3d22 6461 7461 222c 0a20 2020 2020  of="data",.     
+00017600: 2020 206d 6573 7361 6765 3d22 4f70 656e     message="Open
+00017610: 4c69 6e6b 222c 0a20 2020 2029 0a20 2020  Link",.    ).   
+00017620: 206f 7065 6e5f 6479 6e61 6d69 635f 6c69   open_dynamic_li
+00017630: 6e6b 5f61 6374 696f 6e3a 2022 4163 7469  nk_action: "Acti
+00017640: 6f6e 2220 3d20 7072 6f74 6f2e 4669 656c  on" = proto.Fiel
+00017650: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
+00017660: 2e4d 4553 5341 4745 2c0a 2020 2020 2020  .MESSAGE,.      
+00017670: 2020 6e75 6d62 6572 3d33 2c0a 2020 2020    number=3,.    
+00017680: 2020 2020 6f6e 656f 663d 2264 6174 6122      oneof="data"
+00017690: 2c0a 2020 2020 2020 2020 6d65 7373 6167  ,.        messag
+000176a0: 653d 2241 6374 696f 6e22 2c0a 2020 2020  e="Action",.    
+000176b0: 290a 2020 2020 6361 7264 3a20 2243 6172  ).    card: "Car
+000176c0: 6422 203d 2070 726f 746f 2e46 6965 6c64  d" = proto.Field
+000176d0: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
+000176e0: 4d45 5353 4147 452c 0a20 2020 2020 2020  MESSAGE,.       
+000176f0: 206e 756d 6265 723d 342c 0a20 2020 2020   number=4,.     
+00017700: 2020 206f 6e65 6f66 3d22 6461 7461 222c     oneof="data",
+00017710: 0a20 2020 2020 2020 206d 6573 7361 6765  .        message
+00017720: 3d22 4361 7264 222c 0a20 2020 2029 0a0a  ="Card",.    )..
+00017730: 0a63 6c61 7373 204f 7065 6e4c 696e 6b28  .class OpenLink(
+00017740: 7072 6f74 6f2e 4d65 7373 6167 6529 3a0a  proto.Message):.
+00017750: 2020 2020 7222 2222 5265 7072 6573 656e      r"""Represen
+00017760: 7473 2061 6e20 6060 6f6e 436c 6963 6b60  ts an ``onClick`
+00017770: 6020 6576 656e 7420 7468 6174 206f 7065  ` event that ope
+00017780: 6e73 2061 2068 7970 6572 6c69 6e6b 2e0a  ns a hyperlink..
+00017790: 0a20 2020 2060 476f 6f67 6c65 2057 6f72  .    `Google Wor
+000177a0: 6b73 7061 6365 2041 6464 2d6f 6e73 2061  kspace Add-ons a
+000177b0: 6e64 2043 6861 740a 2020 2020 6170 7073  nd Chat.    apps
+000177c0: 203c 6874 7470 733a 2f2f 6465 7665 6c6f   <https://develo
+000177d0: 7065 7273 2e67 6f6f 676c 652e 636f 6d2f  pers.google.com/
+000177e0: 776f 726b 7370 6163 652f 6578 7465 6e64  workspace/extend
+000177f0: 3e60 5f5f 3a0a 0a20 2020 2041 7474 7269  >`__:..    Attri
+00017800: 6275 7465 733a 0a20 2020 2020 2020 2075  butes:.        u
+00017810: 726c 2028 7374 7229 3a0a 2020 2020 2020  rl (str):.      
+00017820: 2020 2020 2020 5468 6520 5552 4c20 746f        The URL to
+00017830: 206f 7065 6e2e 0a20 2020 2020 2020 206f   open..        o
+00017840: 7065 6e5f 6173 2028 676f 6f67 6c65 2e61  pen_as (google.a
+00017850: 7070 732e 6361 7264 5f76 312e 7479 7065  pps.card_v1.type
+00017860: 732e 4f70 656e 4c69 6e6b 2e4f 7065 6e41  s.OpenLink.OpenA
+00017870: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+00017880: 486f 7720 746f 206f 7065 6e20 6120 6c69  How to open a li
+00017890: 6e6b 2e0a 0a20 2020 2020 2020 2020 2020  nk...           
+000178a0: 2060 476f 6f67 6c65 2057 6f72 6b73 7061   `Google Workspa
+000178b0: 6365 0a20 2020 2020 2020 2020 2020 2041  ce.            A
+000178c0: 6464 2d6f 6e73 203c 6874 7470 733a 2f2f  dd-ons <https://
+000178d0: 6465 7665 6c6f 7065 7273 2e67 6f6f 676c  developers.googl
+000178e0: 652e 636f 6d2f 776f 726b 7370 6163 652f  e.com/workspace/
+000178f0: 6164 642d 6f6e 733e 605f 5f3a 0a20 2020  add-ons>`__:.   
+00017900: 2020 2020 206f 6e5f 636c 6f73 6520 2867       on_close (g
+00017910: 6f6f 676c 652e 6170 7073 2e63 6172 645f  oogle.apps.card_
+00017920: 7631 2e74 7970 6573 2e4f 7065 6e4c 696e  v1.types.OpenLin
+00017930: 6b2e 4f6e 436c 6f73 6529 3a0a 2020 2020  k.OnClose):.    
+00017940: 2020 2020 2020 2020 5768 6574 6865 7220          Whether 
+00017950: 7468 6520 636c 6965 6e74 2066 6f72 6765  the client forge
+00017960: 7473 2061 626f 7574 2061 206c 696e 6b20  ts about a link 
+00017970: 6166 7465 7220 6f70 656e 696e 6720 6974  after opening it
+00017980: 2c20 6f72 0a20 2020 2020 2020 2020 2020  , or.           
+00017990: 206f 6273 6572 7665 7320 6974 2075 6e74   observes it unt
+000179a0: 696c 2074 6865 2077 696e 646f 7720 636c  il the window cl
+000179b0: 6f73 6573 2e0a 0a20 2020 2020 2020 2020  oses...         
+000179c0: 2020 2060 476f 6f67 6c65 2057 6f72 6b73     `Google Works
+000179d0: 7061 6365 0a20 2020 2020 2020 2020 2020  pace.           
+000179e0: 2041 6464 2d6f 6e73 203c 6874 7470 733a   Add-ons <https:
+000179f0: 2f2f 6465 7665 6c6f 7065 7273 2e67 6f6f  //developers.goo
+00017a00: 676c 652e 636f 6d2f 776f 726b 7370 6163  gle.com/workspac
+00017a10: 652f 6164 642d 6f6e 733e 605f 5f3a 0a20  e/add-ons>`__:. 
+00017a20: 2020 2022 2222 0a0a 2020 2020 636c 6173     """..    clas
+00017a30: 7320 4f70 656e 4173 2870 726f 746f 2e45  s OpenAs(proto.E
+00017a40: 6e75 6d29 3a0a 2020 2020 2020 2020 7222  num):.        r"
+00017a50: 2222 5768 656e 2061 6e20 6060 4f6e 436c  ""When an ``OnCl
+00017a60: 6963 6b60 6020 6163 7469 6f6e 206f 7065  ick`` action ope
+00017a70: 6e73 2061 206c 696e 6b2c 2074 6865 6e20  ns a link, then 
+00017a80: 7468 6520 636c 6965 6e74 2063 616e 2065  the client can e
+00017a90: 6974 6865 720a 2020 2020 2020 2020 6f70  ither.        op
+00017aa0: 656e 2069 7420 6173 2061 2066 756c 6c2d  en it as a full-
+00017ab0: 7369 7a65 2077 696e 646f 7720 2869 6620  size window (if 
+00017ac0: 7468 6174 2773 2074 6865 2066 7261 6d65  that's the frame
+00017ad0: 2075 7365 6420 6279 2074 6865 0a20 2020   used by the.   
+00017ae0: 2020 2020 2063 6c69 656e 7429 2c20 6f72       client), or
+00017af0: 2061 6e20 6f76 6572 6c61 7920 2873 7563   an overlay (suc
+00017b00: 6820 6173 2061 2070 6f70 2d75 7029 2e20  h as a pop-up). 
+00017b10: 5468 6520 696d 706c 656d 656e 7461 7469  The implementati
+00017b20: 6f6e 0a20 2020 2020 2020 2064 6570 656e  on.        depen
+00017b30: 6473 206f 6e20 7468 6520 636c 6965 6e74  ds on the client
+00017b40: 2070 6c61 7466 6f72 6d20 6361 7061 6269   platform capabi
+00017b50: 6c69 7469 6573 2c20 616e 6420 7468 6520  lities, and the 
+00017b60: 7661 6c75 6520 7365 6c65 6374 6564 0a20  value selected. 
+00017b70: 2020 2020 2020 206d 6967 6874 2062 6520         might be 
+00017b80: 6967 6e6f 7265 6420 6966 2074 6865 2063  ignored if the c
+00017b90: 6c69 656e 7420 646f 6573 6e27 7420 7375  lient doesn't su
+00017ba0: 7070 6f72 7420 6974 2e20 6060 4655 4c4c  pport it. ``FULL
+00017bb0: 5f53 495a 4560 6020 6973 0a20 2020 2020  _SIZE`` is.     
+00017bc0: 2020 2073 7570 706f 7274 6564 2062 7920     supported by 
+00017bd0: 616c 6c20 636c 6965 6e74 732e 0a0a 2020  all clients...  
+00017be0: 2020 2020 2020 6047 6f6f 676c 6520 576f        `Google Wo
+00017bf0: 726b 7370 6163 650a 2020 2020 2020 2020  rkspace.        
+00017c00: 4164 642d 6f6e 7320 3c68 7474 7073 3a2f  Add-ons <https:/
+00017c10: 2f64 6576 656c 6f70 6572 732e 676f 6f67  /developers.goog
+00017c20: 6c65 2e63 6f6d 2f77 6f72 6b73 7061 6365  le.com/workspace
+00017c30: 2f61 6464 2d6f 6e73 3e60 5f5f 3a0a 0a20  /add-ons>`__:.. 
+00017c40: 2020 2020 2020 2056 616c 7565 733a 0a20         Values:. 
+00017c50: 2020 2020 2020 2020 2020 2046 554c 4c5f             FULL_
+00017c60: 5349 5a45 2028 3029 3a0a 2020 2020 2020  SIZE (0):.      
+00017c70: 2020 2020 2020 2020 2020 5468 6520 6c69            The li
+00017c80: 6e6b 206f 7065 6e73 2061 7320 6120 6675  nk opens as a fu
+00017c90: 6c6c 2d73 697a 6520 7769 6e64 6f77 2028  ll-size window (
+00017ca0: 6966 0a20 2020 2020 2020 2020 2020 2020  if.             
+00017cb0: 2020 2074 6861 7427 7320 7468 6520 6672     that's the fr
+00017cc0: 616d 6520 7573 6564 2062 7920 7468 6520  ame used by the 
+00017cd0: 636c 6965 6e74 292e 0a20 2020 2020 2020  client)..       
+00017ce0: 2020 2020 204f 5645 524c 4159 2028 3129       OVERLAY (1)
+00017cf0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00017d00: 2020 5468 6520 6c69 6e6b 206f 7065 6e73    The link opens
+00017d10: 2061 7320 616e 206f 7665 726c 6179 2c20   as an overlay, 
+00017d20: 7375 6368 2061 7320 610a 2020 2020 2020  such as a.      
+00017d30: 2020 2020 2020 2020 2020 706f 702d 7570            pop-up
+00017d40: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00017d50: 2020 2020 2020 4655 4c4c 5f53 495a 4520        FULL_SIZE 
+00017d60: 3d20 300a 2020 2020 2020 2020 4f56 4552  = 0.        OVER
+00017d70: 4c41 5920 3d20 310a 0a20 2020 2063 6c61  LAY = 1..    cla
+00017d80: 7373 204f 6e43 6c6f 7365 2870 726f 746f  ss OnClose(proto
+00017d90: 2e45 6e75 6d29 3a0a 2020 2020 2020 2020  .Enum):.        
+00017da0: 7222 2222 5768 6174 2074 6865 2063 6c69  r"""What the cli
+00017db0: 656e 7420 646f 6573 2077 6865 6e20 6120  ent does when a 
+00017dc0: 6c69 6e6b 206f 7065 6e65 6420 6279 2061  link opened by a
+00017dd0: 6e20 6060 4f6e 436c 6963 6b60 6020 6163  n ``OnClick`` ac
+00017de0: 7469 6f6e 2069 730a 2020 2020 2020 2020  tion is.        
+00017df0: 636c 6f73 6564 2e0a 0a20 2020 2020 2020  closed...       
+00017e00: 2049 6d70 6c65 6d65 6e74 6174 696f 6e20   Implementation 
+00017e10: 6465 7065 6e64 7320 6f6e 2063 6c69 656e  depends on clien
+00017e20: 7420 706c 6174 666f 726d 2063 6170 6162  t platform capab
+00017e30: 696c 6974 6965 732e 2046 6f72 2065 7861  ilities. For exa
+00017e40: 6d70 6c65 2c0a 2020 2020 2020 2020 6120  mple,.        a 
+00017e50: 7765 6220 6272 6f77 7365 7220 6d69 6768  web browser migh
+00017e60: 7420 6f70 656e 2061 206c 696e 6b20 696e  t open a link in
+00017e70: 2061 2070 6f70 2d75 7020 7769 6e64 6f77   a pop-up window
+00017e80: 2077 6974 6820 616e 0a20 2020 2020 2020   with an.       
+00017e90: 2060 604f 6e43 6c6f 7365 6060 2068 616e   ``OnClose`` han
+00017ea0: 646c 6572 2e0a 0a20 2020 2020 2020 2049  dler...        I
+00017eb0: 6620 626f 7468 2060 604f 6e4f 7065 6e60  f both ``OnOpen`
+00017ec0: 6020 616e 6420 6060 4f6e 436c 6f73 6560  ` and ``OnClose`
+00017ed0: 6020 6861 6e64 6c65 7273 2061 7265 2073  ` handlers are s
+00017ee0: 6574 2c20 616e 6420 7468 6520 636c 6965  et, and the clie
+00017ef0: 6e74 0a20 2020 2020 2020 2070 6c61 7466  nt.        platf
+00017f00: 6f72 6d20 6361 6e27 7420 7375 7070 6f72  orm can't suppor
+00017f10: 7420 626f 7468 2076 616c 7565 732c 2060  t both values, `
+00017f20: 604f 6e43 6c6f 7365 6060 2074 616b 6573  `OnClose`` takes
+00017f30: 2070 7265 6365 6465 6e63 652e 0a0a 2020   precedence...  
+00017f40: 2020 2020 2020 6047 6f6f 676c 6520 576f        `Google Wo
+00017f50: 726b 7370 6163 650a 2020 2020 2020 2020  rkspace.        
+00017f60: 4164 642d 6f6e 7320 3c68 7474 7073 3a2f  Add-ons <https:/
+00017f70: 2f64 6576 656c 6f70 6572 732e 676f 6f67  /developers.goog
+00017f80: 6c65 2e63 6f6d 2f77 6f72 6b73 7061 6365  le.com/workspace
+00017f90: 2f61 6464 2d6f 6e73 3e60 5f5f 3a0a 0a20  /add-ons>`__:.. 
+00017fa0: 2020 2020 2020 2056 616c 7565 733a 0a20         Values:. 
+00017fb0: 2020 2020 2020 2020 2020 204e 4f54 4849             NOTHI
+00017fc0: 4e47 2028 3029 3a0a 2020 2020 2020 2020  NG (0):.        
+00017fd0: 2020 2020 2020 2020 4465 6661 756c 7420          Default 
+00017fe0: 7661 6c75 652e 2054 6865 2063 6172 6420  value. The card 
+00017ff0: 646f 6573 6e27 7420 7265 6c6f 6164 3b0a  doesn't reload;.
+00018000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018010: 6e6f 7468 696e 6720 6861 7070 656e 732e  nothing happens.
+00018020: 0a20 2020 2020 2020 2020 2020 2052 454c  .            REL
+00018030: 4f41 4420 2831 293a 0a20 2020 2020 2020  OAD (1):.       
+00018040: 2020 2020 2020 2020 2052 656c 6f61 6473           Reloads
+00018050: 2074 6865 2063 6172 6420 6166 7465 7220   the card after 
+00018060: 7468 6520 6368 696c 6420 7769 6e64 6f77  the child window
+00018070: 2063 6c6f 7365 732e 0a0a 2020 2020 2020   closes...      
+00018080: 2020 2020 2020 2020 2020 4966 2075 7365            If use
+00018090: 6420 696e 2063 6f6e 6a75 6e63 7469 6f6e  d in conjunction
+000180a0: 2077 6974 680a 2020 2020 2020 2020 2020   with.          
+000180b0: 2020 2020 2020 6060 604f 7065 6e41 732e        ```OpenAs.
+000180c0: 4f56 4552 4c41 5960 6020 3c68 7474 7073  OVERLAY`` <https
+000180d0: 3a2f 2f64 6576 656c 6f70 6572 732e 676f  ://developers.go
+000180e0: 6f67 6c65 2e63 6f6d 2f77 6f72 6b73 7061  ogle.com/workspa
+000180f0: 6365 2f61 6464 2d6f 6e73 2f72 6566 6572  ce/add-ons/refer
+00018100: 656e 6365 2f72 7063 2f67 6f6f 676c 652e  ence/rpc/google.
+00018110: 6170 7073 2e63 6172 642e 7631 236f 7065  apps.card.v1#ope
+00018120: 6e61 733e 605f 5f2c 0a20 2020 2020 2020  nas>`__,.       
+00018130: 2020 2020 2020 2020 2074 6865 2063 6869           the chi
+00018140: 6c64 2077 696e 646f 7720 6163 7473 2061  ld window acts a
+00018150: 7320 6120 6d6f 6461 6c20 6469 616c 6f67  s a modal dialog
+00018160: 2061 6e64 2074 6865 2070 6172 656e 7420   and the parent 
+00018170: 6361 7264 0a20 2020 2020 2020 2020 2020  card.           
+00018180: 2020 2020 2069 7320 626c 6f63 6b65 6420       is blocked 
+00018190: 756e 7469 6c20 7468 6520 6368 696c 6420  until the child 
+000181a0: 7769 6e64 6f77 2063 6c6f 7365 732e 0a20  window closes.. 
+000181b0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000181c0: 2020 204e 4f54 4849 4e47 203d 2030 0a20     NOTHING = 0. 
+000181d0: 2020 2020 2020 2052 454c 4f41 4420 3d20         RELOAD = 
+000181e0: 310a 0a20 2020 2075 726c 3a20 7374 7220  1..    url: str 
+000181f0: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
+00018200: 2020 2020 2020 2070 726f 746f 2e53 5452         proto.STR
+00018210: 494e 472c 0a20 2020 2020 2020 206e 756d  ING,.        num
+00018220: 6265 723d 312c 0a20 2020 2029 0a20 2020  ber=1,.    ).   
+00018230: 206f 7065 6e5f 6173 3a20 4f70 656e 4173   open_as: OpenAs
+00018240: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
+00018250: 2020 2020 2020 2020 7072 6f74 6f2e 454e          proto.EN
+00018260: 554d 2c0a 2020 2020 2020 2020 6e75 6d62  UM,.        numb
+00018270: 6572 3d32 2c0a 2020 2020 2020 2020 656e  er=2,.        en
+00018280: 756d 3d4f 7065 6e41 732c 0a20 2020 2029  um=OpenAs,.    )
+00018290: 0a20 2020 206f 6e5f 636c 6f73 653a 204f  .    on_close: O
+000182a0: 6e43 6c6f 7365 203d 2070 726f 746f 2e46  nClose = proto.F
+000182b0: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
+000182c0: 6f74 6f2e 454e 554d 2c0a 2020 2020 2020  oto.ENUM,.      
+000182d0: 2020 6e75 6d62 6572 3d33 2c0a 2020 2020    number=3,.    
+000182e0: 2020 2020 656e 756d 3d4f 6e43 6c6f 7365      enum=OnClose
+000182f0: 2c0a 2020 2020 290a 0a0a 636c 6173 7320  ,.    )...class 
+00018300: 4163 7469 6f6e 2870 726f 746f 2e4d 6573  Action(proto.Mes
+00018310: 7361 6765 293a 0a20 2020 2072 2222 2241  sage):.    r"""A
+00018320: 6e20 6163 7469 6f6e 2074 6861 7420 6465  n action that de
+00018330: 7363 7269 6265 7320 7468 6520 6265 6861  scribes the beha
+00018340: 7669 6f72 2077 6865 6e20 7468 6520 666f  vior when the fo
+00018350: 726d 2069 7320 7375 626d 6974 7465 642e  rm is submitted.
+00018360: 0a20 2020 2046 6f72 2065 7861 6d70 6c65  .    For example
+00018370: 2c20 796f 7520 6361 6e20 696e 766f 6b65  , you can invoke
+00018380: 2061 6e20 4170 7073 2053 6372 6970 7420   an Apps Script 
+00018390: 7363 7269 7074 2074 6f20 6861 6e64 6c65  script to handle
+000183a0: 2074 6865 0a20 2020 2066 6f72 6d2e 2049   the.    form. I
+000183b0: 6620 7468 6520 6163 7469 6f6e 2069 7320  f the action is 
+000183c0: 7472 6967 6765 7265 642c 2074 6865 2066  triggered, the f
+000183d0: 6f72 6d20 7661 6c75 6573 2061 7265 2073  orm values are s
+000183e0: 656e 7420 746f 2074 6865 0a20 2020 2073  ent to the.    s
+000183f0: 6572 7665 722e 0a0a 2020 2020 6047 6f6f  erver...    `Goo
+00018400: 676c 6520 576f 726b 7370 6163 6520 4164  gle Workspace Ad
+00018410: 642d 6f6e 7320 616e 6420 4368 6174 0a20  d-ons and Chat. 
+00018420: 2020 2061 7070 7320 3c68 7474 7073 3a2f     apps <https:/
+00018430: 2f64 6576 656c 6f70 6572 732e 676f 6f67  /developers.goog
+00018440: 6c65 2e63 6f6d 2f77 6f72 6b73 7061 6365  le.com/workspace
+00018450: 2f65 7874 656e 643e 605f 5f3a 0a0a 2020  /extend>`__:..  
+00018460: 2020 4174 7472 6962 7574 6573 3a0a 2020    Attributes:.  
+00018470: 2020 2020 2020 6675 6e63 7469 6f6e 2028        function (
+00018480: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
+00018490: 2020 4120 6375 7374 6f6d 2066 756e 6374    A custom funct
+000184a0: 696f 6e20 746f 2069 6e76 6f6b 6520 7768  ion to invoke wh
+000184b0: 656e 2074 6865 2063 6f6e 7461 696e 696e  en the containin
+000184c0: 6720 656c 656d 656e 7420 6973 0a20 2020  g element is.   
+000184d0: 2020 2020 2020 2020 2063 6c69 636b 6564           clicked
+000184e0: 206f 7220 6f74 6872 7769 7365 2061 6374   or othrwise act
+000184f0: 6976 6174 6564 2e0a 0a20 2020 2020 2020  ivated...       
+00018500: 2020 2020 2046 6f72 2065 7861 6d70 6c65       For example
+00018510: 2075 7361 6765 2c20 7365 6520 6052 6561   usage, see `Rea
+00018520: 6420 666f 726d 0a20 2020 2020 2020 2020  d form.         
+00018530: 2020 2064 6174 6120 3c68 7474 7073 3a2f     data <https:/
+00018540: 2f64 6576 656c 6f70 6572 732e 676f 6f67  /developers.goog
+00018550: 6c65 2e63 6f6d 2f77 6f72 6b73 7061 6365  le.com/workspace
+00018560: 2f63 6861 742f 7265 6164 2d66 6f72 6d2d  /chat/read-form-
+00018570: 6461 7461 3e60 5f5f 2e0a 2020 2020 2020  data>`__..      
+00018580: 2020 7061 7261 6d65 7465 7273 2028 4d75    parameters (Mu
+00018590: 7461 626c 6553 6571 7565 6e63 655b 676f  tableSequence[go
+000185a0: 6f67 6c65 2e61 7070 732e 6361 7264 5f76  ogle.apps.card_v
+000185b0: 312e 7479 7065 732e 4163 7469 6f6e 2e41  1.types.Action.A
+000185c0: 6374 696f 6e50 6172 616d 6574 6572 5d29  ctionParameter])
+000185d0: 3a0a 2020 2020 2020 2020 2020 2020 4c69  :.            Li
+000185e0: 7374 206f 6620 6163 7469 6f6e 2070 6172  st of action par
+000185f0: 616d 6574 6572 732e 0a20 2020 2020 2020  ameters..       
+00018600: 206c 6f61 645f 696e 6469 6361 746f 7220   load_indicator 
+00018610: 2867 6f6f 676c 652e 6170 7073 2e63 6172  (google.apps.car
+00018620: 645f 7631 2e74 7970 6573 2e41 6374 696f  d_v1.types.Actio
+00018630: 6e2e 4c6f 6164 496e 6469 6361 746f 7229  n.LoadIndicator)
+00018640: 3a0a 2020 2020 2020 2020 2020 2020 5370  :.            Sp
+00018650: 6563 6966 6965 7320 7468 6520 6c6f 6164  ecifies the load
+00018660: 696e 6720 696e 6469 6361 746f 7220 7468  ing indicator th
+00018670: 6174 2074 6865 0a20 2020 2020 2020 2020  at the.         
+00018680: 2020 2061 6374 696f 6e20 6469 7370 6c61     action displa
+00018690: 7973 2077 6869 6c65 206d 616b 696e 6720  ys while making 
+000186a0: 7468 6520 6361 6c6c 2074 6f20 7468 650a  the call to the.
+000186b0: 2020 2020 2020 2020 2020 2020 6163 7469              acti
+000186c0: 6f6e 2e0a 2020 2020 2020 2020 7065 7273  on..        pers
+000186d0: 6973 745f 7661 6c75 6573 2028 626f 6f6c  ist_values (bool
+000186e0: 293a 0a20 2020 2020 2020 2020 2020 2049  ):.            I
+000186f0: 6e64 6963 6174 6573 2077 6865 7468 6572  ndicates whether
+00018700: 2066 6f72 6d20 7661 6c75 6573 2070 6572   form values per
+00018710: 7369 7374 2061 6674 6572 2074 6865 2061  sist after the a
+00018720: 6374 696f 6e2e 2054 6865 0a20 2020 2020  ction. The.     
+00018730: 2020 2020 2020 2064 6566 6175 6c74 2076         default v
+00018740: 616c 7565 2069 7320 6060 6661 6c73 6560  alue is ``false`
+00018750: 602e 0a0a 2020 2020 2020 2020 2020 2020  `...            
+00018760: 4966 2060 6074 7275 6560 602c 2066 6f72  If ``true``, for
+00018770: 6d20 7661 6c75 6573 2072 656d 6169 6e20  m values remain 
+00018780: 6166 7465 7220 7468 6520 6163 7469 6f6e  after the action
+00018790: 2069 730a 2020 2020 2020 2020 2020 2020   is.            
+000187a0: 7472 6967 6765 7265 642e 2054 6f20 6c65  triggered. To le
+000187b0: 7420 7468 6520 7573 6572 206d 616b 6520  t the user make 
+000187c0: 6368 616e 6765 7320 7768 696c 6520 7468  changes while th
+000187d0: 6520 6163 7469 6f6e 2069 730a 2020 2020  e action is.    
+000187e0: 2020 2020 2020 2020 6265 696e 6720 7072          being pr
+000187f0: 6f63 6573 7365 642c 2073 6574 0a20 2020  ocessed, set.   
+00018800: 2020 2020 2020 2020 2060 6060 4c6f 6164           ```Load
+00018810: 496e 6469 6361 746f 7260 6020 3c68 7474  Indicator`` <htt
+00018820: 7073 3a2f 2f64 6576 656c 6f70 6572 732e  ps://developers.
+00018830: 676f 6f67 6c65 2e63 6f6d 2f77 6f72 6b73  google.com/works
+00018840: 7061 6365 2f61 6464 2d6f 6e73 2f72 6566  pace/add-ons/ref
+00018850: 6572 656e 6365 2f72 7063 2f67 6f6f 676c  erence/rpc/googl
+00018860: 652e 6170 7073 2e63 6172 642e 7631 236c  e.apps.card.v1#l
+00018870: 6f61 6469 6e64 6963 6174 6f72 3e60 5f5f  oadindicator>`__
+00018880: 0a20 2020 2020 2020 2020 2020 2074 6f20  .            to 
+00018890: 6060 4e4f 4e45 6060 2e20 466f 7220 6063  ``NONE``. For `c
+000188a0: 6172 640a 2020 2020 2020 2020 2020 2020  ard.            
+000188b0: 6d65 7373 6167 6573 203c 6874 7470 733a  messages <https:
+000188c0: 2f2f 6465 7665 6c6f 7065 7273 2e67 6f6f  //developers.goo
+000188d0: 676c 652e 636f 6d2f 776f 726b 7370 6163  gle.com/workspac
+000188e0: 652f 6368 6174 2f61 7069 2f67 7569 6465  e/chat/api/guide
+000188f0: 732f 7631 2f6d 6573 7361 6765 732f 6372  s/v1/messages/cr
+00018900: 6561 7465 2363 7265 6174 653e 605f 5f0a  eate#create>`__.
+00018910: 2020 2020 2020 2020 2020 2020 696e 2043              in C
+00018920: 6861 7420 6170 7073 2c20 796f 7520 6d75  hat apps, you mu
+00018930: 7374 2061 6c73 6f20 7365 7420 7468 6520  st also set the 
+00018940: 6163 7469 6f6e 2773 0a20 2020 2020 2020  action's.       
+00018950: 2020 2020 2060 6060 5265 7370 6f6e 7365       ```Response
+00018960: 5479 7065 6060 203c 6874 7470 733a 2f2f  Type`` <https://
+00018970: 6465 7665 6c6f 7065 7273 2e67 6f6f 676c  developers.googl
+00018980: 652e 636f 6d2f 776f 726b 7370 6163 652f  e.com/workspace/
+00018990: 6368 6174 2f61 7069 2f72 6566 6572 656e  chat/api/referen
+000189a0: 6365 2f72 6573 742f 7631 2f73 7061 6365  ce/rest/v1/space
+000189b0: 732e 6d65 7373 6167 6573 2372 6573 706f  s.messages#respo
+000189c0: 6e73 6574 7970 653e 605f 5f0a 2020 2020  nsetype>`__.    
+000189d0: 2020 2020 2020 2020 746f 2060 6055 5044          to ``UPD
+000189e0: 4154 455f 4d45 5353 4147 4560 6020 616e  ATE_MESSAGE`` an
+000189f0: 6420 7573 6520 7468 6520 7361 6d65 0a20  d use the same. 
+00018a00: 2020 2020 2020 2020 2020 2060 6060 6361             ```ca
+00018a10: 7264 5f69 6460 6020 3c68 7474 7073 3a2f  rd_id`` <https:/
+00018a20: 2f64 6576 656c 6f70 6572 732e 676f 6f67  /developers.goog
+00018a30: 6c65 2e63 6f6d 2f77 6f72 6b73 7061 6365  le.com/workspace
+00018a40: 2f63 6861 742f 6170 692f 7265 6665 7265  /chat/api/refere
+00018a50: 6e63 652f 7265 7374 2f76 312f 7370 6163  nce/rest/v1/spac
+00018a60: 6573 2e6d 6573 7361 6765 7323 4361 7264  es.messages#Card
+00018a70: 5769 7468 4964 3e60 5f5f 0a20 2020 2020  WithId>`__.     
+00018a80: 2020 2020 2020 2066 726f 6d20 7468 6520         from the 
+00018a90: 6361 7264 2074 6861 7420 636f 6e74 6169  card that contai
+00018aa0: 6e65 6420 7468 6520 6163 7469 6f6e 2e0a  ned the action..
+00018ab0: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
+00018ac0: 6060 6661 6c73 6560 602c 2074 6865 2066  ``false``, the f
+00018ad0: 6f72 6d20 7661 6c75 6573 2061 7265 2063  orm values are c
+00018ae0: 6c65 6172 6564 2077 6865 6e20 7468 6520  leared when the 
+00018af0: 6163 7469 6f6e 2069 730a 2020 2020 2020  action is.      
+00018b00: 2020 2020 2020 7472 6967 6765 7265 642e        triggered.
+00018b10: 2054 6f20 7072 6576 656e 7420 7468 6520   To prevent the 
+00018b20: 7573 6572 2066 726f 6d20 6d61 6b69 6e67  user from making
+00018b30: 2063 6861 6e67 6573 2077 6869 6c65 2074   changes while t
+00018b40: 6865 0a20 2020 2020 2020 2020 2020 2061  he.            a
+00018b50: 6374 696f 6e20 6973 2062 6569 6e67 2070  ction is being p
+00018b60: 726f 6365 7373 6564 2c20 7365 740a 2020  rocessed, set.  
+00018b70: 2020 2020 2020 2020 2020 6060 604c 6f61            ```Loa
+00018b80: 6449 6e64 6963 6174 6f72 6060 203c 6874  dIndicator`` <ht
+00018b90: 7470 733a 2f2f 6465 7665 6c6f 7065 7273  tps://developers
+00018ba0: 2e67 6f6f 676c 652e 636f 6d2f 776f 726b  .google.com/work
+00018bb0: 7370 6163 652f 6164 642d 6f6e 732f 7265  space/add-ons/re
+00018bc0: 6665 7265 6e63 652f 7270 632f 676f 6f67  ference/rpc/goog
+00018bd0: 6c65 2e61 7070 732e 6361 7264 2e76 3123  le.apps.card.v1#
+00018be0: 6c6f 6164 696e 6469 6361 746f 723e 605f  loadindicator>`_
+00018bf0: 5f0a 2020 2020 2020 2020 2020 2020 746f  _.            to
+00018c00: 2060 6053 5049 4e4e 4552 6060 2e0a 2020   ``SPINNER``..  
+00018c10: 2020 2020 2020 696e 7465 7261 6374 696f        interactio
+00018c20: 6e20 2867 6f6f 676c 652e 6170 7073 2e63  n (google.apps.c
+00018c30: 6172 645f 7631 2e74 7970 6573 2e41 6374  ard_v1.types.Act
+00018c40: 696f 6e2e 496e 7465 7261 6374 696f 6e29  ion.Interaction)
+00018c50: 3a0a 2020 2020 2020 2020 2020 2020 4f70  :.            Op
+00018c60: 7469 6f6e 616c 2e20 5265 7175 6972 6564  tional. Required
+00018c70: 2077 6865 6e20 6f70 656e 696e 6720 610a   when opening a.
+00018c80: 2020 2020 2020 2020 2020 2020 6064 6961              `dia
+00018c90: 6c6f 6720 3c68 7474 7073 3a2f 2f64 6576  log <https://dev
+00018ca0: 656c 6f70 6572 732e 676f 6f67 6c65 2e63  elopers.google.c
+00018cb0: 6f6d 2f77 6f72 6b73 7061 6365 2f63 6861  om/workspace/cha
+00018cc0: 742f 6469 616c 6f67 733e 605f 5f2e 0a0a  t/dialogs>`__...
+00018cd0: 2020 2020 2020 2020 2020 2020 5768 6174              What
+00018ce0: 2074 6f20 646f 2069 6e20 7265 7370 6f6e   to do in respon
+00018cf0: 7365 2074 6f20 616e 2069 6e74 6572 6163  se to an interac
+00018d00: 7469 6f6e 2077 6974 6820 6120 7573 6572  tion with a user
+00018d10: 2c20 7375 6368 0a20 2020 2020 2020 2020  , such.         
+00018d20: 2020 2061 7320 6120 7573 6572 2063 6c69     as a user cli
+00018d30: 636b 696e 6720 6120 6275 7474 6f6e 2069  cking a button i
+00018d40: 6e20 6120 6361 7264 206d 6573 7361 6765  n a card message
+00018d50: 2e0a 0a20 2020 2020 2020 2020 2020 2049  ...            I
+00018d60: 6620 756e 7370 6563 6966 6965 642c 2074  f unspecified, t
+00018d70: 6865 2061 7070 2072 6573 706f 6e64 7320  he app responds 
+00018d80: 6279 2065 7865 6375 7469 6e67 2061 6e0a  by executing an.
+00018d90: 2020 2020 2020 2020 2020 2020 6060 6163              ``ac
+00018da0: 7469 6f6e 6060 e280 946c 696b 6520 6f70  tion``...like op
+00018db0: 656e 696e 6720 6120 6c69 6e6b 206f 7220  ening a link or 
+00018dc0: 7275 6e6e 696e 6720 6120 6675 6e63 7469  running a functi
+00018dd0: 6f6e e280 9461 730a 2020 2020 2020 2020  on...as.        
+00018de0: 2020 2020 6e6f 726d 616c 2e0a 0a20 2020      normal...   
+00018df0: 2020 2020 2020 2020 2042 7920 7370 6563           By spec
+00018e00: 6966 7969 6e67 2061 6e20 6060 696e 7465  ifying an ``inte
+00018e10: 7261 6374 696f 6e60 602c 2074 6865 2061  raction``, the a
+00018e20: 7070 2063 616e 2072 6573 706f 6e64 2069  pp can respond i
+00018e30: 6e0a 2020 2020 2020 2020 2020 2020 7370  n.            sp
+00018e40: 6563 6961 6c20 696e 7465 7261 6374 6976  ecial interactiv
+00018e50: 6520 7761 7973 2e20 466f 7220 6578 616d  e ways. For exam
+00018e60: 706c 652c 2062 7920 7365 7474 696e 670a  ple, by setting.
+00018e70: 2020 2020 2020 2020 2020 2020 6060 696e              ``in
+00018e80: 7465 7261 6374 696f 6e60 6020 746f 2060  teraction`` to `
+00018e90: 604f 5045 4e5f 4449 414c 4f47 6060 2c20  `OPEN_DIALOG``, 
+00018ea0: 7468 6520 6170 7020 6361 6e20 6f70 656e  the app can open
+00018eb0: 2061 0a20 2020 2020 2020 2020 2020 2060   a.            `
+00018ec0: 6469 616c 6f67 203c 6874 7470 733a 2f2f  dialog <https://
+00018ed0: 6465 7665 6c6f 7065 7273 2e67 6f6f 676c  developers.googl
+00018ee0: 652e 636f 6d2f 776f 726b 7370 6163 652f  e.com/workspace/
+00018ef0: 6368 6174 2f64 6961 6c6f 6773 3e60 5f5f  chat/dialogs>`__
+00018f00: 2e0a 2020 2020 2020 2020 2020 2020 5768  ..            Wh
+00018f10: 656e 2073 7065 6369 6669 6564 2c20 6120  en specified, a 
+00018f20: 6c6f 6164 696e 6720 696e 6469 6361 746f  loading indicato
+00018f30: 7220 6973 6e27 7420 7368 6f77 6e2e 2049  r isn't shown. I
+00018f40: 660a 2020 2020 2020 2020 2020 2020 7370  f.            sp
+00018f50: 6563 6966 6965 6420 666f 7220 616e 2061  ecified for an a
+00018f60: 6464 2d6f 6e2c 2074 6865 2065 6e74 6972  dd-on, the entir
+00018f70: 6520 6361 7264 2069 7320 7374 7269 7070  e card is stripp
+00018f80: 6564 2061 6e64 0a20 2020 2020 2020 2020  ed and.         
+00018f90: 2020 206e 6f74 6869 6e67 2069 7320 7368     nothing is sh
+00018fa0: 6f77 6e20 696e 2074 6865 2063 6c69 656e  own in the clien
+00018fb0: 742e 0a0a 2020 2020 2020 2020 2020 2020  t...            
+00018fc0: 6047 6f6f 676c 6520 4368 6174 0a20 2020  `Google Chat.   
+00018fd0: 2020 2020 2020 2020 2061 7070 7320 3c68           apps <h
+00018fe0: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
+00018ff0: 732e 676f 6f67 6c65 2e63 6f6d 2f77 6f72  s.google.com/wor
+00019000: 6b73 7061 6365 2f63 6861 743e 605f 5f3a  kspace/chat>`__:
+00019010: 0a20 2020 2022 2222 0a0a 2020 2020 636c  .    """..    cl
+00019020: 6173 7320 4c6f 6164 496e 6469 6361 746f  ass LoadIndicato
+00019030: 7228 7072 6f74 6f2e 456e 756d 293a 0a20  r(proto.Enum):. 
+00019040: 2020 2020 2020 2072 2222 2253 7065 6369         r"""Speci
+00019050: 6669 6573 2074 6865 206c 6f61 6469 6e67  fies the loading
+00019060: 2069 6e64 6963 6174 6f72 2074 6861 7420   indicator that 
+00019070: 7468 6520 6163 7469 6f6e 2064 6973 706c  the action displ
+00019080: 6179 7320 7768 696c 650a 2020 2020 2020  ays while.      
+00019090: 2020 6d61 6b69 6e67 2074 6865 2063 616c    making the cal
+000190a0: 6c20 746f 2074 6865 2061 6374 696f 6e2e  l to the action.
+000190b0: 0a0a 2020 2020 2020 2020 6047 6f6f 676c  ..        `Googl
+000190c0: 6520 576f 726b 7370 6163 6520 4164 642d  e Workspace Add-
+000190d0: 6f6e 7320 616e 6420 4368 6174 0a20 2020  ons and Chat.   
+000190e0: 2020 2020 2061 7070 7320 3c68 7474 7073       apps <https
+000190f0: 3a2f 2f64 6576 656c 6f70 6572 732e 676f  ://developers.go
+00019100: 6f67 6c65 2e63 6f6d 2f77 6f72 6b73 7061  ogle.com/workspa
+00019110: 6365 2f65 7874 656e 643e 605f 5f3a 0a0a  ce/extend>`__:..
+00019120: 2020 2020 2020 2020 5661 6c75 6573 3a0a          Values:.
+00019130: 2020 2020 2020 2020 2020 2020 5350 494e              SPIN
+00019140: 4e45 5220 2830 293a 0a20 2020 2020 2020  NER (0):.       
+00019150: 2020 2020 2020 2020 2044 6973 706c 6179           Display
+00019160: 7320 6120 7370 696e 6e65 7220 746f 2069  s a spinner to i
+00019170: 6e64 6963 6174 6520 7468 6174 2063 6f6e  ndicate that con
+00019180: 7465 6e74 0a20 2020 2020 2020 2020 2020  tent.           
+00019190: 2020 2020 2069 7320 6c6f 6164 696e 672e       is loading.
+000191a0: 0a20 2020 2020 2020 2020 2020 204e 4f4e  .            NON
+000191b0: 4520 2831 293a 0a20 2020 2020 2020 2020  E (1):.         
+000191c0: 2020 2020 2020 204e 6f74 6869 6e67 2069         Nothing i
+000191d0: 7320 6469 7370 6c61 7965 642e 0a20 2020  s displayed..   
+000191e0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000191f0: 2053 5049 4e4e 4552 203d 2030 0a20 2020   SPINNER = 0.   
+00019200: 2020 2020 204e 4f4e 4520 3d20 310a 0a20       NONE = 1.. 
+00019210: 2020 2063 6c61 7373 2049 6e74 6572 6163     class Interac
+00019220: 7469 6f6e 2870 726f 746f 2e45 6e75 6d29  tion(proto.Enum)
+00019230: 3a0a 2020 2020 2020 2020 7222 2222 4f70  :.        r"""Op
+00019240: 7469 6f6e 616c 2e20 5265 7175 6972 6564  tional. Required
+00019250: 2077 6865 6e20 6f70 656e 696e 6720 610a   when opening a.
+00019260: 2020 2020 2020 2020 6064 6961 6c6f 6720          `dialog 
+00019270: 3c68 7474 7073 3a2f 2f64 6576 656c 6f70  <https://develop
+00019280: 6572 732e 676f 6f67 6c65 2e63 6f6d 2f77  ers.google.com/w
+00019290: 6f72 6b73 7061 6365 2f63 6861 742f 6469  orkspace/chat/di
+000192a0: 616c 6f67 733e 605f 5f2e 0a0a 2020 2020  alogs>`__...    
+000192b0: 2020 2020 5768 6174 2074 6f20 646f 2069      What to do i
+000192c0: 6e20 7265 7370 6f6e 7365 2074 6f20 616e  n response to an
+000192d0: 2069 6e74 6572 6163 7469 6f6e 2077 6974   interaction wit
+000192e0: 6820 6120 7573 6572 2c20 7375 6368 2061  h a user, such a
+000192f0: 7320 6120 7573 6572 0a20 2020 2020 2020  s a user.       
+00019300: 2063 6c69 636b 696e 6720 6120 6275 7474   clicking a butt
+00019310: 6f6e 2069 6e20 6120 6361 7264 206d 6573  on in a card mes
+00019320: 7361 6765 2e0a 0a20 2020 2020 2020 2049  sage...        I
+00019330: 6620 756e 7370 6563 6966 6965 642c 2074  f unspecified, t
+00019340: 6865 2061 7070 2072 6573 706f 6e64 7320  he app responds 
+00019350: 6279 2065 7865 6375 7469 6e67 2061 6e20  by executing an 
+00019360: 6060 6163 7469 6f6e 6060 e280 946c 696b  ``action``...lik
+00019370: 650a 2020 2020 2020 2020 6f70 656e 696e  e.        openin
+00019380: 6720 6120 6c69 6e6b 206f 7220 7275 6e6e  g a link or runn
+00019390: 696e 6720 6120 6675 6e63 7469 6f6e e280  ing a function..
+000193a0: 9461 7320 6e6f 726d 616c 2e0a 0a20 2020  .as normal...   
+000193b0: 2020 2020 2042 7920 7370 6563 6966 7969       By specifyi
+000193c0: 6e67 2061 6e20 6060 696e 7465 7261 6374  ng an ``interact
+000193d0: 696f 6e60 602c 2074 6865 2061 7070 2063  ion``, the app c
+000193e0: 616e 2072 6573 706f 6e64 2069 6e20 7370  an respond in sp
+000193f0: 6563 6961 6c0a 2020 2020 2020 2020 696e  ecial.        in
+00019400: 7465 7261 6374 6976 6520 7761 7973 2e20  teractive ways. 
+00019410: 466f 7220 6578 616d 706c 652c 2062 7920  For example, by 
+00019420: 7365 7474 696e 6720 6060 696e 7465 7261  setting ``intera
+00019430: 6374 696f 6e60 6020 746f 0a20 2020 2020  ction`` to.     
+00019440: 2020 2060 604f 5045 4e5f 4449 414c 4f47     ``OPEN_DIALOG
+00019450: 6060 2c20 7468 6520 6170 7020 6361 6e20  ``, the app can 
+00019460: 6f70 656e 2061 0a20 2020 2020 2020 2060  open a.        `
+00019470: 6469 616c 6f67 203c 6874 7470 733a 2f2f  dialog <https://
+00019480: 6465 7665 6c6f 7065 7273 2e67 6f6f 676c  developers.googl
+00019490: 652e 636f 6d2f 776f 726b 7370 6163 652f  e.com/workspace/
+000194a0: 6368 6174 2f64 6961 6c6f 6773 3e60 5f5f  chat/dialogs>`__
+000194b0: 2e0a 0a20 2020 2020 2020 2057 6865 6e20  ...        When 
+000194c0: 7370 6563 6966 6965 642c 2061 206c 6f61  specified, a loa
+000194d0: 6469 6e67 2069 6e64 6963 6174 6f72 2069  ding indicator i
+000194e0: 736e 2774 2073 686f 776e 2e20 4966 2073  sn't shown. If s
+000194f0: 7065 6369 6669 6564 2066 6f72 2061 6e0a  pecified for an.
+00019500: 2020 2020 2020 2020 6164 642d 6f6e 2c20          add-on, 
+00019510: 7468 6520 656e 7469 7265 2063 6172 6420  the entire card 
+00019520: 6973 2073 7472 6970 7065 6420 616e 6420  is stripped and 
+00019530: 6e6f 7468 696e 6720 6973 2073 686f 776e  nothing is shown
+00019540: 2069 6e20 7468 650a 2020 2020 2020 2020   in the.        
+00019550: 636c 6965 6e74 2e0a 0a20 2020 2020 2020  client...       
+00019560: 2060 476f 6f67 6c65 2043 6861 7420 6170   `Google Chat ap
+00019570: 7073 203c 6874 7470 733a 2f2f 6465 7665  ps <https://deve
+00019580: 6c6f 7065 7273 2e67 6f6f 676c 652e 636f  lopers.google.co
+00019590: 6d2f 776f 726b 7370 6163 652f 6368 6174  m/workspace/chat
+000195a0: 3e60 5f5f 3a0a 0a20 2020 2020 2020 2056  >`__:..        V
+000195b0: 616c 7565 733a 0a20 2020 2020 2020 2020  alues:.         
+000195c0: 2020 2049 4e54 4552 4143 5449 4f4e 5f55     INTERACTION_U
+000195d0: 4e53 5045 4349 4649 4544 2028 3029 3a0a  NSPECIFIED (0):.
+000195e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000195f0: 4465 6661 756c 7420 7661 6c75 652e 2054  Default value. T
+00019600: 6865 2060 6061 6374 696f 6e60 6020 6578  he ``action`` ex
+00019610: 6563 7574 6573 2061 7320 6e6f 726d 616c  ecutes as normal
+00019620: 2e0a 2020 2020 2020 2020 2020 2020 4f50  ..            OP
+00019630: 454e 5f44 4941 4c4f 4720 2831 293a 0a20  EN_DIALOG (1):. 
+00019640: 2020 2020 2020 2020 2020 2020 2020 204f                 O
+00019650: 7065 6e73 2061 0a20 2020 2020 2020 2020  pens a.         
+00019660: 2020 2020 2020 2060 6469 616c 6f67 203c         `dialog <
+00019670: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
+00019680: 7273 2e67 6f6f 676c 652e 636f 6d2f 776f  rs.google.com/wo
+00019690: 726b 7370 6163 652f 6368 6174 2f64 6961  rkspace/chat/dia
+000196a0: 6c6f 6773 3e60 5f5f 2c0a 2020 2020 2020  logs>`__,.      
+000196b0: 2020 2020 2020 2020 2020 6120 7769 6e64            a wind
+000196c0: 6f77 6564 2c20 6361 7264 2d62 6173 6564  owed, card-based
+000196d0: 2069 6e74 6572 6661 6365 2074 6861 7420   interface that 
+000196e0: 4368 6174 2061 7070 7320 7573 6520 746f  Chat apps use to
+000196f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019700: 2069 6e74 6572 6163 7420 7769 7468 2075   interact with u
+00019710: 7365 7273 2e0a 0a20 2020 2020 2020 2020  sers...         
+00019720: 2020 2020 2020 204f 6e6c 7920 7375 7070         Only supp
+00019730: 6f72 7465 6420 6279 2043 6861 7420 6170  orted by Chat ap
+00019740: 7073 2069 6e20 7265 7370 6f6e 7365 2074  ps in response t
+00019750: 6f20 6275 7474 6f6e 2d63 6c69 636b 7320  o button-clicks 
+00019760: 6f6e 0a20 2020 2020 2020 2020 2020 2020  on.             
+00019770: 2020 2063 6172 6420 6d65 7373 6167 6573     card messages
+00019780: 2e20 4966 2073 7065 6369 6669 6564 2066  . If specified f
+00019790: 6f72 2061 6e20 6164 642d 6f6e 2c20 7468  or an add-on, th
+000197a0: 6520 656e 7469 7265 2063 6172 640a 2020  e entire card.  
+000197b0: 2020 2020 2020 2020 2020 2020 2020 6973                is
+000197c0: 2073 7472 6970 7065 6420 616e 6420 6e6f   stripped and no
+000197d0: 7468 696e 6720 6973 2073 686f 776e 2069  thing is shown i
+000197e0: 6e20 7468 6520 636c 6965 6e74 2e0a 0a20  n the client... 
+000197f0: 2020 2020 2020 2020 2020 2020 2020 2060                 `
+00019800: 476f 6f67 6c65 2043 6861 740a 2020 2020  Google Chat.    
+00019810: 2020 2020 2020 2020 2020 2020 6170 7073              apps
+00019820: 203c 6874 7470 733a 2f2f 6465 7665 6c6f   <https://develo
+00019830: 7065 7273 2e67 6f6f 676c 652e 636f 6d2f  pers.google.com/
+00019840: 776f 726b 7370 6163 652f 6368 6174 3e60  workspace/chat>`
+00019850: 5f5f 3a0a 2020 2020 2020 2020 2222 220a  __:.        """.
+00019860: 2020 2020 2020 2020 494e 5445 5241 4354          INTERACT
+00019870: 494f 4e5f 554e 5350 4543 4946 4945 4420  ION_UNSPECIFIED 
+00019880: 3d20 300a 2020 2020 2020 2020 4f50 454e  = 0.        OPEN
+00019890: 5f44 4941 4c4f 4720 3d20 310a 0a20 2020  _DIALOG = 1..   
+000198a0: 2063 6c61 7373 2041 6374 696f 6e50 6172   class ActionPar
+000198b0: 616d 6574 6572 2870 726f 746f 2e4d 6573  ameter(proto.Mes
+000198c0: 7361 6765 293a 0a20 2020 2020 2020 2072  sage):.        r
+000198d0: 2222 224c 6973 7420 6f66 2073 7472 696e  """List of strin
+000198e0: 6720 7061 7261 6d65 7465 7273 2074 6f20  g parameters to 
+000198f0: 7375 7070 6c79 2077 6865 6e20 7468 6520  supply when the 
+00019900: 6163 7469 6f6e 206d 6574 686f 6420 6973  action method is
+00019910: 0a20 2020 2020 2020 2069 6e76 6f6b 6564  .        invoked
+00019920: 2e20 466f 7220 6578 616d 706c 652c 2063  . For example, c
+00019930: 6f6e 7369 6465 7220 7468 7265 6520 736e  onsider three sn
+00019940: 6f6f 7a65 2062 7574 746f 6e73 3a20 736e  ooze buttons: sn
+00019950: 6f6f 7a65 206e 6f77 2c0a 2020 2020 2020  ooze now,.      
+00019960: 2020 736e 6f6f 7a65 206f 6e65 2064 6179    snooze one day
+00019970: 2c20 6f72 2073 6e6f 6f7a 6520 6e65 7874  , or snooze next
+00019980: 2077 6565 6b2e 2059 6f75 206d 6967 6874   week. You might
+00019990: 2075 7365 0a20 2020 2020 2020 2060 6061   use.        ``a
+000199a0: 6374 696f 6e20 6d65 7468 6f64 203d 2073  ction method = s
+000199b0: 6e6f 6f7a 6528 2960 602c 2070 6173 7369  nooze()``, passi
+000199c0: 6e67 2074 6865 2073 6e6f 6f7a 6520 7479  ng the snooze ty
+000199d0: 7065 2061 6e64 2073 6e6f 6f7a 650a 2020  pe and snooze.  
+000199e0: 2020 2020 2020 7469 6d65 2069 6e20 7468        time in th
+000199f0: 6520 6c69 7374 206f 6620 7374 7269 6e67  e list of string
+00019a00: 2070 6172 616d 6574 6572 732e 0a0a 2020   parameters...  
+00019a10: 2020 2020 2020 546f 206c 6561 726e 206d        To learn m
+00019a20: 6f72 652c 2073 6565 0a20 2020 2020 2020  ore, see.       
+00019a30: 2060 6060 436f 6d6d 6f6e 4576 656e 744f   ```CommonEventO
+00019a40: 626a 6563 7460 6020 3c68 7474 7073 3a2f  bject`` <https:/
+00019a50: 2f64 6576 656c 6f70 6572 732e 676f 6f67  /developers.goog
+00019a60: 6c65 2e63 6f6d 2f77 6f72 6b73 7061 6365  le.com/workspace
+00019a70: 2f63 6861 742f 6170 692f 7265 6665 7265  /chat/api/refere
+00019a80: 6e63 652f 7265 7374 2f76 312f 4576 656e  nce/rest/v1/Even
+00019a90: 7423 636f 6d6d 6f6e 6576 656e 746f 626a  t#commoneventobj
+00019aa0: 6563 743e 605f 5f2e 0a0a 2020 2020 2020  ect>`__...      
+00019ab0: 2020 6047 6f6f 676c 6520 576f 726b 7370    `Google Worksp
+00019ac0: 6163 6520 4164 642d 6f6e 7320 616e 6420  ace Add-ons and 
+00019ad0: 4368 6174 0a20 2020 2020 2020 2061 7070  Chat.        app
+00019ae0: 7320 3c68 7474 7073 3a2f 2f64 6576 656c  s <https://devel
+00019af0: 6f70 6572 732e 676f 6f67 6c65 2e63 6f6d  opers.google.com
+00019b00: 2f77 6f72 6b73 7061 6365 2f65 7874 656e  /workspace/exten
+00019b10: 643e 605f 5f3a 0a0a 2020 2020 2020 2020  d>`__:..        
+00019b20: 4174 7472 6962 7574 6573 3a0a 2020 2020  Attributes:.    
+00019b30: 2020 2020 2020 2020 6b65 7920 2873 7472          key (str
+00019b40: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00019b50: 2020 2054 6865 206e 616d 6520 6f66 2074     The name of t
+00019b60: 6865 2070 6172 616d 6574 6572 2066 6f72  he parameter for
+00019b70: 2074 6865 2061 6374 696f 6e0a 2020 2020   the action.    
+00019b80: 2020 2020 2020 2020 2020 2020 7363 7269              scri
+00019b90: 7074 2e0a 2020 2020 2020 2020 2020 2020  pt..            
+00019ba0: 7661 6c75 6520 2873 7472 293a 0a20 2020  value (str):.   
+00019bb0: 2020 2020 2020 2020 2020 2020 2054 6865               The
+00019bc0: 2076 616c 7565 206f 6620 7468 6520 7061   value of the pa
+00019bd0: 7261 6d65 7465 722e 0a20 2020 2020 2020  rameter..       
+00019be0: 2022 2222 0a0a 2020 2020 2020 2020 6b65   """..        ke
+00019bf0: 793a 2073 7472 203d 2070 726f 746f 2e46  y: str = proto.F
+00019c00: 6965 6c64 280a 2020 2020 2020 2020 2020  ield(.          
+00019c10: 2020 7072 6f74 6f2e 5354 5249 4e47 2c0a    proto.STRING,.
+00019c20: 2020 2020 2020 2020 2020 2020 6e75 6d62              numb
+00019c30: 6572 3d31 2c0a 2020 2020 2020 2020 290a  er=1,.        ).
+00019c40: 2020 2020 2020 2020 7661 6c75 653a 2073          value: s
+00019c50: 7472 203d 2070 726f 746f 2e46 6965 6c64  tr = proto.Field
+00019c60: 280a 2020 2020 2020 2020 2020 2020 7072  (.            pr
+00019c70: 6f74 6f2e 5354 5249 4e47 2c0a 2020 2020  oto.STRING,.    
+00019c80: 2020 2020 2020 2020 6e75 6d62 6572 3d32          number=2
+00019c90: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
+00019ca0: 2066 756e 6374 696f 6e3a 2073 7472 203d   function: str =
+00019cb0: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
+00019cc0: 2020 2020 2020 7072 6f74 6f2e 5354 5249        proto.STRI
+00019cd0: 4e47 2c0a 2020 2020 2020 2020 6e75 6d62  NG,.        numb
+00019ce0: 6572 3d31 2c0a 2020 2020 290a 2020 2020  er=1,.    ).    
+00019cf0: 7061 7261 6d65 7465 7273 3a20 4d75 7461  parameters: Muta
+00019d00: 626c 6553 6571 7565 6e63 655b 4163 7469  bleSequence[Acti
+00019d10: 6f6e 5061 7261 6d65 7465 725d 203d 2070  onParameter] = p
+00019d20: 726f 746f 2e52 6570 6561 7465 6446 6965  roto.RepeatedFie
+00019d30: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
+00019d40: 6f2e 4d45 5353 4147 452c 0a20 2020 2020  o.MESSAGE,.     
+00019d50: 2020 206e 756d 6265 723d 322c 0a20 2020     number=2,.   
+00019d60: 2020 2020 206d 6573 7361 6765 3d41 6374       message=Act
+00019d70: 696f 6e50 6172 616d 6574 6572 2c0a 2020  ionParameter,.  
+00019d80: 2020 290a 2020 2020 6c6f 6164 5f69 6e64    ).    load_ind
+00019d90: 6963 6174 6f72 3a20 4c6f 6164 496e 6469  icator: LoadIndi
+00019da0: 6361 746f 7220 3d20 7072 6f74 6f2e 4669  cator = proto.Fi
+00019db0: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
+00019dc0: 746f 2e45 4e55 4d2c 0a20 2020 2020 2020  to.ENUM,.       
+00019dd0: 206e 756d 6265 723d 332c 0a20 2020 2020   number=3,.     
+00019de0: 2020 2065 6e75 6d3d 4c6f 6164 496e 6469     enum=LoadIndi
+00019df0: 6361 746f 722c 0a20 2020 2029 0a20 2020  cator,.    ).   
+00019e00: 2070 6572 7369 7374 5f76 616c 7565 733a   persist_values:
+00019e10: 2062 6f6f 6c20 3d20 7072 6f74 6f2e 4669   bool = proto.Fi
+00019e20: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
+00019e30: 746f 2e42 4f4f 4c2c 0a20 2020 2020 2020  to.BOOL,.       
+00019e40: 206e 756d 6265 723d 342c 0a20 2020 2029   number=4,.    )
+00019e50: 0a20 2020 2069 6e74 6572 6163 7469 6f6e  .    interaction
+00019e60: 3a20 496e 7465 7261 6374 696f 6e20 3d20  : Interaction = 
+00019e70: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
+00019e80: 2020 2020 2070 726f 746f 2e45 4e55 4d2c       proto.ENUM,
+00019e90: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
+00019ea0: 352c 0a20 2020 2020 2020 2065 6e75 6d3d  5,.        enum=
+00019eb0: 496e 7465 7261 6374 696f 6e2c 0a20 2020  Interaction,.   
+00019ec0: 2029 0a0a 0a5f 5f61 6c6c 5f5f 203d 2074   )...__all__ = t
+00019ed0: 7570 6c65 2873 6f72 7465 6428 5f5f 7072  uple(sorted(__pr
+00019ee0: 6f74 6f62 7566 5f5f 2e6d 616e 6966 6573  otobuf__.manifes
+00019ef0: 7429 290a                                t)).
```

### Comparing `google-apps-card-0.1.1/google_apps_card.egg-info/PKG-INFO` & `google-apps-card-0.1.2/google_apps_card.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-apps-card
-Version: 0.1.1
+Version: 0.1.2
 Summary: Google Apps Card API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-apps-card
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-apps-card-0.1.1/google_apps_card.egg-info/SOURCES.txt` & `google-apps-card-0.1.2/google_apps_card.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-apps-card-0.1.1/setup.py` & `google-apps-card-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-apps-card-0.1.1/tests/__init__.py` & `google-apps-card-0.1.2/tests/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-apps-card-0.1.1/tests/unit/__init__.py` & `google-apps-card-0.1.2/tests/unit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-apps-card-0.1.1/tests/unit/gapic/__init__.py` & `google-apps-card-0.1.2/tests/unit/gapic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-apps-card-0.1.1/tests/unit/gapic/card_v1/__init__.py` & `google-apps-card-0.1.2/tests/unit/gapic/card_v1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-apps-card-0.1.1/tests/unit/gapic/card_v1/test_card.py` & `google-apps-card-0.1.2/tests/unit/gapic/card_v1/test_card.py`

 * *Files identical despite different names*

