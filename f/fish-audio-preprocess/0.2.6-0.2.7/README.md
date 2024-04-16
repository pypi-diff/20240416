# Comparing `tmp/fish-audio-preprocess-0.2.6.tar.gz` & `tmp/fish_audio_preprocess-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fish-audio-preprocess-0.2.6.tar", last modified: Thu Nov  2 10:37:50 2023, max compression
+gzip compressed data, was "fish_audio_preprocess-0.2.7.tar", last modified: Tue Apr 16 07:01:58 2024, max compression
```

## Comparing `fish-audio-preprocess-0.2.6.tar` & `fish_audio_preprocess-0.2.7.tar`

### file list

```diff
@@ -1,39 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 10:37:50.212516 fish-audio-preprocess-0.2.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 10:37:50.200516 fish-audio-preprocess-0.2.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 10:37:50.204516 fish-audio-preprocess-0.2.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2023-11-02 10:34:34.000000 fish-audio-preprocess-0.2.6/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2023-11-02 10:34:34.000000 fish-audio-preprocess-0.2.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      358 2023-11-02 10:34:34.000000 fish-audio-preprocess-0.2.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2023-11-02 10:34:34.000000 fish-audio-preprocess-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2023-11-02 10:37:50.212516 fish-audio-preprocess-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      715 2023-11-02 10:34:34.000000 fish-audio-preprocess-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      663 2023-11-02 10:34:34.000000 fish-audio-preprocess-0.2.6/README.zh.md
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-11-02 10:34:34.000000 fish-audio-preprocess-0.2.6/fap-complete.zsh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 10:37:50.204516 fish-audio-preprocess-0.2.6/fish_audio_preprocess/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-02 10:34:34.000000 fish-audio-preprocess-0.2.6/fish_audio_preprocess/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 10:37:50.208516 fish-audio-preprocess-0.2.6/fish_audio_preprocess/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      808 2023-11-02 10:34:34.000000 fish-audio-preprocess-0.2.6/fish_audio_preprocess/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2023-11-02 10:34:34.000000 fish-audio-preprocess-0.2.6/fish_audio_preprocess/cli/convert_to_wav.py
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2023-11-02 10:34:34.000000 fish-audio-preprocess-0.2.6/fish_audio_preprocess/cli/frequency.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2023-11-02 10:34:34.000000 fish-audio-preprocess-0.2.6/fish_audio_preprocess/cli/length.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2023-11-02 10:34:34.000000 fish-audio-preprocess-0.2.6/fish_audio_preprocess/cli/loudness_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2023-11-02 10:34:34.000000 fish-audio-preprocess-0.2.6/fish_audio_preprocess/cli/resample.py
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2023-11-02 10:34:34.000000 fish-audio-preprocess-0.2.6/fish_audio_preprocess/cli/separate_audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     7504 2023-11-02 10:34:34.000000 fish-audio-preprocess-0.2.6/fish_audio_preprocess/cli/slice_audio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 10:37:50.212516 fish-audio-preprocess-0.2.6/fish_audio_preprocess/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2023-11-02 10:34:34.000000 fish-audio-preprocess-0.2.6/fish_audio_preprocess/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2023-11-02 10:34:34.000000 fish-audio-preprocess-0.2.6/fish_audio_preprocess/utils/loudness_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2023-11-02 10:34:34.000000 fish-audio-preprocess-0.2.6/fish_audio_preprocess/utils/separate_audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3869 2023-11-02 10:34:34.000000 fish-audio-preprocess-0.2.6/fish_audio_preprocess/utils/slice_audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     8619 2023-11-02 10:34:34.000000 fish-audio-preprocess-0.2.6/fish_audio_preprocess/utils/slice_audio_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 10:37:50.204516 fish-audio-preprocess-0.2.6/fish_audio_preprocess.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2023-11-02 10:37:50.000000 fish-audio-preprocess-0.2.6/fish_audio_preprocess.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      981 2023-11-02 10:37:50.000000 fish-audio-preprocess-0.2.6/fish_audio_preprocess.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-02 10:37:50.000000 fish-audio-preprocess-0.2.6/fish_audio_preprocess.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-11-02 10:37:50.000000 fish-audio-preprocess-0.2.6/fish_audio_preprocess.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      145 2023-11-02 10:37:50.000000 fish-audio-preprocess-0.2.6/fish_audio_preprocess.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-02 10:37:50.000000 fish-audio-preprocess-0.2.6/fish_audio_preprocess.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      701 2023-11-02 10:34:34.000000 fish-audio-preprocess-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-02 10:37:50.212516 fish-audio-preprocess-0.2.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 10:37:50.212516 fish-audio-preprocess-0.2.6/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-11-02 10:34:34.000000 fish-audio-preprocess-0.2.6/tools/lint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:01:58.104560 fish_audio_preprocess-0.2.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:01:58.096560 fish_audio_preprocess-0.2.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:01:58.096560 fish_audio_preprocess-0.2.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-16 07:01:58.104560 fish_audio_preprocess-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/README.zh.md
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/fap-complete.zsh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:01:58.100560 fish_audio_preprocess-0.2.7/fish_audio_preprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:01:58.100560 fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/convert_to_wav.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/frequency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/loudness_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/merge_short.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/resample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/separate_audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8369 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/slice_audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/transcribe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:01:58.104560 fish_audio_preprocess-0.2.7/fish_audio_preprocess/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess/utils/loudness_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess/utils/separate_audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess/utils/slice_audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9832 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess/utils/slice_audio_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess/utils/transcribe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:01:58.104560 fish_audio_preprocess-0.2.7/fish_audio_preprocess.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-16 07:01:58.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-16 07:01:58.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 07:01:58.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-16 07:01:58.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-16 07:01:58.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 07:01:58.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 07:01:58.104560 fish_audio_preprocess-0.2.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:01:58.104560 fish_audio_preprocess-0.2.7/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/tools/lint.py
```

### Comparing `fish-audio-preprocess-0.2.6/.github/workflows/ci.yml` & `fish_audio_preprocess-0.2.7/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fish-audio-preprocess-0.2.6/.gitignore` & `fish_audio_preprocess-0.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `fish-audio-preprocess-0.2.6/LICENSE` & `fish_audio_preprocess-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fish-audio-preprocess-0.2.6/PKG-INFO` & `fish_audio_preprocess-0.2.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fish-audio-preprocess
-Version: 0.2.6
+Version: 0.2.7
 Summary: Preprocess audio data
 Author-email: Lengyue <lengyue@lengyue.me>
 License: Apache
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tqdm>=4.64.1
@@ -12,14 +12,15 @@
 Requires-Dist: loguru>=0.6.0
 Requires-Dist: pyloudnorm>=0.1.1
 Requires-Dist: matplotlib>=3.6.2
 Requires-Dist: librosa>=0.9.0
 Requires-Dist: richuru>=0.1.1
 Requires-Dist: praat-parselmouth>=0.4.3
 Requires-Dist: click>=8.0.0
+Requires-Dist: openai-whisper
 
 # Fish Audio Preprocessor
 
 [![PyPI Version](https://img.shields.io/pypi/v/fish-audio-preprocess.svg)](https://pypi.python.org/pypi/fish-audio-preprocess)
 
 [中文文档](README.zh.md)
 
@@ -27,18 +28,25 @@
 
 - [x] Video/audio to wav
 - [x] Audio vocal separation
 - [x] Automatic audio slicing
 - [x] Audio loudness matching
 - [x] Audio data statistics (supports determining audio length)
 - [x] Audio resampling
+- [x] Audio transcribe (.lab)
+- [ ] Audio transcribe via WhisperX
 
 ([ ] indicates not completed, [x] indicates completed)
 
 **This code has been tested on Ubuntu 22.04 / 20.04 + Python 3.10. If you encounter problems on other versions, feedback is welcome.**
 
 ## Getting Started:
 
 ```
 pip install -e . 
 fap --help
 ```
+
+## Reference
+
+- [Batch Whisper](https://github.com/Blair-Johnson/batch-whisper)
+
```

