# Comparing `tmp/flavpy-1.0.1.tar.gz` & `tmp/flavpy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flavpy-1.0.1.tar", last modified: Fri Nov 24 06:54:09 2023, max compression
+gzip compressed data, was "flavpy-1.0.2.tar", last modified: Tue Apr 16 15:36:26 2024, max compression
```

## Comparing `flavpy-1.0.1.tar` & `flavpy-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 taiyuu     (501) staff       (20)        0 2023-11-24 06:54:09.307060 flavpy-1.0.1/
--rw-r--r--   0 taiyuu     (501) staff       (20)     1776 2023-11-24 06:54:09.306931 flavpy-1.0.1/PKG-INFO
--rw-r--r--   0 taiyuu     (501) staff       (20)     1322 2023-11-24 05:23:19.000000 flavpy-1.0.1/README.md
-drwxr-xr-x   0 taiyuu     (501) staff       (20)        0 2023-11-24 06:54:09.304718 flavpy-1.0.1/flavpy/
--rw-r--r--   0 taiyuu     (501) staff       (20)      148 2023-11-24 06:53:39.000000 flavpy-1.0.1/flavpy/__init__.py
-drwxr-xr-x   0 taiyuu     (501) staff       (20)        0 2023-11-24 06:54:09.305765 flavpy-1.0.1/flavpy/capture/
--rw-r--r--   0 taiyuu     (501) staff       (20)       84 2023-11-14 15:21:10.000000 flavpy-1.0.1/flavpy/capture/__init__.py
--rw-r--r--   0 taiyuu     (501) staff       (20)     6119 2023-11-24 04:10:06.000000 flavpy-1.0.1/flavpy/capture/_capture.py
-drwxr-xr-x   0 taiyuu     (501) staff       (20)        0 2023-11-24 06:54:09.306169 flavpy-1.0.1/flavpy/inspector/
--rw-r--r--   0 taiyuu     (501) staff       (20)       32 2023-11-24 06:53:39.000000 flavpy-1.0.1/flavpy/inspector/__init__.py
--rw-r--r--   0 taiyuu     (501) staff       (20)      844 2023-11-24 04:10:06.000000 flavpy-1.0.1/flavpy/inspector/inspector.py
-drwxr-xr-x   0 taiyuu     (501) staff       (20)        0 2023-11-24 06:54:09.306644 flavpy-1.0.1/flavpy/writer/
--rw-r--r--   0 taiyuu     (501) staff       (20)       31 2023-11-18 12:37:09.000000 flavpy-1.0.1/flavpy/writer/__init__.py
--rw-r--r--   0 taiyuu     (501) staff       (20)     3656 2023-11-24 04:14:23.000000 flavpy-1.0.1/flavpy/writer/_writer.py
-drwxr-xr-x   0 taiyuu     (501) staff       (20)        0 2023-11-24 06:54:09.305406 flavpy-1.0.1/flavpy.egg-info/
--rw-r--r--   0 taiyuu     (501) staff       (20)     1776 2023-11-24 06:54:09.000000 flavpy-1.0.1/flavpy.egg-info/PKG-INFO
--rw-r--r--   0 taiyuu     (501) staff       (20)      350 2023-11-24 06:54:09.000000 flavpy-1.0.1/flavpy.egg-info/SOURCES.txt
--rw-r--r--   0 taiyuu     (501) staff       (20)        1 2023-11-24 06:54:09.000000 flavpy-1.0.1/flavpy.egg-info/dependency_links.txt
--rw-r--r--   0 taiyuu     (501) staff       (20)        9 2023-11-24 06:54:09.000000 flavpy-1.0.1/flavpy.egg-info/requires.txt
--rw-r--r--   0 taiyuu     (501) staff       (20)        7 2023-11-24 06:54:09.000000 flavpy-1.0.1/flavpy.egg-info/top_level.txt
--rw-r--r--   0 taiyuu     (501) staff       (20)       38 2023-11-24 06:54:09.307097 flavpy-1.0.1/setup.cfg
--rw-r--r--   0 taiyuu     (501) staff       (20)      724 2023-11-24 06:54:05.000000 flavpy-1.0.1/setup.py
+drwxr-xr-x   0 taiyuu     (501) staff       (20)        0 2024-04-16 15:36:26.180201 flavpy-1.0.2/
+-rw-r--r--   0 taiyuu     (501) staff       (20)     1877 2024-04-16 15:36:26.179958 flavpy-1.0.2/PKG-INFO
+-rw-r--r--   0 taiyuu     (501) staff       (20)     1322 2023-11-24 05:23:19.000000 flavpy-1.0.2/README.md
+drwxr-xr-x   0 taiyuu     (501) staff       (20)        0 2024-04-16 15:36:26.176847 flavpy-1.0.2/flavpy/
+-rw-r--r--   0 taiyuu     (501) staff       (20)      189 2023-12-15 12:40:18.000000 flavpy-1.0.2/flavpy/__init__.py
+drwxr-xr-x   0 taiyuu     (501) staff       (20)        0 2024-04-16 15:36:26.178194 flavpy-1.0.2/flavpy/capture/
+-rw-r--r--   0 taiyuu     (501) staff       (20)       84 2023-11-14 15:21:10.000000 flavpy-1.0.2/flavpy/capture/__init__.py
+-rw-r--r--   0 taiyuu     (501) staff       (20)     6545 2023-12-17 16:07:35.000000 flavpy-1.0.2/flavpy/capture/_capture.py
+drwxr-xr-x   0 taiyuu     (501) staff       (20)        0 2024-04-16 15:36:26.178901 flavpy-1.0.2/flavpy/inspector/
+-rw-r--r--   0 taiyuu     (501) staff       (20)       32 2023-11-24 06:53:39.000000 flavpy-1.0.2/flavpy/inspector/__init__.py
+-rw-r--r--   0 taiyuu     (501) staff       (20)      844 2023-11-24 04:10:06.000000 flavpy-1.0.2/flavpy/inspector/inspector.py
+drwxr-xr-x   0 taiyuu     (501) staff       (20)        0 2024-04-16 15:36:26.179413 flavpy-1.0.2/flavpy/writer/
+-rw-r--r--   0 taiyuu     (501) staff       (20)      267 2024-02-24 15:01:51.000000 flavpy-1.0.2/flavpy/writer/__init__.py
+-rw-r--r--   0 taiyuu     (501) staff       (20)     4158 2024-02-19 07:20:34.000000 flavpy-1.0.2/flavpy/writer/_writer.py
+drwxr-xr-x   0 taiyuu     (501) staff       (20)        0 2024-04-16 15:36:26.179733 flavpy-1.0.2/flavpy.egg-info/
+-rw-r--r--   0 taiyuu     (501) staff       (20)     1877 2024-04-16 15:36:26.000000 flavpy-1.0.2/flavpy.egg-info/PKG-INFO
+-rw-r--r--   0 taiyuu     (501) staff       (20)      350 2024-04-16 15:36:26.000000 flavpy-1.0.2/flavpy.egg-info/SOURCES.txt
+-rw-r--r--   0 taiyuu     (501) staff       (20)        1 2024-04-16 15:36:26.000000 flavpy-1.0.2/flavpy.egg-info/dependency_links.txt
+-rw-r--r--   0 taiyuu     (501) staff       (20)       41 2024-04-16 15:36:26.000000 flavpy-1.0.2/flavpy.egg-info/requires.txt
+-rw-r--r--   0 taiyuu     (501) staff       (20)        7 2024-04-16 15:36:26.000000 flavpy-1.0.2/flavpy.egg-info/top_level.txt
+-rw-r--r--   0 taiyuu     (501) staff       (20)       38 2024-04-16 15:36:26.180240 flavpy-1.0.2/setup.cfg
+-rw-r--r--   0 taiyuu     (501) staff       (20)      765 2024-04-16 15:34:39.000000 flavpy-1.0.2/setup.py
```

### Comparing `flavpy-1.0.1/PKG-INFO` & `flavpy-1.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: flavpy
-Version: 1.0.1
+Version: 1.0.2
 Summary: 味覚情報を埋め込み可能なファイル形式:FlavMP4のキャプチャ、書き出しを行う
 Home-page: https://github.com/hmwri/flavtool
 Author: Taiyu Honma
 Author-email: ev220526@meiji.ac.jp
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+Requires-Dist: flavtool
+Requires-Dist: coloredlogs
+Requires-Dist: opencv-python
+Requires-Dist: numpy
 
 # flavpy
 
 flavpyは、味覚情報を埋め込み可能なファイル形式:FlavMP4のキャプチャ、書き込みを行います
 
 ## インストール方法
