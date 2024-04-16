# Comparing `tmp/icad_tone_detection-0.7.tar.gz` & `tmp/icad_tone_detection-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icad_tone_detection-0.7.tar", last modified: Sat Apr 13 22:35:34 2024, max compression
+gzip compressed data, was "icad_tone_detection-0.8.tar", last modified: Tue Apr 16 05:21:29 2024, max compression
```

## Comparing `icad_tone_detection-0.7.tar` & `icad_tone_detection-0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 ian       (2000) ian       (2000)        0 2024-04-13 22:35:34.677511 icad_tone_detection-0.7/
-drwxrwxr-x   0 ian       (2000) ian       (2000)        0 2024-04-13 22:35:34.677511 icad_tone_detection-0.7/.github/
-drwxrwxr-x   0 ian       (2000) ian       (2000)        0 2024-04-13 22:35:34.677511 icad_tone_detection-0.7/.github/workflows/
--rw-rw-r--   0 ian       (2000) ian       (2000)     1301 2024-03-18 00:28:15.000000 icad_tone_detection-0.7/.github/workflows/python-package.yml
--rw-rw-r--   0 ian       (2000) ian       (2000)     3084 2024-03-14 21:16:01.000000 icad_tone_detection-0.7/.gitignore
--rw-rw-r--   0 ian       (2000) ian       (2000)      555 2024-03-17 23:53:26.000000 icad_tone_detection-0.7/LICENSE
--rw-r--r--   0 ian       (2000) ian       (2000)     1166 2024-04-13 22:35:34.677511 icad_tone_detection-0.7/PKG-INFO
--rw-rw-r--   0 ian       (2000) ian       (2000)      457 2024-03-18 00:11:11.000000 icad_tone_detection-0.7/README.md
--rw-rw-r--   0 ian       (2000) ian       (2000)      592 2024-03-17 23:50:50.000000 icad_tone_detection-0.7/detect_test.py
--rw-rw-r--   0 ian       (2000) ian       (2000)      779 2024-04-13 22:34:32.000000 icad_tone_detection-0.7/pyproject.toml
--rw-rw-r--   0 ian       (2000) ian       (2000)       38 2024-04-13 22:35:34.677511 icad_tone_detection-0.7/setup.cfg
--rw-rw-r--   0 ian       (2000) ian       (2000)       38 2024-03-18 00:11:11.000000 icad_tone_detection-0.7/setup.py
-drwxrwxr-x   0 ian       (2000) ian       (2000)        0 2024-04-13 22:35:34.677511 icad_tone_detection-0.7/src/
-drwxrwxr-x   0 ian       (2000) ian       (2000)        0 2024-04-13 22:35:34.677511 icad_tone_detection-0.7/src/icad_tone_detection/
--rw-rw-r--   0 ian       (2000) ian       (2000)       57 2024-03-14 20:41:31.000000 icad_tone_detection-0.7/src/icad_tone_detection/__init__.py
--rw-rw-r--   0 ian       (2000) ian       (2000)     2599 2024-03-18 01:16:38.000000 icad_tone_detection-0.7/src/icad_tone_detection/audio_loader.py
--rw-rw-r--   0 ian       (2000) ian       (2000)     5855 2024-03-12 18:45:10.000000 icad_tone_detection-0.7/src/icad_tone_detection/frequency_extraction.py
--rw-rw-r--   0 ian       (2000) ian       (2000)     2454 2024-03-16 00:09:53.000000 icad_tone_detection-0.7/src/icad_tone_detection/main.py
--rw-rw-r--   0 ian       (2000) ian       (2000)    11538 2024-04-13 22:34:32.000000 icad_tone_detection-0.7/src/icad_tone_detection/tone_detection.py
-drwxrwxr-x   0 ian       (2000) ian       (2000)        0 2024-04-13 22:35:34.677511 icad_tone_detection-0.7/src/icad_tone_detection.egg-info/
--rw-r--r--   0 ian       (2000) ian       (2000)     1166 2024-04-13 22:35:34.000000 icad_tone_detection-0.7/src/icad_tone_detection.egg-info/PKG-INFO
--rw-rw-r--   0 ian       (2000) ian       (2000)      536 2024-04-13 22:35:34.000000 icad_tone_detection-0.7/src/icad_tone_detection.egg-info/SOURCES.txt
--rw-rw-r--   0 ian       (2000) ian       (2000)        1 2024-04-13 22:35:34.000000 icad_tone_detection-0.7/src/icad_tone_detection.egg-info/dependency_links.txt
--rw-rw-r--   0 ian       (2000) ian       (2000)       59 2024-04-13 22:35:34.000000 icad_tone_detection-0.7/src/icad_tone_detection.egg-info/requires.txt
--rw-rw-r--   0 ian       (2000) ian       (2000)       20 2024-04-13 22:35:34.000000 icad_tone_detection-0.7/src/icad_tone_detection.egg-info/top_level.txt
+drwxrwxr-x   0 ian       (2000) ian       (2000)        0 2024-04-16 05:21:29.621400 icad_tone_detection-0.8/
+drwxrwxr-x   0 ian       (2000) ian       (2000)        0 2024-04-16 05:21:29.621400 icad_tone_detection-0.8/.github/
+drwxrwxr-x   0 ian       (2000) ian       (2000)        0 2024-04-16 05:21:29.621400 icad_tone_detection-0.8/.github/workflows/
+-rw-rw-r--   0 ian       (2000) ian       (2000)     1301 2024-03-18 00:28:15.000000 icad_tone_detection-0.8/.github/workflows/python-package.yml
+-rw-rw-r--   0 ian       (2000) ian       (2000)     3084 2024-03-14 21:16:01.000000 icad_tone_detection-0.8/.gitignore
+-rw-rw-r--   0 ian       (2000) ian       (2000)      555 2024-03-17 23:53:26.000000 icad_tone_detection-0.8/LICENSE
+-rw-r--r--   0 ian       (2000) ian       (2000)     1166 2024-04-16 05:21:29.621400 icad_tone_detection-0.8/PKG-INFO
+-rw-rw-r--   0 ian       (2000) ian       (2000)      457 2024-03-18 00:11:11.000000 icad_tone_detection-0.8/README.md
+-rw-rw-r--   0 ian       (2000) ian       (2000)      627 2024-04-16 04:52:45.000000 icad_tone_detection-0.8/detect_test.py
+-rw-rw-r--   0 ian       (2000) ian       (2000)      779 2024-04-16 04:42:10.000000 icad_tone_detection-0.8/pyproject.toml
+-rw-rw-r--   0 ian       (2000) ian       (2000)       38 2024-04-16 05:21:29.621400 icad_tone_detection-0.8/setup.cfg
+-rw-rw-r--   0 ian       (2000) ian       (2000)       38 2024-03-18 00:11:11.000000 icad_tone_detection-0.8/setup.py
+drwxrwxr-x   0 ian       (2000) ian       (2000)        0 2024-04-16 05:21:29.621400 icad_tone_detection-0.8/src/
+drwxrwxr-x   0 ian       (2000) ian       (2000)        0 2024-04-16 05:21:29.621400 icad_tone_detection-0.8/src/icad_tone_detection/
+-rw-rw-r--   0 ian       (2000) ian       (2000)       57 2024-03-14 20:41:31.000000 icad_tone_detection-0.8/src/icad_tone_detection/__init__.py
+-rw-rw-r--   0 ian       (2000) ian       (2000)     2599 2024-03-18 01:16:38.000000 icad_tone_detection-0.8/src/icad_tone_detection/audio_loader.py
+-rw-rw-r--   0 ian       (2000) ian       (2000)     5855 2024-03-12 18:45:10.000000 icad_tone_detection-0.8/src/icad_tone_detection/frequency_extraction.py
+-rw-rw-r--   0 ian       (2000) ian       (2000)     2977 2024-04-16 05:12:10.000000 icad_tone_detection-0.8/src/icad_tone_detection/main.py
+-rw-rw-r--   0 ian       (2000) ian       (2000)    13039 2024-04-16 05:05:49.000000 icad_tone_detection-0.8/src/icad_tone_detection/tone_detection.py
+drwxrwxr-x   0 ian       (2000) ian       (2000)        0 2024-04-16 05:21:29.621400 icad_tone_detection-0.8/src/icad_tone_detection.egg-info/
+-rw-r--r--   0 ian       (2000) ian       (2000)     1166 2024-04-16 05:21:29.000000 icad_tone_detection-0.8/src/icad_tone_detection.egg-info/PKG-INFO
+-rw-rw-r--   0 ian       (2000) ian       (2000)      536 2024-04-16 05:21:29.000000 icad_tone_detection-0.8/src/icad_tone_detection.egg-info/SOURCES.txt
+-rw-rw-r--   0 ian       (2000) ian       (2000)        1 2024-04-16 05:21:29.000000 icad_tone_detection-0.8/src/icad_tone_detection.egg-info/dependency_links.txt
+-rw-rw-r--   0 ian       (2000) ian       (2000)       59 2024-04-16 05:21:29.000000 icad_tone_detection-0.8/src/icad_tone_detection.egg-info/requires.txt
+-rw-rw-r--   0 ian       (2000) ian       (2000)       20 2024-04-16 05:21:29.000000 icad_tone_detection-0.8/src/icad_tone_detection.egg-info/top_level.txt
```

### Comparing `icad_tone_detection-0.7/.github/workflows/python-package.yml` & `icad_tone_detection-0.8/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `icad_tone_detection-0.7/.gitignore` & `icad_tone_detection-0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `icad_tone_detection-0.7/LICENSE` & `icad_tone_detection-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `icad_tone_detection-0.7/PKG-INFO` & `icad_tone_detection-0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icad_tone_detection
-Version: 0.7
+Version: 0.8
 Summary: A Python library for extracting scanner radio tones from scanner audio.
 Author-email: TheGreatCodeholio <ian@icarey.net>
 Project-URL: Homepage, https://github.com/thegreatcodeholio/icad_tone_detection
 Project-URL: Issues, https://github.com/thegreatcodeholio/icad_tone_detection/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `icad_tone_detection-0.7/detect_test.py` & `icad_tone_detection-0.8/detect_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 if len(sys.argv) > 1:
     audio_path = sys.argv[1]
 else:
     print("Requires a audio path provided. Either file path, or URL.")
     exit(0)
 
