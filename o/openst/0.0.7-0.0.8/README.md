# Comparing `tmp/openst-0.0.7.tar.gz` & `tmp/openst-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openst-0.0.7.tar", max compression
+gzip compressed data, was "openst-0.0.8.tar", max compression
```

## Comparing `openst-0.0.7.tar` & `openst-0.0.8.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0      896 2024-02-14 16:40:20.599326 openst-0.0.7/LICENSE
--rw-r--r--   0        0        0     4235 2024-04-15 10:07:14.979891 openst-0.0.7/README.md
--rw-r--r--   0        0        0       21 2024-02-14 16:40:22.603322 openst-0.0.7/openst/__init__.py
--rw-r--r--   0        0        0      231 2024-04-11 08:32:57.910641 openst-0.0.7/openst/__main__.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.611322 openst-0.0.7/openst/alignment/__init__.py
--rw-r--r--   0        0        0     6349 2024-04-15 10:07:08.223908 openst-0.0.7/openst/alignment/apply_transform.py
--rw-r--r--   0        0        0    11893 2024-02-14 16:40:22.619322 openst-0.0.7/openst/alignment/feature_matching.py
--rw-r--r--   0        0        0     3628 2024-02-14 16:40:22.623322 openst-0.0.7/openst/alignment/fiducial_detection.py
--rw-r--r--   0        0        0    51224 2024-04-15 10:07:08.227908 openst-0.0.7/openst/alignment/manual_pairwise_aligner.py
--rw-r--r--   0        0        0    25802 2024-04-15 10:07:08.227908 openst-0.0.7/openst/alignment/pairwise_aligner.py
--rw-r--r--   0        0        0     5373 2024-04-15 10:07:08.227908 openst-0.0.7/openst/alignment/transcript_assign.py
--rw-r--r--   0        0        0      798 2024-04-15 10:07:08.231908 openst-0.0.7/openst/alignment/transformation.py
--rw-r--r--   0        0        0    47876 2024-04-15 10:07:08.231908 openst-0.0.7/openst/cli.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.655321 openst-0.0.7/openst/metadata/__init__.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.659321 openst-0.0.7/openst/metadata/classes/__init__.py
--rw-r--r--   0        0        0     2906 2024-02-14 16:40:22.663322 openst-0.0.7/openst/metadata/classes/base.py
--rw-r--r--   0        0        0     3286 2024-02-14 16:40:22.671321 openst-0.0.7/openst/metadata/classes/pairwise_alignment.py
--rw-r--r--   0        0        0     1798 2024-02-14 16:40:22.679321 openst-0.0.7/openst/metadata/classes/segmentation.py
--rw-r--r--   0        0        0     3787 2024-02-14 16:40:22.683321 openst-0.0.7/openst/metadata/example_json.json
--rw-r--r--   0        0        0     1450 2024-04-12 13:55:27.459067 openst-0.0.7/openst/metadata/report.py
--rw-r--r--   0        0        0  1187390 2024-02-14 16:40:22.715321 openst-0.0.7/openst/metadata/templates/pairwise_alignment.html
--rw-r--r--   0        0        0     1745 2024-02-14 16:40:22.723321 openst-0.0.7/openst/preprocessing/CUT/README.md
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.723321 openst-0.0.7/openst/preprocessing/CUT/__init__.py
--rw-r--r--   0        0        0     3072 2024-02-14 16:40:22.731321 openst-0.0.7/openst/preprocessing/CUT/models/__init__.py
--rw-r--r--   0        0        0    11223 2024-02-14 16:40:22.735321 openst-0.0.7/openst/preprocessing/CUT/models/base_model.py
--rw-r--r--   0        0        0    10228 2024-02-14 16:40:22.739321 openst-0.0.7/openst/preprocessing/CUT/models/cut_model.py
--rw-r--r--   0        0        0    60639 2024-02-14 16:40:22.747321 openst-0.0.7/openst/preprocessing/CUT/models/networks.py
--rw-r--r--   0        0        0     5953 2024-02-14 16:40:22.751321 openst-0.0.7/openst/preprocessing/CUT/models/template_model.py
--rw-r--r--   0        0        0      136 2024-02-14 16:40:22.755321 openst-0.0.7/openst/preprocessing/CUT/options/__init__.py
--rw-r--r--   0        0        0     9720 2024-02-14 16:40:22.763321 openst-0.0.7/openst/preprocessing/CUT/options/base_options.py
--rw-r--r--   0        0        0      975 2024-02-14 16:40:22.767321 openst-0.0.7/openst/preprocessing/CUT/options/test_options.py
--rw-r--r--   0        0        0      102 2024-02-14 16:40:22.775321 openst-0.0.7/openst/preprocessing/CUT/util/__init__.py
--rw-r--r--   0        0        0     2226 2024-02-14 16:40:22.779321 openst-0.0.7/openst/preprocessing/CUT/util/image_pool.py
--rw-r--r--   0        0        0     5135 2024-02-14 16:40:22.783321 openst-0.0.7/openst/preprocessing/CUT/util/util.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.787321 openst-0.0.7/openst/preprocessing/__init__.py
--rw-r--r--   0        0        0     4005 2024-04-12 13:55:27.459067 openst-0.0.7/openst/preprocessing/barcode_preprocessing.py
--rw-r--r--   0        0        0     3027 2024-04-13 10:23:49.385865 openst-0.0.7/openst/preprocessing/image_preprocess.py
--rw-r--r--   0        0        0     4607 2024-04-15 10:07:08.231908 openst-0.0.7/openst/preprocessing/image_stitch.py
--rw-r--r--   0        0        0      690 2024-02-14 16:40:22.811321 openst-0.0.7/openst/preprocessing/imagej_macros/keyence_stitch.ijm
--rw-r--r--   0        0        0      833 2024-04-12 13:55:27.459067 openst-0.0.7/openst/preprocessing/merge_modalities.py
--rw-r--r--   0        0        0     8996 2024-04-15 10:07:08.235908 openst-0.0.7/openst/preprocessing/spatial_stitch.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.819321 openst-0.0.7/openst/segmentation/__init__.py
--rw-r--r--   0        0        0    14684 2024-04-12 13:55:27.463067 openst-0.0.7/openst/segmentation/segment.py
--rw-r--r--   0        0        0     3842 2024-04-15 10:07:08.235908 openst-0.0.7/openst/segmentation/segment_merge.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.827321 openst-0.0.7/openst/threed/__init__.py
--rw-r--r--   0        0        0     9811 2024-04-12 13:55:27.463067 openst-0.0.7/openst/threed/from_3d_registration.py
--rw-r--r--   0        0        0     2500 2024-04-12 13:55:27.467067 openst-0.0.7/openst/threed/to_3d_registration.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.843321 openst-0.0.7/openst/utils/__init__.py
--rw-r--r--   0        0        0     7992 2024-04-15 10:07:08.235908 openst-0.0.7/openst/utils/file.py
--rw-r--r--   0        0        0    13424 2024-04-15 10:07:08.235908 openst-0.0.7/openst/utils/from_spacemake.py
--rw-r--r--   0        0        0     9651 2024-04-15 10:07:08.235908 openst-0.0.7/openst/utils/pimage.py
--rw-r--r--   0        0        0     3018 2024-02-14 16:40:22.859321 openst-0.0.7/openst/utils/points.py
--rw-r--r--   0        0        0     2419 2024-04-15 10:07:08.239908 openst-0.0.7/openst/utils/preview.py
--rw-r--r--   0        0        0    10068 2024-04-15 10:07:08.239908 openst-0.0.7/openst/utils/pseudoimage.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.867321 openst-0.0.7/openst/utils/scanpy/__init__.py
--rw-r--r--   0        0        0       37 2024-02-14 16:40:22.875321 openst-0.0.7/openst/utils/scanpy/pp/__init__.py
--rw-r--r--   0        0        0    10779 2024-02-14 16:40:22.879321 openst-0.0.7/openst/utils/scanpy/pp/_qc.py
--rw-r--r--   0        0        0     3715 2024-02-14 16:40:22.883321 openst-0.0.7/openst/utils/spacemake.py
--rw-r--r--   0        0        0     1985 2024-04-15 10:08:00.915773 openst-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     6373 1970-01-01 00:00:00.000000 openst-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      896 2024-02-14 16:40:20.599326 openst-0.0.8/LICENSE
+-rw-r--r--   0        0        0     4235 2024-04-15 10:07:14.979891 openst-0.0.8/README.md
+-rw-r--r--   0        0        0       21 2024-02-14 16:40:22.603322 openst-0.0.8/openst/__init__.py
+-rw-r--r--   0        0        0      231 2024-04-11 08:32:57.910641 openst-0.0.8/openst/__main__.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.611322 openst-0.0.8/openst/alignment/__init__.py
+-rw-r--r--   0        0        0     5878 2024-04-15 11:40:37.200872 openst-0.0.8/openst/alignment/apply_transform.py
+-rw-r--r--   0        0        0    11893 2024-02-14 16:40:22.619322 openst-0.0.8/openst/alignment/feature_matching.py
+-rw-r--r--   0        0        0     3628 2024-02-14 16:40:22.623322 openst-0.0.8/openst/alignment/fiducial_detection.py
+-rw-r--r--   0        0        0    51224 2024-04-15 10:07:08.227908 openst-0.0.8/openst/alignment/manual_pairwise_aligner.py
+-rw-r--r--   0        0        0    25213 2024-04-15 14:18:10.314354 openst-0.0.8/openst/alignment/pairwise_aligner.py
+-rw-r--r--   0        0        0     5505 2024-04-15 11:42:56.504675 openst-0.0.8/openst/alignment/transcript_assign.py
+-rw-r--r--   0        0        0      798 2024-04-15 10:07:08.231908 openst-0.0.8/openst/alignment/transformation.py
+-rw-r--r--   0        0        0    47613 2024-04-15 14:45:02.598230 openst-0.0.8/openst/cli.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.655321 openst-0.0.8/openst/metadata/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.659321 openst-0.0.8/openst/metadata/classes/__init__.py
+-rw-r--r--   0        0        0     2906 2024-02-14 16:40:22.663322 openst-0.0.8/openst/metadata/classes/base.py
+-rw-r--r--   0        0        0     3406 2024-04-15 13:57:54.682361 openst-0.0.8/openst/metadata/classes/pairwise_alignment.py
+-rw-r--r--   0        0        0     1798 2024-02-14 16:40:22.679321 openst-0.0.8/openst/metadata/classes/segmentation.py
+-rw-r--r--   0        0        0     3787 2024-02-14 16:40:22.683321 openst-0.0.8/openst/metadata/example_json.json
+-rw-r--r--   0        0        0     1450 2024-04-12 13:55:27.459067 openst-0.0.8/openst/metadata/report.py
+-rw-r--r--   0        0        0  1187390 2024-02-14 16:40:22.715321 openst-0.0.8/openst/metadata/templates/pairwise_alignment.html
+-rw-r--r--   0        0        0     1745 2024-02-14 16:40:22.723321 openst-0.0.8/openst/preprocessing/CUT/README.md
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.723321 openst-0.0.8/openst/preprocessing/CUT/__init__.py
+-rw-r--r--   0        0        0     3072 2024-02-14 16:40:22.731321 openst-0.0.8/openst/preprocessing/CUT/models/__init__.py
+-rw-r--r--   0        0        0    11223 2024-02-14 16:40:22.735321 openst-0.0.8/openst/preprocessing/CUT/models/base_model.py
+-rw-r--r--   0        0        0    10228 2024-02-14 16:40:22.739321 openst-0.0.8/openst/preprocessing/CUT/models/cut_model.py
+-rw-r--r--   0        0        0    60639 2024-02-14 16:40:22.747321 openst-0.0.8/openst/preprocessing/CUT/models/networks.py
+-rw-r--r--   0        0        0     5953 2024-02-14 16:40:22.751321 openst-0.0.8/openst/preprocessing/CUT/models/template_model.py
+-rw-r--r--   0        0        0      136 2024-02-14 16:40:22.755321 openst-0.0.8/openst/preprocessing/CUT/options/__init__.py
+-rw-r--r--   0        0        0     9720 2024-02-14 16:40:22.763321 openst-0.0.8/openst/preprocessing/CUT/options/base_options.py
+-rw-r--r--   0        0        0      975 2024-02-14 16:40:22.767321 openst-0.0.8/openst/preprocessing/CUT/options/test_options.py
+-rw-r--r--   0        0        0      102 2024-02-14 16:40:22.775321 openst-0.0.8/openst/preprocessing/CUT/util/__init__.py
+-rw-r--r--   0        0        0     2226 2024-02-14 16:40:22.779321 openst-0.0.8/openst/preprocessing/CUT/util/image_pool.py
+-rw-r--r--   0        0        0     5135 2024-02-14 16:40:22.783321 openst-0.0.8/openst/preprocessing/CUT/util/util.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.787321 openst-0.0.8/openst/preprocessing/__init__.py
+-rw-r--r--   0        0        0     4005 2024-04-12 13:55:27.459067 openst-0.0.8/openst/preprocessing/barcode_preprocessing.py
+-rw-r--r--   0        0        0     3027 2024-04-13 10:23:49.385865 openst-0.0.8/openst/preprocessing/image_preprocess.py
+-rw-r--r--   0        0        0     4607 2024-04-15 10:07:08.231908 openst-0.0.8/openst/preprocessing/image_stitch.py
+-rw-r--r--   0        0        0      690 2024-02-14 16:40:22.811321 openst-0.0.8/openst/preprocessing/imagej_macros/keyence_stitch.ijm
+-rw-r--r--   0        0        0      833 2024-04-12 13:55:27.459067 openst-0.0.8/openst/preprocessing/merge_modalities.py
+-rw-r--r--   0        0        0     8996 2024-04-15 10:07:08.235908 openst-0.0.8/openst/preprocessing/spatial_stitch.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.819321 openst-0.0.8/openst/segmentation/__init__.py
+-rw-r--r--   0        0        0    14684 2024-04-12 13:55:27.463067 openst-0.0.8/openst/segmentation/segment.py
+-rw-r--r--   0        0        0     3842 2024-04-15 10:07:08.235908 openst-0.0.8/openst/segmentation/segment_merge.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.827321 openst-0.0.8/openst/threed/__init__.py
+-rw-r--r--   0        0        0     9811 2024-04-12 13:55:27.463067 openst-0.0.8/openst/threed/from_3d_registration.py
+-rw-r--r--   0        0        0     2500 2024-04-12 13:55:27.467067 openst-0.0.8/openst/threed/to_3d_registration.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.843321 openst-0.0.8/openst/utils/__init__.py
+-rw-r--r--   0        0        0     8010 2024-04-15 13:56:11.270437 openst-0.0.8/openst/utils/file.py
+-rw-r--r--   0        0        0    13953 2024-04-15 13:46:46.786692 openst-0.0.8/openst/utils/from_spacemake.py
+-rw-r--r--   0        0        0     9651 2024-04-15 10:07:08.235908 openst-0.0.8/openst/utils/pimage.py
+-rw-r--r--   0        0        0     3018 2024-02-14 16:40:22.859321 openst-0.0.8/openst/utils/points.py
+-rw-r--r--   0        0        0     2419 2024-04-15 10:07:08.239908 openst-0.0.8/openst/utils/preview.py
+-rw-r--r--   0        0        0    10068 2024-04-15 13:44:23.802687 openst-0.0.8/openst/utils/pseudoimage.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.867321 openst-0.0.8/openst/utils/scanpy/__init__.py
+-rw-r--r--   0        0        0       37 2024-02-14 16:40:22.875321 openst-0.0.8/openst/utils/scanpy/pp/__init__.py
+-rw-r--r--   0        0        0    10779 2024-02-14 16:40:22.879321 openst-0.0.8/openst/utils/scanpy/pp/_qc.py
+-rw-r--r--   0        0        0     3715 2024-02-14 16:40:22.883321 openst-0.0.8/openst/utils/spacemake.py
+-rw-r--r--   0        0        0     1985 2024-04-15 13:44:33.982689 openst-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     6373 1970-01-01 00:00:00.000000 openst-0.0.8/PKG-INFO
```

### Comparing `openst-0.0.7/LICENSE` & `openst-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `openst-0.0.7/README.md` & `openst-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `openst-0.0.7/openst/alignment/apply_transform.py` & `openst-0.0.8/openst/alignment/apply_transform.py`

 * *Files 15% similar despite different names*

```diff
@@ -98,20 +98,14 @@
     return keypoints_json_to_dict(keypoints_json)
 
 def _run_apply_transform(args):
     # Check input and output data
     check_file_exists(args.h5_in)
     check_adata_structure(args.h5_in)
 
