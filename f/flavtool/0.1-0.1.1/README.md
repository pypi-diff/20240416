# Comparing `tmp/flavtool-0.1.tar.gz` & `tmp/flavtool-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flavtool-0.1.tar", last modified: Fri Nov 24 05:07:26 2023, max compression
+gzip compressed data, was "flavtool-0.1.1.tar", last modified: Tue Apr 16 15:19:04 2024, max compression
```

## Comparing `flavtool-0.1.tar` & `flavtool-0.1.1.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 taiyuu     (501) staff       (20)        0 2023-11-24 05:07:26.880031 flavtool-0.1/
--rw-r--r--   0 taiyuu     (501) staff       (20)     2649 2023-11-24 05:07:26.879884 flavtool-0.1/PKG-INFO
--rw-r--r--   0 taiyuu     (501) staff       (20)     2184 2023-11-24 05:01:47.000000 flavtool-0.1/README.md
-drwxr-xr-x   0 taiyuu     (501) staff       (20)        0 2023-11-24 05:07:26.872548 flavtool-0.1/flavtool/
--rw-r--r--   0 taiyuu     (501) staff       (20)        0 2023-11-24 03:51:07.000000 flavtool-0.1/flavtool/__init__.py
-drwxr-xr-x   0 taiyuu     (501) staff       (20)        0 2023-11-24 05:07:26.873653 flavtool-0.1/flavtool/analyzer/
--rw-r--r--   0 taiyuu     (501) staff       (20)       93 2023-11-24 03:51:07.000000 flavtool-0.1/flavtool/analyzer/__init__.py
--rw-r--r--   0 taiyuu     (501) staff       (20)      166 2023-11-24 03:54:45.000000 flavtool-0.1/flavtool/analyzer/analyze.py
-drwxr-xr-x   0 taiyuu     (501) staff       (20)        0 2023-11-24 05:07:26.874239 flavtool-0.1/flavtool/analyzer/components/
--rw-r--r--   0 taiyuu     (501) staff       (20)       25 2023-11-24 03:51:07.000000 flavtool-0.1/flavtool/analyzer/components/__init__.py
--rw-r--r--   0 taiyuu     (501) staff       (20)     1594 2023-11-24 03:54:45.000000 flavtool-0.1/flavtool/analyzer/components/components.py
--rw-r--r--   0 taiyuu     (501) staff       (20)     2830 2023-11-24 03:54:45.000000 flavtool-0.1/flavtool/analyzer/flavMp4.py
-drwxr-xr-x   0 taiyuu     (501) staff       (20)        0 2023-11-24 05:07:26.875181 flavtool-0.1/flavtool/analyzer/media_data/
--rw-r--r--   0 taiyuu     (501) staff       (20)      116 2023-11-24 03:51:07.000000 flavtool-0.1/flavtool/analyzer/media_data/__init__.py
--rw-r--r--   0 taiyuu     (501) staff       (20)     1131 2023-11-24 03:51:07.000000 flavtool-0.1/flavtool/analyzer/media_data/chunk.py
--rw-r--r--   0 taiyuu     (501) staff       (20)     3302 2023-11-24 03:54:45.000000 flavtool-0.1/flavtool/analyzer/media_data/media_data.py
--rw-r--r--   0 taiyuu     (501) staff       (20)      570 2023-11-24 03:51:07.000000 flavtool-0.1/flavtool/analyzer/media_data/sample.py
-drwxr-xr-x   0 taiyuu     (501) staff       (20)        0 2023-11-24 05:07:26.875747 flavtool-0.1/flavtool/codec/
--rw-r--r--   0 taiyuu     (501) staff       (20)      596 2023-11-24 03:51:07.000000 flavtool-0.1/flavtool/codec/__init__.py
--rw-r--r--   0 taiyuu     (501) staff       (20)      284 2023-11-24 03:51:07.000000 flavtool-0.1/flavtool/codec/decoder.py
--rw-r--r--   0 taiyuu     (501) staff       (20)      496 2023-11-24 03:51:07.000000 flavtool-0.1/flavtool/codec/encoder.py
-drwxr-xr-x   0 taiyuu     (501) staff       (20)        0 2023-11-24 05:07:26.876057 flavtool-0.1/flavtool/composer/
--rw-r--r--   0 taiyuu     (501) staff       (20)       30 2023-11-24 03:51:07.000000 flavtool-0.1/flavtool/composer/__init__.py
--rw-r--r--   0 taiyuu     (501) staff       (20)     8959 2023-11-24 03:54:45.000000 flavtool-0.1/flavtool/composer/composer.py
-drwxr-xr-x   0 taiyuu     (501) staff       (20)        0 2023-11-24 05:07:26.877046 flavtool-0.1/flavtool/composer/utils/
--rw-r--r--   0 taiyuu     (501) staff       (20)      146 2023-11-24 03:51:07.000000 flavtool-0.1/flavtool/composer/utils/__init__.py
--rw-r--r--   0 taiyuu     (501) staff       (20)     1401 2023-11-24 03:54:45.000000 flavtool-0.1/flavtool/composer/utils/empty_mp4_creator.py
--rw-r--r--   0 taiyuu     (501) staff       (20)     4670 2023-11-24 03:54:45.000000 flavtool-0.1/flavtool/composer/utils/sample_table_creator.py
--rw-r--r--   0 taiyuu     (501) staff       (20)     4324 2023-11-24 03:54:45.000000 flavtool-0.1/flavtool/composer/utils/track_box_creator.py
-drwxr-xr-x   0 taiyuu     (501) staff       (20)        0 2023-11-24 05:07:26.877279 flavtool-0.1/flavtool/logger/
--rw-r--r--   0 taiyuu     (501) staff       (20)      145 2023-11-24 03:51:07.000000 flavtool-0.1/flavtool/logger/__init__.py
-drwxr-xr-x   0 taiyuu     (501) staff       (20)        0 2023-11-24 05:07:26.877747 flavtool-0.1/flavtool/parser/
--rw-r--r--   0 taiyuu     (501) staff       (20)       29 2023-11-24 03:51:07.000000 flavtool-0.1/flavtool/parser/__init__.py
--rw-r--r--   0 taiyuu     (501) staff       (20)      827 2023-11-24 03:54:45.000000 flavtool-0.1/flavtool/parser/_parser.py
-drwxr-xr-x   0 taiyuu     (501) staff       (20)        0 2023-11-24 05:07:26.878734 flavtool-0.1/flavtool/parser/boxs/
--rw-r--r--   0 taiyuu     (501) staff       (20)       19 2023-11-24 03:51:07.000000 flavtool-0.1/flavtool/parser/boxs/__init__.py
--rw-r--r--   0 taiyuu     (501) staff       (20)     4291 2023-11-24 03:51:07.000000 flavtool-0.1/flavtool/parser/boxs/box.py
--rw-r--r--   0 taiyuu     (501) staff       (20)     3703 2023-11-24 03:54:45.000000 flavtool-0.1/flavtool/parser/boxs/container.py
--rw-r--r--   0 taiyuu     (501) staff       (20)    39009 2023-11-24 03:54:45.000000 flavtool-0.1/flavtool/parser/boxs/leaf.py
-drwxr-xr-x   0 taiyuu     (501) staff       (20)        0 2023-11-24 05:07:26.873004 flavtool-0.1/flavtool.egg-info/
--rw-r--r--   0 taiyuu     (501) staff       (20)     2649 2023-11-24 05:07:26.000000 flavtool-0.1/flavtool.egg-info/PKG-INFO
--rw-r--r--   0 taiyuu     (501) staff       (20)     1020 2023-11-24 05:07:26.000000 flavtool-0.1/flavtool.egg-info/SOURCES.txt
--rw-r--r--   0 taiyuu     (501) staff       (20)        1 2023-11-24 05:07:26.000000 flavtool-0.1/flavtool.egg-info/dependency_links.txt
--rw-r--r--   0 taiyuu     (501) staff       (20)        9 2023-11-24 05:07:26.000000 flavtool-0.1/flavtool.egg-info/top_level.txt
--rw-r--r--   0 taiyuu     (501) staff       (20)       38 2023-11-24 05:07:26.880076 flavtool-0.1/setup.cfg
--rw-r--r--   0 taiyuu     (501) staff       (20)      705 2023-11-24 05:06:38.000000 flavtool-0.1/setup.py
+drwxr-xr-x   0 taiyuu     (501) staff       (20)        0 2024-04-16 15:19:04.352197 flavtool-0.1.1/
+-rw-r--r--   0 taiyuu     (501) staff       (20)     2651 2024-04-16 15:19:04.351912 flavtool-0.1.1/PKG-INFO
+-rw-r--r--   0 taiyuu     (501) staff       (20)     2184 2023-11-24 05:01:47.000000 flavtool-0.1.1/README.md
+drwxr-xr-x   0 taiyuu     (501) staff       (20)        0 2024-04-16 15:19:04.340937 flavtool-0.1.1/flavtool/
+-rw-------   0 taiyuu     (501) staff       (20)        0 2023-11-24 03:51:07.000000 flavtool-0.1.1/flavtool/__init__.py
+drwxr-xr-x   0 taiyuu     (501) staff       (20)        0 2024-04-16 15:19:04.347774 flavtool-0.1.1/flavtool/analyzer/
+-rw-r--r--   0 taiyuu     (501) staff       (20)       93 2023-11-24 03:51:07.000000 flavtool-0.1.1/flavtool/analyzer/__init__.py
+-rw-r--r--   0 taiyuu     (501) staff       (20)      166 2023-11-24 03:54:45.000000 flavtool-0.1.1/flavtool/analyzer/analyze.py
+drwxr-xr-x   0 taiyuu     (501) staff       (20)        0 2024-04-16 15:19:04.348212 flavtool-0.1.1/flavtool/analyzer/components/
+-rw-r--r--   0 taiyuu     (501) staff       (20)       25 2023-11-24 03:51:07.000000 flavtool-0.1.1/flavtool/analyzer/components/__init__.py
+-rw-r--r--   0 taiyuu     (501) staff       (20)     1594 2023-11-24 03:54:45.000000 flavtool-0.1.1/flavtool/analyzer/components/components.py
+-rw-r--r--   0 taiyuu     (501) staff       (20)     2830 2023-11-24 03:54:45.000000 flavtool-0.1.1/flavtool/analyzer/flavMp4.py
+drwxr-xr-x   0 taiyuu     (501) staff       (20)        0 2024-04-16 15:19:04.348750 flavtool-0.1.1/flavtool/analyzer/media_data/
+-rw-r--r--   0 taiyuu     (501) staff       (20)      116 2023-11-24 03:51:07.000000 flavtool-0.1.1/flavtool/analyzer/media_data/__init__.py
+-rw-r--r--   0 taiyuu     (501) staff       (20)     1131 2023-11-24 03:51:07.000000 flavtool-0.1.1/flavtool/analyzer/media_data/chunk.py
+-rw-r--r--   0 taiyuu     (501) staff       (20)     3302 2023-11-24 03:54:45.000000 flavtool-0.1.1/flavtool/analyzer/media_data/media_data.py
+-rw-r--r--   0 taiyuu     (501) staff       (20)      570 2023-11-24 03:51:07.000000 flavtool-0.1.1/flavtool/analyzer/media_data/sample.py
+drwxr-xr-x   0 taiyuu     (501) staff       (20)        0 2024-04-16 15:19:04.349277 flavtool-0.1.1/flavtool/codec/
+-rw-r--r--   0 taiyuu     (501) staff       (20)      612 2023-12-15 08:30:35.000000 flavtool-0.1.1/flavtool/codec/__init__.py
+-rw-r--r--   0 taiyuu     (501) staff       (20)     2158 2024-02-24 14:59:01.000000 flavtool-0.1.1/flavtool/codec/codec_options.py
+-rw-r--r--   0 taiyuu     (501) staff       (20)      432 2024-02-25 07:52:07.000000 flavtool-0.1.1/flavtool/codec/decoder.py
+-rw-r--r--   0 taiyuu     (501) staff       (20)      735 2024-02-19 06:27:27.000000 flavtool-0.1.1/flavtool/codec/encoder.py
+drwxr-xr-x   0 taiyuu     (501) staff       (20)        0 2024-04-16 15:19:04.349524 flavtool-0.1.1/flavtool/composer/
+-rw-r--r--   0 taiyuu     (501) staff       (20)       30 2023-11-24 03:51:07.000000 flavtool-0.1.1/flavtool/composer/__init__.py
+-rw-r--r--   0 taiyuu     (501) staff       (20)     8957 2023-12-15 12:08:48.000000 flavtool-0.1.1/flavtool/composer/composer.py
+drwxr-xr-x   0 taiyuu     (501) staff       (20)        0 2024-04-16 15:19:04.350200 flavtool-0.1.1/flavtool/composer/utils/
+-rw-r--r--   0 taiyuu     (501) staff       (20)      146 2023-11-24 03:51:07.000000 flavtool-0.1.1/flavtool/composer/utils/__init__.py
+-rw-r--r--   0 taiyuu     (501) staff       (20)     1401 2023-11-24 03:54:45.000000 flavtool-0.1.1/flavtool/composer/utils/empty_mp4_creator.py
+-rw-r--r--   0 taiyuu     (501) staff       (20)     5265 2024-02-19 06:48:07.000000 flavtool-0.1.1/flavtool/composer/utils/sample_table_creator.py
+-rw-r--r--   0 taiyuu     (501) staff       (20)     4324 2023-11-24 03:54:45.000000 flavtool-0.1.1/flavtool/composer/utils/track_box_creator.py
+drwxr-xr-x   0 taiyuu     (501) staff       (20)        0 2024-04-16 15:19:04.350371 flavtool-0.1.1/flavtool/logger/
+-rw-r--r--   0 taiyuu     (501) staff       (20)      145 2023-11-24 03:51:07.000000 flavtool-0.1.1/flavtool/logger/__init__.py
+drwxr-xr-x   0 taiyuu     (501) staff       (20)        0 2024-04-16 15:19:04.350641 flavtool-0.1.1/flavtool/parser/
+-rw-r--r--   0 taiyuu     (501) staff       (20)       29 2023-11-24 03:51:07.000000 flavtool-0.1.1/flavtool/parser/__init__.py
+-rw-r--r--   0 taiyuu     (501) staff       (20)      827 2023-11-24 03:54:45.000000 flavtool-0.1.1/flavtool/parser/_parser.py
+drwxr-xr-x   0 taiyuu     (501) staff       (20)        0 2024-04-16 15:19:04.351266 flavtool-0.1.1/flavtool/parser/boxs/
+-rw-r--r--   0 taiyuu     (501) staff       (20)       19 2023-11-24 03:51:07.000000 flavtool-0.1.1/flavtool/parser/boxs/__init__.py
+-rw-r--r--   0 taiyuu     (501) staff       (20)     4291 2023-11-24 03:51:07.000000 flavtool-0.1.1/flavtool/parser/boxs/box.py
+-rw-r--r--   0 taiyuu     (501) staff       (20)     3703 2023-11-24 03:54:45.000000 flavtool-0.1.1/flavtool/parser/boxs/container.py
+-rw-r--r--   0 taiyuu     (501) staff       (20)    41448 2024-02-21 06:02:32.000000 flavtool-0.1.1/flavtool/parser/boxs/leaf.py
+drwxr-xr-x   0 taiyuu     (501) staff       (20)        0 2024-04-16 15:19:04.351590 flavtool-0.1.1/flavtool.egg-info/
+-rw-r--r--   0 taiyuu     (501) staff       (20)     2651 2024-04-16 15:19:04.000000 flavtool-0.1.1/flavtool.egg-info/PKG-INFO
+-rw-r--r--   0 taiyuu     (501) staff       (20)     1052 2024-04-16 15:19:04.000000 flavtool-0.1.1/flavtool.egg-info/SOURCES.txt
+-rw-r--r--   0 taiyuu     (501) staff       (20)        1 2024-04-16 15:19:04.000000 flavtool-0.1.1/flavtool.egg-info/dependency_links.txt
+-rw-r--r--   0 taiyuu     (501) staff       (20)        9 2024-04-16 15:19:04.000000 flavtool-0.1.1/flavtool.egg-info/top_level.txt
+-rw-r--r--   0 taiyuu     (501) staff       (20)       38 2024-04-16 15:19:04.352242 flavtool-0.1.1/setup.cfg
+-rw-r--r--   0 taiyuu     (501) staff       (20)      707 2024-04-16 15:18:57.000000 flavtool-0.1.1/setup.py
```

### Comparing `flavtool-0.1/PKG-INFO` & `flavtool-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flavtool
-Version: 0.1
+Version: 0.1.1
 Summary: 味覚情報を埋め込み可能なファイル形式:FlavMP4の解析、編集を可能にするツールキット
 Home-page: https://github.com/hmwri/flavtool
 Author: Taiyu Honma
 Author-email: ev220526@meiji.ac.jp
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `flavtool-0.1/README.md` & `flavtool-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `flavtool-0.1/flavtool/analyzer/components/components.py` & `flavtool-0.1.1/flavtool/analyzer/components/components.py`

 * *Files identical despite different names*

### Comparing `flavtool-0.1/flavtool/analyzer/flavMp4.py` & `flavtool-0.1.1/flavtool/analyzer/flavMp4.py`

 * *Files identical despite different names*

### Comparing `flavtool-0.1/flavtool/analyzer/media_data/chunk.py` & `flavtool-0.1.1/flavtool/analyzer/media_data/chunk.py`

 * *Files identical despite different names*

### Comparing `flavtool-0.1/flavtool/analyzer/media_data/media_data.py` & `flavtool-0.1.1/flavtool/analyzer/media_data/media_data.py`

 * *Files identical despite different names*

### Comparing `flavtool-0.1/flavtool/analyzer/media_data/sample.py` & `flavtool-0.1.1/flavtool/analyzer/media_data/sample.py`

 * *Files identical despite different names*

### Comparing `flavtool-0.1/flavtool/codec/__init__.py` & `flavtool-0.1.1/flavtool/codec/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Literal
 from .decoder import decoders, decoder_func_type
 from .encoder import encoders, encoder_func_type
