# Comparing `tmp/ondewo-s2t-client-5.6.0.tar.gz` & `tmp/ondewo-s2t-client-5.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ondewo-s2t-client-5.6.0.tar", last modified: Sat Jan 27 14:49:27 2024, max compression
+gzip compressed data, was "ondewo-s2t-client-5.7.0.tar", last modified: Tue Apr 16 13:21:12 2024, max compression
```

## Comparing `ondewo-s2t-client-5.6.0.tar` & `ondewo-s2t-client-5.7.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-27 14:49:27.965034 ondewo-s2t-client-5.6.0/
--rw-r--r--   0 root         (0) root         (0)     6574 2024-01-27 14:49:27.965034 ondewo-s2t-client-5.6.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     6020 2024-01-27 14:49:07.000000 ondewo-s2t-client-5.6.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-27 14:49:27.965034 ondewo-s2t-client-5.6.0/ondewo/
--rw-rw-r--   0 root         (0) root         (0)       81 2024-01-27 14:49:07.000000 ondewo-s2t-client-5.6.0/ondewo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-27 14:49:27.965034 ondewo-s2t-client-5.6.0/ondewo/s2t/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-01-27 14:49:07.000000 ondewo-s2t-client-5.6.0/ondewo/s2t/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-27 14:49:27.965034 ondewo-s2t-client-5.6.0/ondewo/s2t/client/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-01-27 14:49:07.000000 ondewo-s2t-client-5.6.0/ondewo/s2t/client/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      756 2024-01-27 14:49:07.000000 ondewo-s2t-client-5.6.0/ondewo/s2t/client/client.py
--rw-rw-r--   0 root         (0) root         (0)      262 2024-01-27 14:49:07.000000 ondewo-s2t-client-5.6.0/ondewo/s2t/client/client_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-27 14:49:27.965034 ondewo-s2t-client-5.6.0/ondewo/s2t/client/services/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-01-27 14:49:07.000000 ondewo-s2t-client-5.6.0/ondewo/s2t/client/services/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3514 2024-01-27 14:49:07.000000 ondewo-s2t-client-5.6.0/ondewo/s2t/client/services/speech_to_text.py
--rw-rw-r--   0 root         (0) root         (0)      265 2024-01-27 14:49:07.000000 ondewo-s2t-client-5.6.0/ondewo/s2t/client/services_container.py
--rw-rw-r--   0 root         (0) root         (0)    18271 2024-01-27 14:49:13.000000 ondewo-s2t-client-5.6.0/ondewo/s2t/speech_to_text_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    27703 2024-01-27 14:49:13.000000 ondewo-s2t-client-5.6.0/ondewo/s2t/speech_to_text_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-27 14:49:27.965034 ondewo-s2t-client-5.6.0/ondewo_s2t_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6574 2024-01-27 14:49:27.000000 ondewo-s2t-client-5.6.0/ondewo_s2t_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      562 2024-01-27 14:49:27.000000 ondewo-s2t-client-5.6.0/ondewo_s2t_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-27 14:49:27.000000 ondewo-s2t-client-5.6.0/ondewo_s2t_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       89 2024-01-27 14:49:27.000000 ondewo-s2t-client-5.6.0/ondewo_s2t_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-01-27 14:49:27.000000 ondewo-s2t-client-5.6.0/ondewo_s2t_client.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       67 2024-01-27 14:49:27.965034 ondewo-s2t-client-5.6.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1094 2024-01-27 14:49:17.000000 ondewo-s2t-client-5.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:21:12.567415 ondewo-s2t-client-5.7.0/
+-rw-r--r--   0 root         (0) root         (0)     6574 2024-04-16 13:21:12.567415 ondewo-s2t-client-5.7.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     6020 2024-04-16 13:19:12.000000 ondewo-s2t-client-5.7.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:21:12.567415 ondewo-s2t-client-5.7.0/ondewo/
+-rw-rw-r--   0 root         (0) root         (0)       81 2024-04-16 13:19:12.000000 ondewo-s2t-client-5.7.0/ondewo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:21:12.567415 ondewo-s2t-client-5.7.0/ondewo/s2t/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-16 13:19:12.000000 ondewo-s2t-client-5.7.0/ondewo/s2t/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:21:12.567415 ondewo-s2t-client-5.7.0/ondewo/s2t/client/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-16 13:19:12.000000 ondewo-s2t-client-5.7.0/ondewo/s2t/client/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      756 2024-04-16 13:19:12.000000 ondewo-s2t-client-5.7.0/ondewo/s2t/client/client.py
+-rw-rw-r--   0 root         (0) root         (0)      262 2024-04-16 13:19:12.000000 ondewo-s2t-client-5.7.0/ondewo/s2t/client/client_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:21:12.567415 ondewo-s2t-client-5.7.0/ondewo/s2t/client/services/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-16 13:19:12.000000 ondewo-s2t-client-5.7.0/ondewo/s2t/client/services/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3514 2024-04-16 13:19:12.000000 ondewo-s2t-client-5.7.0/ondewo/s2t/client/services/speech_to_text.py
+-rw-rw-r--   0 root         (0) root         (0)      265 2024-04-16 13:19:12.000000 ondewo-s2t-client-5.7.0/ondewo/s2t/client/services_container.py
+-rw-rw-r--   0 root         (0) root         (0)    18309 2024-04-16 13:19:19.000000 ondewo-s2t-client-5.7.0/ondewo/s2t/speech_to_text_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    27703 2024-04-16 13:19:19.000000 ondewo-s2t-client-5.7.0/ondewo/s2t/speech_to_text_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:21:12.567415 ondewo-s2t-client-5.7.0/ondewo_s2t_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6574 2024-04-16 13:21:12.000000 ondewo-s2t-client-5.7.0/ondewo_s2t_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      562 2024-04-16 13:21:12.000000 ondewo-s2t-client-5.7.0/ondewo_s2t_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 13:21:12.000000 ondewo-s2t-client-5.7.0/ondewo_s2t_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       89 2024-04-16 13:21:12.000000 ondewo-s2t-client-5.7.0/ondewo_s2t_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-16 13:21:12.000000 ondewo-s2t-client-5.7.0/ondewo_s2t_client.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)       67 2024-04-16 13:21:12.571415 ondewo-s2t-client-5.7.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1094 2024-04-16 13:19:24.000000 ondewo-s2t-client-5.7.0/setup.py
```

### Comparing `ondewo-s2t-client-5.6.0/PKG-INFO` & `ondewo-s2t-client-5.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ondewo-s2t-client
-Version: 5.6.0
+Version: 5.7.0
 Summary: exposes the ondewo-s2t-grpc-server endpoints in a user-friendly way
 Home-page: https://github.com/ondewo/ondewo-s2t-client-python
 Author: ONDEWO GbmH
 Author-email: info@ondewo.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ondewo-s2t-client Version: 5.6.0 Summary: exposes