-    if args.h5_out == "" and not check_directory_exists(args.h5_out):
-        raise FileNotFoundError("Parent directory for --h5-out does not exist")
-    
-    if args.h5_out == "":
-        args.h5_out = args.h5_in
-
     _to_load = ["obs/total_counts"]
     if args.per_tile:
         _to_load += ["obs/tile_id"]
     _to_load += [f"{args.spatial_key_in}"]
 
     _tile_ids = None
 
@@ -130,27 +124,21 @@
     
     _coords_transformed = apply_transform_to_coords(
         _coords,
         _tile_ids,
         keypoints
     )
 
-    if check_file_exists(args.h5_out, exception = False):
-        logging.info(f"The output file exists at {args.h5_out}")  
-    else:
-        logging.info(f"Creating new {args.h5_out} from {args.h5_in}")  
-        shutil.copy(args.h5_in, args.h5_out)
-
-    logging.info(f"Modifying coordinates in {args.h5_out}")
-    with h5py.File(args.h5_out, 'r+') as adata:
+    logging.info(f"Modifying coordinates in {args.h5_in}")
+    with h5py.File(args.h5_in, 'r+') as adata:
         if f"{args.spatial_key_out}" in adata:
             # reconvert to YX (same axes as the images)
             adata[f"{args.spatial_key_out}"][...] = _coords_transformed[:][..., ::-1]
         else:
             adata[f"{args.spatial_key_out}"] = _coords_transformed[:][..., ::-1]
 