```

### Comparing `flavpy-1.0.1/README.md` & `flavpy-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `flavpy-1.0.1/flavpy/capture/_capture.py` & `flavpy-1.0.2/flavpy/capture/_capture.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 
 import numpy as np
 
 from flavtool.parser import Parser
 from flavtool.analyzer import analyze
 from flavtool.analyzer.media_data import StreamingSampleData, ChunkData
 from flavtool.codec import supported_codecs, get_decoder ,supported_codec_type
+from flavtool.codec.codec_options import  *
 from typing import Literal, BinaryIO, Final
+import cv2
 
 SEEK_FRAME_INDEX : Final[int] = 0
 SEEK_MEDIA_TIME : Final[int] = 1
 SEEK_REAL_TIME: Final[int] = 2
 class ChunkReader :
     def __init__(self, f:BinaryIO, chunk:ChunkData):
         self.chunk = chunk
@@ -53,17 +55,25 @@
         else:
             raise Exception(f"seek_mode{seek_mode} is not supported")
 
 
 
 class FlavCapture:
     def __init__(self, path:str, modal:Literal['taste', 'scent']):
+
+        cap = cv2.VideoCapture(path)
+
+        self.video_width = int(cap.get(cv2.CAP_PROP_FRAME_WIDTH))
+        self.video_height = int(cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
+
         self.__f = open(path, "rb")
         self.parsed = Parser(path, fp=self.__f).parse(read_mdat_bytes=False)
         self.flavMp4 = analyze(self.parsed)
+
+
         component_subtype : Literal['tast', 'scnt']
         if modal == "taste":
             component_subtype = "tast"
         elif modal=="scent":
             component_subtype = "scnt"
         else:
             raise Exception(f"modal:{modal} is not supported.")
@@ -75,17 +85,21 @@
         self.media_data = self.flavMp4.media_datas[component_subtype]
         if self.media_data is None:
             raise Exception(f"media data corresponding {modal} is not found")
 
         self.media_duration = track.media.header.duration
 
         self.sample_table = self.flavMp4.sample_tables[component_subtype]
+
         self.time_scale = track.media.header.time_scale
 
         self.codec = self.sample_table.sample_description.sample_description_table[0].data_format
+        self.codec_option = None
+        if self.codec == "rmix":
+            self.codec_option = MixCodecOption(self.sample_table.sample_description.sample_description_table[0].mix_info.infos)
 
         if self.codec not in supported_codecs:
             raise Exception(f"codec : {self.codec} is not supported")
         self.codec: supported_codec_type
 
         self.decoder = get_decoder(self.codec)
```

