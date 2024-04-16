# Comparing `tmp/lindi-0.2.0.tar.gz` & `tmp/lindi-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lindi-0.2.0.tar", max compression
+gzip compressed data, was "lindi-0.2.1.tar", max compression
```

## Comparing `lindi-0.2.0.tar` & `lindi-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,35 @@
--rw-r--r--   0        0        0     1512 2024-03-13 15:25:45.816228 lindi-0.2.0/LICENSE
--rw-r--r--   0        0        0     3557 2024-04-04 18:54:34.995198 lindi-0.2.0/README.md
--rw-r--r--   0        0        0     1501 2024-04-04 18:54:34.995198 lindi-0.2.0/lindi/LindiH5ZarrStore/FloatJsonEncoder.py
--rw-r--r--   0        0        0    24641 2024-04-04 18:54:34.995198 lindi-0.2.0/lindi/LindiH5ZarrStore/LindiH5ZarrStore.py
--rw-r--r--   0        0        0      136 2024-03-21 11:16:09.352672 lindi-0.2.0/lindi/LindiH5ZarrStore/__init__.py
--rw-r--r--   0        0        0     4626 2024-04-04 18:54:34.995198 lindi-0.2.0/lindi/LindiH5ZarrStore/_h5_attr_to_zarr_attr.py
--rw-r--r--   0        0        0     2440 2024-04-04 18:54:34.995198 lindi-0.2.0/lindi/LindiH5ZarrStore/_h5_filters_to_codecs.py
--rw-r--r--   0        0        0     1939 2024-04-04 18:54:34.995198 lindi-0.2.0/lindi/LindiH5ZarrStore/_util.py
--rw-r--r--   0        0        0     1204 2024-04-04 18:54:34.995198 lindi-0.2.0/lindi/LindiH5ZarrStore/_utils.py
--rw-r--r--   0        0        0     9314 2024-04-04 18:54:34.995198 lindi-0.2.0/lindi/LindiH5ZarrStore/_zarr_info_for_h5_dataset.py
--rw-r--r--   0        0        0     3709 2024-04-04 18:54:34.995198 lindi-0.2.0/lindi/LindiH5pyFile/FileSegmentReader/DandiFileSegmentReader.py
--rw-r--r--   0        0        0     1045 2024-03-21 18:16:58.794258 lindi-0.2.0/lindi/LindiH5pyFile/FileSegmentReader/FileSegmentReader.py
--rw-r--r--   0        0        0        0 2024-03-21 18:16:58.794258 lindi-0.2.0/lindi/LindiH5pyFile/FileSegmentReader/__init__.py
--rw-r--r--   0        0        0     3072 2024-04-04 18:54:34.995198 lindi-0.2.0/lindi/LindiH5pyFile/LindiH5pyAttributes.py
--rw-r--r--   0        0        0    10718 2024-04-04 18:54:34.995198 lindi-0.2.0/lindi/LindiH5pyFile/LindiH5pyDataset.py
--rw-r--r--   0        0        0     8155 2024-04-04 18:54:34.995198 lindi-0.2.0/lindi/LindiH5pyFile/LindiH5pyFile.py
--rw-r--r--   0        0        0     5243 2024-04-04 18:54:34.995198 lindi-0.2.0/lindi/LindiH5pyFile/LindiH5pyGroup.py
--rw-r--r--   0        0        0      255 2024-03-21 11:16:09.352672 lindi-0.2.0/lindi/LindiH5pyFile/LindiH5pyLink.py
--rw-r--r--   0        0        0      454 2024-04-04 18:54:34.995198 lindi-0.2.0/lindi/LindiH5pyFile/LindiH5pyReference.py
--rw-r--r--   0        0        0     5959 2024-04-04 18:54:34.995198 lindi-0.2.0/lindi/LindiH5pyFile/LindiReferenceFileSystemStore.py
--rw-r--r--   0        0        0      327 2024-03-21 11:16:09.352672 lindi-0.2.0/lindi/LindiH5pyFile/__init__.py
--rw-r--r--   0        0        0      210 2024-03-21 11:16:09.352672 lindi-0.2.0/lindi/__init__.py
--rw-r--r--   0        0        0      625 2024-04-04 18:54:46.263044 lindi-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4189 1970-01-01 00:00:00.000000 lindi-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1512 2024-03-13 15:25:45.816228 lindi-0.2.1/LICENSE
+-rw-r--r--   0        0        0     5169 2024-04-16 15:35:00.582419 lindi-0.2.1/README.md
+-rw-r--r--   0        0        0    28733 2024-04-16 15:35:00.582419 lindi-0.2.1/lindi/LindiH5ZarrStore/LindiH5ZarrStore.py
+-rw-r--r--   0        0        0      136 2024-03-21 11:16:09.352672 lindi-0.2.1/lindi/LindiH5ZarrStore/__init__.py
+-rw-r--r--   0        0        0     2886 2024-04-04 18:56:02.142012 lindi-0.2.1/lindi/LindiH5ZarrStore/_util.py
+-rw-r--r--   0        0        0     3710 2024-04-04 18:56:02.142012 lindi-0.2.1/lindi/LindiH5pyFile/FileSegmentReader/DandiFileSegmentReader.py
+-rw-r--r--   0        0        0     1045 2024-03-21 18:16:58.794258 lindi-0.2.1/lindi/LindiH5pyFile/FileSegmentReader/FileSegmentReader.py
+-rw-r--r--   0        0        0        0 2024-03-21 18:16:58.794258 lindi-0.2.1/lindi/LindiH5pyFile/FileSegmentReader/__init__.py
+-rw-r--r--   0        0        0     3236 2024-04-04 18:56:02.142012 lindi-0.2.1/lindi/LindiH5pyFile/LindiH5pyAttributes.py
+-rw-r--r--   0        0        0    12266 2024-04-16 15:35:00.582419 lindi-0.2.1/lindi/LindiH5pyFile/LindiH5pyDataset.py
+-rw-r--r--   0        0        0    18016 2024-04-16 15:35:00.582419 lindi-0.2.1/lindi/LindiH5pyFile/LindiH5pyFile.py
+-rw-r--r--   0        0        0     8485 2024-04-16 15:35:00.582419 lindi-0.2.1/lindi/LindiH5pyFile/LindiH5pyGroup.py
+-rw-r--r--   0        0        0      255 2024-03-21 11:16:09.352672 lindi-0.2.1/lindi/LindiH5pyFile/LindiH5pyLink.py
+-rw-r--r--   0        0        0      478 2024-04-04 18:56:02.146012 lindi-0.2.1/lindi/LindiH5pyFile/LindiH5pyReference.py
+-rw-r--r--   0        0        0     7868 2024-04-16 15:35:00.582419 lindi-0.2.1/lindi/LindiH5pyFile/LindiReferenceFileSystemStore.py
+-rw-r--r--   0        0        0      327 2024-03-21 11:16:09.352672 lindi-0.2.1/lindi/LindiH5pyFile/__init__.py
+-rw-r--r--   0        0        0      747 2024-04-04 18:56:02.146012 lindi-0.2.1/lindi/LindiH5pyFile/writers/LindiH5pyAttributesWriter.py
+-rw-r--r--   0        0        0     1961 2024-04-04 18:56:02.146012 lindi-0.2.1/lindi/LindiH5pyFile/writers/LindiH5pyDatasetWriter.py
+-rw-r--r--   0        0        0     5349 2024-04-16 15:35:00.586419 lindi-0.2.1/lindi/LindiH5pyFile/writers/LindiH5pyGroupWriter.py
+-rw-r--r--   0        0        0        0 2024-04-04 18:56:02.146012 lindi-0.2.1/lindi/LindiH5pyFile/writers/__init__.py
+-rw-r--r--   0        0        0     9558 2024-04-16 15:35:00.586419 lindi-0.2.1/lindi/LindiStagingStore/LindiStagingStore.py
+-rw-r--r--   0        0        0     2915 2024-04-16 15:35:00.586419 lindi-0.2.1/lindi/LindiStagingStore/StagingArea.py
+-rw-r--r--   0        0        0       76 2024-04-16 15:35:00.586419 lindi-0.2.1/lindi/LindiStagingStore/__init__.py
+-rw-r--r--   0        0        0      286 2024-04-16 15:35:00.586419 lindi-0.2.1/lindi/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 18:56:02.146012 lindi-0.2.1/lindi/conversion/__init__.py
+-rw-r--r--   0        0        0      167 2024-04-04 18:56:02.146012 lindi-0.2.1/lindi/conversion/_util.py
+-rw-r--r--   0        0        0     5907 2024-04-04 18:56:02.146012 lindi-0.2.1/lindi/conversion/attr_conversion.py
+-rw-r--r--   0        0        0    10819 2024-04-16 15:35:00.586419 lindi-0.2.1/lindi/conversion/create_zarr_dataset_from_h5_data.py
+-rw-r--r--   0        0        0     1079 2024-04-15 13:56:49.245944 lindi-0.2.1/lindi/conversion/decode_references.py
+-rw-r--r--   0        0        0     2887 2024-04-15 13:02:34.168232 lindi-0.2.1/lindi/conversion/h5_filters_to_codecs.py
+-rw-r--r--   0        0        0     2041 2024-04-15 15:43:24.681869 lindi-0.2.1/lindi/conversion/h5_ref_to_zarr_attr.py
+-rw-r--r--   0        0        0      936 2024-04-15 12:47:02.787743 lindi-0.2.1/lindi/conversion/nan_inf_ninf.py
+-rw-r--r--   0        0        0      503 2024-04-15 12:44:19.013722 lindi-0.2.1/lindi/conversion/reformat_json.py
+-rw-r--r--   0        0        0      748 2024-04-16 15:35:20.118151 lindi-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5869 1970-01-01 00:00:00.000000 lindi-0.2.1/PKG-INFO
```

### Comparing `lindi-0.2.0/LICENSE` & `lindi-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lindi-0.2.0/lindi/LindiH5ZarrStore/LindiH5ZarrStore.py` & `lindi-0.2.1/lindi/LindiH5ZarrStore/LindiH5ZarrStore.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,22 +3,26 @@
 from typing import Union, List, IO, Any, Dict, Literal
 from dataclasses import dataclass
 import numpy as np
 import zarr
 import remfile
 from zarr.storage import Store, MemoryStore
 import h5py