-    logging.info(f"Output {args.h5_out} file was written. Finished!")
+    logging.info(f"Output {args.h5_in} file was written. Finished!")
 
 if __name__ == "__main__":
     from openst.cli import get_apply_transform_parser
     args = get_apply_transform_parser().parse_args()
     _run_apply_transform(args)
```

### Comparing `openst-0.0.7/openst/alignment/feature_matching.py` & `openst-0.0.8/openst/alignment/feature_matching.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.7/openst/alignment/fiducial_detection.py` & `openst-0.0.8/openst/alignment/fiducial_detection.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.7/openst/alignment/manual_pairwise_aligner.py` & `openst-0.0.8/openst/alignment/manual_pairwise_aligner.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.7/openst/alignment/pairwise_aligner.py` & `openst-0.0.8/openst/alignment/pairwise_aligner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,17 @@
 """
 Automatic Pairwise Alignment of Spatial Transcriptomics and Imaging Data (Open-ST)
 
 Author: Daniel León-Periñán @ N.Rajewsky Lab (BIMSB)
-Date: August 30, 2023
-Version: 0.1.0
+Date: April 15, 2024
+Version: 0.2.0
 
 Description:
 This script performs automatic pairwise alignment between spatial transcriptomics data and imaging data.
 It aligns the spatial transcriptomics data onto the imaging data to enable spatial comparison and analysis.
-
-Usage example:
-openst pairwise_aligner --image-in input_image.jpg --h5-in input_data.h5ad --h5-out aligned_data.h5ad
-                     --metadata-out metadata.pkl --save-image-in-h5 --rescale-factor-coarse 20
-                     --rescale-factor-fine 5 --tissue-masking-gaussian-sigma 5 --fine-registration-gaussian-sigma 2
-                     --keep-black-background --threshold-counts-coarse 1 --threshold-counts-fine 0
-                     --pseudoimage-size-coarse 4000 --pseudoimage-size-fine 6000 --ransac-coarse-min-samples 3
-                     --ransac-coarse-residual-threshold 2 --ransac-coarse-max-trials 10000 --ransac-fine-min-samples 10
-                     --ransac-fine-residual-threshold 2 --ransac-fine-max-trials 10000 --max-image-pixels 933120000
-                     --feature-matcher 'LoFTR' --n-threads 2 --fine-min-matches 50 --fiducial-model model.pt
 """
 
 import logging
 from itertools import product
 
 import cv2
 import numpy as np