### Comparing `flavpy-1.0.1/flavpy/inspector/inspector.py` & `flavpy-1.0.2/flavpy/inspector/inspector.py`

 * *Files identical despite different names*

### Comparing `flavpy-1.0.1/flavpy/writer/_writer.py` & `flavpy-1.0.2/flavpy/writer/_writer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import os
 from io import BytesIO
-
+import cv2
 import numpy as np
 from flavtool.analyzer.components import SampleTableComponent
 from flavtool.parser import Parser
 from flavtool.analyzer import analyze, FlavMP4
 from flavtool.analyzer.components import TrackComponent
 from flavtool.analyzer.media_data import StreamingSampleData, ChunkData, SampleData, MediaData
 from flavtool.codec import supported_codecs, get_encoder, supported_codec_type
+from flavtool.codec.codec_options import MixCodecOption, CodecOption
 from flavtool.composer.utils import EmptyMp4Creator, TrackBoxCreator, SampleTableCreator
 from flavtool.composer import Composer
 from typing import Literal, BinaryIO, Final
 
 
 class FlavWriter:
     def __init__(self, path, modal: Literal["taste", "scent"], codec: supported_codec_type, fps: float,
-                 add_modal_on:str|None=None):
+                 add_modal_on:str|None=None,codec_option : CodecOption | None = None):
         self.path = path
         if codec not in supported_codecs:
             raise Exception(f"codec : {codec} is not supported")
         self.codec: supported_codec_type = codec