-detect_result = tone_detect(audio_path)
+detect_result = tone_detect(audio_path, time_resolution_ms=50, debug=True)
 
 if len(detect_result.two_tone_result) == 0 and len(detect_result.long_result) == 0 and len(detect_result.hi_low_result) == 0:
     print("No tones")
 
 data_dict = {"two_tone": detect_result.two_tone_result, "long_tone": detect_result.long_result, "hl_tone": detect_result.hi_low_result}
 
 print(json.dumps(data_dict))
```

### Comparing `icad_tone_detection-0.7/pyproject.toml` & `icad_tone_detection-0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "icad_tone_detection"
-version = "0.7"
+version = "0.8"
 authors = [
   {name = "TheGreatCodeholio", email = "ian@icarey.net"},
 ]
 description = "A Python library for extracting scanner radio tones from scanner audio."
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
```

### Comparing `icad_tone_detection-0.7/src/icad_tone_detection/audio_loader.py` & `icad_tone_detection-0.8/src/icad_tone_detection/audio_loader.py`

 * *Files identical despite different names*

### Comparing `icad_tone_detection-0.7/src/icad_tone_detection/frequency_extraction.py` & `icad_tone_detection-0.8/src/icad_tone_detection/frequency_extraction.py`

 * *Files identical despite different names*

### Comparing `icad_tone_detection-0.7/src/icad_tone_detection/main.py` & `icad_tone_detection-0.8/src/icad_tone_detection/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 from .audio_loader import load_audio
 from .frequency_extraction import FrequencyExtraction