-supported_codec_type = Literal["raw5"]
-supported_codecs = ["raw5"]
+supported_codec_type = Literal["raw5", "rmix"]
+supported_codecs = ["raw5", "rmix"]
 
 def get_decoder(codec : supported_codec_type) -> decoder_func_type :
     if codec not in supported_codecs:
         raise Exception(f"This codec : {codec} is not supported")
     return decoders[codec]
 
 def get_encoder(codec : supported_codec_type) -> encoder_func_type :
```

### Comparing `flavtool-0.1/flavtool/composer/composer.py` & `flavtool-0.1.1/flavtool/composer/composer.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,16 +39,14 @@
         streaming : bool
             strea
 
         """
         self.flav_mp4 : FlavMP4 = flav_mp4
 
 
-
-
     def __generate_interleave_chunks(self, criteria_media_type: media_types, target_media_types: list[media_types]) -> \
             tuple[list[ChunkData], dict[media_types, list[int]]]:
         """
         各メディアデータから、指定メディアタイプを基準とした適切なChunkリストとオフセットを作成
         Parameters
         ----------
         criteria_media_type
```

### Comparing `flavtool-0.1/flavtool/composer/utils/empty_mp4_creator.py` & `flavtool-0.1.1/flavtool/composer/utils/empty_mp4_creator.py`

 * *Files identical despite different names*

### Comparing `flavtool-0.1/flavtool/composer/utils/sample_table_creator.py` & `flavtool-0.1.1/flavtool/composer/utils/sample_table_creator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 from flavtool.analyzer.media_data import ChunkData
 from flavtool.parser.boxs.container import ContainerBox
 from flavtool.parser.boxs.leaf import *