-from ._zarr_info_for_h5_dataset import _zarr_info_for_h5_dataset
 from ._util import (
     _read_bytes,
     _get_chunk_byte_range,
     _get_byte_range_for_contiguous_dataset,
+    _join,
+    _get_chunk_names_for_dataset
 )
-from ._h5_attr_to_zarr_attr import _h5_attr_to_zarr_attr
-from ._utils import _join, _get_chunk_names_for_dataset, _reformat_json
+from ..conversion.attr_conversion import h5_to_zarr_attr
+from ..conversion.reformat_json import reformat_json
+from ..conversion.h5_filters_to_codecs import h5_filters_to_codecs
+from ..conversion.create_zarr_dataset_from_h5_data import create_zarr_dataset_from_h5_data
+from ..LindiH5pyFile.LindiReferenceFileSystemStore import LindiReferenceFileSystemStore
 
 
 @dataclass
 class LindiH5ZarrStoreOpts:
     """
     Options for the LindiH5ZarrStore class.
 
@@ -62,17 +66,16 @@
         self._h5f: Union[h5py.File, None] = h5py.File(_file, "r")
         self._url = _url
         self._opts = _opts
         self._entities_to_close = _entities_to_close + [self._h5f]
 
         # Some datasets do not correspond to traditional chunked datasets. For
         # those datasets, we need to store the inline data so that we can return
-        # it when the chunk is requested. We store the inline data in a
-        # dictionary with the dataset name as the key. The values are the bytes.
-        self._inline_data_for_arrays: Dict[str, bytes] = {}
+        # it when the chunk is requested.
+        self._inline_arrays: Dict[str, InlineArray] = {}
 
         self._external_array_links: Dict[str, Union[dict, None]] = {}
 
     @staticmethod
     def from_file(
         hdf5_file_name_or_url: str,
         *,
@@ -132,14 +135,20 @@
         elif key_name == ".zarray":
             # Get the .zarray JSON text for a dataset
             return self._get_zarray_bytes(key_parent)
         else:
             # Otherwise, we assume it is a chunk file
             return self._get_chunk_file_bytes(key_parent=key_parent, key_name=key_name)
 
+    def get(self, key, default=None):
+        try:
+            return self.__getitem__(key)
+        except KeyError:
+            return default
+
     def __contains__(self, key):
         """Check if a key is in the store (used by zarr)."""
         # it would be nice if we didn't have to repeat the logic from __getitem__
         if self._h5f is None:
             raise Exception("Store is closed")
         parts = [part for part in key.split("/") if part]
         if len(parts) == 0:
@@ -171,24 +180,31 @@
                 return False
             if not isinstance(h5_item, h5py.Dataset):
                 return False
             external_array_link = self._get_external_array_link(key_parent, h5_item)
             if external_array_link is not None:
                 # The chunk files do not exist for external array links
                 return False
+            if np.prod(h5_item.shape) == 0:
+                return False
             if h5_item.ndim == 0:
                 return key_name == "0"
             chunk_name_parts = key_name.split(".")
             if len(chunk_name_parts) != h5_item.ndim:
                 return False
-            shape = h5_item.shape
-            chunks = h5_item.chunks or shape
-            chunk_coords_shape = [
-                (shape[i] + chunks[i] - 1) // chunks[i] for i in range(len(shape))
-            ]
+            inline_array = self._get_inline_array(key, h5_item)
+            if inline_array.is_inline:
+                chunk_coords_shape = (1,) * h5_item.ndim
+            else:
+                shape = h5_item.shape
+                chunks = h5_item.chunks or shape
+                chunk_coords_shape = [
+                    (shape[i] + chunks[i] - 1) // chunks[i] if chunks[i] != 0 else 0
+                    for i in range(len(shape))
+                ]
             chunk_coords = tuple(int(x) for x in chunk_name_parts)
             for i, c in enumerate(chunk_coords):
                 if c < 0 or c >= chunk_coords_shape[i]:
                     return False
             return True
 
     def __delitem__(self, key):
@@ -218,92 +234,95 @@
             link = self._h5f.get('/' + parent_key, getlink=True)
             if isinstance(link, h5py.ExternalLink):
                 raise Exception(f"External links not supported: {parent_key}")
             elif isinstance(link, h5py.SoftLink):
                 # if it's a soft link, we return a special attribute and ignore
                 # the rest of the attributes because they should be stored in
                 # the target of the soft link
-                return _reformat_json(json.dumps({
+                return reformat_json(json.dumps({
                     "_SOFT_LINK": {
                         "path": link.path
                     }
                 }).encode("utf-8"))
 
         # We create a dummy zarr group and copy the attributes to it. That way
         # we know that zarr has accepted them and they are serialized in the
         # correct format.
         memory_store = MemoryStore()
         dummy_group = zarr.group(store=memory_store)
         for k, v in h5_item.attrs.items():
-            v2 = _h5_attr_to_zarr_attr(v, label=f"{parent_key} {k}", h5f=self._h5f)
+            v2 = h5_to_zarr_attr(v, label=f"{parent_key} {k}", h5f=self._h5f)
             if v2 is not None:
                 dummy_group.attrs[k] = v2
         if isinstance(h5_item, h5py.Dataset):
-            if h5_item.ndim == 0:
-                dummy_group.attrs["_SCALAR"] = True
-            if h5_item.dtype.kind == "V":  # compound type
-                compound_dtype = [
-                    [name, str(h5_item.dtype[name])]
-                    for name in h5_item.dtype.names
-                ]
-                # For example: [['x', 'uint32'], ['y', 'uint32'], ['weight', 'float32']]
-                dummy_group.attrs["_COMPOUND_DTYPE"] = compound_dtype
+            inline_array = self._get_inline_array(parent_key, h5_item)
+            for k, v in inline_array.additional_zarr_attrs.items():
+                dummy_group.attrs[k] = v
             external_array_link = self._get_external_array_link(parent_key, h5_item)
             if external_array_link is not None:
                 dummy_group.attrs["_EXTERNAL_ARRAY_LINK"] = external_array_link
-        zattrs_content = _reformat_json(memory_store.get(".zattrs"))
-        if zattrs_content is not None:
-            return zattrs_content
-        else:
-            # No attributes, so we return an empty JSON object
-            return "{}".encode("utf-8")
+        zattrs_content = reformat_json(memory_store.get(".zattrs") or "{}".encode("utf-8"))
+        return zattrs_content
 
     def _get_zgroup_bytes(self, parent_key: str):
         """Get the .zgroup JSON text for a group"""
         if self._h5f is None:
             raise Exception("Store is closed")
         h5_item = self._h5f.get('/' + parent_key, None)
         if not isinstance(h5_item, h5py.Group):
-            raise Exception(f"Item {parent_key} is not a group")
+            # Important to raise a KeyError here because that's what zarr expects
+            raise KeyError(f"Item {parent_key} is not a group")
         # We create a dummy zarr group and then get the .zgroup JSON text
         # from it.
         memory_store = MemoryStore()
         zarr.group(store=memory_store)
-        return _reformat_json(memory_store.get(".zgroup"))
+        return reformat_json(memory_store.get(".zgroup"))
+
+    def _get_inline_array(self, key: str, h5_dataset: h5py.Dataset):
+        if key in self._inline_arrays:
+            return self._inline_arrays[key]
+        self._inline_arrays[key] = InlineArray(h5_dataset)
+        return self._inline_arrays[key]
 
     def _get_zarray_bytes(self, parent_key: str):
         """Get the .zarray JSON text for a dataset"""
         if self._h5f is None:
             raise Exception("Store is closed")
         h5_item = self._h5f.get('/' + parent_key, None)
         if not isinstance(h5_item, h5py.Dataset):
-            raise Exception(f"Item {parent_key} is not a dataset")
+            # Important to raise a KeyError here because that's what zarr expects
+            raise KeyError(f"Item {parent_key} is not a dataset")
         # get the shape, chunks, dtype, and filters from the h5 dataset
-        info = _zarr_info_for_h5_dataset(h5_item)
-        if info.inline_data is not None:
-            self._inline_data_for_arrays[parent_key] = info.inline_data
+        inline_array = self._get_inline_array(parent_key, h5_item)
+        if inline_array.is_inline:
+            return inline_array.zarray_bytes
+
+        filters = h5_filters_to_codecs(h5_item)
+
         # We create a dummy zarr dataset with the appropriate shape, chunks,
         # dtype, and filters and then copy the .zarray JSON text from it
         memory_store = MemoryStore()
         dummy_group = zarr.group(store=memory_store)
         # Importantly, I'm pretty sure this doesn't actually create the
         # chunks in the memory store. That's important because we just need
         # to get the .zarray JSON text from the dummy group.
         dummy_group.create_dataset(
             name="dummy_array",
-            shape=info.shape,
-            chunks=info.chunks,
-            dtype=info.dtype,
+            shape=h5_item.shape,
+            # It's important to not have chunks be None here because that would
+            # let zarr choose an optimal chunking, whereas we need this to reflect
+            # the actual chunking in the HDF5 file.
+            chunks=h5_item.chunks if h5_item.chunks is not None else h5_item.shape,
+            dtype=h5_item.dtype,
             compressor=None,
             order="C",
-            fill_value=info.fill_value,
-            filters=info.filters,
-            object_codec=info.object_codec,
+            fill_value=h5_item.fillvalue,
+            filters=filters
         )
-        zarray_text = _reformat_json(memory_store.get("dummy_array/.zarray"))
+        zarray_text = reformat_json(memory_store.get("dummy_array/.zarray"))
 
         return zarray_text
 
     def _get_chunk_file_bytes(self, key_parent: str, key_name: str):
         if self._file is None:
             raise Exception("Store is closed")
         byte_offset, byte_count, inline_data = self._get_chunk_file_bytes_data(
@@ -337,50 +356,51 @@
                     f"Unable to handle case where chunks is not None but ndim is 0 for dataset {key_parent}"
                 )
             if key_name != "0":
                 raise Exception(
                     f"Chunk name {key_name} does not match dataset dimensions"
                 )
 
-        # Check whether we have inline data for this array. This would be set
-        # when we created the .zarray JSON text for the dataset. Note that this
-        # means that the .zarray file needs to be read before the chunk files,
-        # which should always be the case (I assume).
-        if key_parent in self._inline_data_for_arrays:
-            x = self._inline_data_for_arrays[key_parent]
-            if isinstance(x, bytes):
-                return None, None, x
-            else:
+        # In the case of shape 0, we raise an exception because we shouldn't be here
+        if np.prod(h5_item.shape) == 0:
+            raise Exception(
+                f"Chunk file {key_parent}/{key_name} is not present because the dataset has shape 0."
+            )
+
+        inline_array = self._get_inline_array(key_parent, h5_item)
+        if inline_array.is_inline:
+            if key_name != inline_array.chunk_fname:
                 raise Exception(
-                    f"Inline data for dataset {key_parent} is not bytes. It is {type(x)}"
+                    f"Chunk name {key_name} does not match dataset dimensions for inline array {key_parent}"
                 )
+            return None, None, inline_array.chunk_bytes
 
         # If this is a scalar, then the data should have been inline
         if h5_item.ndim == 0:
             raise Exception(f"No inline data for scalar dataset {key_parent}")
 
         # Get the chunk coords from the file name
         chunk_name_parts = key_name.split(".")
         if len(chunk_name_parts) != h5_item.ndim:
             raise Exception(f"Chunk name {key_name} does not match dataset dimensions")
         chunk_coords = tuple(int(x) for x in chunk_name_parts)
         for i, c in enumerate(chunk_coords):
             if c < 0 or c >= h5_item.shape[i]:
                 raise Exception(
-                    f"Chunk coordinates {chunk_coords} out of range for dataset {key_parent}"
+                    f"Chunk coordinates {chunk_coords} out of range for dataset {key_parent} with dtype {h5_item.dtype}"
                 )
         if h5_item.chunks is not None:
             # Get the byte range in the file for the chunk.
             byte_offset, byte_count = _get_chunk_byte_range(h5_item, chunk_coords)
         else:
             # In this case (contiguous dataset), we need to check that the chunk
             # coordinates are (0, 0, 0, ...)
             if chunk_coords != (0,) * h5_item.ndim:
                 raise Exception(
-                    f"Chunk coordinates {chunk_coords} are not (0, 0, 0, ...) for contiguous dataset {key_parent}"
+                    f"Chunk coordinates {chunk_coords} are not (0, 0, 0, ...) for contiguous dataset {key_parent} with dtype {h5_item.dtype} and shape {h5_item.shape}"
                 )
             # Get the byte range in the file for the contiguous dataset
             byte_offset, byte_count = _get_byte_range_for_contiguous_dataset(h5_item)
         return byte_offset, byte_count, None
 
     def _get_external_array_link(self, parent_key: str, h5_item: h5py.Dataset):
         # First check the memory cache
@@ -391,15 +411,16 @@
         if h5_item.chunks and self._opts.num_dataset_chunks_threshold is not None:
             # We compute the expected number of chunks using the shape and chunks
             # and compare it to the threshold. If it's greater, then we create an
             # external array link.
             shape = h5_item.shape
             chunks = h5_item.chunks
             chunk_coords_shape = [
-                (shape[i] + chunks[i] - 1) // chunks[i] for i in range(len(shape))
+                (shape[i] + chunks[i] - 1) // chunks[i] if chunks[i] != 0 else 0
+                for i in range(len(shape))
             ]
             num_chunks = np.prod(chunk_coords_shape)
             if num_chunks > self._opts.num_dataset_chunks_threshold:
                 if self._url is not None:
                     self._external_array_links[parent_key] = {
                         "link_type": "hdf5_dataset",
                         "url": self._url,  # url is not going to be null based on the check in __init__
@@ -505,16 +526,16 @@
                     if isinstance(subitem, h5py.Group):
                         # recursively process subgroups
                         _process_group(_join(key, k), subitem)
                     elif isinstance(subitem, h5py.Dataset):
                         _process_dataset(_join(key, k))
 
         def _process_dataset(key):
-            # Add the .zattrs and .zarray files for the dataset
-            zattrs_bytes = self.get(f"{key}/.zattrs")
+            # Add the .zattrs and .zarray files for the dataset=
+            zattrs_bytes = self[f"{key}/.zattrs"]
             assert zattrs_bytes is not None
             if zattrs_bytes != b"{}":  # don't include empty zattrs
                 _add_ref(f"{key}/.zattrs", zattrs_bytes)
             zattrs_dict = json.loads(zattrs_bytes.decode("utf-8"))
             external_array_link = zattrs_dict.get(
                 "_EXTERNAL_ARRAY_LINK", None
             )
@@ -524,15 +545,16 @@
             zarray_dict = json.loads(zarray_bytes.decode("utf-8"))
 
             if external_array_link is None:
                 # Only add chunk references for datasets without an external array link
                 shape = zarray_dict["shape"]
                 chunks = zarray_dict.get("chunks", None)
                 chunk_coords_shape = [
-                    (shape[i] + chunks[i] - 1) // chunks[i]
+                    # the shape could be zero -- for example dandiset 000559 - acquisition/depth_video/data has shape [0, 0, 0]
+                    (shape[i] + chunks[i] - 1) // chunks[i] if chunks[i] != 0 else 0
                     for i in range(len(shape))
                 ]
                 # For example, chunk_names could be ['0', '1', '2', ...]
                 # or ['0.0', '0.1', '0.2', ...]
                 chunk_names = _get_chunk_names_for_dataset(
                     chunk_coords_shape
                 )
@@ -551,8 +573,85 @@
                             self._url,
                             byte_offset,
                             byte_count,
                         ]
 
         # Process the groups recursively starting with the root group
         _process_group("", self._h5f)
+
+        LindiReferenceFileSystemStore.replace_meta_file_contents_with_dicts(ret)
         return ret
+
+
+class InlineArray:
+    def __init__(self, h5_dataset: h5py.Dataset):
+        self._additional_zarr_attributes = {}
+        if h5_dataset.shape == ():
+            self._additional_zarr_attributes["_SCALAR"] = True
+            self._is_inline = True
+            ...
+        elif h5_dataset.dtype.kind in ['i', 'u', 'f']:  # integer or float
+            self._is_inline = False
+        else:
+            self._is_inline = True
+            if h5_dataset.dtype.kind == "V" and h5_dataset.dtype.fields is not None:  # compound type
+                compound_dtype = []
+                for name in h5_dataset.dtype.names:
+                    tt = h5_dataset.dtype[name]
+                    if tt == h5py.special_dtype(ref=h5py.Reference):
+                        tt = "<REFERENCE>"
+                    compound_dtype.append((name, str(tt)))
+                # For example: [['x', 'uint32'], ['y', 'uint32'], ['weight', 'float32']]
+                self._additional_zarr_attributes["_COMPOUND_DTYPE"] = compound_dtype
+        if self._is_inline:
+            memory_store = MemoryStore()
+            dummy_group = zarr.group(store=memory_store)
+            size_is_zero = np.prod(h5_dataset.shape) == 0
+            create_zarr_dataset_from_h5_data(
+                zarr_parent_group=dummy_group,
+                name='X',
+                # For inline data it's important for now that we enforce a
+                # single chunk because the rest of the code assumes a single
+                # chunk for inline data. The assumption is that the inline
+                # arrays are not going to be very large.
+                h5_chunks=h5_dataset.shape if h5_dataset.shape != () and not size_is_zero else None,
+                label=f'{h5_dataset.name}',
+                h5_shape=h5_dataset.shape,
+                h5_dtype=h5_dataset.dtype,
+                h5f=h5_dataset.file,
+                h5_data=h5_dataset[...]
+            )
+            self._zarray_bytes = reformat_json(memory_store['X/.zarray'])
+            if not size_is_zero:
+                if h5_dataset.ndim == 0:
+                    chunk_fname = '0'
+                else:
+                    chunk_fname = '.'.join(['0'] * h5_dataset.ndim)
+                self._chunk_fname = chunk_fname
+                self._chunk_bytes = memory_store[f'X/{chunk_fname}']
+            else:
+                self._chunk_fname = None
+                self._chunk_bytes = None
+        else:
+            self._zarray_bytes = None
+            self._chunk_fname = None
+            self._chunk_bytes = None
+
+    @property
+    def is_inline(self):
+        return self._is_inline
+
+    @property
+    def additional_zarr_attrs(self):
+        return self._additional_zarr_attributes
+
+    @property
+    def zarray_bytes(self):
+        return self._zarray_bytes
+
+    @property
+    def chunk_fname(self):
+        return self._chunk_fname
+
+    @property
+    def chunk_bytes(self):
+        return self._chunk_bytes
```

### Comparing `lindi-0.2.0/lindi/LindiH5ZarrStore/_h5_filters_to_codecs.py` & `lindi-0.2.1/lindi/conversion/h5_filters_to_codecs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 from typing import List, Union
 import h5py
 import numcodecs
 from numcodecs.abc import Codec
 
+# The purpose of _h5_filters_to_codecs it to translate the filters that are
+# defined on an HDF5 dataset into numcodecs filters for use with Zarr so that
+# the raw data chunks can stay within the the HDF5 file and be read by Zarr
+# without having to copy/convert the data.
+
 
 # This is adapted from _decode_filters from kerchunk source
 # https://github.com/fsspec/kerchunk
 # Copyright (c) 2020 Intake
 # MIT License
-def _h5_filters_to_codecs(h5obj: h5py.Dataset) -> Union[List[Codec], None]:
+def h5_filters_to_codecs(h5obj: h5py.Dataset) -> Union[List[Codec], None]:
     """Decode HDF5 filters to numcodecs filters."""
     if h5obj.scaleoffset:
         raise RuntimeError(
             f"{h5obj.name} uses HDF5 scaleoffset filter - not supported"
         )
     if h5obj.compression in ("szip", "lzf"):
         raise RuntimeError(
@@ -59,13 +64,16 @@
         elif str(filter_id) == "32008":
             raise RuntimeError(
                 f"{h5obj.name} uses bitshuffle compression - not supported"
             )
         elif str(filter_id) == "shuffle":
             # already handled before this loop
             pass
+        elif str(filter_id) == "fletcher32":
+            # added by lindi (not in kerchunk) -- required by dandiset 000117
+            filters.append(numcodecs.Fletcher32())
         else:
             raise RuntimeError(
                 f"{h5obj.name} uses filter id {filter_id} with properties {properties},"
                 f" not supported."
             )
     return filters
```

### Comparing `lindi-0.2.0/lindi/LindiH5ZarrStore/_util.py` & `lindi-0.2.1/lindi/LindiH5ZarrStore/_util.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import IO
+from typing import IO, List
 import numpy as np
 import h5py
 
 
 def _read_bytes(file: IO, offset: int, count: int):
     """Read a range of bytes from a file-like object."""
     file.seek(offset)
@@ -16,15 +16,16 @@
     to get the chunk index. Then we call _get_chunk_byte_range_for_chunk_index.
     """
     shape = h5_dataset.shape
     chunk_shape = h5_dataset.chunks
     assert chunk_shape is not None
 
     chunk_coords_shape = [
-        (shape[i] + chunk_shape[i] - 1) // chunk_shape[i]
+        # the shape could be zero -- for example dandiset 000559 - acquisition/depth_video/data has shape [0, 0, 0]
+        (shape[i] + chunk_shape[i] - 1) // chunk_shape[i] if chunk_shape[i] != 0 else 0
         for i in range(len(shape))
     ]
     ndim = h5_dataset.ndim
     assert len(chunk_coords) == ndim
     chunk_index = 0
     for i in range(ndim):
         chunk_index += int(chunk_coords[i] * np.prod(chunk_coords_shape[i + 1:]))
