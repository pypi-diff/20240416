# Comparing `tmp/nyckel-0.3.4.tar.gz` & `tmp/nyckel-0.4.0.tar.gz`

## Comparing `nyckel-0.3.4.tar` & `nyckel-0.4.0.tar`

### file list

```diff
@@ -1,64 +1,66 @@
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 nyckel-0.3.4/mkdocs.yml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nyckel-0.3.4/requirements.txt
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 nyckel-0.3.4/.github/workflows/build.yml
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 nyckel-0.3.4/.github/workflows/docs.yml
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nyckel-0.3.4/.github/workflows/test.yml
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 nyckel-0.3.4/.vscode/extensions.json
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 nyckel-0.3.4/.vscode/settings.json
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 nyckel-0.3.4/docs/copy_function.md
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 nyckel-0.3.4/docs/credentials.md
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 nyckel-0.3.4/docs/data_classes.md
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 nyckel-0.3.4/docs/delete_label.md
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 nyckel-0.3.4/docs/delete_samples.md
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nyckel-0.3.4/docs/image_classification.md
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 nyckel-0.3.4/docs/index.md
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 nyckel-0.3.4/docs/merge_labels.md
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 nyckel-0.3.4/docs/multimodal_classification.md
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 nyckel-0.3.4/docs/quickstart.md
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 nyckel-0.3.4/docs/requirements.txt
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 nyckel-0.3.4/docs/tabular_classification.md
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 nyckel-0.3.4/docs/text_classification.md
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 nyckel-0.3.4/docs/text_tags.md
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 nyckel-0.3.4/docs/assets/favicon.ico
--rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 nyckel-0.3.4/docs/assets/nyckel-logo.png
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nyckel-0.3.4/docs/stylesheets/extra.css
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 nyckel-0.3.4/src/nyckel/__init__.py
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 nyckel-0.3.4/src/nyckel/auth.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 nyckel-0.3.4/src/nyckel/config.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 nyckel-0.3.4/src/nyckel/data_classes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.3.4/src/nyckel/py.typed
--rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 nyckel-0.3.4/src/nyckel/request_utils.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 nyckel-0.3.4/src/nyckel/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.3.4/src/nyckel/functions/__init__.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nyckel-0.3.4/src/nyckel/functions/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.3.4/src/nyckel/functions/classification/__init__.py
--rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 nyckel-0.3.4/src/nyckel/functions/classification/classification.py
--rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 nyckel-0.3.4/src/nyckel/functions/classification/factory.py
--rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 nyckel-0.3.4/src/nyckel/functions/classification/function_handler.py
--rw-r--r--   0        0        0    13947 2020-02-02 00:00:00.000000 nyckel-0.3.4/src/nyckel/functions/classification/image_classification.py
--rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 nyckel-0.3.4/src/nyckel/functions/classification/label_handler.py
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 nyckel-0.3.4/src/nyckel/functions/classification/sample_handler.py
--rw-r--r--   0        0        0    17493 2020-02-02 00:00:00.000000 nyckel-0.3.4/src/nyckel/functions/classification/tabular_classification.py
--rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 nyckel-0.3.4/src/nyckel/functions/classification/text_classification.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.3.4/src/nyckel/functions/tags/__init__.py
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 nyckel-0.3.4/src/nyckel/functions/tags/tags.py
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 nyckel-0.3.4/src/nyckel/functions/tags/tags_function_factory.py
--rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 nyckel-0.3.4/src/nyckel/functions/tags/tags_function_handler.py
--rw-r--r--   0        0        0     6701 2020-02-02 00:00:00.000000 nyckel-0.3.4/src/nyckel/functions/tags/tags_sample_handler.py
--rw-r--r--   0        0        0     8189 2020-02-02 00:00:00.000000 nyckel-0.3.4/src/nyckel/functions/tags/text_tags.py
--rw-r--r--   0        0        0     6904 2020-02-02 00:00:00.000000 nyckel-0.3.4/tests/conftest.py
--rw-r--r--   0        0        0   107239 2020-02-02 00:00:00.000000 nyckel-0.3.4/tests/flower.jpg
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 nyckel-0.3.4/tests/test_duplicates_handling.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 nyckel-0.3.4/tests/test_field_handler.py
--rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 nyckel-0.3.4/tests/test_image_classification_function.py
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 nyckel-0.3.4/tests/test_image_decoder.py
--rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 nyckel-0.3.4/tests/test_label_handler.py
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 nyckel-0.3.4/tests/test_sample_handler.py
--rw-r--r--   0        0        0     5418 2020-02-02 00:00:00.000000 nyckel-0.3.4/tests/test_tabular_classification_function.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 nyckel-0.3.4/tests/test_text_classification_function.py
--rw-r--r--   0        0        0     4288 2020-02-02 00:00:00.000000 nyckel-0.3.4/tests/test_text_tags_function.py
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 nyckel-0.3.4/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 nyckel-0.3.4/LICENSE
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 nyckel-0.3.4/README.md
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 nyckel-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 nyckel-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 nyckel-0.4.0/mkdocs.yml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nyckel-0.4.0/requirements.txt
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 nyckel-0.4.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 nyckel-0.4.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nyckel-0.4.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 nyckel-0.4.0/.vscode/extensions.json
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 nyckel-0.4.0/.vscode/settings.json
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 nyckel-0.4.0/docs/copy_function.md
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 nyckel-0.4.0/docs/credentials.md
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 nyckel-0.4.0/docs/data_classes.md
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 nyckel-0.4.0/docs/delete_label.md
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 nyckel-0.4.0/docs/delete_samples.md
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nyckel-0.4.0/docs/image_classification.md
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 nyckel-0.4.0/docs/index.md
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 nyckel-0.4.0/docs/merge_labels.md
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 nyckel-0.4.0/docs/multimodal_classification.md
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 nyckel-0.4.0/docs/quickstart.md
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 nyckel-0.4.0/docs/requirements.txt
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 nyckel-0.4.0/docs/tabular_classification.md
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 nyckel-0.4.0/docs/text_classification.md
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 nyckel-0.4.0/docs/text_tags.md
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 nyckel-0.4.0/docs/assets/favicon.ico
+-rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 nyckel-0.4.0/docs/assets/nyckel-logo.png
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nyckel-0.4.0/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/__init__.py
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/auth.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/config.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/data_classes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/py.typed
+-rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/request_utils.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/functions/__init__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/functions/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/functions/classification/__init__.py
+-rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/functions/classification/classification.py
+-rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/functions/classification/factory.py
+-rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/functions/classification/function_handler.py
+-rw-r--r--   0        0        0    14404 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/functions/classification/image_classification.py
+-rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/functions/classification/label_handler.py
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/functions/classification/sample_handler.py
+-rw-r--r--   0        0        0    17493 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/functions/classification/tabular_classification.py
+-rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/functions/classification/text_classification.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/functions/tags/__init__.py
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/functions/tags/tags.py
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/functions/tags/tags_function_factory.py
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/functions/tags/tags_function_handler.py
+-rw-r--r--   0        0        0     6701 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/functions/tags/tags_sample_handler.py
+-rw-r--r--   0        0        0     8189 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/functions/tags/text_tags.py
+-rw-r--r--   0        0        0     6904 2020-02-02 00:00:00.000000 nyckel-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 nyckel-0.4.0/tests/test_duplicates_handling.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 nyckel-0.4.0/tests/test_field_handler.py
+-rw-r--r--   0        0        0     5332 2020-02-02 00:00:00.000000 nyckel-0.4.0/tests/test_image_classification_function.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 nyckel-0.4.0/tests/test_image_decoder.py
+-rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 nyckel-0.4.0/tests/test_label_handler.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 nyckel-0.4.0/tests/test_sample_handler.py
+-rw-r--r--   0        0        0     5436 2020-02-02 00:00:00.000000 nyckel-0.4.0/tests/test_tabular_classification_function.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 nyckel-0.4.0/tests/test_text_classification_function.py
+-rw-r--r--   0        0        0     4288 2020-02-02 00:00:00.000000 nyckel-0.4.0/tests/test_text_tags_function.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 nyckel-0.4.0/tests/test_white_background.py
+-rw-r--r--   0        0        0   107239 2020-02-02 00:00:00.000000 nyckel-0.4.0/tests/fixtures/flower.jpg
+-rw-r--r--   0        0        0    26189 2020-02-02 00:00:00.000000 nyckel-0.4.0/tests/fixtures/mixed-alpha-background.png
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 nyckel-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 nyckel-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 nyckel-0.4.0/README.md
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 nyckel-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 nyckel-0.4.0/PKG-INFO
```