+from flavtool.codec.codec_options import CodecOption, MixCodecOption
+
 
 class SampleTableCreator:
     """
     サンプルテーブルを作るクラス
     """
-    def __init__(self, chunks: list[ChunkData], codec:str):
+
+    def __init__(self, chunks: list[ChunkData], codec: str, codec_option: CodecOption=None):
         """
         サンプルテーブルを作るクラス
 
         Parameters
         ----------
         chunks : list[ChunkData]
             対象のチャンクデータ
         codec : str
             コーデック
         """
+
+
         self.chunks = chunks
         self.codec = codec
+        self.codec_option = codec_option
+        if self.codec_option is not None and codec_option.corresponding_codec != codec:
+            Exception("invalid codec option")
 
     def __make_sample_to_chunk_table(self) -> list[SampleToChunk]:
         """
         SampleToChunkテーブル(どのサンプルがどのチャンクに属するか)を作成する
 
         Returns
         ----------
@@ -50,49 +58,63 @@
         first = True
         all_same = True
         for c in self.chunks:
             for s in c.samples:
                 if not first:
                     size = len(s.data)
                     if size != sizes[-1]:
-                        all_same =False
-                        break
+                        all_same = False
                     sizes.append(size)
                 first = False
 
         if all_same:
             return sizes[0], []
         else:
             return 0, sizes
 
-
     def __make_time_to_sample_table(self) -> list[TimeToSample]:
         deltas = [self.chunks[0][0].delta]
-        table : list[TimeToSample] = [
+        table: list[TimeToSample] = [
             TimeToSample(1, deltas[0])
         ]
         first = True
         for c in self.chunks:
             for s in c.samples:
                 if not first:
                     delta = s.delta
-                    if delta != table[-1].sample_delta :
+                    if delta != table[-1].sample_delta:
                         table.append(TimeToSample(1, delta))
                     else:
                         table[-1].sample_count += 1
                     deltas.append(delta)
                 first = False
         return table
 
+    def __make_sample_description_table(self) -> StsdBox:
+        option = None
+        if self.codec == "rmix":
+            self.codec_option :MixCodecOption = self.codec_option
+            option = RawMixCodec(
+                number_of_entries=len(self.codec_option.infos),
+                mix_info=self.codec_option.infos
+            )
+
+        return StsdBox(
+            box_type="stsd",
+            number_of_entries=1,
+            sample_description_table=[
+                SampleDescription(
+                    sample_description_size=None,
+                    data_format=self.codec,
+                    data_reference_index=1,
+                    mix_info=option
 
-
-
-
-
-
+                )
+            ],
+        )
 
     def make_sample_table(self) -> ContainerBox:
         """
         サンプルテーブルを作成する(Stcoの中身を除く)
         Returns
         -------
         sample_table : ContainerBox