+        self.codec_option = codec_option
         self.fps = fps
         self.media_time_scale: int = int(fps * 1000)
 
         component_subtype: Literal['tast', 'scnt']
         if modal == "taste":
             self.component_subtype : Literal["tast", "scnt"] = "tast"
         elif modal == "scent":
@@ -38,47 +40,61 @@
                 "mp41",
                 ["isom", "mp41", "mp42"],
                 self.media_time_scale,
                 0
             )
 
 
+        cap = cv2.VideoCapture(path)
+
+        self.video_width = int(cap.get(cv2.CAP_PROP_FRAME_WIDTH))
+        self.video_height = int(cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
 
         self.flavMp4 = analyze(self.parsed)
         self.data : list[np.ndarray] = []
         self.__sampler_per_chunk = 50
         self.chunks : list[ChunkData] = [ChunkData(samples=[], media_type=self.component_subtype, begin_time=0)]
 
 
 
+
+
     def write(self, data:np.ndarray, frame_delta=1):
         encoder = get_encoder(self.codec)
         sample = SampleData(encoder(data), delta=int(frame_delta/self.fps*self.media_time_scale))
         if len(self.chunks[-1]) >= self.__sampler_per_chunk:
-            self.chunks.append(ChunkData(samples=[sample], media_type=self.component_subtype,
+            self.chunks.append(ChunkData(samples=[], media_type=self.component_subtype,
                                          begin_time=self.chunks[-1].end_time))
         self.chunks[-1].samples.append(sample)
 
 
 
 
 
 
     def __enter__(self):
+
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.export()
 
     def export(self):
         if len(self.chunks[0]) == 0:
             raise Exception("There is no data")
-        sample_table = SampleTableCreator(self.chunks, codec=self.codec).make_sample_table()
+
+        if self.codec == "rmix":
+            if self.codec_option is None:
+                self.codec_option = MixCodecOption.default()
+
+
+        sample_table = SampleTableCreator(self.chunks, codec=self.codec, codec_option=self.codec_option).make_sample_table()
         mov_time_scale = self.flavMp4.mov_header.time_scale
         track_duration = int(self.chunks[-1].end_time * mov_time_scale / self.media_time_scale)
+
         if self.flavMp4.mov_header.duration < track_duration:
             self.flavMp4.mov_header.duration = track_duration
         composer = Composer(flav_mp4=self.flavMp4)
         composer.set_new_modal(
             self.component_subtype,
             TrackComponent(
                 TrackBoxCreator(
```

### Comparing `flavpy-1.0.1/flavpy.egg-info/PKG-INFO` & `flavpy-1.0.2/flavpy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: flavpy
-Version: 1.0.1
+Version: 1.0.2
 Summary: 味覚情報を埋め込み可能なファイル形式:FlavMP4のキャプチャ、書き出しを行う
 Home-page: https://github.com/hmwri/flavtool
 Author: Taiyu Honma
 Author-email: ev220526@meiji.ac.jp
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+Requires-Dist: flavtool
+Requires-Dist: coloredlogs
+Requires-Dist: opencv-python
+Requires-Dist: numpy
 
 # flavpy
 
 flavpyは、味覚情報を埋め込み可能なファイル形式:FlavMP4のキャプチャ、書き込みを行います
 
 ## インストール方法
```

### Comparing `flavpy-1.0.1/setup.py` & `flavpy-1.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='flavpy',
-    version='1.0.1',
+    version='1.0.2',
     author="Taiyu Honma",
     author_email="ev220526@meiji.ac.jp",
     description="味覚情報を埋め込み可能なファイル形式:FlavMP4のキャプチャ、書き出しを行う",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hmwri/flavtool",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3.7",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    install_requires=["flavtool"],
+    install_requires=["flavtool", "coloredlogs", "opencv-python", "numpy"],
 
 )
```

