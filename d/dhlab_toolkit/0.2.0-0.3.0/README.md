# Comparing `tmp/dhlab_toolkit-0.2.0.tar.gz` & `tmp/dhlab_toolkit-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhlab_toolkit-0.2.0.tar", max compression
+gzip compressed data, was "dhlab_toolkit-0.3.0.tar", max compression
```

## Comparing `dhlab_toolkit-0.2.0.tar` & `dhlab_toolkit-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1076 2024-03-15 09:20:54.635045 dhlab_toolkit-0.2.0/LICENSE
--rw-r--r--   0        0        0      104 2024-03-15 09:20:54.635045 dhlab_toolkit-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-03-15 09:20:54.635045 dhlab_toolkit-0.2.0/dhlab_toolkit/__init__.py
--rw-r--r--   0        0        0      363 2024-03-15 09:20:54.635045 dhlab_toolkit-0.2.0/dhlab_toolkit/constants.py
--rw-r--r--   0        0        0        0 2024-04-08 14:01:41.019045 dhlab_toolkit-0.2.0/dhlab_toolkit/g2p/__init__.py
--rw-r--r--   0        0        0     2016 2024-04-08 14:03:01.831614 dhlab_toolkit-0.2.0/dhlab_toolkit/g2p/g2p_models.py
--rw-r--r--   0        0        0     4261 2024-03-15 09:20:54.635045 dhlab_toolkit-0.2.0/dhlab_toolkit/geo_data.py
--rw-r--r--   0        0        0    15394 2024-03-15 09:20:54.635045 dhlab_toolkit-0.2.0/dhlab_toolkit/graph_networkx_louvain.py
--rw-r--r--   0        0        0   126476 2024-03-15 09:20:54.639045 dhlab_toolkit-0.2.0/dhlab_toolkit/trigram_lang_model/nno_trilangmodel.json
--rw-r--r--   0        0        0   126751 2024-03-15 09:20:54.643045 dhlab_toolkit-0.2.0/dhlab_toolkit/trigram_lang_model/nob_trilangmodel.json
--rw-r--r--   0        0        0       41 2024-03-15 09:20:54.643045 dhlab_toolkit-0.2.0/dhlab_toolkit/visualization/__init__.py
--rw-r--r--   0        0        0     1677 2024-03-15 09:20:54.643045 dhlab_toolkit-0.2.0/dhlab_toolkit/visualization/cloud.py
--rw-r--r--   0        0        0      286 2024-03-15 09:20:54.643045 dhlab_toolkit-0.2.0/dhlab_toolkit/visualization/heatmap.py
--rw-r--r--   0        0        0       54 2024-03-15 09:20:54.643045 dhlab_toolkit-0.2.0/dhlab_toolkit/wordbank/__init__.py
--rw-r--r--   0        0        0     2462 2024-03-15 09:20:54.643045 dhlab_toolkit-0.2.0/dhlab_toolkit/wordbank/api.py
--rw-r--r--   0        0        0     1959 2024-03-15 09:20:54.643045 dhlab_toolkit-0.2.0/dhlab_toolkit/wordbank/wordbank.py
--rw-r--r--   0        0        0      490 2024-04-08 14:02:40.563462 dhlab_toolkit-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      803 1970-01-01 00:00:00.000000 dhlab_toolkit-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-03-15 09:20:54.635045 dhlab_toolkit-0.3.0/LICENSE
+-rw-r--r--   0        0        0      104 2024-03-15 09:20:54.635045 dhlab_toolkit-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-03-15 09:20:54.635045 dhlab_toolkit-0.3.0/dhlab_toolkit/__init__.py
+-rw-r--r--   0        0        0      363 2024-03-15 09:20:54.635045 dhlab_toolkit-0.3.0/dhlab_toolkit/constants.py
+-rw-r--r--   0        0        0        0 2024-04-08 14:01:41.019045 dhlab_toolkit-0.3.0/dhlab_toolkit/g2p/__init__.py
+-rw-r--r--   0        0        0     2435 2024-04-16 12:44:17.708395 dhlab_toolkit-0.3.0/dhlab_toolkit/g2p/g2p_models.py
+-rw-r--r--   0        0        0     4261 2024-03-15 09:20:54.635045 dhlab_toolkit-0.3.0/dhlab_toolkit/geo_data.py
+-rw-r--r--   0        0        0    15394 2024-03-15 09:20:54.635045 dhlab_toolkit-0.3.0/dhlab_toolkit/graph_networkx_louvain.py
+-rw-r--r--   0        0        0   126476 2024-03-15 09:20:54.639045 dhlab_toolkit-0.3.0/dhlab_toolkit/trigram_lang_model/nno_trilangmodel.json
+-rw-r--r--   0        0        0   126751 2024-03-15 09:20:54.643045 dhlab_toolkit-0.3.0/dhlab_toolkit/trigram_lang_model/nob_trilangmodel.json
+-rw-r--r--   0        0        0       41 2024-03-15 09:20:54.643045 dhlab_toolkit-0.3.0/dhlab_toolkit/visualization/__init__.py
+-rw-r--r--   0        0        0     1677 2024-03-15 09:20:54.643045 dhlab_toolkit-0.3.0/dhlab_toolkit/visualization/cloud.py
+-rw-r--r--   0        0        0      286 2024-03-15 09:20:54.643045 dhlab_toolkit-0.3.0/dhlab_toolkit/visualization/heatmap.py
+-rw-r--r--   0        0        0       54 2024-03-15 09:20:54.643045 dhlab_toolkit-0.3.0/dhlab_toolkit/wordbank/__init__.py
+-rw-r--r--   0        0        0     2462 2024-03-15 09:20:54.643045 dhlab_toolkit-0.3.0/dhlab_toolkit/wordbank/api.py
+-rw-r--r--   0        0        0     1959 2024-03-15 09:20:54.643045 dhlab_toolkit-0.3.0/dhlab_toolkit/wordbank/wordbank.py
+-rw-r--r--   0        0        0      529 2024-04-16 12:44:50.048480 dhlab_toolkit-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      846 1970-01-01 00:00:00.000000 dhlab_toolkit-0.3.0/PKG-INFO
```

### Comparing `dhlab_toolkit-0.2.0/LICENSE` & `dhlab_toolkit-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dhlab_toolkit-0.2.0/dhlab_toolkit/g2p/g2p_models.py` & `dhlab_toolkit-0.3.0/dhlab_toolkit/g2p/g2p_models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #%% 
 from pathlib import Path
