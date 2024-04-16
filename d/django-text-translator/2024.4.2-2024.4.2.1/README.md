# Comparing `tmp/django_text_translator-2024.4.2.tar.gz` & `tmp/django_text_translator-2024.4.2.1.tar.gz`

## Comparing `django_text_translator-2024.4.2.tar` & `django_text_translator-2024.4.2.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/.github/FUNDING.yml
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/__init__.py
--rw-r--r--   0        0        0     5255 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/admin.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/apps.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/tests.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/views.py
--rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/migrations/0001_initial.py
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/migrations/0002_openaitranslator_base_url_and_more.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/migrations/0003_azureaitranslator_openaitranslator_frequency_penalty_and_more.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/migrations/0004_alter_openaitranslator_model.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/migrations/0005_caiyuntranslator_deeplxtranslator.py
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/migrations/0006_testtranslator_alter_openaitranslator_prompt.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/migrations/0007_caiyuntranslator_max_characters_and_more.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/migrations/0008_geminitranslator.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/migrations/0009_deepltranslator_proxy_deepltranslator_server_url.py
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/migrations/0010_claudetranslator.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/migrations/0011_googletranslatewebtranslator_and_more.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/migrations/0012_geminitranslator_interval.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/migrations/0013_deeplwebtranslator.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/migrations/0014_testtranslator_interval.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/migrations/0015_googletranslatewebtranslator_max_characters.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/migrations/0016_alter_deeplwebtranslator_max_characters_and_more.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/migrations/0017_remove_translated_content_id_and_more.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/migrations/0018_alter_claudetranslator_model.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/migrations/0019_alter_openaitranslator_model.py
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/migrations/0020_moonshotaitranslator.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/migrations/0021_alter_claudetranslator_model.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/migrations/0022_alter_geminitranslator_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/migrations/__init__.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/models/__init__.py
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/models/azureai.py
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/models/base.py
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/models/caiyun.py
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/models/claude.py
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/models/deepl.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/models/deeplweb.py
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/models/deeplx.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/models/dev.py
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/models/gemini.py
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/models/google_translate_web.py
--rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/models/microsoft_translate.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/models/moonshotai.py
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/models/openai.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/django_text_translator/static/img/icon-loading.svg
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/LICENSE
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/README.md
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/pyproject.toml
--rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2/PKG-INFO
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/__init__.py
+-rw-r--r--   0        0        0     5255 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/admin.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/apps.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/tests.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/views.py
+-rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0002_openaitranslator_base_url_and_more.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0003_azureaitranslator_openaitranslator_frequency_penalty_and_more.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0004_alter_openaitranslator_model.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0005_caiyuntranslator_deeplxtranslator.py
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0006_testtranslator_alter_openaitranslator_prompt.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0007_caiyuntranslator_max_characters_and_more.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0008_geminitranslator.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0009_deepltranslator_proxy_deepltranslator_server_url.py
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0010_claudetranslator.py
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0011_googletranslatewebtranslator_and_more.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0012_geminitranslator_interval.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0013_deeplwebtranslator.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0014_testtranslator_interval.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0015_googletranslatewebtranslator_max_characters.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0016_alter_deeplwebtranslator_max_characters_and_more.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0017_remove_translated_content_id_and_more.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0018_alter_claudetranslator_model.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0019_alter_openaitranslator_model.py
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0020_moonshotaitranslator.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0021_alter_claudetranslator_model.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0022_alter_geminitranslator_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/__init__.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/models/__init__.py
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/models/azureai.py
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/models/base.py
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/models/caiyun.py
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/models/claude.py
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/models/deepl.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/models/deeplweb.py
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/models/deeplx.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/models/dev.py
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/models/gemini.py
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/models/google_translate_web.py
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/models/microsoft_translate.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/models/moonshotai.py
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/models/openai.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/static/img/icon-loading.svg
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/LICENSE
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/README.md
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/PKG-INFO
```

### Comparing `django_text_translator-2024.4.2/.github/workflows/python-publish.yml` & `django_text_translator-2024.4.2.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2/django_text_translator/admin.py` & `django_text_translator-2024.4.2.1/django_text_translator/admin.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2/django_text_translator/migrations/0001_initial.py` & `django_text_translator-2024.4.2.1/django_text_translator/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2/django_text_translator/migrations/0002_openaitranslator_base_url_and_more.py` & `django_text_translator-2024.4.2.1/django_text_translator/migrations/0002_openaitranslator_base_url_and_more.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2/django_text_translator/migrations/0003_azureaitranslator_openaitranslator_frequency_penalty_and_more.py` & `django_text_translator-2024.4.2.1/django_text_translator/migrations/0003_azureaitranslator_openaitranslator_frequency_penalty_and_more.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2/django_text_translator/migrations/0004_alter_openaitranslator_model.py` & `django_text_translator-2024.4.2.1/django_text_translator/migrations/0004_alter_openaitranslator_model.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2/django_text_translator/migrations/0005_caiyuntranslator_deeplxtranslator.py` & `django_text_translator-2024.4.2.1/django_text_translator/migrations/0005_caiyuntranslator_deeplxtranslator.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2/django_text_translator/migrations/0006_testtranslator_alter_openaitranslator_prompt.py` & `django_text_translator-2024.4.2.1/django_text_translator/migrations/0006_testtranslator_alter_openaitranslator_prompt.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2/django_text_translator/migrations/0007_caiyuntranslator_max_characters_and_more.py` & `django_text_translator-2024.4.2.1/django_text_translator/migrations/0007_caiyuntranslator_max_characters_and_more.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2/django_text_translator/migrations/0008_geminitranslator.py` & `django_text_translator-2024.4.2.1/django_text_translator/migrations/0008_geminitranslator.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2/django_text_translator/migrations/0009_deepltranslator_proxy_deepltranslator_server_url.py` & `django_text_translator-2024.4.2.1/django_text_translator/migrations/0009_deepltranslator_proxy_deepltranslator_server_url.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2/django_text_translator/migrations/0010_claudetranslator.py` & `django_text_translator-2024.4.2.1/django_text_translator/migrations/0010_claudetranslator.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2/django_text_translator/migrations/0011_googletranslatewebtranslator_and_more.py` & `django_text_translator-2024.4.2.1/django_text_translator/migrations/0011_googletranslatewebtranslator_and_more.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2/django_text_translator/migrations/0013_deeplwebtranslator.py` & `django_text_translator-2024.4.2.1/django_text_translator/migrations/0013_deeplwebtranslator.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2/django_text_translator/migrations/0016_alter_deeplwebtranslator_max_characters_and_more.py` & `django_text_translator-2024.4.2.1/django_text_translator/migrations/0016_alter_deeplwebtranslator_max_characters_and_more.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2/django_text_translator/migrations/0017_remove_translated_content_id_and_more.py` & `django_text_translator-2024.4.2.1/django_text_translator/migrations/0017_remove_translated_content_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2/django_text_translator/migrations/0018_alter_claudetranslator_model.py` & `django_text_translator-2024.4.2.1/django_text_translator/migrations/0018_alter_claudetranslator_model.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2/django_text_translator/migrations/0019_alter_openaitranslator_model.py` & `django_text_translator-2024.4.2.1/django_text_translator/migrations/0019_alter_openaitranslator_model.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2/django_text_translator/migrations/0020_moonshotaitranslator.py` & `django_text_translator-2024.4.2.1/django_text_translator/migrations/0020_moonshotaitranslator.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2/django_text_translator/migrations/0021_alter_claudetranslator_model.py` & `django_text_translator-2024.4.2.1/django_text_translator/migrations/0021_alter_claudetranslator_model.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2/django_text_translator/models/__init__.py` & `django_text_translator-2024.4.2.1/django_text_translator/models/__init__.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2/django_text_translator/models/azureai.py` & `django_text_translator-2024.4.2.1/django_text_translator/models/azureai.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2/django_text_translator/models/base.py` & `django_text_translator-2024.4.2.1/django_text_translator/models/base.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2/django_text_translator/models/caiyun.py` & `django_text_translator-2024.4.2.1/django_text_translator/models/caiyun.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2/django_text_translator/models/claude.py` & `django_text_translator-2024.4.2.1/django_text_translator/models/claude.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2/django_text_translator/models/deepl.py` & `django_text_translator-2024.4.2.1/django_text_translator/models/deepl.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2/django_text_translator/models/deeplweb.py` & `django_text_translator-2024.4.2.1/django_text_translator/models/deeplweb.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2/django_text_translator/models/deeplx.py` & `django_text_translator-2024.4.2.1/django_text_translator/models/deeplx.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2/django_text_translator/models/dev.py` & `django_text_translator-2024.4.2.1/django_text_translator/models/dev.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2/django_text_translator/models/gemini.py` & `django_text_translator-2024.4.2.1/django_text_translator/models/gemini.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2/django_text_translator/models/google_translate_web.py` & `django_text_translator-2024.4.2.1/django_text_translator/models/google_translate_web.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,13 +54,17 @@
                 "sl": "auto",
                 "tl": target_language,
                 "dt": "t",
                 "q": text,
             }
             resp = httpx.get(self.base_url, params=params, timeout=10, proxy=self.proxy)
             resp.raise_for_status()