-from .tone_detection import detect_quickcall, detect_long_tones, detect_warble_tones
+from .tone_detection import detect_two_tone, detect_long_tones, detect_warble_tones
 
 
 class ToneDetectionResult:
     def __init__(self, two_tone_result, long_result, hi_low_result):
         self.two_tone_result = two_tone_result
         self.long_result = long_result
         self.hi_low_result = hi_low_result
 
 
-def tone_detect(audio_path, matching_threshold=2, time_resolution_ms=100, hi_low_interval=0.2,
-                hi_low_min_alternations=2, debug=False):
+def tone_detect(audio_path, matching_threshold=2, time_resolution_ms=100, tone_a_min_length=0.8, tone_b_min_length=2.8, hi_low_interval=0.2,
+                hi_low_min_alternations=3, long_tone_min_length=2.0, debug=False):
     """
         Loads audio from various sources including local path, URL, BytesIO object, or a PyDub AudioSegment.
 
         Parameters:
            - audio_input: Can be a string (path or URL), bytes like object, or AudioSegment.
            - matching_threshold (float): The percentage threshold used to determine if two frequencies
                 are considered a match. For example, a threshold of 2 means that two frequencies are considered matching
                 if they are within 2% of each other.
            - time_resolution_ms (int): The time resolution in milliseconds for the STFT. Default is 100ms.
-           - hi_low_interval (float): The maximum allowed interval in seconds between two consecutive alternating tones. Default is 0.2
+           - tone_a_min_length (float): The minimum length in seconds of an A tone for two tone detections. Default 0.8 Seconds
+           - tone_b_min_length (float): The minimum length in seconds of a B tone for two tone detections. Default 2.8 Seconds
+           - long_tone_min_length (float): The minimum length a long tone needs to be to consider it a match. Default 2.0 Seconds
+           - hi_low_interval (float): The maximum allowed interval in seconds between two consecutive alternating tones. Default is 0.2 Seconds
            - hi_low_min_alternations (int): The minimum number of alternations for a hi-low warble tone sequence to be considered valid. Default 2
            - debug (bool): If debug is enabled, print all tones found in audio file. Default is False
 
         Returns:
            - An instance of ToneDetectionResult containing information about the found tones in the audio.
 
         Raises:
@@ -35,11 +38,11 @@
     samples, frame_rate, duration_seconds = load_audio(audio_path)
 
     matched_frequencies = FrequencyExtraction(samples, frame_rate, duration_seconds, matching_threshold,
                                               time_resolution_ms).get_audio_frequencies()
     if debug is True:
         print("Matched frequencies: ", matched_frequencies)
 
-    two_tone_result = detect_quickcall(matched_frequencies)
-    long_result = detect_long_tones(matched_frequencies, two_tone_result)
+    two_tone_result = detect_two_tone(matched_frequencies, tone_a_min_length, tone_b_min_length)
+    long_result = detect_long_tones(matched_frequencies, two_tone_result, long_tone_min_length)
     hi_low_result = detect_warble_tones(matched_frequencies, hi_low_interval, hi_low_min_alternations)
     return ToneDetectionResult(two_tone_result, long_result, hi_low_result)
```

### Comparing `icad_tone_detection-0.7/src/icad_tone_detection/tone_detection.py` & `icad_tone_detection-0.8/src/icad_tone_detection/tone_detection.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,90 @@
-def detect_quickcall(frequency_matches):
-    qc2_matches = []
+# def detect_quickcall(frequency_matches):
+#     qc2_matches = []
+#     tone_id = 0
+#     last_set = None
+#     if not frequency_matches or len(frequency_matches) < 1:
+#         return qc2_matches
+#     for x in frequency_matches:
+#         if last_set is None and len(x[2]) >= 8 and 0 not in x[2] and 0.0 not in x[2]:
+#             last_set = x
+#         else:
+#             if len(x[2]) >= 8 and 0 not in x[2] and 0.0 not in x[2]:
+#                 if len(last_set[2]) <= 12 and len(x[2]) >= 28:
+#                     tone_data = {"tone_id": f'qc_{tone_id + 1}', "detected": [last_set[2][0], x[2][0]],
+#                                  "start": last_set[0], "end": x[1]}
+#                     tone_id += 1
+#                     qc2_matches.append(tone_data)
+#                     last_set = x
+#                 else:
+#                     last_set = x
+#
+#     return qc2_matches
+
+
+def detect_two_tone(frequency_matches, min_tone_a_length=0.8, min_tone_b_length=2.8):
+    two_tone_matches = []
     tone_id = 0
     last_set = None
     if not frequency_matches or len(frequency_matches) < 1:
-        return qc2_matches
-    for x in frequency_matches:
-        if last_set is None and len(x[2]) >= 8 and 0 not in x[2] and 0.0 not in x[2]:
-            last_set = x
-        else:
-            if len(x[2]) >= 8 and 0 not in x[2] and 0.0 not in x[2]:
-                if len(last_set[2]) <= 12 and len(x[2]) >= 28:
-                    tone_data = {"tone_id": f'qc_{tone_id + 1}', "detected": [last_set[2][0], x[2][0]],
-                                 "start": last_set[0], "end": x[1]}
+        return two_tone_matches
+
+    for current_set in frequency_matches:
+        if all(f > 0 for f in current_set[2]):  # Ensure frequencies are non-zero
+            current_duration = current_set[1] - current_set[0]  # Calculate the duration of the current tone
+
+            if last_set is None:
+                last_set = current_set
+            else:
+                last_duration = last_set[1] - last_set[0]  # Calculate the duration of the last tone
+                # Check if the last tone is a valid A tone and the current is a valid B tone
+                if last_duration >= min_tone_a_length and current_duration >= min_tone_b_length:
+                    tone_data = {
+                        "tone_id": f'qc_{tone_id + 1}',
+                        "detected": [last_set[2][0], current_set[2][0]],  # Frequency values of A and B tones
+                        "start": last_set[0],  # Start time of tone A
+                        "end": current_set[1]  # End time of tone B
+                    }
                     tone_id += 1
-                    qc2_matches.append(tone_data)
-                    last_set = x
-                else:
-                    last_set = x
+                    two_tone_matches.append(tone_data)
+                # Update last_set to current_set for next iteration
+                last_set = current_set
 
-    return qc2_matches
+    return two_tone_matches
 
 
-def detect_long_tones(frequency_matches, detected_quickcall):
-    tone_id = 0
+def detect_long_tones(frequency_matches, detected_quickcall, min_duration=2.0):
     long_tone_matches = []
-    excluded_frequencies = set([])
+    excluded_frequencies = set([0.0])  # Initializing with 0.0 Hz to exclude it
 
-    if not frequency_matches or len(frequency_matches) < 1:
-        return long_tone_matches
-
-    last_set = frequency_matches[0]
-    # add detected quick call tones to a list, so we can exclude them from long tone matches.
-    for ttd in detected_quickcall:
-        excluded_frequencies.update(ttd["detected"][:2])
-
-    for x in frequency_matches:
-        if len(x[2]) >= 10:
-            if 12 >= len(last_set) >= 8 and len(x[2]) >= 20:
-                last_set = x[2]
-            elif len(x[2]) >= 15:
-                if x[2][0] == 0 or x[2][0] == 0.0:
-                    continue
-                if x[2][0] in excluded_frequencies:
-                    continue
-
-                if x[2][0] > 250:
-                    tone_data = {"tone_id": f'lt_{tone_id + 1}', "detected": x[2][0], "start": round(x[0], 3),
-                                 "end": round(x[1], 3)}
-                    tone_id += 1
-                    long_tone_matches.append(tone_data)
+    # Add detected quick call tones to the excluded list
+    for quickcall in detected_quickcall:
+        excluded_frequencies.update(quickcall["detected"][:2])
+
+    for start, end, frequencies in frequency_matches:
+        duration = end - start
+        if not frequencies:
+            continue
+
+        current_frequency = frequencies[0]
+
+        # Skip the loop iteration if the current frequency is in the excluded frequencies
+        if current_frequency in excluded_frequencies or current_frequency <= 500:
+            continue
+
+        # Check if the duration meets the minimum requirement
+        if duration >= min_duration:
+            tone_data = {
+                "tone_id": f"lt_{len(long_tone_matches) + 1}",
+                "detected": current_frequency,
+                "start": start,
+                "end": end,
+                "length": duration
+            }
+            long_tone_matches.append(tone_data)
 
     return long_tone_matches
 
 
 # def extract_warble_tones(frequency_matches, interval_length, min_alternations):
 #     """
 #     Extract sequences of alternating tones (warble tones) from detected tones,
```

### Comparing `icad_tone_detection-0.7/src/icad_tone_detection.egg-info/PKG-INFO` & `icad_tone_detection-0.8/src/icad_tone_detection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icad_tone_detection
-Version: 0.7
+Version: 0.8
 Summary: A Python library for extracting scanner radio tones from scanner audio.
 Author-email: TheGreatCodeholio <ian@icarey.net>
 Project-URL: Homepage, https://github.com/thegreatcodeholio/icad_tone_detection
 Project-URL: Issues, https://github.com/thegreatcodeholio/icad_tone_detection/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `icad_tone_detection-0.7/src/icad_tone_detection.egg-info/SOURCES.txt` & `icad_tone_detection-0.8/src/icad_tone_detection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