+from unittest import result
 from google.cloud import storage
 import phonetisaurus
 import logging
 
 
 def download_public_file(bucket_name, source_blob_name, destination_file_name):
     """Downloads a public blob from the bucket."""
@@ -36,26 +37,36 @@
         except Exception as e:
             logging.error(e)
             logging.info(f'No pre-trained g2p model available for {dialect} {style}.')
     
     logging.debug(f"Path to the G2P model: {download_path}.")
     return download_path
 
+def format_transcription(pronunciation):
+    return " ".join(pronunciation)
 
-def transcribe(words, dialect='e', style= "written"):
+def transcribe(text, dialect='e', style= "written"):
+    """
+    Transcribe a text of whitespace-separated words using a pre-trained g2p model.
+    """
+    words= text.split()
+    transcriptions = transcribe_words(words, dialect=dialect, style=style)
+    return [(word, format_transcription(pron)) for word, pron in transcriptions]
+
+def transcribe_words(words, dialect='e', style= "written"):
     """
     Transcribe a list of words using a pre-trained g2p model.
     """
     model_path = download_g2p_model(dialect=dialect, style=style)
     transcriptions = phonetisaurus.predict(words, model_path = model_path)
     return transcriptions
 
-
 if __name__ == "__main__":
     logging.basicConfig(level=logging.DEBUG)
 
-    download_g2p_model(dialect='t', style= "written")
-    #result = transcribe(["I", "Nasjonalbiblioteket", "har", "vi", "veldig", "mange", "gamle", "og", "sjeldne", "bøker"])
-    #for word, pronunciation in result:
-     #   print(f"{word}\t{' '.join(pronunciation)}")
+    #download_g2p_model(dialect='t', style= "written")
+    text = "I Nasjonalbiblioteket har vi veldig mange gamle og sjeldne bøker"
+    result = transcribe(text)
+    for word, pronunciation in result:
+       print(word, pronunciation, sep="\t")
     
 # %%
```

### Comparing `dhlab_toolkit-0.2.0/dhlab_toolkit/geo_data.py` & `dhlab_toolkit-0.3.0/dhlab_toolkit/geo_data.py`

 * *Files identical despite different names*

### Comparing `dhlab_toolkit-0.2.0/dhlab_toolkit/graph_networkx_louvain.py` & `dhlab_toolkit-0.3.0/dhlab_toolkit/graph_networkx_louvain.py`

 * *Files identical despite different names*

### Comparing `dhlab_toolkit-0.2.0/dhlab_toolkit/trigram_lang_model/nno_trilangmodel.json` & `dhlab_toolkit-0.3.0/dhlab_toolkit/trigram_lang_model/nno_trilangmodel.json`

 * *Files identical despite different names*

### Comparing `dhlab_toolkit-0.2.0/dhlab_toolkit/trigram_lang_model/nob_trilangmodel.json` & `dhlab_toolkit-0.3.0/dhlab_toolkit/trigram_lang_model/nob_trilangmodel.json`

 * *Files identical despite different names*

### Comparing `dhlab_toolkit-0.2.0/dhlab_toolkit/visualization/cloud.py` & `dhlab_toolkit-0.3.0/dhlab_toolkit/visualization/cloud.py`

 * *Files identical despite different names*

### Comparing `dhlab_toolkit-0.2.0/dhlab_toolkit/wordbank/api.py` & `dhlab_toolkit-0.3.0/dhlab_toolkit/wordbank/api.py`

 * *Files identical despite different names*

### Comparing `dhlab_toolkit-0.2.0/dhlab_toolkit/wordbank/wordbank.py` & `dhlab_toolkit-0.3.0/dhlab_toolkit/wordbank/wordbank.py`

 * *Files identical despite different names*

### Comparing `dhlab_toolkit-0.2.0/PKG-INFO` & `dhlab_toolkit-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: dhlab_toolkit
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 Author: Nasjonalbiblioteket 
 Author-email: dhlab@nb.no
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: convert-pa (>=0.1.0,<0.2.0)
+Requires-Dist: dhlab (>=2.32.0,<3.0.0)
 Requires-Dist: google-cloud-storage (>=2.16.0,<3.0.0)
 Requires-Dist: matplotlib (>=3.7.2,<4.0.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: phonetisaurus (>=0.3.0,<0.4.0)
-Requires-Dist: pytest (>=7.4.0,<8.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: seaborn (>=0.12.2,<0.13.0)
+Requires-Dist: seaborn (>=0.13.2,<0.14.0)
 Description-Content-Type: text/markdown
 
 # dhlab toolkit
 Toolkit and models for working with National Library digital humanities laboratory data
```