@@ -387,17 +377,22 @@
 
         min_lim, max_lim = _t_sts_coords_to_transform[_t_valid_coords].min(axis=0).astype(
             int
         ), _t_sts_coords_to_transform[_t_valid_coords].max(axis=0).astype(int)
         x_min, y_min = min_lim
         x_max, y_max = max_lim
 
+        _fn_prepare_image_for_feature_matching = prepare_image_for_feature_matching
+
+        if is_grayscale(src):
+            _fn_prepare_image_for_feature_matching = prepare_image_for_feature_matching_grayscale
+
         # Preparing image and pseudoimage modalities for feature detection (imaging modality has optimal flip)
         def src_preprocessor(x, flip, rotation):
-            return prepare_image_for_feature_matching(
+            return _fn_prepare_image_for_feature_matching(
                 image=x,
                 gaussian_blur=args.fine_registration_gaussian_sigma,
                 crop=[x_min, x_max, y_min, y_max],
                 mask_tissue=args.mask_tissue,
                 keep_black_background=args.keep_black_background,
                 mask_gaussian_blur=args.tissue_masking_gaussian_sigma,
             )
@@ -449,32 +444,35 @@
         # Compute similarity matrix and compute point transformation
         if len(_t_mkpts0) > args.fine_min_matches:
             _t_tform_points = estimate_transform("similarity", _t_mkpts0, _t_mkpts1)
 
             _t_sts_coords_fine_transformed = apply_transform(
                 _t_sts_coords_fine_to_transform, _t_tform_points, check_bounds=True
             )[:, :-1]
+
+            _tform_params = _t_tform_points.params
         else:
             logging.warning(f"There were not enough matching points ({len(_t_mkpts0)} out of selected {args.fine_min_matches})")
             _t_sts_coords_fine_transformed = _t_sts_coords_fine_to_transform[:, ::-1]
+            _tform_params = None
             
 
         # Rescale points to original HE dimensions
         _t_sts_coords_fine_transformed = _t_sts_coords_fine_transformed + np.array([[y_min, x_min]])
         _t_sts_coords_fine_transformed = _t_sts_coords_fine_transformed * args.rescale_factor_fine
 
         out_coords_output_fine[_t_tile_id] = _t_sts_coords_fine_transformed[:, ::-1]
 
         # Saving alignment results here (only when passed)
         # TODO: check order of keypoints (in all functions throughout package)
         _align_result = AlignmentResult(
             name=f"fine_alignment_tile_{tile_code}",
             im_0=src[x_min:x_max, y_min:y_max],
             im_1=_t_sts_pseudoimage["pseudoimage"][x_min:x_max, y_min:y_max],
-            transformation_matrix=_t_tform_points.params,
+            transformation_matrix=_tform_params,
             ransac_results=None,
             sift_results=None,
             keypoints0=_t_mkpts1,
             keypoints1=_t_mkpts0,
         )
         metadata.add_alignment_result(_align_result)
 
@@ -539,15 +537,15 @@
             if "obsm/spatial_pairwise_aligned_fine" in adata:
                 adata["obsm/spatial_pairwise_aligned_fine"][:] = sts_aligned_fine
             else:
                 adata["obsm/spatial_pairwise_aligned_fine"] = sts_aligned_fine
 
 
 def _run_pairwise_aligner(args):
-    with threadpool_limits(limits=args.n_threads):
+    with threadpool_limits(limits=args.num_workers):
         run_pairwise_aligner(args)
 
 
 if __name__ == "__main__":
     from openst.cli import get_pairwise_aligner_parser
     args = get_pairwise_aligner_parser().parse_args()
     _run_pairwise_aligner(args)
```

### Comparing `openst-0.0.7/openst/alignment/transcript_assign.py` & `openst-0.0.8/openst/alignment/transcript_assign.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,18 @@
         adata_by_cell.uns[_missing_key] = adata_transformed_coords.uns[_missing_key]
 
     return adata_by_cell
 
 
 def subset_adata_to_mask(mask, adata, spatial_key: str = 'spatial'):
     # Subset adata to the valid coordinates from the mask
-    adata = adata[(adata.obsm[spatial_key][:, 0] <= mask.shape[0]) & (adata.obsm[spatial_key][:, 1] <= mask.shape[1])].copy()
+    adata = adata[(adata.obsm[spatial_key][:, 0] >= 0) & 
+                  (adata.obsm[spatial_key][:, 1] <= 0)
+                  (adata.obsm[spatial_key][:, 0] <= mask.shape[0]) & 
+                  (adata.obsm[spatial_key][:, 1] <= mask.shape[1])].copy()
 
     # Subset the labels to those in the mask
     labels = mask[adata.obsm[spatial_key][:, 0].astype(int), adata.obsm[spatial_key][:, 1].astype(int)]
 
     # Assign label as cell_ID
     adata.obs["cell_ID"] = labels
```

### Comparing `openst-0.0.7/openst/alignment/transformation.py` & `openst-0.0.8/openst/alignment/transformation.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.7/openst/cli.py` & `openst-0.0.8/openst/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -922,21 +922,14 @@
     parser.add_argument(
         "--h5-in",
         type=str,
         required=True,
         help="Path to the input h5ad file containing spatial coordinates",
     )
     parser.add_argument(
-        "--h5-out",
-        type=str,
-        default="",
-        help="""(Optional) Path where to copy a new Open-ST h5 object file after coordinate transformation.
-        If not specified, data is written in place at --h5-in""",
-    )
-    parser.add_argument(
         "--per-tile",
         action="store_true",
         help="""(Optional) If set, transformations are applied per tile, from their keypoints. 
                 Otherwise, a single transform is computed for all tiles.""",
     )
     parser.add_argument(
         "--spatial-key-in",
```

### Comparing `openst-0.0.7/openst/metadata/classes/base.py` & `openst-0.0.8/openst/metadata/classes/base.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.7/openst/metadata/classes/pairwise_alignment.py` & `openst-0.0.8/openst/metadata/classes/pairwise_alignment.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import base64
 import io
 
 import numpy as np
 from skimage.transform import SimilarityTransform
 
 from openst.metadata.classes.base import BaseMetadata
+from openst.utils.pimage import is_grayscale
 
 
 class PairwiseAlignmentMetadata(BaseMetadata):
     def __init__(self, args):
         super().__init__(args)
 
         # it must be the same as the name of the HTML template under the templates dir
@@ -64,17 +65,20 @@
         import matplotlib.pyplot as plt
         from skimage.feature import plot_matches
 
         if axes is None:
             fig, axes = plt.subplots(1, 1)
 
         # TODO: automatically manage the number of channels to avoid errors here!
+        if not is_grayscale(self.im_0):
+            self.im_0 = self.im_0[..., 0]
+
         plot_matches(
             axes,
-            self.im_0[..., 0],
+            self.im_0,
             self.im_1,
             self.keypoints0,
             self.keypoints1,
             np.repeat(np.arange(len(self.keypoints0)), 2).reshape(len(self.keypoints0), 2),
         ),
 
         if show:
```

### Comparing `openst-0.0.7/openst/metadata/classes/segmentation.py` & `openst-0.0.8/openst/metadata/classes/segmentation.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.7/openst/metadata/example_json.json` & `openst-0.0.8/openst/metadata/example_json.json`

 * *Files identical despite different names*

### Comparing `openst-0.0.7/openst/metadata/report.py` & `openst-0.0.8/openst/metadata/report.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.7/openst/metadata/templates/pairwise_alignment.html` & `openst-0.0.8/openst/metadata/templates/pairwise_alignment.html`

 * *Files identical despite different names*

### Comparing `openst-0.0.7/openst/preprocessing/CUT/README.md` & `openst-0.0.8/openst/preprocessing/CUT/README.md`

 * *Files identical despite different names*

### Comparing `openst-0.0.7/openst/preprocessing/CUT/models/__init__.py` & `openst-0.0.8/openst/preprocessing/CUT/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.7/openst/preprocessing/CUT/models/base_model.py` & `openst-0.0.8/openst/preprocessing/CUT/models/base_model.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.7/openst/preprocessing/CUT/models/cut_model.py` & `openst-0.0.8/openst/preprocessing/CUT/models/cut_model.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.7/openst/preprocessing/CUT/models/networks.py` & `openst-0.0.8/openst/preprocessing/CUT/models/networks.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.7/openst/preprocessing/CUT/models/template_model.py` & `openst-0.0.8/openst/preprocessing/CUT/models/template_model.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.7/openst/preprocessing/CUT/options/base_options.py` & `openst-0.0.8/openst/preprocessing/CUT/options/base_options.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.7/openst/preprocessing/CUT/options/test_options.py` & `openst-0.0.8/openst/preprocessing/CUT/options/test_options.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.7/openst/preprocessing/CUT/util/image_pool.py` & `openst-0.0.8/openst/preprocessing/CUT/util/image_pool.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.7/openst/preprocessing/CUT/util/util.py` & `openst-0.0.8/openst/preprocessing/CUT/util/util.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.7/openst/preprocessing/barcode_preprocessing.py` & `openst-0.0.8/openst/preprocessing/barcode_preprocessing.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.7/openst/preprocessing/image_preprocess.py` & `openst-0.0.8/openst/preprocessing/image_preprocess.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.7/openst/preprocessing/image_stitch.py` & `openst-0.0.8/openst/preprocessing/image_stitch.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.7/openst/preprocessing/imagej_macros/keyence_stitch.ijm` & `openst-0.0.8/openst/preprocessing/imagej_macros/keyence_stitch.ijm`

 * *Files identical despite different names*

### Comparing `openst-0.0.7/openst/preprocessing/merge_modalities.py` & `openst-0.0.8/openst/preprocessing/merge_modalities.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.7/openst/preprocessing/spatial_stitch.py` & `openst-0.0.8/openst/preprocessing/spatial_stitch.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.7/openst/segmentation/segment.py` & `openst-0.0.8/openst/segmentation/segment.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.7/openst/segmentation/segment_merge.py` & `openst-0.0.8/openst/segmentation/segment_merge.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.7/openst/threed/from_3d_registration.py` & `openst-0.0.8/openst/threed/from_3d_registration.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.7/openst/threed/to_3d_registration.py` & `openst-0.0.8/openst/threed/to_3d_registration.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.7/openst/utils/file.py` & `openst-0.0.8/openst/utils/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,16 @@
     if os.path.isdir(path):
         _ret_val = os.path.exists(path)
     else:
         path = os.path.dirname(path)
         # handle file created in the same directory
         if path == "":
             _ret_val = True
-        _ret_val = os.path.exists(path)
+        else:
+            _ret_val = os.path.exists(path)
     
     if exception and not _ret_val:
         raise FileNotFoundError(f"The directory '{path}' does not exist")
     
     return _ret_val
```

### Comparing `openst-0.0.7/openst/utils/from_spacemake.py` & `openst-0.0.8/openst/utils/from_spacemake.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,17 +246,32 @@
     stitched_segmented_dge = get_stitched_segmented_dge(sample_config, sample_metadata)
     required_arguments = ["--mask-in", 'uns/spatial/staining_image_mask', "--h5-in"] + [stitched_dge]
     required_arguments += ["--h5-out", stitched_segmented_dge]
 
     return required_arguments
 
 def _run_merge_modalities(sample_config, sample_metadata):
+    import shutil
+
     stitched_dge = get_stitched_dge(sample_config, sample_metadata, check_exists=True)
     image_out = get_stitched_image_path(sample_config, sample_metadata, check_exists=True)
-    required_arguments = ["--h5-in", stitched_dge, "--image-in", image_out]
+    merged_dge = get_multimodal_dge(sample_config, sample_metadata)
+
+    if not check_directory_exists(merged_dge):
+        _parent_dir = os.path.dirname(merged_dge)
+        logging.info(f"Creating directory at {_parent_dir}")
+        os.mkdir(_parent_dir)
+
+    if check_file_exists(merged_dge, exception=False):
+        logging.warn(f"No need to create {merged_dge} - it exists")  
+    else:
+        logging.info(f"Copying {stitched_dge} into {merged_dge}")  
+        shutil.copy(stitched_dge, merged_dge)
+    
+    required_arguments = ["--h5-in", merged_dge, "--image-in", image_out]
 
     return required_arguments
 
 def _run_manual_pairwise_aligner(sample_config, sample_metadata):
     stitched_dge = get_multimodal_dge(sample_config, sample_metadata, check_exists=True)
     required_arguments = ["--h5-in", stitched_dge]
```

### Comparing `openst-0.0.7/openst/utils/pimage.py` & `openst-0.0.8/openst/utils/pimage.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.7/openst/utils/points.py` & `openst-0.0.8/openst/utils/points.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.7/openst/utils/preview.py` & `openst-0.0.8/openst/utils/preview.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.7/openst/utils/pseudoimage.py` & `openst-0.0.8/openst/utils/pseudoimage.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.7/openst/utils/scanpy/pp/_qc.py` & `openst-0.0.8/openst/utils/scanpy/pp/_qc.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.7/openst/utils/spacemake.py` & `openst-0.0.8/openst/utils/spacemake.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.7/pyproject.toml` & `openst-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "openst"
-version = "0.0.7"
+version = "0.0.8"
 description = "The computational pipeline for the Open-ST method."
 license = "GPL-2.0"
 authors = [
     "Daniel León-Periñán <daniel.leonperinan@mdc-berlin.de>",
     "Nikolaos Karaiskos <nikolaos.karaiskos@mdc-berlin.de>",
 ]
 maintainers = [
```

### Comparing `openst-0.0.7/PKG-INFO` & `openst-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openst
-Version: 0.0.7
+Version: 0.0.8
 Summary: The computational pipeline for the Open-ST method.
 License: GPL-2.0
 Author: Daniel León-Periñán
 Author-email: daniel.leonperinan@mdc-berlin.de
 Maintainer: Daniel León-Periñán
 Maintainer-email: daniel.leonperinan@mdc-berlin.de
 Requires-Python: >=3.8,<4.0
```

