# Comparing `tmp/spine_segmentation-0.2.8.tar.gz` & `tmp/spine_segmentation-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spine_segmentation-0.2.8.tar", max compression
+gzip compressed data, was "spine_segmentation-0.2.9.tar", max compression
```

## Comparing `spine_segmentation-0.2.8.tar` & `spine_segmentation-0.2.9.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     1211 2024-04-11 11:32:29.446351 spine_segmentation-0.2.8/README.md
--rw-r--r--   0        0        0     2382 2024-04-15 15:29:06.384108 spine_segmentation-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      122 2024-04-11 12:53:48.914194 spine_segmentation-0.2.8/spine_segmentation/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.2.8/spine_segmentation/annotators/__init__.py
--rw-r--r--   0        0        0    16308 2024-04-11 12:53:48.934194 spine_segmentation-0.2.8/spine_segmentation/annotators/annotator_base.py
--rw-r--r--   0        0        0     8225 2024-04-11 12:53:48.814193 spine_segmentation-0.2.8/spine_segmentation/annotators/vector_annotator.py
--rw-r--r--   0        0        0     2190 2024-04-11 12:53:48.766192 spine_segmentation-0.2.8/spine_segmentation/cli/cli.py
--rw-r--r--   0        0        0    12072 2024-04-10 12:31:20.207512 spine_segmentation-0.2.8/spine_segmentation/dataloader/statistics.py
--rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.2.8/spine_segmentation/datasets/__init__.py
--rw-r--r--   0        0        0     2868 2024-04-10 12:31:20.207512 spine_segmentation-0.2.8/spine_segmentation/datasets/augmentation.py
--rw-r--r--   0        0        0     4312 2024-04-11 12:53:48.806193 spine_segmentation-0.2.8/spine_segmentation/datasets/feature_dataset.py
--rw-r--r--   0        0        0     6696 2024-04-11 15:53:29.418496 spine_segmentation-0.2.8/spine_segmentation/datasets/metadata_prediction_dataset.py
--rw-r--r--   0        0        0     6372 2024-04-11 15:53:29.430496 spine_segmentation-0.2.8/spine_segmentation/datasets/patch_segmentation_dataset.py
--rw-r--r--   0        0        0     1360 2024-04-11 15:53:29.410496 spine_segmentation-0.2.8/spine_segmentation/datasets/path_helper.py
--rw-r--r--   0        0        0    14744 2024-04-11 15:47:48.534212 spine_segmentation-0.2.8/spine_segmentation/datasets/sample.py
--rw-r--r--   0        0        0    14989 2024-04-11 15:53:29.422496 spine_segmentation-0.2.8/spine_segmentation/datasets/segmentation_dataset.py
--rw-r--r--   0        0        0     2037 2024-04-11 12:53:48.782192 spine_segmentation-0.2.8/spine_segmentation/datasets/vector_table_graphs_dataset.py
--rw-r--r--   0        0        0     2581 2024-04-11 12:53:48.890194 spine_segmentation-0.2.8/spine_segmentation/evaluate/analyze_edge_cases.py
--rw-r--r--   0        0        0     2520 2024-04-11 12:53:48.798193 spine_segmentation-0.2.8/spine_segmentation/evaluate/analyze_index_list.py
--rw-r--r--   0        0        0     1659 2024-04-11 12:53:48.854193 spine_segmentation-0.2.8/spine_segmentation/evaluate/classic_ml.py
--rw-r--r--   0        0        0     1108 2024-04-10 12:31:20.207512 spine_segmentation-0.2.8/spine_segmentation/evaluate/eval_created_stats.py
--rw-r--r--   0        0        0    15527 2024-04-11 15:52:07.339228 spine_segmentation-0.2.8/spine_segmentation/evaluate/eval_instance_seg_model.py
--rw-r--r--   0        0        0     8215 2024-04-11 12:53:48.746192 spine_segmentation-0.2.8/spine_segmentation/evaluate/eval_splitting.py
--rw-r--r--   0        0        0     6109 2024-04-11 15:52:07.363228 spine_segmentation-0.2.8/spine_segmentation/evaluate/load_model.py
--rw-r--r--   0        0        0     4885 2024-04-11 12:53:48.882194 spine_segmentation-0.2.8/spine_segmentation/evaluate/metadata.py
--rw-r--r--   0        0        0     1627 2024-04-11 12:53:48.894194 spine_segmentation-0.2.8/spine_segmentation/evaluate/volume_size_in_gt.py
--rw-r--r--   0        0        0     8647 2024-04-15 15:28:55.187932 spine_segmentation-0.2.8/spine_segmentation/inference/instance_segmentation.py
--rw-r--r--   0        0        0     6761 2024-04-11 12:53:48.846193 spine_segmentation-0.2.8/spine_segmentation/inference/onnx_model.py
--rw-r--r--   0        0        0     7515 2024-04-11 12:53:48.906194 spine_segmentation-0.2.8/spine_segmentation/instance_separation/instance_separation.py
--rw-r--r--   0        0        0      304 2024-04-10 12:31:20.207512 spine_segmentation-0.2.8/spine_segmentation/losses/diffis1.py
--rw-r--r--   0        0        0     2080 2024-04-11 15:40:00.222464 spine_segmentation-0.2.8/spine_segmentation/model_downloader/model_downloader.py
--rw-r--r--   0        0        0      712 2024-04-11 12:53:48.850193 spine_segmentation-0.2.8/spine_segmentation/plotting/bmi.py
--rw-r--r--   0        0        0     8132 2024-04-11 12:53:48.778192 spine_segmentation-0.2.8/spine_segmentation/plotting/classification_correlation.py
--rw-r--r--   0        0        0     2566 2024-04-11 12:53:48.886194 spine_segmentation-0.2.8/spine_segmentation/plotting/patient_metadata.py
--rw-r--r--   0        0        0    10404 2024-04-11 12:53:48.826193 spine_segmentation-0.2.8/spine_segmentation/plotting/plot_slice.py
--rw-r--r--   0        0        0     1795 2024-04-11 12:53:48.938195 spine_segmentation-0.2.8/spine_segmentation/plotting/plot_statistics.py
--rw-r--r--   0        0        0     5823 2024-04-11 12:53:48.834193 spine_segmentation-0.2.8/spine_segmentation/plotting/read_npz_eval_per_roi_accuracy.py
--rw-r--r--   0        0        0     5767 2024-04-11 12:53:48.786192 spine_segmentation-0.2.8/spine_segmentation/plotting/show_plane_splitting_3d.py
--rw-r--r--   0        0        0      266 2024-04-11 12:53:48.858193 spine_segmentation-0.2.8/spine_segmentation/plotting/ydata_profile_report.py
--rw-r--r--   0        0        0      930 2024-04-11 15:55:12.773382 spine_segmentation-0.2.8/spine_segmentation/resources/paths.py
--rw-r--r--   0        0        0      933 2024-04-11 12:53:48.842193 spine_segmentation-0.2.8/spine_segmentation/resources/preloaded.py
--rw-r--r--   0        0        0       63 2024-04-11 09:34:14.336647 spine_segmentation-0.2.8/spine_segmentation/run.py
--rw-r--r--   0        0        0     4575 2024-04-10 12:31:20.207512 spine_segmentation-0.2.8/spine_segmentation/scripts/format_results.py
--rw-r--r--   0        0        0     4546 2024-04-11 12:53:48.866193 spine_segmentation-0.2.8/spine_segmentation/scripts/split_train_val_test.py
--rw-r--r--   0        0        0      210 2024-04-10 12:31:20.207512 spine_segmentation-0.2.8/spine_segmentation/scripts/test_patient_ids.txt
--rw-r--r--   0        0        0      112 2024-04-10 18:52:49.798849 spine_segmentation-0.2.8/spine_segmentation/spine_types/disc.py
--rw-r--r--   0        0        0     1033 2024-04-10 12:31:20.207512 spine_segmentation-0.2.8/spine_segmentation/spine_types/labels.py
--rw-r--r--   0        0        0      219 2024-04-10 12:31:20.207512 spine_segmentation-0.2.8/spine_segmentation/spine_types/line_segment.py
--rw-r--r--   0        0        0     2409 2024-04-10 12:31:20.207512 spine_segmentation-0.2.8/spine_segmentation/spine_types/plane.py
--rw-r--r--   0        0        0       67 2024-04-10 12:31:20.207512 spine_segmentation-0.2.8/spine_segmentation/spine_types/roi.py
--rw-r--r--   0        0        0      246 2024-04-10 12:31:20.207512 spine_segmentation-0.2.8/spine_segmentation/spine_types/spine.py
--rw-r--r--   0        0        0      116 2024-04-10 18:52:49.974852 spine_segmentation-0.2.8/spine_segmentation/spine_types/vertebra.py
--rw-r--r--   0        0        0     1190 2024-04-11 12:53:48.874194 spine_segmentation-0.2.8/spine_segmentation/trainer/learning_rate_finder.py
--rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.2.8/spine_segmentation/utils/__init__.py
--rw-r--r--   0        0        0      685 2024-04-10 12:31:20.207512 spine_segmentation-0.2.8/spine_segmentation/utils/fix_validations_step_bar.py
--rw-r--r--   0        0        0      218 2024-04-10 12:31:20.207512 spine_segmentation-0.2.8/spine_segmentation/utils/globals.py
--rw-r--r--   0        0        0      552 2024-04-10 12:31:20.207512 spine_segmentation-0.2.8/spine_segmentation/utils/log_dir.py
--rw-r--r--   0        0        0      690 2024-04-10 12:31:20.207512 spine_segmentation-0.2.8/spine_segmentation/utils/profiling.py
--rw-r--r--   0        0        0      930 2024-04-10 12:31:20.207512 spine_segmentation-0.2.8/spine_segmentation/utils/proxy_class.py
--rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.2.8/spine_segmentation/visualisation/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.2.8/spine_segmentation/visualisation/blender/__init__.py
--rw-r--r--   0        0        0    11971 2024-04-10 12:31:20.207512 spine_segmentation-0.2.8/spine_segmentation/visualisation/blender/blender_script.py
--rw-r--r--   0        0        0     9179 2024-04-11 12:53:48.830193 spine_segmentation-0.2.8/spine_segmentation/visualisation/blender/gen_obj.py
--rw-r--r--   0        0        0     8158 2024-04-11 12:53:48.822193 spine_segmentation-0.2.8/spine_segmentation/visualisation/blender/open_in_blender.py
--rw-r--r--   0        0        0    12036 2024-04-10 12:31:20.207512 spine_segmentation-0.2.8/spine_segmentation/visualisation/color.py
--rw-r--r--   0        0        0     1705 2024-04-11 12:53:48.794192 spine_segmentation-0.2.8/spine_segmentation/visualisation/color_palettes.py
--rw-r--r--   0        0        0     2602 1970-01-01 00:00:00.000000 spine_segmentation-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-11 11:32:29.446351 spine_segmentation-0.2.9/README.md
+-rw-r--r--   0        0        0     2382 2024-04-15 15:42:57.396422 spine_segmentation-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      122 2024-04-11 12:53:48.914194 spine_segmentation-0.2.9/spine_segmentation/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.2.9/spine_segmentation/annotators/__init__.py
+-rw-r--r--   0        0        0    16308 2024-04-11 12:53:48.934194 spine_segmentation-0.2.9/spine_segmentation/annotators/annotator_base.py
+-rw-r--r--   0        0        0     8225 2024-04-11 12:53:48.814193 spine_segmentation-0.2.9/spine_segmentation/annotators/vector_annotator.py
+-rw-r--r--   0        0        0     2190 2024-04-11 12:53:48.766192 spine_segmentation-0.2.9/spine_segmentation/cli/cli.py
+-rw-r--r--   0        0        0    12072 2024-04-10 12:31:20.207512 spine_segmentation-0.2.9/spine_segmentation/dataloader/statistics.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.2.9/spine_segmentation/datasets/__init__.py
+-rw-r--r--   0        0        0     2868 2024-04-10 12:31:20.207512 spine_segmentation-0.2.9/spine_segmentation/datasets/augmentation.py
+-rw-r--r--   0        0        0     4312 2024-04-11 12:53:48.806193 spine_segmentation-0.2.9/spine_segmentation/datasets/feature_dataset.py
+-rw-r--r--   0        0        0     6696 2024-04-11 15:53:29.418496 spine_segmentation-0.2.9/spine_segmentation/datasets/metadata_prediction_dataset.py
+-rw-r--r--   0        0        0     6372 2024-04-11 15:53:29.430496 spine_segmentation-0.2.9/spine_segmentation/datasets/patch_segmentation_dataset.py
+-rw-r--r--   0        0        0     1360 2024-04-11 15:53:29.410496 spine_segmentation-0.2.9/spine_segmentation/datasets/path_helper.py
+-rw-r--r--   0        0        0    14744 2024-04-11 15:47:48.534212 spine_segmentation-0.2.9/spine_segmentation/datasets/sample.py
+-rw-r--r--   0        0        0    14989 2024-04-11 15:53:29.422496 spine_segmentation-0.2.9/spine_segmentation/datasets/segmentation_dataset.py
+-rw-r--r--   0        0        0     2037 2024-04-11 12:53:48.782192 spine_segmentation-0.2.9/spine_segmentation/datasets/vector_table_graphs_dataset.py
+-rw-r--r--   0        0        0     2581 2024-04-11 12:53:48.890194 spine_segmentation-0.2.9/spine_segmentation/evaluate/analyze_edge_cases.py
+-rw-r--r--   0        0        0     2520 2024-04-11 12:53:48.798193 spine_segmentation-0.2.9/spine_segmentation/evaluate/analyze_index_list.py
+-rw-r--r--   0        0        0     1659 2024-04-11 12:53:48.854193 spine_segmentation-0.2.9/spine_segmentation/evaluate/classic_ml.py
+-rw-r--r--   0        0        0     1108 2024-04-10 12:31:20.207512 spine_segmentation-0.2.9/spine_segmentation/evaluate/eval_created_stats.py
+-rw-r--r--   0        0        0    15527 2024-04-11 15:52:07.339228 spine_segmentation-0.2.9/spine_segmentation/evaluate/eval_instance_seg_model.py
+-rw-r--r--   0        0        0     8215 2024-04-11 12:53:48.746192 spine_segmentation-0.2.9/spine_segmentation/evaluate/eval_splitting.py
+-rw-r--r--   0        0        0     6109 2024-04-11 15:52:07.363228 spine_segmentation-0.2.9/spine_segmentation/evaluate/load_model.py
+-rw-r--r--   0        0        0     4885 2024-04-11 12:53:48.882194 spine_segmentation-0.2.9/spine_segmentation/evaluate/metadata.py
+-rw-r--r--   0        0        0     1627 2024-04-11 12:53:48.894194 spine_segmentation-0.2.9/spine_segmentation/evaluate/volume_size_in_gt.py
+-rw-r--r--   0        0        0     8685 2024-04-15 15:42:40.700782 spine_segmentation-0.2.9/spine_segmentation/inference/instance_segmentation.py
+-rw-r--r--   0        0        0     6761 2024-04-11 12:53:48.846193 spine_segmentation-0.2.9/spine_segmentation/inference/onnx_model.py
+-rw-r--r--   0        0        0     7515 2024-04-11 12:53:48.906194 spine_segmentation-0.2.9/spine_segmentation/instance_separation/instance_separation.py
+-rw-r--r--   0        0        0      304 2024-04-10 12:31:20.207512 spine_segmentation-0.2.9/spine_segmentation/losses/diffis1.py
+-rw-r--r--   0        0        0     2080 2024-04-11 15:40:00.222464 spine_segmentation-0.2.9/spine_segmentation/model_downloader/model_downloader.py
+-rw-r--r--   0        0        0      712 2024-04-11 12:53:48.850193 spine_segmentation-0.2.9/spine_segmentation/plotting/bmi.py
+-rw-r--r--   0        0        0     8132 2024-04-11 12:53:48.778192 spine_segmentation-0.2.9/spine_segmentation/plotting/classification_correlation.py
+-rw-r--r--   0        0        0     2566 2024-04-11 12:53:48.886194 spine_segmentation-0.2.9/spine_segmentation/plotting/patient_metadata.py
+-rw-r--r--   0        0        0    10404 2024-04-11 12:53:48.826193 spine_segmentation-0.2.9/spine_segmentation/plotting/plot_slice.py
+-rw-r--r--   0        0        0     1795 2024-04-11 12:53:48.938195 spine_segmentation-0.2.9/spine_segmentation/plotting/plot_statistics.py
+-rw-r--r--   0        0        0     5823 2024-04-11 12:53:48.834193 spine_segmentation-0.2.9/spine_segmentation/plotting/read_npz_eval_per_roi_accuracy.py
+-rw-r--r--   0        0        0     5767 2024-04-11 12:53:48.786192 spine_segmentation-0.2.9/spine_segmentation/plotting/show_plane_splitting_3d.py
+-rw-r--r--   0        0        0      266 2024-04-11 12:53:48.858193 spine_segmentation-0.2.9/spine_segmentation/plotting/ydata_profile_report.py
+-rw-r--r--   0        0        0      930 2024-04-11 15:55:12.773382 spine_segmentation-0.2.9/spine_segmentation/resources/paths.py
+-rw-r--r--   0        0        0      933 2024-04-11 12:53:48.842193 spine_segmentation-0.2.9/spine_segmentation/resources/preloaded.py
+-rw-r--r--   0        0        0       63 2024-04-11 09:34:14.336647 spine_segmentation-0.2.9/spine_segmentation/run.py
+-rw-r--r--   0        0        0     4575 2024-04-10 12:31:20.207512 spine_segmentation-0.2.9/spine_segmentation/scripts/format_results.py
+-rw-r--r--   0        0        0     4546 2024-04-11 12:53:48.866193 spine_segmentation-0.2.9/spine_segmentation/scripts/split_train_val_test.py
+-rw-r--r--   0        0        0      210 2024-04-10 12:31:20.207512 spine_segmentation-0.2.9/spine_segmentation/scripts/test_patient_ids.txt
+-rw-r--r--   0        0        0      112 2024-04-10 18:52:49.798849 spine_segmentation-0.2.9/spine_segmentation/spine_types/disc.py
+-rw-r--r--   0        0        0     1314 2024-04-15 15:42:51.276552 spine_segmentation-0.2.9/spine_segmentation/spine_types/labels.py
+-rw-r--r--   0        0        0      219 2024-04-10 12:31:20.207512 spine_segmentation-0.2.9/spine_segmentation/spine_types/line_segment.py
+-rw-r--r--   0        0        0     2409 2024-04-10 12:31:20.207512 spine_segmentation-0.2.9/spine_segmentation/spine_types/plane.py
+-rw-r--r--   0        0        0       67 2024-04-10 12:31:20.207512 spine_segmentation-0.2.9/spine_segmentation/spine_types/roi.py
+-rw-r--r--   0        0        0      246 2024-04-10 12:31:20.207512 spine_segmentation-0.2.9/spine_segmentation/spine_types/spine.py
+-rw-r--r--   0        0        0      116 2024-04-10 18:52:49.974852 spine_segmentation-0.2.9/spine_segmentation/spine_types/vertebra.py
+-rw-r--r--   0        0        0     1190 2024-04-11 12:53:48.874194 spine_segmentation-0.2.9/spine_segmentation/trainer/learning_rate_finder.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.2.9/spine_segmentation/utils/__init__.py
+-rw-r--r--   0        0        0      685 2024-04-10 12:31:20.207512 spine_segmentation-0.2.9/spine_segmentation/utils/fix_validations_step_bar.py
+-rw-r--r--   0        0        0      218 2024-04-10 12:31:20.207512 spine_segmentation-0.2.9/spine_segmentation/utils/globals.py
+-rw-r--r--   0        0        0      552 2024-04-10 12:31:20.207512 spine_segmentation-0.2.9/spine_segmentation/utils/log_dir.py
+-rw-r--r--   0        0        0      690 2024-04-10 12:31:20.207512 spine_segmentation-0.2.9/spine_segmentation/utils/profiling.py
+-rw-r--r--   0        0        0      930 2024-04-10 12:31:20.207512 spine_segmentation-0.2.9/spine_segmentation/utils/proxy_class.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.2.9/spine_segmentation/visualisation/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.2.9/spine_segmentation/visualisation/blender/__init__.py
+-rw-r--r--   0        0        0    11971 2024-04-10 12:31:20.207512 spine_segmentation-0.2.9/spine_segmentation/visualisation/blender/blender_script.py
+-rw-r--r--   0        0        0     9179 2024-04-11 12:53:48.830193 spine_segmentation-0.2.9/spine_segmentation/visualisation/blender/gen_obj.py
+-rw-r--r--   0        0        0     8158 2024-04-11 12:53:48.822193 spine_segmentation-0.2.9/spine_segmentation/visualisation/blender/open_in_blender.py
+-rw-r--r--   0        0        0    12036 2024-04-10 12:31:20.207512 spine_segmentation-0.2.9/spine_segmentation/visualisation/color.py
+-rw-r--r--   0        0        0     1705 2024-04-11 12:53:48.794192 spine_segmentation-0.2.9/spine_segmentation/visualisation/color_palettes.py
+-rw-r--r--   0        0        0     2602 1970-01-01 00:00:00.000000 spine_segmentation-0.2.9/PKG-INFO
```

### Comparing `spine_segmentation-0.2.8/README.md` & `spine_segmentation-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/pyproject.toml` & `spine_segmentation-0.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spine-segmentation"
-version = "0.2.8"
+version = "0.2.9"
 description = "Anatomical labeling of the spine in small field-of-view MRI scans"
 authors = [
     "Brutenis Gliwa <brutenis@gmail.com>",
 ]
 readme = "README.md"
 
 classifiers = [
```

### Comparing `spine_segmentation-0.2.8/spine_segmentation/annotators/annotator_base.py` & `spine_segmentation-0.2.9/spine_segmentation/annotators/annotator_base.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/annotators/vector_annotator.py` & `spine_segmentation-0.2.9/spine_segmentation/annotators/vector_annotator.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/cli/cli.py` & `spine_segmentation-0.2.9/spine_segmentation/cli/cli.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/dataloader/statistics.py` & `spine_segmentation-0.2.9/spine_segmentation/dataloader/statistics.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/datasets/augmentation.py` & `spine_segmentation-0.2.9/spine_segmentation/datasets/augmentation.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/datasets/feature_dataset.py` & `spine_segmentation-0.2.9/spine_segmentation/datasets/feature_dataset.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/datasets/metadata_prediction_dataset.py` & `spine_segmentation-0.2.9/spine_segmentation/datasets/metadata_prediction_dataset.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/datasets/patch_segmentation_dataset.py` & `spine_segmentation-0.2.9/spine_segmentation/datasets/patch_segmentation_dataset.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/datasets/path_helper.py` & `spine_segmentation-0.2.9/spine_segmentation/datasets/path_helper.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/datasets/sample.py` & `spine_segmentation-0.2.9/spine_segmentation/datasets/sample.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/datasets/segmentation_dataset.py` & `spine_segmentation-0.2.9/spine_segmentation/datasets/segmentation_dataset.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/datasets/vector_table_graphs_dataset.py` & `spine_segmentation-0.2.9/spine_segmentation/datasets/vector_table_graphs_dataset.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/evaluate/analyze_edge_cases.py` & `spine_segmentation-0.2.9/spine_segmentation/evaluate/analyze_edge_cases.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/evaluate/analyze_index_list.py` & `spine_segmentation-0.2.9/spine_segmentation/evaluate/analyze_index_list.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/evaluate/classic_ml.py` & `spine_segmentation-0.2.9/spine_segmentation/evaluate/classic_ml.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/evaluate/eval_created_stats.py` & `spine_segmentation-0.2.9/spine_segmentation/evaluate/eval_created_stats.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/evaluate/eval_instance_seg_model.py` & `spine_segmentation-0.2.9/spine_segmentation/evaluate/eval_instance_seg_model.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/evaluate/eval_splitting.py` & `spine_segmentation-0.2.9/spine_segmentation/evaluate/eval_splitting.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/evaluate/load_model.py` & `spine_segmentation-0.2.9/spine_segmentation/evaluate/load_model.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/evaluate/metadata.py` & `spine_segmentation-0.2.9/spine_segmentation/evaluate/metadata.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/evaluate/volume_size_in_gt.py` & `spine_segmentation-0.2.9/spine_segmentation/evaluate/volume_size_in_gt.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/inference/instance_segmentation.py` & `spine_segmentation-0.2.9/spine_segmentation/inference/instance_segmentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from spine_segmentation.inference.onnx_model import ONNXInferenceModel
 from spine_segmentation.instance_separation.instance_separation import (
     get_planes_from_rois,
     mask_rare_rois,
     separate_rois_with_labels,
     separate_segmented_rois_by_planes,
 )
-from spine_segmentation.spine_types.labels import get_labels_for_n_classes
+from spine_segmentation.spine_types.labels import get_labels_for_n_classes, get_label_lookup_for_n_classes
 from spine_segmentation.utils.log_dir import get_next_log_dir
 from spine_segmentation.visualisation.blender.open_in_blender import open_in_blender
 
 import numpy as np
 
 
 def post_process_instances(vertebra_instances, segmentation, plot_dir=None):
@@ -155,15 +155,15 @@
         new_npz["instances"] = new_npz["instances"] * 2 - (new_npz["instances"] != 0)
         # new_npz["id_to_label"] = gt_npz["id_to_label"]
         # new_npz["gt_id_to_label"] = gt_npz["id_to_label"]
         new_npz["instances_post_processed"] = post_process_instances(
             new_npz["instances"], cropped_inst_seg_input[:, 0, :, :], plot_dir=cache_dir
         )
         new_npz["cropped_segmentation"] = cropped_inst_seg_input[:, 0, :, :]
-        id_to_labels = get_labels_for_n_classes(49)
+        id_to_labels = get_label_lookup_for_n_classes(49)
 
         instances = new_npz["instances_post_processed"]
         segmentation = seg_npz["segmentation"]
         if self._output_same_shape_as_input:
             segmentation = self._crop_and_pad_to_shape(segmentation, initial_shape[1], initial_shape[2])
             instances = self._crop_and_pad_to_shape(instances, initial_shape[1], initial_shape[2])
             assert segmentation.shape == initial_shape
```

### Comparing `spine_segmentation-0.2.8/spine_segmentation/inference/onnx_model.py` & `spine_segmentation-0.2.9/spine_segmentation/inference/onnx_model.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/instance_separation/instance_separation.py` & `spine_segmentation-0.2.9/spine_segmentation/instance_separation/instance_separation.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/model_downloader/model_downloader.py` & `spine_segmentation-0.2.9/spine_segmentation/model_downloader/model_downloader.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/plotting/bmi.py` & `spine_segmentation-0.2.9/spine_segmentation/plotting/bmi.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/plotting/classification_correlation.py` & `spine_segmentation-0.2.9/spine_segmentation/plotting/classification_correlation.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/plotting/patient_metadata.py` & `spine_segmentation-0.2.9/spine_segmentation/plotting/patient_metadata.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/plotting/plot_slice.py` & `spine_segmentation-0.2.9/spine_segmentation/plotting/plot_slice.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/plotting/plot_statistics.py` & `spine_segmentation-0.2.9/spine_segmentation/plotting/plot_statistics.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/plotting/read_npz_eval_per_roi_accuracy.py` & `spine_segmentation-0.2.9/spine_segmentation/plotting/read_npz_eval_per_roi_accuracy.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/plotting/show_plane_splitting_3d.py` & `spine_segmentation-0.2.9/spine_segmentation/plotting/show_plane_splitting_3d.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/resources/paths.py` & `spine_segmentation-0.2.9/spine_segmentation/resources/paths.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/resources/preloaded.py` & `spine_segmentation-0.2.9/spine_segmentation/resources/preloaded.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/scripts/format_results.py` & `spine_segmentation-0.2.9/spine_segmentation/scripts/format_results.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/scripts/split_train_val_test.py` & `spine_segmentation-0.2.9/spine_segmentation/scripts/split_train_val_test.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/spine_types/labels.py` & `spine_segmentation-0.2.9/spine_segmentation/spine_types/labels.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 from itertools import zip_longest
+from typing import List, Dict
 
 
 def get_vertebra_labels(c_range=range(2, 8), t_range=range(1, 13), l_range=range(1, 6)):
     return [*[f"C{i}" for i in c_range], *[f"T{i}" for i in t_range], *[f"L{i}" for i in l_range], "S1"]
 
 
 def get_disc_labels(vertebra_labels):
     return [
         *[f"{upper}-{lower}" for upper, lower in zip(vertebra_labels[:-1], vertebra_labels[1:])],
     ]
 
 
 # 6 + 12 + 5 + 1
-def get_labels_for_n_classes(n=47):
+def get_labels_for_n_classes(n=47) -> List[str]:
     while n not in [0, 45, 47, 49] and n > 45:
         print(f"Only 45, 47, 49 classes are supported, got {n}, downscaling for now")
         n -= 1
 
     # assert n in [45, 47, 49], "Only 45, 47, 49 classes are supported"
     lumbar_vertebra_count = 4 + (n >= 47) + (n >= 49)
     lumbar_range = range(1, lumbar_vertebra_count + 1)
     vertebra_labels = get_vertebra_labels(c_range=range(2, 8), t_range=range(1, 13), l_range=lumbar_range)
     disc_labels = get_disc_labels(vertebra_labels)
 
     labels = list(filter(None, sum(zip_longest(vertebra_labels, disc_labels), ())))
     return labels
+
+
+def get_label_lookup_for_n_classes(n=47) -> Dict[int, str]:
+    labels = get_labels_for_n_classes(n=n)
+    label_lookup = {0: "0_unknown"}
+    for i, label in enumerate(labels, 1):
+        label_lookup[label] = i
+    return label_lookup
```

### Comparing `spine_segmentation-0.2.8/spine_segmentation/spine_types/plane.py` & `spine_segmentation-0.2.9/spine_segmentation/spine_types/plane.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/trainer/learning_rate_finder.py` & `spine_segmentation-0.2.9/spine_segmentation/trainer/learning_rate_finder.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/utils/fix_validations_step_bar.py` & `spine_segmentation-0.2.9/spine_segmentation/utils/fix_validations_step_bar.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/utils/log_dir.py` & `spine_segmentation-0.2.9/spine_segmentation/utils/log_dir.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/utils/profiling.py` & `spine_segmentation-0.2.9/spine_segmentation/utils/profiling.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/utils/proxy_class.py` & `spine_segmentation-0.2.9/spine_segmentation/utils/proxy_class.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/visualisation/blender/blender_script.py` & `spine_segmentation-0.2.9/spine_segmentation/visualisation/blender/blender_script.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/visualisation/blender/gen_obj.py` & `spine_segmentation-0.2.9/spine_segmentation/visualisation/blender/gen_obj.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/visualisation/blender/open_in_blender.py` & `spine_segmentation-0.2.9/spine_segmentation/visualisation/blender/open_in_blender.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/visualisation/color.py` & `spine_segmentation-0.2.9/spine_segmentation/visualisation/color.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/spine_segmentation/visualisation/color_palettes.py` & `spine_segmentation-0.2.9/spine_segmentation/visualisation/color_palettes.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.2.8/PKG-INFO` & `spine_segmentation-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spine-segmentation
-Version: 0.2.8
+Version: 0.2.9
 Summary: Anatomical labeling of the spine in small field-of-view MRI scans
 Author: Brutenis Gliwa
 Author-email: brutenis@gmail.com
 Requires-Python: >=3.8.1,<3.13.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