@@ -102,25 +124,15 @@
 
         sample_to_chunk_table = self.__make_sample_to_chunk_table()
         sample_size, sample_size_table = self.__get_sample_size()
         time_to_sample = self.__make_time_to_sample_table()
         sample_table = ContainerBox(
             box_type="stbl",
             children=[
-                StsdBox(
-                    box_type="stsd",
-                    number_of_entries=1,
-                    sample_description_table=[
-                        SampleDescription(
-                            sample_description_size=None,
-                            data_format=self.codec,
-                            data_reference_index=1
-                        )
-                    ],
-                ),
+                self.__make_sample_description_table(),
                 SttsBox(
                     box_type="stts",
                     number_of_entries=len(time_to_sample),
                     time_to_sample_table=self.__make_time_to_sample_table()
                 ),
                 StscBox(
                     box_type="stsc",
@@ -136,8 +148,7 @@
                 StcoBox(
                     box_type="stco",
                     number_of_entries=len(self.chunks)
                 )
             ]
         )
         return sample_table
-
```

### Comparing `flavtool-0.1/flavtool/composer/utils/track_box_creator.py` & `flavtool-0.1.1/flavtool/composer/utils/track_box_creator.py`

 * *Files identical despite different names*

### Comparing `flavtool-0.1/flavtool/parser/_parser.py` & `flavtool-0.1.1/flavtool/parser/_parser.py`

 * *Files identical despite different names*

### Comparing `flavtool-0.1/flavtool/parser/boxs/box.py` & `flavtool-0.1.1/flavtool/parser/boxs/box.py`

 * *Files identical despite different names*

### Comparing `flavtool-0.1/flavtool/parser/boxs/container.py` & `flavtool-0.1.1/flavtool/parser/boxs/container.py`

 * *Files identical despite different names*

### Comparing `flavtool-0.1/flavtool/parser/boxs/leaf.py` & `flavtool-0.1.1/flavtool/parser/boxs/leaf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from typing import BinaryIO
 from datetime import datetime, timedelta
 from flavtool.parser.boxs.box import Box, Mp4Component
-
+from flavtool.codec.codec_options import MixInfo
 epoch_1904 = datetime(1904, 1, 1)
 
 
 class LeafBox(Box):
 
     def parse(self, f: BinaryIO, body_size: int):
         raise NotImplemented
@@ -482,23 +482,23 @@
         self.version = f.read(1)
         self.flags = f.read(3)
         self.balance = self.read_int(f, 2)
         self.reserved = f.read(2)
         return self
 
     def print(self, depth=0):
-        self.print_with_indent("smhd", depth)
+        self.print_with_indent("tmhd", depth)
         depth += 1  # Increase the depth for nested printing
         self.print_with_indent(f" - version: {self.version.hex()}", depth)
         self.print_with_indent(f" - flags: {self.flags.hex()}", depth)
         self.print_with_indent(f" - balance: {self.balance}", depth)
         self.print_with_indent(f" - reserved: {self.reserved}", depth)
 
     def write(self, f: BinaryIO):
-        self.write_type_and_size(f, "smhd", self.get_size())
+        self.write_type_and_size(f, "tmhd", self.get_size())
         f.write(self.version)
         f.write(self.flags)
         self.write_int(f, self.balance, 2)
         f.write(self.reserved)
 
     def get_size(self) -> int:
         return self.get_overall_size(1 + 3 + 2 * 2)
@@ -575,14 +575,15 @@
     def get_size(self) -> int:
         url_all_size = 0
         for ref in self.data_references:
             url_all_size += ref.get_size()
         return self.get_overall_size(1 + 3 + 4 + url_all_size)
 
 
+
 class StsdBox(LeafBox):
     def __init__(self, box_type: str, version: bytes = b'\x00', flags: bytes = b'\x00\x00\x00',
                  number_of_entries: int = 0, sample_description_table=None):
         super().__init__(box_type)
         if sample_description_table is None:
             sample_description_table = []
         self.version: bytes = version
@@ -619,61 +620,129 @@
     def get_size(self) -> int:
         table_all_size = 0
         for sample_description in self.sample_description_table:
             table_all_size += sample_description.get_size()
         return self.get_overall_size(1 + 3 + 4 + table_all_size)
 
 
+# class SolutionInfo():
+#     def __init__(self, name, concentration : float, max_amount):
+#         self.name :str = name
+#         self.concentration : float = concentration
+#         self.max_amount : float = max_amount
+
+class RawMixCodec(Mp4Component):
+    def __init__(self, number_of_entries: int = 0, mix_info : list[MixInfo] = None):
+        super().__init__()
+        self.number_of_entries = number_of_entries
+        if mix_info is None:
+            self.infos : list[MixInfo] = []
+        else:
+            self.infos : list[MixInfo] = mix_info
+
+    def parse(self, f: BinaryIO):
+        self.number_of_entries = self.read_int(f, 4)
+        if self.number_of_entries == 0:
+            return
+        for i in range(self.number_of_entries):
+            name = self.read_ascii(f, 4)
+            concentration = self.read_fixed_float32(f)
+            max_amount = self.read_fixed_float32(f)
+            self.infos.append(MixInfo(name, concentration, max_amount))
+
+    def print(self, depth=0):
+        if self.number_of_entries == 0:
+            self.print_with_indent("0", depth)
+            return
+        self.print_with_indent(f" - number_of_entries: {self.number_of_entries}", depth)
+
+        for info in self.infos :
+            self.print_with_indent(f" - solution_info: name {info.name},concentration {info.concentration}, max_amount {info.max_amount}", depth)
+
+    def write(self, f: BinaryIO):
+        if self.number_of_entries == 0:
+            self.write_int(f, 0)
+            return
+        self.write_int(f, self.number_of_entries)
+
+        for info in self.infos:
+            self.write_ascii(f, info.name)
+            self.write_fixed_float32(f, info.concentration)
+            self.write_fixed_float32(f, info.max_amount)
+
+
+    def get_size(self) -> int:
+        if self.number_of_entries == 0:
+            return 4
+        return 4 +  self.number_of_entries * (4 + 4 + 4)
+
+
 class SampleDescription(Mp4Component):
     def __init__(self, sample_description_size: int = None, data_format: str = "", reserved1: bytes = bytes(6),
-                 data_reference_index: int = 0, rest: bytes = b''):
+                 data_reference_index: int = 0, rest: bytes = b'', mix_info : RawMixCodec | None = None):
         super().__init__()
         self.sample_description_size: int = sample_description_size
         self.data_format: str = data_format
         self.reserved1: bytes = reserved1
         self.data_reference_index: int = data_reference_index