@@ -51,7 +52,34 @@
     contiguously in the file.
     """
     # got hints from kerchunk source code
     dsid = h5_dataset.id
     byte_offset = dsid.get_offset()
     byte_count = dsid.get_storage_size()
     return byte_offset, byte_count
+
+
+def _join(a: str, b: str) -> str:
+    if a == "":
+        return b
+    else:
+        return f"{a}/{b}"
+
+
+def _get_chunk_names_for_dataset(chunk_coords_shape: List[int]) -> List[str]:
+    """Get the chunk names for a dataset with the given chunk coords shape.
+
+    For example: _get_chunk_names_for_dataset([1, 2, 3]) returns
+    ['0.0.0', '0.0.1', '0.0.2', '0.1.0', '0.1.1', '0.1.2']
+    """
+    ndim = len(chunk_coords_shape)
+    if ndim == 0:
+        return ["0"]
+    elif ndim == 1:
+        return [str(i) for i in range(chunk_coords_shape[0])]
+    else:
+        names0 = _get_chunk_names_for_dataset(chunk_coords_shape[1:])
+        names = []
+        for i in range(chunk_coords_shape[0]):
+            for name0 in names0:
+                names.append(f"{i}.{name0}")
+        return names
```

### Comparing `lindi-0.2.0/lindi/LindiH5ZarrStore/_zarr_info_for_h5_dataset.py` & `lindi-0.2.1/lindi/conversion/create_zarr_dataset_from_h5_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,215 +1,254 @@
-import json
-import struct
-from typing import Union, List, Any, Tuple
+from typing import Union, List, Any, Tuple, Literal
 from dataclasses import dataclass
 import numpy as np
 import numcodecs
-import h5py
 from numcodecs.abc import Codec
-from ._h5_attr_to_zarr_attr import _h5_ref_to_zarr_attr
-from ._h5_filters_to_codecs import _h5_filters_to_codecs
-
-
-@dataclass
-class ZarrInfoForH5Dataset:
-    shape: Tuple[int]
-    chunks: Tuple[int]
-    dtype: Any
-    filters: Union[List[Codec], None]
-    fill_value: Any
-    object_codec: Union[None, Codec]
-    inline_data: Union[bytes, None]
-
-
-def _zarr_info_for_h5_dataset(h5_dataset: h5py.Dataset) -> ZarrInfoForH5Dataset:
-    """Get the information needed to create a zarr dataset from an h5py dataset.
-
-    This is the main workhorse function for LindiH5ZarrStore. It takes an h5py
-    dataset and returns a ZarrInfoForH5Dataset object.
-
-    It handles the following cases:
-
-    For non-scalars, if it is a numeric array, then the data can stay where it
-    is in the hdf5 file. The hdf5 filters are translated into zarr filters using
-    the _h5_filters_to_codecs function.
-
-    If it is a non-scalar object array, then the inline_data will be a JSON
-    string and the JSON codec will be used.
-
-    When the shape is (), we have a scalar dataset. Since zarr doesn't support
-    scalar datasets, we make an array of shape (1,). The _SCALAR attribute will
-    be set to True elsewhere to indicate that it is actually a scalar. The
-    inline_data attribute will be set. In the case of a numeric scalar, it will
-    be a bytes object with the binary representation of the value. In the case
-    of an object, the inline_data will be a JSON string and the JSON codec will
-    be used.
+import h5py
+import zarr
+from .h5_ref_to_zarr_attr import h5_ref_to_zarr_attr
+from .attr_conversion import h5_to_zarr_attr
+from ._util import _is_numeric_dtype
+
+
+def create_zarr_dataset_from_h5_data(
+    zarr_parent_group: zarr.Group,
+    h5_shape: Tuple,
+    h5_dtype: Any,
+    h5_data: Union[Any, None],
+    h5f: Union[h5py.File, None],
+    name: str,
+    label: str,
+    h5_chunks: Union[Tuple, None],
+    zarr_compressor: Union[Codec, Literal['default']] = 'default'
+):
+    """Create a zarr dataset from an h5py dataset.
+
+    Parameters
+    ----------
+    zarr_parent_group : zarr.Group
+        The parent group in the zarr hierarchy. The new dataset will be created
+        in this group.
+    h5_shape : tuple
+        The shape of the h5py dataset.
+    h5_dtype : numpy.dtype
+        The dtype of the h5py dataset.
+    h5_data : any
+        The data of the h5py dataset. If None, the dataset will be created
+        without data.
+    h5f : h5py.File
+        The file that the h5py dataset is in.
+    name : str
+        The name of the new dataset in the zarr hierarchy.
+    label : str
+        The name of the h5py dataset for error messages.
+    h5_chunks : tuple
+        The chunk shape of the h5py dataset.
+    zarr_compressor : numcodecs.abc.Codec
+        The codec compressor to use when writing the dataset. If default, the
+        default compressor will be used.
     """
