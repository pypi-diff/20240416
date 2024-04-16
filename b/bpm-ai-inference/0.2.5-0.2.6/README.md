# Comparing `tmp/bpm_ai_inference-0.2.5.tar.gz` & `tmp/bpm_ai_inference-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpm_ai_inference-0.2.5.tar", max compression
+gzip compressed data, was "bpm_ai_inference-0.2.6.tar", max compression
```

## Comparing `bpm_ai_inference-0.2.5.tar` & `bpm_ai_inference-0.2.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    35128 2024-04-11 14:10:58.522168 bpm_ai_inference-0.2.5/LICENSE
--rw-r--r--   0        0        0       18 2024-04-11 14:10:58.522168 bpm_ai_inference-0.2.5/README.md
--rw-r--r--   0        0        0        0 2024-04-11 14:10:58.522168 bpm_ai_inference-0.2.5/bpm_ai_inference/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 14:10:58.522168 bpm_ai_inference-0.2.5/bpm_ai_inference/classification/__init__.py
--rw-r--r--   0        0        0     2475 2024-04-11 14:10:58.526168 bpm_ai_inference-0.2.5/bpm_ai_inference/classification/transformers_classifier.py
--rw-r--r--   0        0        0     1396 2024-04-11 14:10:58.526168 bpm_ai_inference-0.2.5/bpm_ai_inference/daemon.py
--rw-r--r--   0        0        0        0 2024-04-11 14:10:58.526168 bpm_ai_inference-0.2.5/bpm_ai_inference/llm/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 14:10:58.526168 bpm_ai_inference-0.2.5/bpm_ai_inference/ocr/__init__.py
--rw-r--r--   0        0        0     3213 2024-04-11 14:10:58.526168 bpm_ai_inference-0.2.5/bpm_ai_inference/ocr/tesseract.py
--rw-r--r--   0        0        0        0 2024-04-11 14:10:58.526168 bpm_ai_inference-0.2.5/bpm_ai_inference/pos/__init__.py
--rw-r--r--   0        0        0     1848 2024-04-11 14:10:58.526168 bpm_ai_inference-0.2.5/bpm_ai_inference/pos/spacy_pos_tagger.py
--rw-r--r--   0        0        0        0 2024-04-11 14:10:58.526168 bpm_ai_inference-0.2.5/bpm_ai_inference/question_answering/__init__.py
--rw-r--r--   0        0        0     2110 2024-04-11 14:10:58.526168 bpm_ai_inference-0.2.5/bpm_ai_inference/question_answering/pix2struct_vqa.py
--rw-r--r--   0        0        0     2013 2024-04-11 14:10:58.526168 bpm_ai_inference-0.2.5/bpm_ai_inference/question_answering/transformers_docvqa.py
--rw-r--r--   0        0        0     1882 2024-04-11 14:10:58.526168 bpm_ai_inference-0.2.5/bpm_ai_inference/question_answering/transformers_qa.py
--rw-r--r--   0        0        0        0 2024-04-11 14:10:58.526168 bpm_ai_inference-0.2.5/bpm_ai_inference/speech_recognition/__init__.py
--rw-r--r--   0        0        0     1176 2024-04-11 14:10:58.526168 bpm_ai_inference-0.2.5/bpm_ai_inference/speech_recognition/faster_whisper.py
--rw-r--r--   0        0        0        0 2024-04-11 14:10:58.526168 bpm_ai_inference-0.2.5/bpm_ai_inference/token_classification/__init__.py
--rw-r--r--   0        0        0     1338 2024-04-11 14:10:58.526168 bpm_ai_inference-0.2.5/bpm_ai_inference/token_classification/gliner_token_classifier.py
--rw-r--r--   0        0        0     3115 2024-04-11 14:10:58.526168 bpm_ai_inference-0.2.5/bpm_ai_inference/token_classification/transformers_token_classifier.py
--rw-r--r--   0        0        0        0 2024-04-11 14:10:58.526168 bpm_ai_inference-0.2.5/bpm_ai_inference/translation/__init__.py
--rw-r--r--   0        0        0        2 2024-04-11 14:10:58.526168 bpm_ai_inference-0.2.5/bpm_ai_inference/translation/easy_nmt/__init__.py
--rw-r--r--   0        0        0    18637 2024-04-11 14:10:58.526168 bpm_ai_inference-0.2.5/bpm_ai_inference/translation/easy_nmt/easy_nmt.py
--rw-r--r--   0        0        0     2423 2024-04-11 14:10:58.526168 bpm_ai_inference-0.2.5/bpm_ai_inference/translation/easy_nmt/opus_mt.py
--rw-r--r--   0        0        0     1784 2024-04-11 14:10:58.526168 bpm_ai_inference-0.2.5/bpm_ai_inference/translation/easy_nmt/util.py
--rw-r--r--   0        0        0        0 2024-04-11 14:10:58.526168 bpm_ai_inference-0.2.5/bpm_ai_inference/util/__init__.py
--rw-r--r--   0        0        0      828 2024-04-11 14:10:58.526168 bpm_ai_inference-0.2.5/bpm_ai_inference/util/language.py
--rw-r--r--   0        0        0     6718 2024-04-11 14:10:58.526168 bpm_ai_inference-0.2.5/bpm_ai_inference/util/optimum.py
--rw-r--r--   0        0        0     1471 2024-04-11 14:10:58.530169 bpm_ai_inference-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     1195 1970-01-01 00:00:00.000000 bpm_ai_inference-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    35128 2024-04-16 12:43:03.681380 bpm_ai_inference-0.2.6/LICENSE
+-rw-r--r--   0        0        0       18 2024-04-16 12:43:03.681380 bpm_ai_inference-0.2.6/README.md
+-rw-r--r--   0        0        0        0 2024-04-16 12:43:03.681380 bpm_ai_inference-0.2.6/bpm_ai_inference/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:43:03.681380 bpm_ai_inference-0.2.6/bpm_ai_inference/classification/__init__.py
+-rw-r--r--   0        0        0     2520 2024-04-16 12:43:03.681380 bpm_ai_inference-0.2.6/bpm_ai_inference/classification/transformers_classifier.py
+-rw-r--r--   0        0        0     1519 2024-04-16 12:43:03.681380 bpm_ai_inference-0.2.6/bpm_ai_inference/daemon.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:43:03.681380 bpm_ai_inference-0.2.6/bpm_ai_inference/llm/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:43:03.681380 bpm_ai_inference-0.2.6/bpm_ai_inference/ocr/__init__.py
+-rw-r--r--   0        0        0     3213 2024-04-16 12:43:03.681380 bpm_ai_inference-0.2.6/bpm_ai_inference/ocr/tesseract.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:43:03.681380 bpm_ai_inference-0.2.6/bpm_ai_inference/pos/__init__.py
+-rw-r--r--   0        0        0     1848 2024-04-16 12:43:03.681380 bpm_ai_inference-0.2.6/bpm_ai_inference/pos/spacy_pos_tagger.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:43:03.681380 bpm_ai_inference-0.2.6/bpm_ai_inference/question_answering/__init__.py
+-rw-r--r--   0        0        0     2110 2024-04-16 12:43:03.685380 bpm_ai_inference-0.2.6/bpm_ai_inference/question_answering/pix2struct_vqa.py
+-rw-r--r--   0        0        0     2013 2024-04-16 12:43:03.685380 bpm_ai_inference-0.2.6/bpm_ai_inference/question_answering/transformers_docvqa.py
+-rw-r--r--   0        0        0     1882 2024-04-16 12:43:03.685380 bpm_ai_inference-0.2.6/bpm_ai_inference/question_answering/transformers_qa.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:43:03.685380 bpm_ai_inference-0.2.6/bpm_ai_inference/speech_recognition/__init__.py
+-rw-r--r--   0        0        0     1176 2024-04-16 12:43:03.685380 bpm_ai_inference-0.2.6/bpm_ai_inference/speech_recognition/faster_whisper.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:43:03.685380 bpm_ai_inference-0.2.6/bpm_ai_inference/token_classification/__init__.py
+-rw-r--r--   0        0        0     1338 2024-04-16 12:43:03.685380 bpm_ai_inference-0.2.6/bpm_ai_inference/token_classification/gliner_token_classifier.py
+-rw-r--r--   0        0        0     3115 2024-04-16 12:43:03.685380 bpm_ai_inference-0.2.6/bpm_ai_inference/token_classification/transformers_token_classifier.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:43:03.685380 bpm_ai_inference-0.2.6/bpm_ai_inference/translation/__init__.py
+-rw-r--r--   0        0        0        2 2024-04-16 12:43:03.685380 bpm_ai_inference-0.2.6/bpm_ai_inference/translation/easy_nmt/__init__.py
+-rw-r--r--   0        0        0    18637 2024-04-16 12:43:03.685380 bpm_ai_inference-0.2.6/bpm_ai_inference/translation/easy_nmt/easy_nmt.py
+-rw-r--r--   0        0        0     2423 2024-04-16 12:43:03.685380 bpm_ai_inference-0.2.6/bpm_ai_inference/translation/easy_nmt/opus_mt.py
+-rw-r--r--   0        0        0     1784 2024-04-16 12:43:03.685380 bpm_ai_inference-0.2.6/bpm_ai_inference/translation/easy_nmt/util.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:43:03.685380 bpm_ai_inference-0.2.6/bpm_ai_inference/util/__init__.py
+-rw-r--r--   0        0        0      828 2024-04-16 12:43:03.685380 bpm_ai_inference-0.2.6/bpm_ai_inference/util/language.py
+-rw-r--r--   0        0        0     6718 2024-04-16 12:43:03.685380 bpm_ai_inference-0.2.6/bpm_ai_inference/util/optimum.py
+-rw-r--r--   0        0        0     1471 2024-04-16 12:43:03.685380 bpm_ai_inference-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     1195 1970-01-01 00:00:00.000000 bpm_ai_inference-0.2.6/PKG-INFO
```

### Comparing `bpm_ai_inference-0.2.5/LICENSE` & `bpm_ai_inference-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.5/bpm_ai_inference/classification/transformers_classifier.py` & `bpm_ai_inference-0.2.6/bpm_ai_inference/classification/transformers_classifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,29 +39,30 @@
         )
 
     @override
     async def _do_classify(
             self,
             text: str,
             classes: list[str],
-            hypothesis_template: str | None = None
+            hypothesis_template: str | None = None,
+            multi_label: bool = False
     ) -> ClassificationResult:
         input_tokens = len(self.tokenizer.encode(text))
         max_tokens = self.tokenizer.model_max_length
         logger.debug(f"Input tokens: {input_tokens}")
         if input_tokens > max_tokens:
             logger.warning(
                 f"Input tokens exceed max model context size: {input_tokens} > {max_tokens}. Input will be truncated."
             )
 
         prediction = self.zeroshot_classifier(
             text,
             candidate_labels=classes,
             hypothesis_template=hypothesis_template or "This example is about {}",
-            multi_label=False
+            multi_label=multi_label
         )
         # Zip the labels and scores together and find the label with the max score
         labels_scores = list(zip(prediction['labels'], prediction['scores']))
         max_label, max_score = max(labels_scores, key=lambda x: x[1])
 
         return ClassificationResult(
             max_label=max_label,
```

### Comparing `bpm_ai_inference-0.2.5/bpm_ai_inference/daemon.py` & `bpm_ai_inference-0.2.6/bpm_ai_inference/daemon.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,20 +6,22 @@
 from bpm_ai_inference.classification.transformers_classifier import TransformersClassifier
 from bpm_ai_inference.ocr.tesseract import TesseractOCR
 from bpm_ai_inference.pos.spacy_pos_tagger import SpacyPOSTagger
 from bpm_ai_inference.question_answering.pix2struct_vqa import Pix2StructVQA
 from bpm_ai_inference.question_answering.transformers_docvqa import TransformersDocVQA
 from bpm_ai_inference.question_answering.transformers_qa import TransformersExtractiveQA
 from bpm_ai_inference.speech_recognition.faster_whisper import FasterWhisperASR
+from bpm_ai_inference.token_classification.gliner_token_classifier import GlinerTokenClassifier
 from bpm_ai_inference.token_classification.transformers_token_classifier import TransformersTokenClassifier
 from bpm_ai_inference.translation.easy_nmt.easy_nmt import EasyNMT
 
 remote_classes = [
     TransformersClassifier,
     TransformersTokenClassifier,
+    GlinerTokenClassifier,
     TesseractOCR,
     SpacyPOSTagger,
     Pix2StructVQA,
     TransformersDocVQA,
     TransformersExtractiveQA,
     FasterWhisperASR,
     EasyNMT
```

### Comparing `bpm_ai_inference-0.2.5/bpm_ai_inference/ocr/tesseract.py` & `bpm_ai_inference-0.2.6/bpm_ai_inference/ocr/tesseract.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.5/bpm_ai_inference/pos/spacy_pos_tagger.py` & `bpm_ai_inference-0.2.6/bpm_ai_inference/pos/spacy_pos_tagger.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.5/bpm_ai_inference/question_answering/pix2struct_vqa.py` & `bpm_ai_inference-0.2.6/bpm_ai_inference/question_answering/pix2struct_vqa.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.5/bpm_ai_inference/question_answering/transformers_docvqa.py` & `bpm_ai_inference-0.2.6/bpm_ai_inference/question_answering/transformers_docvqa.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.5/bpm_ai_inference/question_answering/transformers_qa.py` & `bpm_ai_inference-0.2.6/bpm_ai_inference/question_answering/transformers_qa.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.5/bpm_ai_inference/speech_recognition/faster_whisper.py` & `bpm_ai_inference-0.2.6/bpm_ai_inference/speech_recognition/faster_whisper.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.5/bpm_ai_inference/token_classification/gliner_token_classifier.py` & `bpm_ai_inference-0.2.6/bpm_ai_inference/token_classification/gliner_token_classifier.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.5/bpm_ai_inference/token_classification/transformers_token_classifier.py` & `bpm_ai_inference-0.2.6/bpm_ai_inference/token_classification/transformers_token_classifier.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.5/bpm_ai_inference/translation/easy_nmt/easy_nmt.py` & `bpm_ai_inference-0.2.6/bpm_ai_inference/translation/easy_nmt/easy_nmt.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.5/bpm_ai_inference/translation/easy_nmt/opus_mt.py` & `bpm_ai_inference-0.2.6/bpm_ai_inference/translation/easy_nmt/opus_mt.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.5/bpm_ai_inference/translation/easy_nmt/util.py` & `bpm_ai_inference-0.2.6/bpm_ai_inference/translation/easy_nmt/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.5/bpm_ai_inference/util/language.py` & `bpm_ai_inference-0.2.6/bpm_ai_inference/util/language.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.5/bpm_ai_inference/util/optimum.py` & `bpm_ai_inference-0.2.6/bpm_ai_inference/util/optimum.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.5/pyproject.toml` & `bpm_ai_inference-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "bpm-ai-inference"
-version = "0.2.5"
+version = "0.2.6"
 description = "Inference and server for local AI implementations of bpm-ai-core abstractions."
 authors = ["Bennet Krause <bennet.krause@holisticon.de>"]
 repository = "https://github.com/holunda-io/bpm-ai-inference"
 homepage = "https://www.holisticon.de/"
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
-bpm-ai-core = "^2.2.0"
+bpm-ai-core = "^2.4.0"
 faster-whisper = "^0.10.0"
 lingua-language-detector = "^2.0.2"
 pytesseract = "^0.3.10"
 transformers = "^4.37.2"
 sacremoses = "^0.1.1"
 sentencepiece = "^0.2.0"
 nltk = "^3.8.0"
```

### Comparing `bpm_ai_inference-0.2.5/PKG-INFO` & `bpm_ai_inference-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: bpm-ai-inference
-Version: 0.2.5
+Version: 0.2.6
 Summary: Inference and server for local AI implementations of bpm-ai-core abstractions.
 Home-page: https://www.holisticon.de/
 License: GPL-3.0-or-later
 Author: Bennet Krause
 Author-email: bennet.krause@holisticon.de
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: bpm-ai-core (>=2.2.0,<3.0.0)
+Requires-Dist: bpm-ai-core (>=2.4.0,<3.0.0)
 Requires-Dist: faster-whisper (>=0.10.0,<0.11.0)
 Requires-Dist: gliner (>=0.1.6,<0.2.0)
 Requires-Dist: lingua-language-detector (>=2.0.2,<3.0.0)
 Requires-Dist: nltk (>=3.8.0,<4.0.0)
 Requires-Dist: optimum[onnxruntime] (>=1.18.0,<2.0.0)
 Requires-Dist: py-cpuinfo (>=9.0.0,<10.0.0)
 Requires-Dist: pyro5 (>=5.15,<6.0)
```