+        self.mix_info : RawMixCodec | None = mix_info
         self.rest: bytes = rest
 
     def parse(self, f: BinaryIO):
         begin = f.tell()
         self.sample_description_size = self.read_int(f, 4)
         if self.sample_description_size == 0:
             return self
         self.data_format = self.read_ascii(f, 4)
+
+
         self.reserved1 = f.read(6)
         self.data_reference_index = self.read_int(f, 2)
-        self.rest = f.read(self.sample_description_size - (f.tell() - begin))
+
+        if self.data_format == "rmix":
+            self.mix_info = RawMixCodec()
+            self.mix_info.parse(f)
+        else:
+            self.rest = f.read(self.sample_description_size - (f.tell() - begin))
         return self
 
     def print(self, depth=0):
         if self.sample_description_size == 0:
             self.print_with_indent("0", depth)
             return
         self.print_with_indent(f" - sample_description_size: {self.sample_description_size}", depth)
         self.print_with_indent(f" - data_format: {self.data_format}", depth)
         self.print_with_indent(f" - reserved1: {self.reserved1.hex()}", depth)
         self.print_with_indent(f" - data_reference_index: {self.data_reference_index}", depth)
         self.print_with_indent(f" - rest: {self.rest.hex()} \n", depth)
+        if self.mix_info is not None:
+            self.mix_info.print(depth)
+
 
     def write(self, f: BinaryIO):
         if self.sample_description_size == 0:
             self.write_int(f, 0)
             return
         if self.sample_description_size is None:
             self.sample_description_size = self.get_size() + 8
         self.write_int(f, self.get_size())
         self.write_ascii(f, self.data_format)
         f.write(self.reserved1)
         self.write_int(f, self.data_reference_index, length=2)