-            translated_text = resp.json()[0][0][0]
+            resp_json = resp.json()
+            if resp_json:
+                translated_text = resp_json[0][0][0]
+            else:
+                logging.error("GoogleTranslateWebTranslator->Invalid response: %s", resp.text)
         except Exception as e:
             logging.error("GoogleTranslateWebTranslator->%s: %s", e, text)
         finally:
             sleep(self.interval)
             return {'text': translated_text, "characters": len(text)}
```

### Comparing `django_text_translator-2024.4.2/django_text_translator/models/microsoft_translate.py` & `django_text_translator-2024.4.2.1/django_text_translator/models/microsoft_translate.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2/django_text_translator/models/moonshotai.py` & `django_text_translator-2024.4.2.1/django_text_translator/models/moonshotai.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2/django_text_translator/models/openai.py` & `django_text_translator-2024.4.2.1/django_text_translator/models/openai.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2/django_text_translator/static/img/icon-loading.svg` & `django_text_translator-2024.4.2.1/django_text_translator/static/img/icon-loading.svg`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2/LICENSE` & `django_text_translator-2024.4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2/README.md` & `django_text_translator-2024.4.2.1/README.md`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2/pyproject.toml` & `django_text_translator-2024.4.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["./"]
 
 [project]
 name = "django-text-translator"
-version = "2024.4.2"
+version = "2024.4.2.1"
 authors = [
   { name="Versun", email="django-text-translator@versun.me" },
 ]
 description = "A Django application that supports adding multiple third-party engines for text translation."
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "MIT License"}
```

### Comparing `django_text_translator-2024.4.2/PKG-INFO` & `django_text_translator-2024.4.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: django-text-translator
-Version: 2024.4.2
+Version: 2024.4.2.1
 Summary: A Django application that supports adding multiple third-party engines for text translation.
 Project-URL: Homepage, https://github.com/rss-translator/django-text-translator
 Project-URL: Repository, https://github.com/rss-translator/django-text-translator.git
 Project-URL: Issues, https://github.com/rss-translator/django-text-translator/issues
 Author-email: Versun <django-text-translator@versun.me>
 License: MIT License
 License-File: LICENSE
```