### Comparing `fish-audio-preprocess-0.2.6/README.md` & `fish_audio_preprocess-0.2.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -8,18 +8,25 @@
 
 - [x] Video/audio to wav
 - [x] Audio vocal separation
 - [x] Automatic audio slicing
 - [x] Audio loudness matching
 - [x] Audio data statistics (supports determining audio length)
 - [x] Audio resampling
+- [x] Audio transcribe (.lab)
+- [ ] Audio transcribe via WhisperX
 
 ([ ] indicates not completed, [x] indicates completed)
 
 **This code has been tested on Ubuntu 22.04 / 20.04 + Python 3.10. If you encounter problems on other versions, feedback is welcome.**
 
 ## Getting Started:
 
 ```
 pip install -e . 
 fap --help
 ```
+
+## Reference
+
+- [Batch Whisper](https://github.com/Blair-Johnson/batch-whisper)
+
```

### Comparing `fish-audio-preprocess-0.2.6/README.zh.md` & `fish_audio_preprocess-0.2.7/README.zh.md`

 * *Files 15% similar despite different names*

```diff
@@ -8,18 +8,24 @@
 
 - [x] 视频/音频转 wav
 - [x] 音频人声分离
 - [x] 音频自动切片
 - [x] 音频响度匹配
 - [x] 音频数据统计（支持判断音频长度）
 - [x] 音频重采样
+- [x] 音频打标 (.lab)
 
 ([ ] 表示未完成, [x] 表示已完成)
 
 **本代码已在 Ubuntu 22.04 / 20.04 + Python 3.10 测试过, 如果在其他版本遇到问题, 欢迎反馈**
 
 ## 上手指南:
 
 ```
 pip install -e . 
 fap --help
 ```
+
+## 引用
+
+- [Batch Whisper](https://github.com/Blair-Johnson/batch-whisper)
+
```

### Comparing `fish-audio-preprocess-0.2.6/fap-complete.zsh` & `fish_audio_preprocess-0.2.7/fap-complete.zsh`

 * *Files identical despite different names*

### Comparing `fish-audio-preprocess-0.2.6/fish_audio_preprocess/cli/__main__.py` & `fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 import richuru
 from loguru import logger
 
 from .convert_to_wav import to_wav
 from .frequency import frequency
 from .length import length
 from .loudness_norm import loudness_norm
+from .merge_short import merge_short
 from .resample import resample
 from .separate_audio import separate
 from .slice_audio import slice_audio, slice_audio_v2
+from .transcribe import transcribe
 
 
 @click.group()
 @click.option("--debug/--no-debug", default=False)
 def cli(debug: bool):
     """An audio preprocessing CLI."""
 
@@ -27,11 +29,13 @@
 
 cli.add_command(to_wav)
 cli.add_command(separate)
 cli.add_command(loudness_norm)
 cli.add_command(slice_audio)
 cli.add_command(slice_audio_v2)
 cli.add_command(resample)
+cli.add_command(transcribe)
+cli.add_command(merge_short)
 
 
 if __name__ == "__main__":
     to_wav()
```

### Comparing `fish-audio-preprocess-0.2.6/fish_audio_preprocess/cli/convert_to_wav.py` & `fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/convert_to_wav.py`

 * *Files identical despite different names*

### Comparing `fish-audio-preprocess-0.2.6/fish_audio_preprocess/cli/frequency.py` & `fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/frequency.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,14 +84,15 @@
     for note, count in data:
         logger.info(f"{note}: {count}")
 
     if not visualize:
         return
 
     x_axis_order = librosa.midi_to_note(list(range(300)))
+    x_axis_order = list(x_axis_order)
     data = sorted(counter.items(), key=lambda kv: x_axis_order.index(kv[0]))
 
     plt.rcParams["figure.figsize"] = [10, 4]
     plt.rcParams["figure.autolayout"] = True
     plt.bar([x[0] for x in data], [x[1] for x in data])
     plt.xticks(rotation=90)
     plt.title("Notes distribution")
```

### Comparing `fish-audio-preprocess-0.2.6/fish_audio_preprocess/cli/length.py` & `fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/length.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,30 @@
+from concurrent.futures import ProcessPoolExecutor
 from pathlib import Path
 from typing import Optional
 
 import click
 from loguru import logger
 from tqdm import tqdm
 
 from fish_audio_preprocess.utils.file import AUDIO_EXTENSIONS, list_files
 
 
+def process_one(file, input_dir):
+    import soundfile as sf
+
+    sound = sf.SoundFile(str(file))
+    return (
+        len(sound),
+        sound.samplerate,
+        len(sound) / sound.samplerate,
+        file.relative_to(input_dir),
+    )
+
+
 @click.command()
 @click.argument("input_dir", type=click.Path(exists=True, file_okay=False))
 @click.option("--recursive/--no-recursive", default=True, help="Search recursively")
 @click.option(
     "--visualize/--no-visualize", default=False, help="Visualize the distribution"
 )
 @click.option(
@@ -30,33 +43,29 @@
     visualize: bool,
     long_threshold: Optional[float],
     short_threshold: Optional[float],
 ):
     """
     Get the length of all audio files in a directory
     """
-
     import soundfile as sf
     from matplotlib import pyplot as plt
 
     input_dir = Path(input_dir)
     files = list_files(input_dir, AUDIO_EXTENSIONS, recursive=recursive)
     logger.info(f"Found {len(files)} files, calculating length")
 
     infos = []
-    for file in tqdm(files, desc="Collecting infos"):
-        sound = sf.SoundFile(str(file))
-        infos.append(
-            (
-                len(sound),
-                sound.samplerate,
-                len(sound) / sound.samplerate,
-                file.relative_to(input_dir),
-            )
-        )
+
+    with ProcessPoolExecutor(max_workers=10) as executor:
+        tasks = []
+        for file in tqdm(files, desc="Preparing"):
+            tasks.append(executor.submit(process_one, file, input_dir))
+        for task in tqdm(tasks, desc="Processing"):
+            infos.append(task.result())
 
     # Duration
     total_duration = sum(i[2] for i in infos)
     avg_duration = total_duration / len(infos)
     logger.info(f"Total duration: {total_duration / 3600:.2f} hours")
     logger.info(f"Average duration: {avg_duration:.2f} seconds")
     logger.info(f"Max duration: {max(i[2] for i in infos):.2f} seconds")
```

### Comparing `fish-audio-preprocess-0.2.6/fish_audio_preprocess/cli/loudness_norm.py` & `fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/loudness_norm.py`

 * *Files identical despite different names*

### Comparing `fish-audio-preprocess-0.2.6/fish_audio_preprocess/cli/resample.py` & `fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/resample.py`

 * *Files identical despite different names*

### Comparing `fish-audio-preprocess-0.2.6/fish_audio_preprocess/cli/separate_audio.py` & `fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/separate_audio.py`

 * *Files identical despite different names*

### Comparing `fish-audio-preprocess-0.2.6/fish_audio_preprocess/cli/slice_audio.py` & `fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/slice_audio.py`

 * *Files 4% similar despite different names*

```diff
@@ -191,34 +191,50 @@
 @click.option(
     "--max-silence-kept",
     help="Maximum duration of each slice",
     default=0.5,
     show_default=True,
     type=float,
 )
+@click.option(
+    "--flat-layout/--no-flat-layout", default=False, help="Use flat directory structure"
+)
+@click.option(
+    "--merge-short/--no-merge-short",
+    default=False,
+    help="Merge short slices automatically",
+)
 def slice_audio_v2(
     input_dir: str,
     output_dir: str,
     recursive: bool,
     overwrite: bool,
     clean: bool,
     num_workers: int,
     min_duration: float,
     max_duration: float,
     min_silence_duration: float,
     top_db: int,
     hop_length: int,
     max_silence_kept: float,
+    flat_layout: bool,
+    merge_short: bool,
 ):
     """(OpenVPI version) Slice audio files into smaller chunks by silence."""
 
     from fish_audio_preprocess.utils.slice_audio_v2 import slice_audio_file_v2
 
     input_dir, output_dir = Path(input_dir), Path(output_dir)
 
+    if flat_layout:
+        logger.info("Using flat directory structure")
+
+    if merge_short:
+        logger.info("Merging short slices automatically")
+
     if input_dir == output_dir and clean:
         logger.error("You are trying to clean the input directory, aborting")
         return
 
     make_dirs(output_dir, clean)
 
     files = list_files(input_dir, extensions=AUDIO_EXTENSIONS, recursive=recursive)
@@ -234,28 +250,38 @@
             relative_path = file.relative_to(input_dir)
             save_path = output_dir / relative_path.parent / relative_path.stem
 
             if save_path.exists() and not overwrite:
                 skipped += 1
                 continue
 
-            if save_path.exists() is False:
-                save_path.mkdir(parents=True)
+            if (
+                output_dir / relative_path.parent / relative_path.stem
+                if not flat_layout
+                else output_dir / relative_path.parent
+            ).exists() is False:
+                (
+                    output_dir / relative_path.parent / relative_path.stem
+                    if not flat_layout
+                    else output_dir / relative_path.parent
+                ).mkdir(parents=True)
 
             tasks.append(
                 executor.submit(
                     slice_audio_file_v2,
                     input_file=str(file),
                     output_dir=save_path,
                     min_duration=min_duration,
                     max_duration=max_duration,
                     min_silence_duration=min_silence_duration,
                     top_db=top_db,
                     hop_length=hop_length,
                     max_silence_kept=max_silence_kept,
+                    flat_layout=flat_layout,
+                    merge_short=merge_short,
                 )
             )
 
         for i in tqdm(as_completed(tasks), total=len(tasks), desc="Processing"):
             assert i.exception() is None, i.exception()
 
     logger.info("Done!")
```

### Comparing `fish-audio-preprocess-0.2.6/fish_audio_preprocess/utils/file.py` & `fish_audio_preprocess-0.2.7/fish_audio_preprocess/utils/file.py`

 * *Files 22% similar despite different names*

```diff
@@ -27,14 +27,19 @@
     ".aac",
     ".aiff",
     ".aif",
     ".aifc",
 }
 
 
+def split_list(lst, n):
+    k, m = divmod(len(lst), n)
+    return [lst[i * k + min(i, m) : (i + 1) * k + min(i + 1, m)] for i in range(n)]
+
+
 def list_files(
     path: Union[Path, str],
     extensions: set[str] = None,
     recursive: bool = False,
     sort: bool = True,
 ) -> list[Path]:
     """List files in a directory.
```

### Comparing `fish-audio-preprocess-0.2.6/fish_audio_preprocess/utils/loudness_norm.py` & `fish_audio_preprocess-0.2.7/fish_audio_preprocess/utils/loudness_norm.py`

 * *Files identical despite different names*

### Comparing `fish-audio-preprocess-0.2.6/fish_audio_preprocess/utils/separate_audio.py` & `fish_audio_preprocess-0.2.7/fish_audio_preprocess/utils/separate_audio.py`

 * *Files identical despite different names*

### Comparing `fish-audio-preprocess-0.2.6/fish_audio_preprocess/utils/slice_audio.py` & `fish_audio_preprocess-0.2.7/fish_audio_preprocess/utils/slice_audio.py`

 * *Files identical despite different names*

### Comparing `fish-audio-preprocess-0.2.6/fish_audio_preprocess/utils/slice_audio_v2.py` & `fish_audio_preprocess-0.2.7/fish_audio_preprocess/utils/slice_audio_v2.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,32 @@
 import librosa
 import numpy as np
 import soundfile as sf
 
 from fish_audio_preprocess.utils.slice_audio import slice_by_max_duration
 
 
+def merge_short_chunks(chunks, max_duration, rate):
+    merged_chunks = []
+    buffer, length = [], 0
+
+    for chunk in chunks:
+        if length + len(chunk) > max_duration * rate and len(buffer) > 0:
+            merged_chunks.append(np.concatenate(buffer))
+            buffer, length = [chunk], 0
+        else:
+            buffer.append(chunk)
+            length += len(chunk)
+
+    if len(buffer) > 0:
+        merged_chunks.append(np.concatenate(buffer))
+
+    return merged_chunks
+
+
 class Slicer:
     def __init__(
         self,
         sr: int,
         threshold: float = -40.0,
         min_length: int = 5000,
         min_interval: int = 300,
@@ -178,82 +196,99 @@
     rate: int,
     min_duration: float = 5.0,
     max_duration: float = 30.0,
     min_silence_duration: float = 0.3,
     top_db: int = -40,
     hop_length: int = 10,
     max_silence_kept: float = 0.5,
+    merge_short: bool = False,
 ) -> Iterable[np.ndarray]:
     """Slice audio by silence
 
     Args:
         audio: audio data, in shape (samples, channels)
         rate: sample rate
         min_duration: minimum duration of each slice
         max_duration: maximum duration of each slice
         min_silence_duration: minimum duration of silence
         top_db: threshold to detect silence
         hop_length: hop length to detect silence
         max_silence_kept: maximum duration of silence to be kept
+        merge_short: merge short slices automatically
 
     Returns:
         Iterable of sliced audio
     """
 
     if len(audio) / rate < min_duration:
-        yield from slice_by_max_duration(audio, max_duration, rate)
+        sliced_by_max_duration_chunk = slice_by_max_duration(audio, max_duration, rate)
+        yield from merge_short_chunks(
+            sliced_by_max_duration_chunk, max_duration, rate
+        ) if merge_short else sliced_by_max_duration_chunk
         return
 
     slicer = Slicer(
         sr=rate,
         threshold=top_db,
         min_length=min_duration * 1000,
         min_interval=min_silence_duration * 1000,
         hop_size=hop_length,
         max_sil_kept=max_silence_kept * 1000,
     )
 
-    for chunk in slicer.slice(audio):
-        yield from slice_by_max_duration(chunk, max_duration, rate)
+    sliced_audio = slicer.slice(audio)
+    if merge_short:
+        sliced_audio = merge_short_chunks(sliced_audio, max_duration, rate)
+
+    for chunk in sliced_audio:
+        sliced_by_max_duration_chunk = slice_by_max_duration(chunk, max_duration, rate)
+        yield from sliced_by_max_duration_chunk
 
 
 def slice_audio_file_v2(
     input_file: Union[str, Path],
     output_dir: Union[str, Path],
     min_duration: float = 5.0,
     max_duration: float = 30.0,
     min_silence_duration: float = 0.3,
     top_db: int = -40,
     hop_length: int = 10,
     max_silence_kept: float = 0.5,
+    flat_layout: bool = False,
+    merge_short: bool = False,
 ) -> None:
     """
     Slice audio by silence and save to output folder
 
     Args:
         input_file: input audio file
         output_dir: output folder
         min_duration: minimum duration of each slice
         max_duration: maximum duration of each slice
         min_silence_duration: minimum duration of silence
         top_db: threshold to detect silence
         hop_length: hop length to detect silence
         max_silence_kept: maximum duration of silence to be kept
+        flat_layout: use flat directory structure
+        merge_short: merge short slices automatically
     """
 
     output_dir = Path(output_dir)
-    output_dir.mkdir(parents=True, exist_ok=True)
 
     audio, rate = librosa.load(str(input_file), sr=None, mono=True)
     for idx, sliced in enumerate(
         slice_audio_v2(
             audio,
             rate,
             min_duration=min_duration,
             max_duration=max_duration,
             min_silence_duration=min_silence_duration,
             top_db=top_db,
             hop_length=hop_length,
             max_silence_kept=max_silence_kept,
+            merge_short=merge_short,
         )
     ):
-        sf.write(str(output_dir / f"{idx:04d}.wav"), sliced, rate)
+        if flat_layout:
+            sf.write(str(output_dir) + f"_{idx:04d}.wav", sliced, rate)
+        else:
+            sf.write(str(output_dir / f"{idx:04d}.wav"), sliced, rate)
```

### Comparing `fish-audio-preprocess-0.2.6/fish_audio_preprocess.egg-info/PKG-INFO` & `fish_audio_preprocess-0.2.7/fish_audio_preprocess.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fish-audio-preprocess
-Version: 0.2.6
+Version: 0.2.7
 Summary: Preprocess audio data
 Author-email: Lengyue <lengyue@lengyue.me>
 License: Apache
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tqdm>=4.64.1
@@ -12,14 +12,15 @@
 Requires-Dist: loguru>=0.6.0
 Requires-Dist: pyloudnorm>=0.1.1
 Requires-Dist: matplotlib>=3.6.2
 Requires-Dist: librosa>=0.9.0
 Requires-Dist: richuru>=0.1.1
 Requires-Dist: praat-parselmouth>=0.4.3
 Requires-Dist: click>=8.0.0
+Requires-Dist: openai-whisper
 
 # Fish Audio Preprocessor
 
 [![PyPI Version](https://img.shields.io/pypi/v/fish-audio-preprocess.svg)](https://pypi.python.org/pypi/fish-audio-preprocess)
 
 [中文文档](README.zh.md)
 
@@ -27,18 +28,25 @@
 
 - [x] Video/audio to wav
 - [x] Audio vocal separation
 - [x] Automatic audio slicing
 - [x] Audio loudness matching
 - [x] Audio data statistics (supports determining audio length)
 - [x] Audio resampling
+- [x] Audio transcribe (.lab)
+- [ ] Audio transcribe via WhisperX
 
 ([ ] indicates not completed, [x] indicates completed)
 
 **This code has been tested on Ubuntu 22.04 / 20.04 + Python 3.10. If you encounter problems on other versions, feedback is welcome.**
 
 ## Getting Started:
 
 ```
 pip install -e . 
 fap --help
 ```
+
+## Reference
+
+- [Batch Whisper](https://github.com/Blair-Johnson/batch-whisper)
+
```

### Comparing `fish-audio-preprocess-0.2.6/fish_audio_preprocess.egg-info/SOURCES.txt` & `fish_audio_preprocess-0.2.7/fish_audio_preprocess.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -14,16 +14,19 @@
 fish_audio_preprocess.egg-info/requires.txt
 fish_audio_preprocess.egg-info/top_level.txt
 fish_audio_preprocess/cli/__main__.py
 fish_audio_preprocess/cli/convert_to_wav.py
 fish_audio_preprocess/cli/frequency.py
 fish_audio_preprocess/cli/length.py
 fish_audio_preprocess/cli/loudness_norm.py
+fish_audio_preprocess/cli/merge_short.py
 fish_audio_preprocess/cli/resample.py
 fish_audio_preprocess/cli/separate_audio.py
 fish_audio_preprocess/cli/slice_audio.py
+fish_audio_preprocess/cli/transcribe.py
 fish_audio_preprocess/utils/file.py
 fish_audio_preprocess/utils/loudness_norm.py
 fish_audio_preprocess/utils/separate_audio.py
 fish_audio_preprocess/utils/slice_audio.py
 fish_audio_preprocess/utils/slice_audio_v2.py
+fish_audio_preprocess/utils/transcribe.py
 tools/lint.py
```

### Comparing `fish-audio-preprocess-0.2.6/pyproject.toml` & `fish_audio_preprocess-0.2.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [project]
 authors = [
   {name = "Lengyue", email = "lengyue@lengyue.me"},
 ]
 dependencies = [
-  "tqdm>=4.64.1",
-  "demucs>=4.0.0",
-  "loguru>=0.6.0",
-  "pyloudnorm>=0.1.1",
-  "matplotlib>=3.6.2",
-  "librosa>=0.9.0",
-  "richuru>=0.1.1",
-  "praat-parselmouth>=0.4.3",
-  "click>=8.0.0",
+    "tqdm>=4.64.1",
+    "demucs>=4.0.0",
+    "loguru>=0.6.0",
+    "pyloudnorm>=0.1.1",
+    "matplotlib>=3.6.2",
+    "librosa>=0.9.0",
+    "richuru>=0.1.1",
+    "praat-parselmouth>=0.4.3",
+    "click>=8.0.0",
+    "openai-whisper",
 ]
 description = "Preprocess audio data"
 license = {text = "Apache"}
 name = "fish-audio-preprocess"
 readme = "README.md"
 requires-python = ">=3.9"
-version = "0.2.6"
+version = "0.2.7"
 
 [project.scripts]
 fap = "fish_audio_preprocess.cli.__main__:cli"
 
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
```