### Comparing `nyckel-0.3.4/mkdocs.yml` & `nyckel-0.4.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/.github/workflows/build.yml` & `nyckel-0.4.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/.github/workflows/docs.yml` & `nyckel-0.4.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/.github/workflows/test.yml` & `nyckel-0.4.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/.vscode/settings.json` & `nyckel-0.4.0/.vscode/settings.json`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
         "**/__pycache__": true,
         "**/.pytest_cache": true,
         "**/.ropeproject": true,
         "**/.idea": true,
     },
     "cSpell.words": [
         "chunkify",
+        "getpixel",
         "Gruezi",
         "Hola",
         "Multimodal",
         "ncols",
         "nyckel",
         "pytest",
         "tqdm"
```

### Comparing `nyckel-0.3.4/docs/copy_function.md` & `nyckel-0.4.0/docs/copy_function.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/docs/delete_label.md` & `nyckel-0.4.0/docs/delete_label.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/docs/delete_samples.md` & `nyckel-0.4.0/docs/delete_samples.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/docs/index.md` & `nyckel-0.4.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/docs/merge_labels.md` & `nyckel-0.4.0/docs/merge_labels.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/docs/multimodal_classification.md` & `nyckel-0.4.0/docs/multimodal_classification.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/docs/quickstart.md` & `nyckel-0.4.0/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/docs/assets/favicon.ico` & `nyckel-0.4.0/docs/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/docs/assets/nyckel-logo.png` & `nyckel-0.4.0/docs/assets/nyckel-logo.png`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/src/nyckel/__init__.py` & `nyckel-0.4.0/src/nyckel/__init__.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/src/nyckel/auth.py` & `nyckel-0.4.0/src/nyckel/auth.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/src/nyckel/request_utils.py` & `nyckel-0.4.0/src/nyckel/request_utils.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/src/nyckel/functions/classification/classification.py` & `nyckel-0.4.0/src/nyckel/functions/classification/classification.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/src/nyckel/functions/classification/factory.py` & `nyckel-0.4.0/src/nyckel/functions/classification/factory.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/src/nyckel/functions/classification/function_handler.py` & `nyckel-0.4.0/src/nyckel/functions/classification/function_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/src/nyckel/functions/classification/image_classification.py` & `nyckel-0.4.0/src/nyckel/functions/classification/image_classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,14 +328,22 @@
         return inline_data.split(";base64,")[1]
 
 
 class ImageEncoder:
     def to_base64(self, img: Union[Image.Image, BytesIO]) -> str:
         if isinstance(img, Image.Image):
             im_bytes = BytesIO()
+            if img.mode == "P" and "transparency" in img.info:
+                # Convert to RGBA if the image has transparency.
+                img = img.convert("RGBA")
+            if img.mode == "RGBA":
+                # Explicitly set RGBA backgrounds to white.
+                background = Image.new("RGBA", img.size, (255, 255, 255))
+                background.paste(img, mask=img.split()[3])  # 3 is the alpha channel
+                img = background
             if not img.mode == "RGB":
                 img = img.convert("RGB")
             img.save(im_bytes, format="JPEG", quality=95)
         else:
             im_bytes = img
         encoded_string = base64.b64encode(im_bytes.getvalue()).decode("utf-8")
         return "data:image/jpg;base64," + encoded_string
```

### Comparing `nyckel-0.3.4/src/nyckel/functions/classification/label_handler.py` & `nyckel-0.4.0/src/nyckel/functions/classification/label_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/src/nyckel/functions/classification/sample_handler.py` & `nyckel-0.4.0/src/nyckel/functions/classification/sample_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/src/nyckel/functions/classification/tabular_classification.py` & `nyckel-0.4.0/src/nyckel/functions/classification/tabular_classification.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/src/nyckel/functions/classification/text_classification.py` & `nyckel-0.4.0/src/nyckel/functions/classification/text_classification.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/src/nyckel/functions/tags/tags.py` & `nyckel-0.4.0/src/nyckel/functions/tags/tags.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/src/nyckel/functions/tags/tags_function_factory.py` & `nyckel-0.4.0/src/nyckel/functions/tags/tags_function_factory.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/src/nyckel/functions/tags/tags_function_handler.py` & `nyckel-0.4.0/src/nyckel/functions/tags/tags_function_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/src/nyckel/functions/tags/tags_sample_handler.py` & `nyckel-0.4.0/src/nyckel/functions/tags/tags_sample_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/src/nyckel/functions/tags/text_tags.py` & `nyckel-0.4.0/src/nyckel/functions/tags/text_tags.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/tests/conftest.py` & `nyckel-0.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/tests/flower.jpg` & `nyckel-0.4.0/tests/fixtures/flower.jpg`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/tests/test_duplicates_handling.py` & `nyckel-0.4.0/tests/test_duplicates_handling.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/tests/test_field_handler.py` & `nyckel-0.4.0/tests/test_field_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/tests/test_image_classification_function.py` & `nyckel-0.4.0/tests/test_image_classification_function.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
 @pytest.mark.skipif(
     credentials.server_url == "http://localhost:5000",
     reason="Integrity of image on copy is only implemented for images hosted on S3.",
 )
 def test_image_integrity_on_copy(image_classification_function: ImageClassificationFunction) -> None:
     func: ImageClassificationFunction = image_classification_function
-    local_filepath = os.path.abspath("tests/flower.jpg")
+    local_filepath = os.path.abspath("tests/fixtures/flower.jpg")
 
     # When Nyckel first receives an image, it resizes and recodes it.
     first_sample_id = func.create_samples([ImageClassificationSample(data=local_filepath, external_id="v0")])[0]
     first_sample = func.read_sample(first_sample_id)
 
     # Here we point back to a nyckel owned url, so the images bytes are stored exactly as posted.
     second_sample_id = func.create_samples([ImageClassificationSample(data=first_sample.data, external_id="v1")])[0]
@@ -95,20 +95,20 @@
 
     decoder = ImageDecoder()
     assert np.array_equal(np.array(decoder.to_image(first_sample.data)), np.array(decoder.to_image(second_sample.data)))
 
 
 post_sample_parameter_examples = [
     ImageClassificationSample(
-        data=os.path.abspath("tests/flower.jpg"), annotation=ClassificationAnnotation(label_name="Nice")
+        data=os.path.abspath("tests/fixtures/flower.jpg"), annotation=ClassificationAnnotation(label_name="Nice")
     ),
-    (os.path.abspath("tests/flower.jpg"), "Nice"),
-    (Image.open(os.path.abspath("tests/flower.jpg")), "Nice"),
-    os.path.abspath("tests/flower.jpg"),
-    Image.open(os.path.abspath("tests/flower.jpg")),
+    (os.path.abspath("tests/fixtures/flower.jpg"), "Nice"),
+    (Image.open(os.path.abspath("tests/fixtures/flower.jpg")), "Nice"),
+    os.path.abspath("tests/fixtures/flower.jpg"),
+    Image.open(os.path.abspath("tests/fixtures/flower.jpg")),
 ]
 
 
 @pytest.mark.parametrize("post_samples_input", post_sample_parameter_examples)
 def test_post_sample_overloading(
     image_classification_function: ImageClassificationFunction,
     post_samples_input: Union[ImageClassificationSample, Tuple[str, str], Tuple[Image.Image, str], str, Image.Image],
@@ -116,12 +116,12 @@
     image_classification_function.create_samples([post_samples_input])
     time.sleep(1)
     samples = image_classification_function.list_samples()
     assert len(samples) == 1
 
     decoder = ImageDecoder()
     returned_image = decoder.to_image(samples[0].data)
-    original_image = Image.open(os.path.abspath("tests/flower.jpg"))
+    original_image = Image.open(os.path.abspath("tests/fixtures/flower.jpg"))
 
     assert returned_image.size == original_image.size
     # TODO: test that the image content is the same. It's tricky b/c Nyckel re-codes
     # the image when the sample is created.
```

### Comparing `nyckel-0.3.4/tests/test_image_decoder.py` & `nyckel-0.4.0/tests/test_image_decoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from nyckel.functions.classification.image_classification import ImageDecoder, ImageEncoder
 from PIL import Image
 
 image_url = "https://www.nyckel.com/blog/images/taimi-case-study-header-image.png"
 
 image_base64 = ImageEncoder().to_base64(Image.new(mode="RGB", size=(40, 40)))
 
-image_filepath = os.path.abspath("tests/flower.jpg")
+image_filepath = os.path.abspath("tests/fixtures/flower.jpg")
 
 
 def test_to_bytes() -> None:
     decoder = ImageDecoder()
 
     assert isinstance(decoder.to_stream(image_url), BytesIO)
     assert isinstance(decoder.to_stream(image_base64), BytesIO)
```

### Comparing `nyckel-0.3.4/tests/test_label_handler.py` & `nyckel-0.4.0/tests/test_label_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/tests/test_sample_handler.py` & `nyckel-0.4.0/tests/test_sample_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/tests/test_tabular_classification_function.py` & `nyckel-0.4.0/tests/test_tabular_classification_function.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     func.create_fields(
         [
             TabularFunctionField(name="firstname", type="Text"),
             TabularFunctionField(name="lastname", type="Text"),
             TabularFunctionField(name="mugshot", type="Image"),
         ]
     )
-    local_image_file = os.path.abspath("tests/flower.jpg")
+    local_image_file = os.path.abspath("tests/fixtures/flower.jpg")
     func.create_samples(
         [
             TabularClassificationSample(
                 data={"firstname": "Adam", "lastname": "Art", "mugshot": local_image_file},
                 annotation=ClassificationAnnotation(label_name="happy"),
             ),
             TabularClassificationSample(
@@ -110,15 +110,15 @@
 
 
 def test_image_field(tabular_classification_function: TabularClassificationFunction) -> None:
     tabular_classification_function.create_fields(
         [TabularFunctionField(name="firstname", type="Text"), TabularFunctionField(name="mug", type="Image")]
     )
 
-    local_filepath = os.path.abspath("tests/flower.jpg")
+    local_filepath = os.path.abspath("tests/fixtures/flower.jpg")
 
     tabular_classification_function.create_samples(
         [
             TabularClassificationSample(
                 data={"firstname": "Adam", "mug": local_filepath},
                 annotation=ClassificationAnnotation(label_name="Person"),
             )
```

### Comparing `nyckel-0.3.4/tests/test_text_classification_function.py` & `nyckel-0.4.0/tests/test_text_classification_function.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/tests/test_text_tags_function.py` & `nyckel-0.4.0/tests/test_text_tags_function.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/.gitignore` & `nyckel-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/LICENSE` & `nyckel-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/README.md` & `nyckel-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.3.4/pyproject.toml` & `nyckel-0.4.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/nyckel"]
 
 [project]
 name = "nyckel"
-version = "0.3.4"
+version = "0.4.0"
 authors = [{ name = "Oscar Beijbom", email = "oscar@nyckel.com" }]
 description = "Python package for the Nyckel API"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

### Comparing `nyckel-0.3.4/PKG-INFO` & `nyckel-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nyckel
-Version: 0.3.4
+Version: 0.4.0
 Summary: Python package for the Nyckel API
 Project-URL: Homepage, https://github.com/NyckelAI/python-sdk
 Author-email: Oscar Beijbom <oscar@nyckel.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