+Metadata-Version: 2.1 Name: ondewo-s2t-client Version: 5.7.0 Summary: exposes
 the ondewo-s2t-grpc-server endpoints in a user-friendly way Home-page: https://
 github.com/ondewo/ondewo-s2t-client-python Author: ONDEWO GbmH Author-email:
 info@ondewo.com License: UNKNOWN Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha Classifier: Topic :: Software
 Development :: Libraries Requires-Python: >=2.7, !=3.0.1 Description-Content-
 Type: text/markdown
```

### Comparing `ondewo-s2t-client-5.6.0/README.md` & `ondewo-s2t-client-5.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ondewo-s2t-client-5.6.0/ondewo/s2t/client/client.py` & `ondewo-s2t-client-5.7.0/ondewo/s2t/client/client.py`

 * *Files identical despite different names*

### Comparing `ondewo-s2t-client-5.6.0/ondewo/s2t/client/services/speech_to_text.py` & `ondewo-s2t-client-5.7.0/ondewo/s2t/client/services/speech_to_text.py`

 * *Files identical despite different names*

### Comparing `ondewo-s2t-client-5.6.0/ondewo/s2t/speech_to_text_pb2.py` & `ondewo-s2t-client-5.7.0/ondewo/s2t/speech_to_text_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fondewo/s2t/speech-to-text.proto\x12\nondewo.s2t\x1a\x1bgoogle/protobuf/empty.proto\"\xb0\x04\n\x17TranscribeRequestConfig\x12\x17\n\x0fs2t_pipeline_id\x18\x01 \x01(\t\x12&\n\x08\x64\x65\x63oding\x18\x02 \x01(\x0e\x32\x14.ondewo.s2t.Decoding\x12\x1d\n\x13language_model_name\x18\x03 \x01(\tH\x00\x12<\n\x0fpost_processing\x18\x04 \x01(\x0b\x32!.ondewo.s2t.PostProcessingOptionsH\x01\x12\x44\n\x13utterance_detection\x18\x05 \x01(\x0b\x32%.ondewo.s2t.UtteranceDetectionOptionsH\x02\x12(\n\x08pyannote\x18\x06 \x01(\x0b\x32\x14.ondewo.s2t.PyannoteH\x03\x12@\n\x0ereturn_options\x18\x08 \x01(\x0b\x32&.ondewo.s2t.TranscriptionReturnOptionsH\x04\x12\x15\n\x08language\x18\t \x01(\tH\x05\x88\x01\x01\x12\x11\n\x04task\x18\n \x01(\tH\x06\x88\x01\x01\x42\x1b\n\x19oneof_language_model_nameB\x17\n\x15oneof_post_processingB\x1b\n\x19oneof_utterance_detectionB\x1a\n\x18voice_activity_detectionB\x16\n\x14oneof_return_optionsB\x0b\n\t_languageB\x07\n\x05_task\"\xaf\x02\n\x1aTranscriptionReturnOptions\x12\x1e\n\x16return_start_of_speech\x18\x01 \x01(\x08\x12\x14\n\x0creturn_audio\x18\x02 \x01(\x08\x12\x1f\n\x17return_confidence_score\x18\x03 \x01(\x08\x12)\n!return_alternative_transcriptions\x18\x04 \x01(\x08\x12,\n$return_alternative_transcriptions_nr\x18\x05 \x01(\x05\x12 \n\x18return_alternative_words\x18\x06 \x01(\x08\x12#\n\x1breturn_alternative_words_nr\x18\x07 \x01(\x05\x12\x1a\n\x12return_word_timing\x18\x08 \x01(\x08\"u\n\x19UtteranceDetectionOptions\x12\x1e\n\x14transcribe_not_final\x18\x01 \x01(\x08H\x00\x12\x1a\n\x12next_chunk_timeout\x18\x02 \x01(\x02\x42\x1c\n\x1aoneof_transcribe_not_final\"s\n\x15PostProcessingOptions\x12\x1b\n\x13spelling_correction\x18\x01 \x01(\x08\x12\x11\n\tnormalize\x18\x02 \x01(\x08\x12*\n\x06\x63onfig\x18\x03 \x01(\x0b\x32\x1a.ondewo.s2t.PostProcessing\"\xa3\x01\n\rTranscription\x12\x15\n\rtranscription\x18\x01 \x01(\t\x12\x18\n\x10\x63onfidence_score\x18\x02 \x01(\x02\x12%\n\x05words\x18\x03 \x03(\x0b\x32\x16.ondewo.s2t.WordDetail\x12:\n\x0c\x61lternatives\x18\x04 \x03(\x0b\x32$.ondewo.s2t.TranscriptionAlternative\"i\n\x18TranscriptionAlternative\x12\x12\n\ntranscript\x18\x01 \x01(\t\x12\x12\n\nconfidence\x18\x02 \x01(\x02\x12%\n\x05words\x18\x03 \x03(\x0b\x32\x16.ondewo.s2t.WordDetail\"\x8c\x01\n\nWordDetail\x12\x12\n\nstart_time\x18\x01 \x01(\x02\x12\x10\n\x08\x65nd_time\x18\x02 \x01(\x02\x12\x0c\n\x04word\x18\x03 \x01(\t\x12\x12\n\nconfidence\x18\x04 \x01(\x02\x12\x36\n\x11word_alternatives\x18\x05 \x03(\x0b\x32\x1b.ondewo.s2t.WordAlternative\"3\n\x0fWordAlternative\x12\x0c\n\x04word\x18\x01 \x01(\t\x12\x12\n\nconfidence\x18\x02 \x01(\x02\"\x8e\x01\n\x17TranscribeStreamRequest\x12\x13\n\x0b\x61udio_chunk\x18\x01 \x01(\x0c\x12\x15\n\rend_of_stream\x18\x02 \x01(\x08\x12\x33\n\x06\x63onfig\x18\x03 \x01(\x0b\x32#.ondewo.s2t.TranscribeRequestConfig\x12\x12\n\nmute_audio\x18\x04 \x01(\x08\"\x83\x02\n\x18TranscribeStreamResponse\x12\x31\n\x0etranscriptions\x18\x01 \x03(\x0b\x32\x19.ondewo.s2t.Transcription\x12\x0c\n\x04time\x18\x02 \x01(\x02\x12\r\n\x05\x66inal\x18\x03 \x01(\x08\x12\x14\n\x0creturn_audio\x18\x04 \x01(\x08\x12\r\n\x05\x61udio\x18\x05 \x01(\x0c\x12\x17\n\x0futterance_start\x18\x06 \x01(\x08\x12\x12\n\naudio_uuid\x18\x07 \x01(\t\x12\x35\n\x06\x63onfig\x18\x08 \x01(\x0b\x32#.ondewo.s2t.TranscribeRequestConfigH\x00\x42\x0e\n\x0coneof_config\"`\n\x15TranscribeFileRequest\x12\x12\n\naudio_file\x18\x01 \x01(\x0c\x12\x33\n\x06\x63onfig\x18\x02 \x01(\x0b\x32#.ondewo.s2t.TranscribeRequestConfig\"m\n\x16TranscribeFileResponse\x12\x31\n\x0etranscriptions\x18\x01 \x03(\x0b\x32\x19.ondewo.s2t.Transcription\x12\x0c\n\x04time\x18\x02 \x01(\x02\x12\x12\n\naudio_uuid\x18\x03 \x01(\t\"\x1b\n\rS2tPipelineId\x12\n\n\x02id\x18\x01 \x01(\t\"o\n\x17ListS2tPipelinesRequest\x12\x11\n\tlanguages\x18\x01 \x03(\t\x12\x17\n\x0fpipeline_owners\x18\x02 \x03(\t\x12\x0f\n\x07\x64omains\x18\x03 \x03(\t\x12\x17\n\x0fregistered_only\x18\x04 \x01(\x08\"S\n\x18ListS2tPipelinesResponse\x12\x37\n\x10pipeline_configs\x18\x01 \x03(\x0b\x32\x1d.ondewo.s2t.Speech2TextConfig\"C\n\x17ListS2tLanguagesRequest\x12\x0f\n\x07\x64omains\x18\x01 \x03(\t\x12\x17\n\x0fpipeline_owners\x18\x02 \x03(\t\"-\n\x18ListS2tLanguagesResponse\x12\x11\n\tlanguages\x18\x01 \x03(\t\"C\n\x15ListS2tDomainsRequest\x12\x11\n\tlanguages\x18\x01 \x03(\t\x12\x17\n\x0fpipeline_owners\x18\x02 \x03(\t\")\n\x16ListS2tDomainsResponse\x12\x0f\n\x07\x64omains\x18\x01 \x03(\t\",\n\x19S2TGetServiceInfoResponse\x12\x0f\n\x07version\x18\x01 \x01(\t\"\xe5\x02\n\x11Speech2TextConfig\x12\n\n\x02id\x18\x01 \x01(\t\x12/\n\x0b\x64\x65scription\x18\x02 \x01(\x0b\x32\x1a.ondewo.s2t.S2TDescription\x12\x0e\n\x06\x61\x63tive\x18\x03 \x01(\x08\x12+\n\tinference\x18\x04 \x01(\x0b\x32\x18.ondewo.s2t.S2TInference\x12\x35\n\x10streaming_server\x18\x05 \x01(\x0b\x32\x1b.ondewo.s2t.StreamingServer\x12\x44\n\x18voice_activity_detection\x18\x06 \x01(\x0b\x32\".ondewo.s2t.VoiceActivityDetection\x12\x33\n\x0fpost_processing\x18\x07 \x01(\x0b\x32\x1a.ondewo.s2t.PostProcessing\x12$\n\x07logging\x18\x08 \x01(\x0b\x32\x13.ondewo.s2t.Logging\"\\\n\x0eS2TDescription\x12\x10\n\x08language\x18\x01 \x01(\t\x12\x16\n\x0epipeline_owner\x18\x02 \x01(\t\x12\x0e\n\x06\x64omain\x18\x03 \x01(\t\x12\x10\n\x08\x63omments\x18\x04 \x01(\t\"\xb1\x01\n\x0cS2TInference\x12\x33\n\x0f\x61\x63oustic_models\x18\x01 \x01(\x0b\x32\x1a.ondewo.s2t.AcousticModels\x12\x33\n\x0flanguage_models\x18\x02 \x01(\x0b\x32\x1a.ondewo.s2t.LanguageModels\x12\x37\n\x11inference_backend\x18\x03 \x01(\x0e\x32\x1c.ondewo.s2t.InferenceBackend\"\xd0\x01\n\x0e\x41\x63ousticModels\x12\x0c\n\x04type\x18\x01 \x01(\t\x12$\n\x07wav2vec\x18\x02 \x01(\x0b\x32\x13.ondewo.s2t.Wav2Vec\x12\x31\n\x0ewav2vec_triton\x18\x03 \x01(\x0b\x32\x19.ondewo.s2t.Wav2VecTriton\x12$\n\x07whisper\x18\x04 \x01(\x0b\x32\x13.ondewo.s2t.Whisper\x12\x31\n\x0ewhisper_triton\x18\x05 \x01(\x0b\x32\x19.ondewo.s2t.WhisperTriton\"N\n\x07Whisper\x12\x12\n\nmodel_path\x18\x01 \x01(\t\x12\x0f\n\x07use_gpu\x18\x02 \x01(\x08\x12\x10\n\x08language\x18\x03 \x01(\t\x12\x0c\n\x04task\x18\x04 \x01(\t\"\xd6\x01\n\rWhisperTriton\x12\x16\n\x0eprocessor_path\x18\x01 \x01(\t\x12\x19\n\x11triton_model_name\x18\x02 \x01(\t\x12\x1c\n\x14triton_model_version\x18\x03 \x01(\t\x12\x1c\n\x14\x63heck_status_timeout\x18\x04 \x01(\x03\x12\x10\n\x08language\x18\x05 \x01(\t\x12\x0c\n\x04task\x18\x06 \x01(\t\x12\x1a\n\x12triton_server_host\x18\x07 \x01(\t\x12\x1a\n\x12triton_server_port\x18\x08 \x01(\x03\".\n\x07Wav2Vec\x12\x12\n\nmodel_path\x18\x01 \x01(\t\x12\x0f\n\x07use_gpu\x18\x02 \x01(\x08\"\xb6\x01\n\rWav2VecTriton\x12\x16\n\x0eprocessor_path\x18\x01 \x01(\t\x12\x19\n\x11triton_model_name\x18\x02 \x01(\t\x12\x1c\n\x14triton_model_version\x18\x03 \x01(\t\x12\x1c\n\x14\x63heck_status_timeout\x18\x04 \x01(\x03\x12\x1a\n\x12triton_server_host\x18\x05 \x01(\t\x12\x1a\n\x12triton_server_port\x18\x06 \x01(\x03\"%\n\x07PtFiles\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x0c\n\x04step\x18\x02 \x01(\t\"\x18\n\x08\x43kptFile\x12\x0c\n\x04path\x18\x01 \x01(\t\"\x88\x01\n\x0eLanguageModels\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x11\n\tbeam_size\x18\x02 \x01(\x03\x12\x12\n\ndefault_lm\x18\x03 \x01(\t\x12 \n\x18\x62\x65\x61m_search_scorer_alpha\x18\x04 \x01(\x02\x12\x1f\n\x17\x62\x65\x61m_search_scorer_beta\x18\x05 \x01(\x02\"\x91\x01\n\x0fStreamingServer\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x03\x12\x14\n\x0coutput_style\x18\x03 \x01(\t\x12L\n\x1cstreaming_speech_recognition\x18\x04 \x01(\x0b\x32&.ondewo.s2t.StreamingSpeechRecognition\"\xa4\x01\n\x1aStreamingSpeechRecognition\x12\x1c\n\x14transcribe_not_final\x18\x01 \x01(\x08\x12\x17\n\x0f\x64\x65\x63oding_method\x18\x02 \x01(\t\x12\x15\n\rsampling_rate\x18\x03 \x01(\x03\x12\x1c\n\x14min_audio_chunk_size\x18\x04 \x01(\x03\x12\x1a\n\x12next_chunk_timeout\x18\x05 \x01(\x02\"g\n\x16VoiceActivityDetection\x12\x0e\n\x06\x61\x63tive\x18\x01 \x01(\t\x12\x15\n\rsampling_rate\x18\x02 \x01(\x03\x12&\n\x08pyannote\x18\x03 \x01(\x0b\x32\x14.ondewo.s2t.Pyannote\"\xa1\x01\n\x08Pyannote\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x16\n\x0emin_audio_size\x18\x02 \x01(\x03\x12\x18\n\x10min_duration_off\x18\x03 \x01(\x02\x12\x17\n\x0fmin_duration_on\x18\x04 \x01(\x02\x12\x1a\n\x12triton_server_host\x18\x05 \x01(\t\x12\x1a\n\x12triton_server_port\x18\x06 \x01(\x03\"W\n\x0ePostProcessing\x12\x10\n\x08pipeline\x18\x01 \x03(\t\x12\x33\n\x0fpost_processors\x18\x02 \x01(\x0b\x32\x1a.ondewo.s2t.PostProcessors\"n\n\x0ePostProcessors\x12\'\n\tsym_spell\x18\x01 \x01(\x0b\x32\x14.ondewo.s2t.SymSpell\x12\x33\n\rnormalization\x18\x02 \x01(\x0b\x32\x1c.ondewo.s2t.S2TNormalization\"Z\n\x08SymSpell\x12\x11\n\tdict_path\x18\x01 \x01(\t\x12$\n\x1cmax_dictionary_edit_distance\x18\x02 \x01(\x03\x12\x15\n\rprefix_length\x18\x03 \x01(\x03\"$\n\x10S2TNormalization\x12\x10\n\x08language\x18\x01 \x01(\t\"%\n\x07Logging\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"+\n\x1cListS2tLanguageModelsRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\"C\n\x17LanguageModelPipelineId\x12\x13\n\x0bpipeline_id\x18\x01 \x01(\t\x12\x13\n\x0bmodel_names\x18\x02 \x03(\t\"]\n\x1dListS2tLanguageModelsResponse\x12<\n\x0flm_pipeline_ids\x18\x01 \x03(\x0b\x32#.ondewo.s2t.LanguageModelPipelineId\"=\n\x1e\x43reateUserLanguageModelRequest\x12\x1b\n\x13language_model_name\x18\x01 \x01(\t\"=\n\x1e\x44\x65leteUserLanguageModelRequest\x12\x1b\n\x13language_model_name\x18\x01 \x01(\t\"U\n!AddDataToUserLanguageModelRequest\x12\x1b\n\x13language_model_name\x18\x01 \x01(\t\x12\x13\n\x0bzipped_data\x18\x02 \x01(\x0c\"K\n\x1dTrainUserLanguageModelRequest\x12\x1b\n\x13language_model_name\x18\x01 \x01(\t\x12\r\n\x05order\x18\x02 \x01(\x03*M\n\x08\x44\x65\x63oding\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\n\n\x06GREEDY\x10\x01\x12\x17\n\x13\x42\x45\x41M_SEARCH_WITH_LM\x10\x02\x12\x0f\n\x0b\x42\x45\x41M_SEARCH\x10\x03*l\n\x10InferenceBackend\x12\x1d\n\x19INFERENCE_BACKEND_UNKNOWN\x10\x00\x12\x1d\n\x19INFERENCE_BACKEND_PYTORCH\x10\x01\x12\x1a\n\x16INFERENCE_BACKEND_FLAX\x10\x02\x32\xec\n\n\x0bSpeech2Text\x12Y\n\x0eTranscribeFile\x12!.ondewo.s2t.TranscribeFileRequest\x1a\".ondewo.s2t.TranscribeFileResponse\"\x00\x12\x63\n\x10TranscribeStream\x12#.ondewo.s2t.TranscribeStreamRequest\x1a$.ondewo.s2t.TranscribeStreamResponse\"\x00(\x01\x30\x01\x12L\n\x0eGetS2tPipeline\x12\x19.ondewo.s2t.S2tPipelineId\x1a\x1d.ondewo.s2t.Speech2TextConfig\"\x00\x12O\n\x11\x43reateS2tPipeline\x12\x1d.ondewo.s2t.Speech2TextConfig\x1a\x19.ondewo.s2t.S2tPipelineId\"\x00\x12H\n\x11\x44\x65leteS2tPipeline\x12\x19.ondewo.s2t.S2tPipelineId\x1a\x16.google.protobuf.Empty\"\x00\x12L\n\x11UpdateS2tPipeline\x12\x1d.ondewo.s2t.Speech2TextConfig\x1a\x16.google.protobuf.Empty\"\x00\x12_\n\x10ListS2tPipelines\x12#.ondewo.s2t.ListS2tPipelinesRequest\x1a$.ondewo.s2t.ListS2tPipelinesResponse\"\x00\x12_\n\x10ListS2tLanguages\x12#.ondewo.s2t.ListS2tLanguagesRequest\x1a$.ondewo.s2t.ListS2tLanguagesResponse\"\x00\x12Y\n\x0eListS2tDomains\x12!.ondewo.s2t.ListS2tDomainsRequest\x1a\".ondewo.s2t.ListS2tDomainsResponse\"\x00\x12Q\n\x0eGetServiceInfo\x12\x16.google.protobuf.Empty\x1a%.ondewo.s2t.S2TGetServiceInfoResponse\"\x00\x12n\n\x15ListS2tLanguageModels\x12(.ondewo.s2t.ListS2tLanguageModelsRequest\x1a).ondewo.s2t.ListS2tLanguageModelsResponse\"\x00\x12_\n\x17\x43reateUserLanguageModel\x12*.ondewo.s2t.CreateUserLanguageModelRequest\x1a\x16.google.protobuf.Empty\"\x00\x12_\n\x17\x44\x65leteUserLanguageModel\x12*.ondewo.s2t.DeleteUserLanguageModelRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x65\n\x1a\x41\x64\x64\x44\x61taToUserLanguageModel\x12-.ondewo.s2t.AddDataToUserLanguageModelRequest\x1a\x16.google.protobuf.Empty\"\x00\x12]\n\x16TrainUserLanguageModel\x12).ondewo.s2t.TrainUserLanguageModelRequest\x1a\x16.google.protobuf.Empty\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fondewo/s2t/speech-to-text.proto\x12\nondewo.s2t\x1a\x1bgoogle/protobuf/empty.proto\"\xb0\x04\n\x17TranscribeRequestConfig\x12\x17\n\x0fs2t_pipeline_id\x18\x01 \x01(\t\x12&\n\x08\x64\x65\x63oding\x18\x02 \x01(\x0e\x32\x14.ondewo.s2t.Decoding\x12\x1d\n\x13language_model_name\x18\x03 \x01(\tH\x00\x12<\n\x0fpost_processing\x18\x04 \x01(\x0b\x32!.ondewo.s2t.PostProcessingOptionsH\x01\x12\x44\n\x13utterance_detection\x18\x05 \x01(\x0b\x32%.ondewo.s2t.UtteranceDetectionOptionsH\x02\x12(\n\x08pyannote\x18\x06 \x01(\x0b\x32\x14.ondewo.s2t.PyannoteH\x03\x12@\n\x0ereturn_options\x18\x08 \x01(\x0b\x32&.ondewo.s2t.TranscriptionReturnOptionsH\x04\x12\x15\n\x08language\x18\t \x01(\tH\x05\x88\x01\x01\x12\x11\n\x04task\x18\n \x01(\tH\x06\x88\x01\x01\x42\x1b\n\x19oneof_language_model_nameB\x17\n\x15oneof_post_processingB\x1b\n\x19oneof_utterance_detectionB\x1a\n\x18voice_activity_detectionB\x16\n\x14oneof_return_optionsB\x0b\n\t_languageB\x07\n\x05_task\"\xaf\x02\n\x1aTranscriptionReturnOptions\x12\x1e\n\x16return_start_of_speech\x18\x01 \x01(\x08\x12\x14\n\x0creturn_audio\x18\x02 \x01(\x08\x12\x1f\n\x17return_confidence_score\x18\x03 \x01(\x08\x12)\n!return_alternative_transcriptions\x18\x04 \x01(\x08\x12,\n$return_alternative_transcriptions_nr\x18\x05 \x01(\x05\x12 \n\x18return_alternative_words\x18\x06 \x01(\x08\x12#\n\x1breturn_alternative_words_nr\x18\x07 \x01(\x05\x12\x1a\n\x12return_word_timing\x18\x08 \x01(\x08\"u\n\x19UtteranceDetectionOptions\x12\x1e\n\x14transcribe_not_final\x18\x01 \x01(\x08H\x00\x12\x1a\n\x12next_chunk_timeout\x18\x02 \x01(\x02\x42\x1c\n\x1aoneof_transcribe_not_final\"s\n\x15PostProcessingOptions\x12\x1b\n\x13spelling_correction\x18\x01 \x01(\x08\x12\x11\n\tnormalize\x18\x02 \x01(\x08\x12*\n\x06\x63onfig\x18\x03 \x01(\x0b\x32\x1a.ondewo.s2t.PostProcessing\"\xa3\x01\n\rTranscription\x12\x15\n\rtranscription\x18\x01 \x01(\t\x12\x18\n\x10\x63onfidence_score\x18\x02 \x01(\x02\x12%\n\x05words\x18\x03 \x03(\x0b\x32\x16.ondewo.s2t.WordDetail\x12:\n\x0c\x61lternatives\x18\x04 \x03(\x0b\x32$.ondewo.s2t.TranscriptionAlternative\"i\n\x18TranscriptionAlternative\x12\x12\n\ntranscript\x18\x01 \x01(\t\x12\x12\n\nconfidence\x18\x02 \x01(\x02\x12%\n\x05words\x18\x03 \x03(\x0b\x32\x16.ondewo.s2t.WordDetail\"\x8c\x01\n\nWordDetail\x12\x12\n\nstart_time\x18\x01 \x01(\x02\x12\x10\n\x08\x65nd_time\x18\x02 \x01(\x02\x12\x0c\n\x04word\x18\x03 \x01(\t\x12\x12\n\nconfidence\x18\x04 \x01(\x02\x12\x36\n\x11word_alternatives\x18\x05 \x03(\x0b\x32\x1b.ondewo.s2t.WordAlternative\"3\n\x0fWordAlternative\x12\x0c\n\x04word\x18\x01 \x01(\t\x12\x12\n\nconfidence\x18\x02 \x01(\x02\"\x8e\x01\n\x17TranscribeStreamRequest\x12\x13\n\x0b\x61udio_chunk\x18\x01 \x01(\x0c\x12\x15\n\rend_of_stream\x18\x02 \x01(\x08\x12\x33\n\x06\x63onfig\x18\x03 \x01(\x0b\x32#.ondewo.s2t.TranscribeRequestConfig\x12\x12\n\nmute_audio\x18\x04 \x01(\x08\"\x83\x02\n\x18TranscribeStreamResponse\x12\x31\n\x0etranscriptions\x18\x01 \x03(\x0b\x32\x19.ondewo.s2t.Transcription\x12\x0c\n\x04time\x18\x02 \x01(\x02\x12\r\n\x05\x66inal\x18\x03 \x01(\x08\x12\x14\n\x0creturn_audio\x18\x04 \x01(\x08\x12\r\n\x05\x61udio\x18\x05 \x01(\x0c\x12\x17\n\x0futterance_start\x18\x06 \x01(\x08\x12\x12\n\naudio_uuid\x18\x07 \x01(\t\x12\x35\n\x06\x63onfig\x18\x08 \x01(\x0b\x32#.ondewo.s2t.TranscribeRequestConfigH\x00\x42\x0e\n\x0coneof_config\"`\n\x15TranscribeFileRequest\x12\x12\n\naudio_file\x18\x01 \x01(\x0c\x12\x33\n\x06\x63onfig\x18\x02 \x01(\x0b\x32#.ondewo.s2t.TranscribeRequestConfig\"m\n\x16TranscribeFileResponse\x12\x31\n\x0etranscriptions\x18\x01 \x03(\x0b\x32\x19.ondewo.s2t.Transcription\x12\x0c\n\x04time\x18\x02 \x01(\x02\x12\x12\n\naudio_uuid\x18\x03 \x01(\t\"\x1b\n\rS2tPipelineId\x12\n\n\x02id\x18\x01 \x01(\t\"o\n\x17ListS2tPipelinesRequest\x12\x11\n\tlanguages\x18\x01 \x03(\t\x12\x17\n\x0fpipeline_owners\x18\x02 \x03(\t\x12\x0f\n\x07\x64omains\x18\x03 \x03(\t\x12\x17\n\x0fregistered_only\x18\x04 \x01(\x08\"S\n\x18ListS2tPipelinesResponse\x12\x37\n\x10pipeline_configs\x18\x01 \x03(\x0b\x32\x1d.ondewo.s2t.Speech2TextConfig\"C\n\x17ListS2tLanguagesRequest\x12\x0f\n\x07\x64omains\x18\x01 \x03(\t\x12\x17\n\x0fpipeline_owners\x18\x02 \x03(\t\"-\n\x18ListS2tLanguagesResponse\x12\x11\n\tlanguages\x18\x01 \x03(\t\"C\n\x15ListS2tDomainsRequest\x12\x11\n\tlanguages\x18\x01 \x03(\t\x12\x17\n\x0fpipeline_owners\x18\x02 \x03(\t\")\n\x16ListS2tDomainsResponse\x12\x0f\n\x07\x64omains\x18\x01 \x03(\t\",\n\x19S2TGetServiceInfoResponse\x12\x0f\n\x07version\x18\x01 \x01(\t\"\xe5\x02\n\x11Speech2TextConfig\x12\n\n\x02id\x18\x01 \x01(\t\x12/\n\x0b\x64\x65scription\x18\x02 \x01(\x0b\x32\x1a.ondewo.s2t.S2TDescription\x12\x0e\n\x06\x61\x63tive\x18\x03 \x01(\x08\x12+\n\tinference\x18\x04 \x01(\x0b\x32\x18.ondewo.s2t.S2TInference\x12\x35\n\x10streaming_server\x18\x05 \x01(\x0b\x32\x1b.ondewo.s2t.StreamingServer\x12\x44\n\x18voice_activity_detection\x18\x06 \x01(\x0b\x32\".ondewo.s2t.VoiceActivityDetection\x12\x33\n\x0fpost_processing\x18\x07 \x01(\x0b\x32\x1a.ondewo.s2t.PostProcessing\x12$\n\x07logging\x18\x08 \x01(\x0b\x32\x13.ondewo.s2t.Logging\"\\\n\x0eS2TDescription\x12\x10\n\x08language\x18\x01 \x01(\t\x12\x16\n\x0epipeline_owner\x18\x02 \x01(\t\x12\x0e\n\x06\x64omain\x18\x03 \x01(\t\x12\x10\n\x08\x63omments\x18\x04 \x01(\t\"\xb1\x01\n\x0cS2TInference\x12\x33\n\x0f\x61\x63oustic_models\x18\x01 \x01(\x0b\x32\x1a.ondewo.s2t.AcousticModels\x12\x33\n\x0flanguage_models\x18\x02 \x01(\x0b\x32\x1a.ondewo.s2t.LanguageModels\x12\x37\n\x11inference_backend\x18\x03 \x01(\x0e\x32\x1c.ondewo.s2t.InferenceBackend\"\xd0\x01\n\x0e\x41\x63ousticModels\x12\x0c\n\x04type\x18\x01 \x01(\t\x12$\n\x07wav2vec\x18\x02 \x01(\x0b\x32\x13.ondewo.s2t.Wav2Vec\x12\x31\n\x0ewav2vec_triton\x18\x03 \x01(\x0b\x32\x19.ondewo.s2t.Wav2VecTriton\x12$\n\x07whisper\x18\x04 \x01(\x0b\x32\x13.ondewo.s2t.Whisper\x12\x31\n\x0ewhisper_triton\x18\x05 \x01(\x0b\x32\x19.ondewo.s2t.WhisperTriton\"N\n\x07Whisper\x12\x12\n\nmodel_path\x18\x01 \x01(\t\x12\x0f\n\x07use_gpu\x18\x02 \x01(\x08\x12\x10\n\x08language\x18\x03 \x01(\t\x12\x0c\n\x04task\x18\x04 \x01(\t\"\xd6\x01\n\rWhisperTriton\x12\x16\n\x0eprocessor_path\x18\x01 \x01(\t\x12\x19\n\x11triton_model_name\x18\x02 \x01(\t\x12\x1c\n\x14triton_model_version\x18\x03 \x01(\t\x12\x1c\n\x14\x63heck_status_timeout\x18\x04 \x01(\x03\x12\x10\n\x08language\x18\x05 \x01(\t\x12\x0c\n\x04task\x18\x06 \x01(\t\x12\x1a\n\x12triton_server_host\x18\x07 \x01(\t\x12\x1a\n\x12triton_server_port\x18\x08 \x01(\x03\".\n\x07Wav2Vec\x12\x12\n\nmodel_path\x18\x01 \x01(\t\x12\x0f\n\x07use_gpu\x18\x02 \x01(\x08\"\xb6\x01\n\rWav2VecTriton\x12\x16\n\x0eprocessor_path\x18\x01 \x01(\t\x12\x19\n\x11triton_model_name\x18\x02 \x01(\t\x12\x1c\n\x14triton_model_version\x18\x03 \x01(\t\x12\x1c\n\x14\x63heck_status_timeout\x18\x04 \x01(\x03\x12\x1a\n\x12triton_server_host\x18\x05 \x01(\t\x12\x1a\n\x12triton_server_port\x18\x06 \x01(\x03\"%\n\x07PtFiles\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x0c\n\x04step\x18\x02 \x01(\t\"\x18\n\x08\x43kptFile\x12\x0c\n\x04path\x18\x01 \x01(\t\"\x88\x01\n\x0eLanguageModels\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x11\n\tbeam_size\x18\x02 \x01(\x03\x12\x12\n\ndefault_lm\x18\x03 \x01(\t\x12 \n\x18\x62\x65\x61m_search_scorer_alpha\x18\x04 \x01(\x02\x12\x1f\n\x17\x62\x65\x61m_search_scorer_beta\x18\x05 \x01(\x02\"\x91\x01\n\x0fStreamingServer\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x03\x12\x14\n\x0coutput_style\x18\x03 \x01(\t\x12L\n\x1cstreaming_speech_recognition\x18\x04 \x01(\x0b\x32&.ondewo.s2t.StreamingSpeechRecognition\"\xa4\x01\n\x1aStreamingSpeechRecognition\x12\x1c\n\x14transcribe_not_final\x18\x01 \x01(\x08\x12\x17\n\x0f\x64\x65\x63oding_method\x18\x02 \x01(\t\x12\x15\n\rsampling_rate\x18\x03 \x01(\x03\x12\x1c\n\x14min_audio_chunk_size\x18\x04 \x01(\x03\x12\x1a\n\x12next_chunk_timeout\x18\x05 \x01(\x02\"g\n\x16VoiceActivityDetection\x12\x0e\n\x06\x61\x63tive\x18\x01 \x01(\t\x12\x15\n\rsampling_rate\x18\x02 \x01(\x03\x12&\n\x08pyannote\x18\x03 \x01(\x0b\x32\x14.ondewo.s2t.Pyannote\"\xa1\x01\n\x08Pyannote\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x16\n\x0emin_audio_size\x18\x02 \x01(\x03\x12\x18\n\x10min_duration_off\x18\x03 \x01(\x02\x12\x17\n\x0fmin_duration_on\x18\x04 \x01(\x02\x12\x1a\n\x12triton_server_host\x18\x05 \x01(\t\x12\x1a\n\x12triton_server_port\x18\x06 \x01(\x03\"W\n\x0ePostProcessing\x12\x10\n\x08pipeline\x18\x01 \x03(\t\x12\x33\n\x0fpost_processors\x18\x02 \x01(\x0b\x32\x1a.ondewo.s2t.PostProcessors\"n\n\x0ePostProcessors\x12\'\n\tsym_spell\x18\x01 \x01(\x0b\x32\x14.ondewo.s2t.SymSpell\x12\x33\n\rnormalization\x18\x02 \x01(\x0b\x32\x1c.ondewo.s2t.S2TNormalization\"Z\n\x08SymSpell\x12\x11\n\tdict_path\x18\x01 \x01(\t\x12$\n\x1cmax_dictionary_edit_distance\x18\x02 \x01(\x03\x12\x15\n\rprefix_length\x18\x03 \x01(\x03\"6\n\x10S2TNormalization\x12\x10\n\x08language\x18\x01 \x01(\t\x12\x10\n\x08pipeline\x18\x02 \x03(\t\"%\n\x07Logging\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"+\n\x1cListS2tLanguageModelsRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\"C\n\x17LanguageModelPipelineId\x12\x13\n\x0bpipeline_id\x18\x01 \x01(\t\x12\x13\n\x0bmodel_names\x18\x02 \x03(\t\"]\n\x1dListS2tLanguageModelsResponse\x12<\n\x0flm_pipeline_ids\x18\x01 \x03(\x0b\x32#.ondewo.s2t.LanguageModelPipelineId\"=\n\x1e\x43reateUserLanguageModelRequest\x12\x1b\n\x13language_model_name\x18\x01 \x01(\t\"=\n\x1e\x44\x65leteUserLanguageModelRequest\x12\x1b\n\x13language_model_name\x18\x01 \x01(\t\"U\n!AddDataToUserLanguageModelRequest\x12\x1b\n\x13language_model_name\x18\x01 \x01(\t\x12\x13\n\x0bzipped_data\x18\x02 \x01(\x0c\"K\n\x1dTrainUserLanguageModelRequest\x12\x1b\n\x13language_model_name\x18\x01 \x01(\t\x12\r\n\x05order\x18\x02 \x01(\x03*M\n\x08\x44\x65\x63oding\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\n\n\x06GREEDY\x10\x01\x12\x17\n\x13\x42\x45\x41M_SEARCH_WITH_LM\x10\x02\x12\x0f\n\x0b\x42\x45\x41M_SEARCH\x10\x03*l\n\x10InferenceBackend\x12\x1d\n\x19INFERENCE_BACKEND_UNKNOWN\x10\x00\x12\x1d\n\x19INFERENCE_BACKEND_PYTORCH\x10\x01\x12\x1a\n\x16INFERENCE_BACKEND_FLAX\x10\x02\x32\xec\n\n\x0bSpeech2Text\x12Y\n\x0eTranscribeFile\x12!.ondewo.s2t.TranscribeFileRequest\x1a\".ondewo.s2t.TranscribeFileResponse\"\x00\x12\x63\n\x10TranscribeStream\x12#.ondewo.s2t.TranscribeStreamRequest\x1a$.ondewo.s2t.TranscribeStreamResponse\"\x00(\x01\x30\x01\x12L\n\x0eGetS2tPipeline\x12\x19.ondewo.s2t.S2tPipelineId\x1a\x1d.ondewo.s2t.Speech2TextConfig\"\x00\x12O\n\x11\x43reateS2tPipeline\x12\x1d.ondewo.s2t.Speech2TextConfig\x1a\x19.ondewo.s2t.S2tPipelineId\"\x00\x12H\n\x11\x44\x65leteS2tPipeline\x12\x19.ondewo.s2t.S2tPipelineId\x1a\x16.google.protobuf.Empty\"\x00\x12L\n\x11UpdateS2tPipeline\x12\x1d.ondewo.s2t.Speech2TextConfig\x1a\x16.google.protobuf.Empty\"\x00\x12_\n\x10ListS2tPipelines\x12#.ondewo.s2t.ListS2tPipelinesRequest\x1a$.ondewo.s2t.ListS2tPipelinesResponse\"\x00\x12_\n\x10ListS2tLanguages\x12#.ondewo.s2t.ListS2tLanguagesRequest\x1a$.ondewo.s2t.ListS2tLanguagesResponse\"\x00\x12Y\n\x0eListS2tDomains\x12!.ondewo.s2t.ListS2tDomainsRequest\x1a\".ondewo.s2t.ListS2tDomainsResponse\"\x00\x12Q\n\x0eGetServiceInfo\x12\x16.google.protobuf.Empty\x1a%.ondewo.s2t.S2TGetServiceInfoResponse\"\x00\x12n\n\x15ListS2tLanguageModels\x12(.ondewo.s2t.ListS2tLanguageModelsRequest\x1a).ondewo.s2t.ListS2tLanguageModelsResponse\"\x00\x12_\n\x17\x43reateUserLanguageModel\x12*.ondewo.s2t.CreateUserLanguageModelRequest\x1a\x16.google.protobuf.Empty\"\x00\x12_\n\x17\x44\x65leteUserLanguageModel\x12*.ondewo.s2t.DeleteUserLanguageModelRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x65\n\x1a\x41\x64\x64\x44\x61taToUserLanguageModel\x12-.ondewo.s2t.AddDataToUserLanguageModelRequest\x1a\x16.google.protobuf.Empty\"\x00\x12]\n\x16TrainUserLanguageModel\x12).ondewo.s2t.TrainUserLanguageModelRequest\x1a\x16.google.protobuf.Empty\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'ondewo.s2t.speech_to_text_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
-  _globals['_DECODING']._serialized_start=5799
-  _globals['_DECODING']._serialized_end=5876
-  _globals['_INFERENCEBACKEND']._serialized_start=5878
-  _globals['_INFERENCEBACKEND']._serialized_end=5986
+  _globals['_DECODING']._serialized_start=5817
+  _globals['_DECODING']._serialized_end=5894
+  _globals['_INFERENCEBACKEND']._serialized_start=5896
+  _globals['_INFERENCEBACKEND']._serialized_end=6004
   _globals['_TRANSCRIBEREQUESTCONFIG']._serialized_start=77
   _globals['_TRANSCRIBEREQUESTCONFIG']._serialized_end=637
   _globals['_TRANSCRIPTIONRETURNOPTIONS']._serialized_start=640
   _globals['_TRANSCRIPTIONRETURNOPTIONS']._serialized_end=943
   _globals['_UTTERANCEDETECTIONOPTIONS']._serialized_start=945
   _globals['_UTTERANCEDETECTIONOPTIONS']._serialized_end=1062
   _globals['_POSTPROCESSINGOPTIONS']._serialized_start=1064