-    shape = h5_dataset.shape
-    dtype = h5_dataset.dtype
-
-    if len(shape) == 0:
+    if h5_dtype is None:
+        raise Exception(f'No dtype in h5_to_zarr_dataset_prep for dataset {label}')
+    if len(h5_shape) == 0:
         # scalar dataset
-        value = h5_dataset[()]
         # zarr doesn't support scalar datasets, so we make an array of shape (1,)
         # and the _SCALAR attribute will be set to True elsewhere to indicate that
         # it is a scalar dataset
 
-        # Let's handle all the possible types explicitly
-        numeric_format_str = _get_numeric_format_str(dtype)
-        if numeric_format_str is not None:
+        if h5_data is None:
+            raise Exception(f'Data must be provided for scalar dataset {label}')
+
+        if zarr_compressor != 'default':
+            raise Exception('zarr_compressor is not supported for scalar datasets')
+
+        if _is_numeric_dtype(h5_dtype) or h5_dtype in [bool, np.bool_]:
             # Handle the simple numeric types
-            inline_data = struct.pack(numeric_format_str, value)
-            return ZarrInfoForH5Dataset(
+            ds = zarr_parent_group.create_dataset(
+                name,
                 shape=(1,),
-                chunks=(1,),  # be explicit about chunks
-                dtype=dtype,
-                filters=None,
-                fill_value=0,
-                object_codec=None,
-                inline_data=inline_data
+                chunks=(1,),
+                data=[h5_data[()]] if isinstance(h5_data, h5py.Dataset) or isinstance(h5_data, np.ndarray) else [h5_data],
             )
-        elif dtype == object:
+            ds.attrs['_SCALAR'] = True
+            return ds
+        elif h5_dtype.kind == 'O':
             # For type object, we are going to use the JSON codec
-            # which requires inline data of the form [[val], '|O', [1]]
-            if isinstance(value, (bytes, str)):
-                if isinstance(value, bytes):
-                    value = value.decode()
-                return ZarrInfoForH5Dataset(
+            # for encoding [scalar_value]
+            scalar_value = h5_data[()] if isinstance(h5_data, h5py.Dataset) or isinstance(h5_data, np.ndarray) else h5_data
+            if isinstance(scalar_value, (bytes, str)):
+                if isinstance(scalar_value, bytes):
+                    scalar_value = scalar_value.decode()
+                ds = zarr_parent_group.create_dataset(
+                    name,
                     shape=(1,),
-                    chunks=(1,),  # be explicit about chunks
-                    dtype=dtype,
-                    filters=None,
-                    fill_value=' ',
-                    object_codec=numcodecs.JSON(),
-                    inline_data=json.dumps([value, '|O', [1]], separators=(',', ':')).encode('utf-8')
+                    chunks=(1,),
+                    data=[scalar_value]
                 )
+                ds.attrs['_SCALAR'] = True
+                return ds
             else:
-                raise Exception(f'Not yet implemented (1): object scalar dataset with value {value} and dtype {dtype}')
+                raise Exception(f'Unsupported scalar value type: {type(scalar_value)}')
+        elif h5_dtype.kind == 'S' or h5_dtype.kind == 'U':
+            # byte string
+            if h5_data is None:
+                raise Exception(f'Data must be provided for scalar dataset {label}')
+            scalar_value = h5_data[()] if isinstance(h5_data, h5py.Dataset) or isinstance(h5_data, np.ndarray) else h5_data
+            ds = zarr_parent_group.create_dataset(
+                name,
+                shape=(1,),
+                chunks=(1,),
+                data=[scalar_value]
+            )
+            ds.attrs['_SCALAR'] = True
+            return ds
         else:
-            raise Exception(f'Cannot handle scalar dataset {h5_dataset.name} with dtype {dtype}')
+            raise Exception(f'Cannot handle scalar dataset {label} with dtype {h5_dtype}')
     else:
         # not a scalar dataset
-        if dtype.kind in ['i', 'u', 'f', 'b']:  # integer, unsigned integer, float, boolean
+
+        if isinstance(h5_data, list):
+            # If we have a list, then we need to convert it to an array
+            h5_data = np.array(h5_data)
+
+        if _is_numeric_dtype(h5_dtype) or h5_dtype in [bool, np.bool_]:  # integer, unsigned integer, float, bool
             # This is the normal case of a chunked dataset with a numeric (or boolean) dtype
-            filters = _h5_filters_to_codecs(h5_dataset)
-            chunks = h5_dataset.chunks
-            if chunks is None:
-                # If the dataset is not chunked, we use the entire dataset as a single chunk
-                # It's important to be explicit about the chunks, because I think None means that zarr could decide otherwise
-                chunks = shape
-            return ZarrInfoForH5Dataset(
-                shape=shape,
-                chunks=chunks,
-                dtype=dtype,
-                filters=filters,
-                fill_value=h5_dataset.fillvalue,
-                object_codec=None,
-                inline_data=None
+            if h5_chunks is None:
+                # We require that chunks be specified when writing a dataset with more
+                # than 1 million elements. This is because zarr may default to
+                # suboptimal chunking. Note that the default for h5py is to use the
+                # entire dataset as a single chunk.
+                total_size = np.prod(h5_shape) if len(h5_shape) > 0 else 1
+                if total_size > 1000 * 1000:
+                    raise Exception(f'Chunks must be specified explicitly when writing dataset of shape {h5_shape}')
+            # Note that we are not using the same filters as in the h5py dataset
+            return zarr_parent_group.create_dataset(
+                name,
+                shape=h5_shape,
+                chunks=h5_chunks,
+                dtype=h5_dtype,
+                data=h5_data,
+                compressor=zarr_compressor
             )
-        elif dtype.kind == 'O':
+        elif h5_dtype.kind == 'O':
             # For type object, we are going to use the JSON codec
-            # which requires inline data of the form [list, of, items, ..., '|O', [n1, n2, ...]]
-            object_codec = numcodecs.JSON()
-            data = h5_dataset[:]
-            data_vec_view = data.ravel()
-            for i, val in enumerate(data_vec_view):
-                if isinstance(val, bytes):
-                    data_vec_view[i] = val.decode()
-                elif isinstance(val, str):
-                    data_vec_view[i] = val
-                elif isinstance(val, h5py.Reference):
-                    data_vec_view[i] = _h5_ref_to_zarr_attr(val, label=f'{h5_dataset.name}[{i}]', h5f=h5_dataset.file)
-                else:
-                    raise Exception(f'Cannot handle dataset {h5_dataset.name} with dtype {dtype} and shape {shape}')
-            inline_data = json.dumps(data.tolist() + ['|O', list(shape)], separators=(',', ':')).encode('utf-8')
-            return ZarrInfoForH5Dataset(
-                shape=shape,
-                chunks=shape,  # be explicit about chunks
-                dtype=dtype,
-                filters=None,
-                fill_value=' ',  # not sure what to put here
-                object_codec=object_codec,
-                inline_data=inline_data
-            )
-        elif dtype.kind in 'SU':  # byte string or unicode string
-            raise Exception(f'Not yet implemented (2): dataset {h5_dataset.name} with dtype {dtype} and shape {shape}')
-        elif dtype.kind == 'V':  # void (i.e. compound)
-            if h5_dataset.ndim == 1:
-                # for now we only handle the case of a 1D compound dataset
-                data = h5_dataset[:]
-                # Create an array that would be for example like this
-                # dtype = np.dtype([('x', np.float64), ('y', np.int32), ('weight', np.float64)])
-                # array_list = [[3, 4, 5.3], [2, 1, 7.1], ...]
-                # where the first entry corresponds to x in the example above, the second to y, and the third to weight
-                # This is a more compact representation than [{'x': ...}]
-                # The _COMPOUND_DTYPE attribute will be set on the dataset in the zarr store
-                # which will be used to interpret the data
-                array_list = [
-                    [
-                        _json_serialize(data[name][i], dtype[name], h5_dataset)
-                        for name in dtype.names
-                    ]
-                    for i in range(h5_dataset.shape[0])
-                ]
-                object_codec = numcodecs.JSON()
-                inline_data = array_list + ['|O', list(shape)]
-                return ZarrInfoForH5Dataset(
-                    shape=shape,
-                    chunks=shape,  # be explicit about chunks
-                    dtype='object',
-                    filters=None,
-                    fill_value=' ',  # not sure what to put here
-                    object_codec=object_codec,
-                    inline_data=json.dumps(inline_data, separators=(',', ':')).encode('utf-8')
-                )
+            if zarr_compressor != 'default':
+                raise Exception('zarr_compressor is not supported for object datasets')
+            if h5_data is not None:
+                if isinstance(h5_data, h5py.Dataset):
+                    h5_data = h5_data[:]
+                zarr_data = h5_object_data_to_zarr_data(h5_data, h5f=h5f, label=label)
             else:
-                raise Exception(f'More than one dimension not supported for compound dataset {h5_dataset.name} with dtype {dtype} and shape {shape}')
+                zarr_data = None
+            object_codec = numcodecs.JSON()
+            return zarr_parent_group.create_dataset(
+                name,
+                shape=h5_shape,
+                chunks=h5_chunks,
+                dtype=h5_dtype,
+                data=zarr_data,
+                object_codec=object_codec
+            )
+        elif h5_dtype.kind == 'S':  # byte string
+            if zarr_compressor != 'default':
+                raise Exception('zarr_compressor is not supported for byte string datasets')
+            if h5_data is None:
+                raise Exception(f'Data must be provided when converting dataset {label} with dtype {h5_dtype}')
+            return zarr_parent_group.create_dataset(
+                name,
+                shape=h5_shape,
+                chunks=h5_chunks,
+                dtype=h5_dtype,
+                data=h5_data
+            )
+        elif h5_dtype.kind == 'U':  # unicode string
+            if zarr_compressor != 'default':
+                raise Exception('zarr_compressor is not supported for unicode string datasets')
+            raise Exception(f'Array of unicode strings not supported: dataset {label} with dtype {h5_dtype} and shape {h5_shape}')
+        elif h5_dtype.kind == 'V' and h5_dtype.fields is not None:  # compound dtype
+            if zarr_compressor != 'default':
+                raise Exception('zarr_compressor is not supported for compound datasets')
+            if h5_data is None:
+                raise Exception(f'Data must be provided when converting compound dataset {label}')
+            h5_data_1d_view = h5_data.ravel()
+            zarr_data = np.empty(h5_shape, dtype='object')
+            zarr_data_1d_view = zarr_data.ravel()
+            for i in range(len(h5_data_1d_view)):
+                elmt = tuple([
+                    _make_json_serializable(
+                        h5_data_1d_view[i][field_name],
+                        h5_dtype[field_name],
+                        label=f'{label}[{i}].{field_name}',
+                        h5f=h5f
+                    )
+                    for field_name in h5_dtype.names
+                ])
+                zarr_data_1d_view[i] = elmt
+            ds = zarr_parent_group.create_dataset(
+                name,
+                shape=h5_shape,
+                chunks=h5_chunks,
+                dtype='object',
+                data=zarr_data,
+                object_codec=numcodecs.JSON()
+            )
+            compound_dtype = []
+            for name in h5_dtype.names:
+                tt = h5_dtype[name]
+                if tt == h5py.special_dtype(ref=h5py.Reference):
+                    tt = "<REFERENCE>"
+                compound_dtype.append((name, str(tt)))
+            ds.attrs['_COMPOUND_DTYPE'] = compound_dtype
+            return ds
         else:
-            print(dtype.kind)
-            raise Exception(f'Not yet implemented (3): dataset {h5_dataset.name} with dtype {dtype} and shape {shape}')
+            raise Exception(f'Not yet implemented (3): dataset {label} with dtype {h5_dtype} and shape {h5_shape}')
 
 
-def _json_serialize(val: Any, dtype: np.dtype, h5_dataset: h5py.Dataset) -> Any:
+@dataclass
+class CreateZarrDatasetInfo:
+    shape: Tuple
+    dtype: Any
+    fill_value: Any
+    scalar: bool
+    compound_dtype: Union[List[Tuple[str, str]], None]
+
+
+def _make_json_serializable(val: Any, dtype: np.dtype, label: str, h5f: Union[h5py.File, None]) -> Any:
     if dtype.kind in ['i', 'u']:  # integer, unsigned integer
         return int(val)
     elif dtype.kind == 'f':  # float
         return float(val)
     elif dtype.kind == 'b':  # boolean
         return bool(val)
     elif dtype.kind == 'S':  # byte string
         return val.decode()
     elif dtype.kind == 'U':  # unicode string
         return val
     elif dtype == h5py.Reference:
-        return _h5_ref_to_zarr_attr(val, label=f'{h5_dataset.name}', h5f=h5_dataset.file)
+        return h5_to_zarr_attr(val, label=label, h5f=h5f)
     else:
-        raise Exception(f'Cannot serialize item {val} with dtype {dtype} when serializing dataset {h5_dataset.name} with compound dtype.')
+        raise Exception(f'Cannot serialize item {val} with dtype {dtype} when serializing dataset {label} with compound dtype.')
 
 
-def _get_numeric_format_str(dtype: Any) -> Union[str, None]:
-    """Get the format string for a numeric dtype.
-
-    This is used to convert a scalar dataset to inline data using struct.pack.
-    """
-    if dtype == np.int8:
-        return '<b'
-    elif dtype == np.uint8:
-        return '<B'
-    elif dtype == np.int16:
-        return '<h'
-    elif dtype == np.uint16:
-        return '<H'
-    elif dtype == np.int32:
-        return '<i'
-    elif dtype == np.uint32:
-        return '<I'
-    elif dtype == np.int64:
-        return '<q'
-    elif dtype == np.uint64:
-        return '<Q'
-    elif dtype == np.float32:
-        return '<f'
-    elif dtype == np.float64:
-        return '<d'
-    else:
-        return None
+def h5_object_data_to_zarr_data(h5_data: Union[np.ndarray, list], *, h5f: Union[h5py.File, None], label: str) -> np.ndarray:
+    from ..LindiH5pyFile.LindiH5pyReference import LindiH5pyReference  # Avoid circular import
+    if isinstance(h5_data, list):
+        h5_data = np.array(h5_data)
+    zarr_data = np.empty(h5_data.shape, dtype='object')
+    h5_data_1d_view = h5_data.ravel()
+    zarr_data_1d_view = zarr_data.ravel()
+    for i, val in enumerate(h5_data_1d_view):
+        if isinstance(val, bytes):
+            zarr_data_1d_view[i] = val.decode()
+        elif isinstance(val, str):
+            zarr_data_1d_view[i] = val
+        elif isinstance(val, LindiH5pyReference):
+            zarr_data_1d_view[i] = {
+                '_REFERENCE': val._obj
+            }
+        elif isinstance(val, h5py.Reference):
+            if h5f is None:
+                raise Exception(f'h5f cannot be None when converting h5py.Reference to zarr attribute at {label}')
+            zarr_data_1d_view[i] = h5_ref_to_zarr_attr(val, h5f=h5f)
+        else:
+            raise Exception(f'Cannot handle value of type {type(val)} in dataset {label} with dtype {h5_data.dtype} and shape {h5_data.shape}')
+    return zarr_data
```

### Comparing `lindi-0.2.0/lindi/LindiH5pyFile/FileSegmentReader/DandiFileSegmentReader.py` & `lindi-0.2.1/lindi/LindiH5pyFile/FileSegmentReader/DandiFileSegmentReader.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         self.url = url
 
         # The DandiFile has a get_url() method which is in charge of resolving
         # the URL, possibly using the DANDI API token, caching the result, and
         # renewing periodically. remfile.File will accept such an object, and
         # will call .get_url() as needed.
         dandi_file = DandiFile(url)
-        self.remfile = remfile.File(dandi_file, verbose=True)
+        self.remfile = remfile.File(dandi_file, verbose=False)
 
     def read(self, offset: int, length: int):
         self.remfile.seek(offset)
         return self.remfile.read(length)
 
     @staticmethod
     def is_dandi_url(url: str):
```

### Comparing `lindi-0.2.0/lindi/LindiH5pyFile/FileSegmentReader/FileSegmentReader.py` & `lindi-0.2.1/lindi/LindiH5pyFile/FileSegmentReader/FileSegmentReader.py`

 * *Files identical despite different names*

### Comparing `lindi-0.2.0/lindi/LindiH5pyFile/LindiH5pyAttributes.py` & `lindi-0.2.1/lindi/LindiH5pyFile/LindiH5pyAttributes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 from typing import Literal
 from .LindiH5pyReference import LindiH5pyReference
+from ..conversion.attr_conversion import zarr_to_h5_attr
+from ..conversion.nan_inf_ninf import decode_nan_inf_ninf
+from .writers.LindiH5pyAttributesWriter import LindiH5pyAttributesWriter
 
 _special_attribute_keys = [
     "_SCALAR",
     "_COMPOUND_DTYPE",
     "_REFERENCE",
     "_EXTERNAL_ARRAY_LINK",
     "_SOFT_LINK",
 ]
 
 
 class LindiH5pyAttributes:
-    def __init__(self, attrs, attrs_type: Literal["h5py", "zarr"]):
+    def __init__(self, attrs, attrs_type: Literal["h5py", "zarr"], readonly: bool):
         self._attrs = attrs
         self._attrs_type = attrs_type
+        self._readonly = readonly
+
+        if self._readonly:
+            self._writer = None
+        else:
+            self._writer = LindiH5pyAttributesWriter(self)
 
     def get(self, key, default=None):
         if self._attrs_type == "h5py":
             return self._attrs.get(key, default)
         elif self._attrs_type == "zarr":
             try:
                 if key in _special_attribute_keys:
@@ -28,36 +37,41 @@
         else:
             raise ValueError(f"Unknown attrs_type: {self._attrs_type}")
 
     def __contains__(self, key):
         if self._attrs_type == "h5py":
             return key in self._attrs
         elif self._attrs_type == "zarr":
+            if key in _special_attribute_keys:
+                return False
             return key in self._attrs
         else:
             raise ValueError(f"Unknown attrs_type: {self._attrs_type}")
 
     def __getitem__(self, key):
         val = self._attrs[key]
         if self._attrs_type == "h5py":
             return val
         elif self._attrs_type == "zarr":
             if isinstance(val, dict) and "_REFERENCE" in val:
                 return LindiH5pyReference(val["_REFERENCE"])
 
             # Convert special float values to actual floats (NaN, Inf, -Inf)
             # Note that string versions of these values are not supported
-            val = _decode_nan_inf_ninf_in_attr_val(val)
+            val = decode_nan_inf_ninf(val)
 
-            return val
+            return zarr_to_h5_attr(val)
         else:
             raise ValueError(f"Unknown attrs_type: {self._attrs_type}")
 
     def __setitem__(self, key, value):
-        raise KeyError("Cannot set attributes on read-only object")
+        if self._readonly:
+            raise ValueError("Cannot set items on read-only object")
+        assert self._writer is not None
+        self._writer.__setitem__(key, value)
 
     def __delitem__(self, key):
         raise KeyError("Cannot delete attributes on read-only object")
 
     def __iter__(self):
         if self._attrs_type == "h5py":
             return self._attrs.__iter__()
@@ -81,21 +95,9 @@
 
     def __repr__(self):
         return repr(self._attrs)
 
     def __str__(self):
         return str(self._attrs)
 
-
-def _decode_nan_inf_ninf_in_attr_val(val):
-    if isinstance(val, list):
-        return [_decode_nan_inf_ninf_in_attr_val(v) for v in val]
-    elif isinstance(val, dict):
-        return {k: _decode_nan_inf_ninf_in_attr_val(v) for k, v in val.items()}
-    elif val == 'NaN':
-        return float('nan')
-    elif val == 'Infinity':
-        return float('inf')
-    elif val == '-Infinity':
-        return float('-inf')
-    else:
-        return val
+    def keys(self):
+        return list(self)
```

### Comparing `lindi-0.2.0/lindi/LindiH5pyFile/LindiH5pyDataset.py` & `lindi-0.2.1/lindi/LindiH5pyFile/LindiH5pyDataset.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,62 +3,81 @@
 import h5py
 import zarr
 import remfile
 
 from .LindiH5pyAttributes import LindiH5pyAttributes
 from .LindiH5pyReference import LindiH5pyReference
 
+from ..conversion.decode_references import decode_references
+
 
 if TYPE_CHECKING:
     from .LindiH5pyFile import LindiH5pyFile  # pragma: no cover
 
 
-class LindiH5pyDatasetId:
-    def __init__(self, _h5py_dataset_id):
-        self._h5py_dataset_id = _h5py_dataset_id
-
-
 # This is a global list of external hdf5 clients, which are used by
 # possibly multiple LindiH5pyFile objects. The key is the URL of the
 # external hdf5 file, and the value is the h5py.File object.
 # TODO: figure out how to close these clients
 _external_hdf5_clients: Dict[str, h5py.File] = {}
 
 
 class LindiH5pyDataset(h5py.Dataset):
     def __init__(self, _dataset_object: Union[h5py.Dataset, zarr.Array], _file: "LindiH5pyFile"):
         self._dataset_object = _dataset_object
         self._file = _file
+        self._readonly = _file.mode not in ['r+']
+
+        # see comment in LindiH5pyGroup
+        self._id = f'{id(self._file)}/{self._dataset_object.name}'
 
         # See if we have the _COMPOUND_DTYPE attribute, which signifies that
         # this is a compound dtype
         if isinstance(_dataset_object, zarr.Array):
             compound_dtype_obj = _dataset_object.attrs.get("_COMPOUND_DTYPE", None)
             if compound_dtype_obj is not None:
+                assert isinstance(compound_dtype_obj, list)
+                # compound_dtype_obj is a list of tuples (name, dtype)
+                # where dtype == "<REFERENCE>" if it represents an HDF5 reference
+                for i in range(len(compound_dtype_obj)):
+                    if compound_dtype_obj[i][1] == '<REFERENCE>':
+                        compound_dtype_obj[i][1] = h5py.special_dtype(ref=h5py.Reference)
                 # If we have a compound dtype, then create the numpy dtype
                 self._compound_dtype = np.dtype(
-                    [(compound_dtype_obj[i][0], compound_dtype_obj[i][1]) for i in range(len(compound_dtype_obj))]
+                    [
+                        (
+                            compound_dtype_obj[i][0],
+                            compound_dtype_obj[i][1]
+                        )
+                        for i in range(len(compound_dtype_obj))
+                    ]
                 )
             else:
                 self._compound_dtype = None
         else:
             self._compound_dtype = None
 
         # Check whether this is a scalar dataset
         if isinstance(_dataset_object, zarr.Array):
             self._is_scalar = self._dataset_object.attrs.get("_SCALAR", False)
         else:
             self._is_scalar = self._dataset_object.ndim == 0
 
+        # The self._write object handles all the writing operations
+        from .writers.LindiH5pyDatasetWriter import LindiH5pyDatasetWriter  # avoid circular import
+
+        if self._readonly:
+            self._writer = None
+        else:
+            self._writer = LindiH5pyDatasetWriter(self)
+
     @property
     def id(self):
-        if isinstance(self._dataset_object, h5py.Dataset):
-            return LindiH5pyDatasetId(self._dataset_object.id)
-        else:
-            return LindiH5pyDatasetId(None)
+        # see comment in LindiH5pyGroup
+        return self._id
 
     @property
     def shape(self):  # type: ignore
         if self._is_scalar:
             return ()
         return self._dataset_object.shape
 
@@ -115,24 +134,50 @@
     def attrs(self):  # type: ignore
         if isinstance(self._dataset_object, h5py.Dataset):
             attrs_type = 'h5py'
         elif isinstance(self._dataset_object, zarr.Array):
             attrs_type = 'zarr'
         else:
             raise Exception(f'Unexpected dataset object type: {type(self._dataset_object)}')
-        return LindiH5pyAttributes(self._dataset_object.attrs, attrs_type=attrs_type)
+        return LindiH5pyAttributes(self._dataset_object.attrs, attrs_type=attrs_type, readonly=self._file.mode == 'r')
+
+    @property
+    def fletcher32(self):
+        if isinstance(self._dataset_object, h5py.Dataset):
+            return self._dataset_object.fletcher32
+        elif isinstance(self._dataset_object, zarr.Array):
+            for f in self._dataset_object.filters:
+                if f.__class__.__name__ == 'Fletcher32':
+                    return True
+            return False
+        else:
+            raise Exception(f'Unexpected dataset object type: {type(self._dataset_object)}')
+
+    @property
+    def chunks(self):
+        if isinstance(self._dataset_object, h5py.Dataset):
+            return self._dataset_object.chunks
+        elif isinstance(self._dataset_object, zarr.Array):
+            return self._dataset_object.chunks
+        else:
+            raise Exception(f'Unexpected dataset object type: {type(self._dataset_object)}')
+
+    def __repr__(self):  # type: ignore
+        return f"<{self.__class__.__name__}: {self.name}>"
+
+    def __str__(self):
+        return f"<{self.__class__.__name__}: {self.name}>"
 
     def __getitem__(self, args, new_dtype=None):
         if isinstance(self._dataset_object, h5py.Dataset):
             ret = self._dataset_object.__getitem__(args, new_dtype)
         elif isinstance(self._dataset_object, zarr.Array):
             if new_dtype is not None:
                 raise Exception("new_dtype is not supported for zarr.Array")
             ret = self._get_item_for_zarr(self._dataset_object, args)
-            ret = _resolve_references(ret)
         else:
             raise Exception(f"Unexpected type: {type(self._dataset_object)}")
         return ret
 
     def _get_item_for_zarr(self, zarr_array: zarr.Array, selection: Any):
         # First check whether this is an external array link
         external_array_link = zarr_array.attrs.get("_EXTERNAL_ARRAY_LINK", None)
@@ -174,44 +219,39 @@
 
         # We use zarr's slicing, except in the case of a scalar dataset
         if self.ndim == 0:
             # make sure selection is ()
             if selection != ():
                 raise TypeError(f'Cannot slice a scalar dataset with {selection}')
             return zarr_array[0]
-        return zarr_array[selection]
+        return decode_references(zarr_array[selection])
 
     def _get_external_hdf5_client(self, url: str) -> h5py.File:
         if url not in _external_hdf5_clients:
             if url.startswith("http://") or url.startswith("https://"):
                 ff = remfile.File(url)
             else:
                 ff = open(url, "rb")  # this never gets closed
             _external_hdf5_clients[url] = h5py.File(ff, "r")
         return _external_hdf5_clients[url]
 
-
-def _resolve_references(x: Any):
-    if isinstance(x, dict):
-        # x should only be a dict when x represents a converted reference
-        if '_REFERENCE' in x:
-            return LindiH5pyReference(x['_REFERENCE'])
-        else:  # pragma: no cover
-            raise Exception(f"Unexpected dict in selection: {x}")
-    elif isinstance(x, list):
-        # Replace any references in the list with the resolved ref in-place
-        for i, v in enumerate(x):
-            x[i] = _resolve_references(v)
-    elif isinstance(x, np.ndarray):
-        if x.dtype == object or x.dtype is None:
-            # Replace any references in the object array with the resolved ref in-place
-            view_1d = x.reshape(-1)
-            for i in range(len(view_1d)):
-                view_1d[i] = _resolve_references(view_1d[i])
-    return x
+    @property
+    def ref(self):
+        if self._readonly:
+            raise ValueError("Cannot get ref on read-only object")
+        assert self._writer is not None
+        return self._writer.ref
+
+    ##############################
+    # Write
+    def __setitem__(self, args, val):
+        if self._readonly:
+            raise ValueError("Cannot set items on read-only object")
+        assert self._writer is not None
+        self._writer.__setitem__(args, val)
 
 
 class LindiH5pyDatasetCompoundFieldSelection:
     """
     This class is returned when a compound dataset is indexed with a field name.
     For example, if the dataset has dtype [('x', 'f4'), ('y', 'f4')], then we
     can do dataset['x'][0] to get the first x value. The dataset['x'] returns an
@@ -267,8 +307,8 @@
         self._dtype
 
     @property
     def size(self):
         return self._data.size
 
     def __getitem__(self, selection):
-        return self._data[selection]
+        return decode_references(self._data[selection])
```

### Comparing `lindi-0.2.0/lindi/LindiH5pyFile/LindiH5pyFile.py` & `lindi-0.2.1/lindi/LindiH5pyFile/LindiH5pyGroup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,220 +1,216 @@
-from typing import Union
-import json
-import tempfile
-import urllib.request
+from typing import TYPE_CHECKING, Union, Literal
 import h5py
 import zarr
-from zarr.storage import Store as ZarrStore
+from numcodecs.abc import Codec
 
-from .LindiH5pyGroup import LindiH5pyGroup
 from .LindiH5pyDataset import LindiH5pyDataset
+from .LindiH5pyLink import LindiH5pyHardLink, LindiH5pySoftLink
 from .LindiH5pyAttributes import LindiH5pyAttributes
-from .LindiH5pyReference import LindiH5pyReference
-from .LindiReferenceFileSystemStore import LindiReferenceFileSystemStore
 
 
-class LindiH5pyFile(h5py.File):
-    def __init__(self, _file_object: Union[h5py.File, zarr.Group]):
-        """
-        Do not use this constructor directly. Instead, use:
-        from_reference_file_system, from_zarr_store, from_zarr_group,
-        or from_h5py_file
-        """
-        self._file_object = _file_object
-        self._the_group = LindiH5pyGroup(_file_object, self)
-
-    @staticmethod
-    def from_reference_file_system(rfs: Union[dict, str]):
-        """
-        Create a LindiH5pyFile from a reference file system.
-        """
-        if isinstance(rfs, str):
-            if rfs.startswith("http") or rfs.startswith("https"):
-                with tempfile.TemporaryDirectory() as tmpdir:
-                    filename = f"{tmpdir}/temp.zarr.json"
-                    _download_file(rfs, filename)
-                    with open(filename, "r") as f:
-                        data = json.load(f)
-                    assert isinstance(data, dict)  # prevent infinite recursion
-                    return LindiH5pyFile.from_reference_file_system(data)
-            else:
-                with open(rfs, "r") as f:
-                    data = json.load(f)
-                assert isinstance(data, dict)  # prevent infinite recursion
-                return LindiH5pyFile.from_reference_file_system(data)
-        elif isinstance(rfs, dict):
-            # This store does not need to be closed
-            store = LindiReferenceFileSystemStore(rfs)
-            return LindiH5pyFile.from_zarr_store(store)
-        else:
-            raise Exception(f"Unhandled type for rfs: {type(rfs)}")
-
-    @staticmethod
-    def from_zarr_store(zarr_store: ZarrStore):
-        """
-        Create a LindiH5pyFile from a zarr store.
-        """
-        # note that even though the function is called "open", the zarr_group
-        # does not need to be closed
-        zarr_group = zarr.open(store=zarr_store, mode="r")
-        assert isinstance(zarr_group, zarr.Group)
-        return LindiH5pyFile.from_zarr_group(zarr_group)
-
-    @staticmethod
-    def from_zarr_group(zarr_group: zarr.Group):
-        """
-        Create a LindiH5pyFile from a zarr group.
-        """
-        return LindiH5pyFile(zarr_group)
-
-    @staticmethod
-    def from_h5py_file(h5py_file: h5py.File):
-        """
-        Create a LindiH5pyFile from an h5py file.
-        """
-        return LindiH5pyFile(h5py_file)
+if TYPE_CHECKING:
+    from .LindiH5pyFile import LindiH5pyFile  # pragma: no cover
 
-    @property
-    def attrs(self):  # type: ignore
-        if isinstance(self._file_object, h5py.File):
-            attrs_type = 'h5py'
-        elif isinstance(self._file_object, zarr.Group):
-            attrs_type = 'zarr'
-        else:
-            raise Exception(f'Unexpected file object type: {type(self._file_object)}')
-        return LindiH5pyAttributes(self._file_object.attrs, attrs_type=attrs_type)
 
-    @property
-    def filename(self):
-        # This is not a string, but this is what h5py seems to do
-        if isinstance(self._file_object, h5py.File):
-            return self._file_object.filename
-        elif isinstance(self._file_object, zarr.Group):
-            return ''
+class LindiH5pyGroup(h5py.Group):
+    def __init__(self, _group_object: Union[h5py.Group, zarr.Group], _file: "LindiH5pyFile"):
+        self._group_object = _group_object
+        self._file = _file
+        self._readonly = _file.mode not in ['r+']
+
+        # In h5py, the id property is an object that exposes low-level
+        # operations specific to the HDF5 library. LINDI aims to override the
+        # high-level methods such that the low-level operations on id are not
+        # needed. However, sometimes packages (e.g., pynwb) use the id as a
+        # unique identifier for purposes of caching. Therefore, we make the id
+        # to be a string that is unique for each object. If any of the low-level
+        # operations are attempted on this id string, then an exception will be
+        # raised, which will usually indicate that one of the high-level methods
+        # should be overridden.
+        self._id = f'{id(self._file)}/{self._group_object.name}'
+
+        # The self._write object handles all the writing operations
+        from .writers.LindiH5pyGroupWriter import LindiH5pyGroupWriter  # avoid circular import
+        if self._readonly:
+            self._writer = None
         else:
-            raise Exception(f"Unhandled type for file object: {type(self._file_object)}")
-
-    @property
-    def driver(self):
-        raise Exception("Getting driver is not allowed")
-
-    # @property
-    # def mode(self):
-    #     if isinstance(self._file_object, h5py.File):
-    #         return self._file_object.mode
-    #     elif isinstance(self._file_object, zarr.Group):
-    #         # hard-coded to read-only
-    #         return "r"
-    #     else:
-    #         raise Exception(f"Unhandled type: {type(self._file_object)}")
-
-    @property
-    def libver(self):
-        raise Exception("Getting libver is not allowed")
-
-    @property
-    def userblock_size(self):
-        raise Exception("Getting userblock_size is not allowed")
-
-    @property
-    def meta_block_size(self):
-        raise Exception("Getting meta_block_size is not allowed")
-
-    def swmr_mode(self, value):  # type: ignore
-        raise Exception("Getting swmr_mode is not allowed")
-
-    def close(self):
-        # Nothing was opened, so nothing needs to be closed
-        pass
-
-    def flush(self):
-        if isinstance(self._file_object, h5py.File):
-            return self._file_object.flush()
-
-    def __enter__(self):  # type: ignore
-        return self
-
-    def __exit__(self, *args):
-        self.close()
-
-    def __repr__(self):
-        return f'<LindiH5pyFile "{self._file_object}">'
+            self._writer = LindiH5pyGroupWriter(self)
 
-    # Group methods
-    def __getitem__(self, name):  # type: ignore
-        return self._get_item(name)
-
-    def _get_item(self, name, getlink=False, default=None):
-        if isinstance(name, LindiH5pyReference) and isinstance(self._file_object, zarr.Group):
-            if getlink:
-                raise Exception("Getting link is not allowed for references")
-            zarr_group = self._file_object
-            if name._source != '.':
-                raise Exception(f'For now, source of reference must be ".", got "{name._source}"')
-            if name._source_object_id is not None:
-                if name._source_object_id != zarr_group.attrs.get("object_id"):
-                    raise Exception(f'Mismatch in source object_id: "{name._source_object_id}" and "{zarr_group.attrs.get("object_id")}"')
-            target = self[name._path]
-            if name._object_id is not None:
-                if name._object_id != target.attrs.get("object_id"):
-                    raise Exception(f'Mismatch in object_id: "{name._object_id}" and "{target.attrs.get("object_id")}"')
-            return target
-        elif isinstance(name, h5py.Reference) and isinstance(self._file_object, h5py.File):
-            if getlink:
-                raise Exception("Getting link is not allowed for references")
-            x = self._file_object[name]
+    def __getitem__(self, name):
+        if isinstance(self._group_object, h5py.Group):
+            if isinstance(name, (bytes, str)):
+                x = self._group_object[name]
+            else:
+                raise TypeError(
+                    "Accessing a group is done with bytes or str, "
+                    "not {}".format(type(name))
+                )
             if isinstance(x, h5py.Group):
-                return LindiH5pyGroup(x, self)
+                return LindiH5pyGroup(x, self._file)
             elif isinstance(x, h5py.Dataset):
-                return LindiH5pyDataset(x, self)
+                return LindiH5pyDataset(x, self._file)
             else:
-                raise Exception(f"Unexpected type for resolved reference at path {name}: {type(x)}")
-        # if it contains slashes, it's a path
-        if isinstance(name, str) and "/" in name:
-            parts = name.split("/")
-            x = self._the_group
-            for i, part in enumerate(parts):
-                if i == len(parts) - 1:
-                    assert isinstance(x, LindiH5pyGroup)
-                    x = x.get(part, default=default, getlink=getlink)
-                else:
-                    assert isinstance(x, LindiH5pyGroup)
-                    x = x.get(part)
-            return x
-        return self._the_group.get(name, default=default, getlink=getlink)
+                raise Exception(f"Unknown type: {type(x)}")
+        elif isinstance(self._group_object, zarr.Group):
+            if isinstance(name, (bytes, str)):
+                x = self._group_object[name]
+            else:
+                raise TypeError(
+                    "Accessing a group is done with bytes or str, "
+                    "not {}".format(type(name))
+                )
+            if isinstance(x, zarr.Group):
+                # follow the link if this is a soft link
+                soft_link = x.attrs.get('_SOFT_LINK', None)
+                if soft_link is not None:
+                    link_path = soft_link['path']
+                    target_item = self._file.get(link_path)
+                    if not isinstance(target_item, (LindiH5pyGroup, LindiH5pyDataset)):
+                        raise Exception(
+                            f"Expected a group or dataset at {link_path} but got {type(target_item)}"
+                        )
+                    return target_item
+                return LindiH5pyGroup(x, self._file)
+            elif isinstance(x, zarr.Array):
+                return LindiH5pyDataset(x, self._file)
+            else:
+                raise Exception(f"Unknown type: {type(x)}")
+        else:
+            raise Exception(f"Unhandled type: {type(self._group_object)}")
 
     def get(self, name, default=None, getclass=False, getlink=False):
-        if getclass:
+        if not (getclass or getlink):
+            try:
+                return self[name]
+            except KeyError:
+                return default
+
+        if name not in self:
+            return default
+        elif getclass and not getlink:
             raise Exception("Getting class is not allowed")
-        return self._get_item(name, getlink=getlink, default=default)
+        elif getlink and not getclass:
+            if isinstance(self._group_object, h5py.Group):
+                x = self._group_object.get(name, default=default, getlink=True)
+                if isinstance(x, h5py.HardLink):
+                    return LindiH5pyHardLink()
+                elif isinstance(x, h5py.SoftLink):
+                    return LindiH5pySoftLink(x.path)
+                else:
+                    raise Exception(
+                        f"Unhandled type for get with getlink at {self.name} {name}: {type(x)}"
+                    )
+            elif isinstance(self._group_object, zarr.Group):
+                x = self._group_object.get(name, default=default)
+                if x is None:
+                    return default
+                soft_link = x.attrs.get('_SOFT_LINK', None)
+                if isinstance(x, zarr.Group) and soft_link is not None:
+                    return LindiH5pySoftLink(soft_link['path'])
+                else:
+                    return LindiH5pyHardLink()
+            else:
+                raise Exception(f"Unhandled type: {type(self._group_object)}")
+        else:
+            raise Exception("Impossible")
+
+    @property
+    def name(self):
+        return self._group_object.name
+
+    def keys(self):  # type: ignore
+        return self._group_object.keys()
 
     def __iter__(self):
-        return self._the_group.__iter__()
+        return self._group_object.__iter__()
 
     def __reversed__(self):
-        return self._the_group.__reversed__()
+        raise Exception("Not implemented: __reversed__")
 
     def __contains__(self, name):
-        return self._the_group.__contains__(name)
+        return self._group_object.__contains__(name)
+
+    def __str__(self):
+        return f'<{self.__class__.__name__}: {self.name}>'
+
+    def __repr__(self):
+        return f'<{self.__class__.__name__}: {self.name}>'
 
     @property
     def id(self):
-        return self._the_group.id
+        # see comment above
+        return self._id
 
     @property
     def file(self):
-        return self._the_group.file
+        return self._file
 
     @property
-    def name(self):
-        return self._the_group.name
-
+    def attrs(self):  # type: ignore
+        if isinstance(self._group_object, h5py.Group):
+            attrs_type = 'h5py'
+        elif isinstance(self._group_object, zarr.Group):
+            attrs_type = 'zarr'
+        else:
+            raise Exception(f'Unexpected group object type: {type(self._group_object)}')
+        return LindiH5pyAttributes(self._group_object.attrs, attrs_type=attrs_type, readonly=self._file.mode == 'r')
 
-def _download_file(url: str, filename: str) -> None:
-    headers = {
-        "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3"
-    }
-    req = urllib.request.Request(url, headers=headers)
-    with urllib.request.urlopen(req) as response:
-        with open(filename, "wb") as f:
-            f.write(response.read())
+    @property
+    def ref(self):
+        if self._readonly:
+            raise ValueError("Cannot get ref on read-only object")
+        assert self._writer is not None
+        return self._writer.ref
+
+    ##############################
+    # write
+    def create_group(self, name, track_order=None):
+        if self._readonly:
+            raise Exception('Cannot create group in read-only mode')
+        assert self._writer is not None
+        return self._writer.create_group(name, track_order=track_order)
+
+    def require_group(self, name):
+        if self._readonly:
+            raise Exception('Cannot require group in read-only mode')
+        assert self._writer is not None
+        return self._writer.require_group(name)
+
+    def create_dataset(self, name, shape=None, dtype=None, data=None, **kwds):
+        if self._readonly:
+            raise Exception('Cannot create dataset in read-only mode')
+        assert self._writer is not None
+        return self._writer.create_dataset(name, shape=shape, dtype=dtype, data=data, **kwds)
+
+    def require_dataset(self, name, shape, dtype, exact=False, **kwds):
+        if self._readonly:
+            raise Exception('Cannot require dataset in read-only mode')
+        assert self._writer is not None
+        return self._writer.require_dataset(name, shape, dtype, exact=exact, **kwds)
+
+    def create_dataset_with_zarr_compressor(
+        self,
+        name,
+        shape=None,
+        dtype=None,
+        data=None,
+        *,
+        compressor: Union[Codec, Literal['default']] = 'default',
+        **kwds
+    ):
+        if self._readonly:
+            raise Exception('Cannot create dataset in read-only mode')
+        assert self._writer is not None
+        return self._writer.create_dataset(name, shape=shape, dtype=dtype, data=data, _zarr_compressor=compressor, **kwds)
+
+    def __setitem__(self, name, obj):
+        if self._readonly:
+            raise Exception('Cannot set item in read-only mode')
+        assert self._writer is not None
+        return self._writer.__setitem__(name, obj)
+
+    def __delitem__(self, name):
+        if self._readonly:
+            raise Exception('Cannot delete item in read-only mode')
+        assert self._writer is not None
+        return self._writer.__delitem__(name)
```