-        f.write(self.rest)
+
+        if self.data_format == "rmix":
+            self.mix_info.write(f)
+        else:
+            f.write(self.rest)
 
     def get_size(self) -> int:
         if self.sample_description_size == 0:
             return 4
-        return 4 + 4 + 6 + 2 + len(self.rest)
+        body_len =  self.mix_info.get_size() if self.data_format == "rmix" else len(self.rest)
+        return 4 + 4 + 6 + 2 + body_len
 
 
 class SttsBox(LeafBox):
     def __init__(self, box_type: str, version: bytes = b'\x00', flags: bytes = b'\x00\x00\x00',
                  number_of_entries: int = 0, time_to_sample_table=None):
         super().__init__(box_type)
         if time_to_sample_table is None:
```

### Comparing `flavtool-0.1/flavtool.egg-info/PKG-INFO` & `flavtool-0.1.1/flavtool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flavtool
-Version: 0.1
+Version: 0.1.1
 Summary: 味覚情報を埋め込み可能なファイル形式:FlavMP4の解析、編集を可能にするツールキット
 Home-page: https://github.com/hmwri/flavtool
 Author: Taiyu Honma
 Author-email: ev220526@meiji.ac.jp
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `flavtool-0.1/flavtool.egg-info/SOURCES.txt` & `flavtool-0.1.1/flavtool.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 flavtool/analyzer/components/__init__.py
 flavtool/analyzer/components/components.py
 flavtool/analyzer/media_data/__init__.py
 flavtool/analyzer/media_data/chunk.py
 flavtool/analyzer/media_data/media_data.py
 flavtool/analyzer/media_data/sample.py
 flavtool/codec/__init__.py
+flavtool/codec/codec_options.py
 flavtool/codec/decoder.py
 flavtool/codec/encoder.py
 flavtool/composer/__init__.py
 flavtool/composer/composer.py
 flavtool/composer/utils/__init__.py
 flavtool/composer/utils/empty_mp4_creator.py
 flavtool/composer/utils/sample_table_creator.py
```

### Comparing `flavtool-0.1/setup.py` & `flavtool-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='flavtool',
-    version='0.1',
+    version='0.1.1',
     author="Taiyu Honma",
     author_email="ev220526@meiji.ac.jp",
     description="味覚情報を埋め込み可能なファイル形式:FlavMP4の解析、編集を可能にするツールキット",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hmwri/flavtool",
     packages=find_packages(),
```