@@ -98,27 +98,27 @@
   _globals['_POSTPROCESSING']._serialized_start=4930
   _globals['_POSTPROCESSING']._serialized_end=5017
   _globals['_POSTPROCESSORS']._serialized_start=5019
   _globals['_POSTPROCESSORS']._serialized_end=5129
   _globals['_SYMSPELL']._serialized_start=5131
   _globals['_SYMSPELL']._serialized_end=5221
   _globals['_S2TNORMALIZATION']._serialized_start=5223
-  _globals['_S2TNORMALIZATION']._serialized_end=5259
-  _globals['_LOGGING']._serialized_start=5261
-  _globals['_LOGGING']._serialized_end=5298
-  _globals['_LISTS2TLANGUAGEMODELSREQUEST']._serialized_start=5300
-  _globals['_LISTS2TLANGUAGEMODELSREQUEST']._serialized_end=5343
-  _globals['_LANGUAGEMODELPIPELINEID']._serialized_start=5345
-  _globals['_LANGUAGEMODELPIPELINEID']._serialized_end=5412
-  _globals['_LISTS2TLANGUAGEMODELSRESPONSE']._serialized_start=5414
-  _globals['_LISTS2TLANGUAGEMODELSRESPONSE']._serialized_end=5507
-  _globals['_CREATEUSERLANGUAGEMODELREQUEST']._serialized_start=5509
-  _globals['_CREATEUSERLANGUAGEMODELREQUEST']._serialized_end=5570
-  _globals['_DELETEUSERLANGUAGEMODELREQUEST']._serialized_start=5572
-  _globals['_DELETEUSERLANGUAGEMODELREQUEST']._serialized_end=5633
-  _globals['_ADDDATATOUSERLANGUAGEMODELREQUEST']._serialized_start=5635
-  _globals['_ADDDATATOUSERLANGUAGEMODELREQUEST']._serialized_end=5720
-  _globals['_TRAINUSERLANGUAGEMODELREQUEST']._serialized_start=5722
-  _globals['_TRAINUSERLANGUAGEMODELREQUEST']._serialized_end=5797
-  _globals['_SPEECH2TEXT']._serialized_start=5989
-  _globals['_SPEECH2TEXT']._serialized_end=7377
+  _globals['_S2TNORMALIZATION']._serialized_end=5277
+  _globals['_LOGGING']._serialized_start=5279
+  _globals['_LOGGING']._serialized_end=5316
+  _globals['_LISTS2TLANGUAGEMODELSREQUEST']._serialized_start=5318
+  _globals['_LISTS2TLANGUAGEMODELSREQUEST']._serialized_end=5361
+  _globals['_LANGUAGEMODELPIPELINEID']._serialized_start=5363
+  _globals['_LANGUAGEMODELPIPELINEID']._serialized_end=5430
+  _globals['_LISTS2TLANGUAGEMODELSRESPONSE']._serialized_start=5432
+  _globals['_LISTS2TLANGUAGEMODELSRESPONSE']._serialized_end=5525
+  _globals['_CREATEUSERLANGUAGEMODELREQUEST']._serialized_start=5527
+  _globals['_CREATEUSERLANGUAGEMODELREQUEST']._serialized_end=5588
+  _globals['_DELETEUSERLANGUAGEMODELREQUEST']._serialized_start=5590
+  _globals['_DELETEUSERLANGUAGEMODELREQUEST']._serialized_end=5651
+  _globals['_ADDDATATOUSERLANGUAGEMODELREQUEST']._serialized_start=5653
+  _globals['_ADDDATATOUSERLANGUAGEMODELREQUEST']._serialized_end=5738
+  _globals['_TRAINUSERLANGUAGEMODELREQUEST']._serialized_start=5740
+  _globals['_TRAINUSERLANGUAGEMODELREQUEST']._serialized_end=5815
+  _globals['_SPEECH2TEXT']._serialized_start=6007
+  _globals['_SPEECH2TEXT']._serialized_end=7395
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-s2t-client-5.6.0/ondewo/s2t/speech_to_text_pb2_grpc.py` & `ondewo-s2t-client-5.7.0/ondewo/s2t/speech_to_text_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-s2t-client-5.6.0/ondewo_s2t_client.egg-info/PKG-INFO` & `ondewo-s2t-client-5.7.0/ondewo_s2t_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ondewo-s2t-client
-Version: 5.6.0
+Version: 5.7.0
 Summary: exposes the ondewo-s2t-grpc-server endpoints in a user-friendly way
 Home-page: https://github.com/ondewo/ondewo-s2t-client-python
 Author: ONDEWO GbmH
 Author-email: info@ondewo.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ondewo-s2t-client Version: 5.6.0 Summary: exposes
+Metadata-Version: 2.1 Name: ondewo-s2t-client Version: 5.7.0 Summary: exposes
 the ondewo-s2t-grpc-server endpoints in a user-friendly way Home-page: https://
 github.com/ondewo/ondewo-s2t-client-python Author: ONDEWO GbmH Author-email:
 info@ondewo.com License: UNKNOWN Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha Classifier: Topic :: Software
 Development :: Libraries Requires-Python: >=2.7, !=3.0.1 Description-Content-
 Type: text/markdown
```

### Comparing `ondewo-s2t-client-5.6.0/ondewo_s2t_client.egg-info/SOURCES.txt` & `ondewo-s2t-client-5.7.0/ondewo_s2t_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ondewo-s2t-client-5.6.0/setup.py` & `ondewo-s2t-client-5.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open('requirements.txt') as f:
     requires = f.read().splitlines()
 
 setup(
     name="ondewo-s2t-client",
-    version='5.6.0',
+    version='5.7.0',
     author="ONDEWO GbmH",
     author_email="info@ondewo.com",
     description="exposes the ondewo-s2t-grpc-server endpoints in a user-friendly way",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/ondewo/ondewo-s2t-client-python',
     packages=[
```

