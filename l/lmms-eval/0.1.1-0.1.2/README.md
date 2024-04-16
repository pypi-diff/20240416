# Comparing `tmp/lmms_eval-0.1.1.tar.gz` & `tmp/lmms_eval-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmms_eval-0.1.1.tar", last modified: Thu Mar 14 06:39:03 2024, max compression
+gzip compressed data, was "lmms_eval-0.1.2.tar", last modified: Tue Apr 16 16:41:59 2024, max compression
```

## Comparing `lmms_eval-0.1.1.tar` & `lmms_eval-0.1.2.tar`

### file list

```diff
@@ -1,343 +1,369 @@
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.569057 lmms_eval-0.1.1/
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.553057 lmms_eval-0.1.1/.github/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      272 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/.github/issue_template.md
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      284 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/.github/pull_request_template.md
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.553057 lmms_eval-0.1.1/.github/workflows/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      386 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/.github/workflows/black.yml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      340 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/.gitignore
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      125 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 fypu      (1003) fypu      (1004)    16936 2024-03-14 06:39:03.569057 lmms_eval-0.1.1/PKG-INFO
--rw-rw-r--   0 fypu      (1003) fypu      (1004)    15460 2024-03-14 06:28:25.000000 lmms_eval-0.1.1/README.md
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.553057 lmms_eval-0.1.1/docs/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      449 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/docs/README.md
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     2701 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/docs/commands.md
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     5277 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/docs/model_guide.md
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     6819 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/docs/task_guide.md
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      345 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/example_eval.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      477 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/llava_repr_requirements.txt
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.553057 lmms_eval-0.1.1/lmms_eval/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)        0 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/__init__.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)    13586 2024-03-14 06:28:25.000000 lmms_eval-0.1.1/lmms_eval/__main__.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.553057 lmms_eval-0.1.1/lmms_eval/api/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)        0 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/api/__init__.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     2025 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/api/filter.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      914 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/api/instance.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)    12174 2024-03-08 15:14:28.000000 lmms_eval-0.1.1/lmms_eval/api/metrics.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     7308 2024-03-08 15:14:28.000000 lmms_eval-0.1.1/lmms_eval/api/model.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     3896 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/api/registry.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     3548 2024-03-14 06:28:25.000000 lmms_eval-0.1.1/lmms_eval/api/samplers.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)    48258 2024-03-08 15:14:28.000000 lmms_eval-0.1.1/lmms_eval/api/task.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)    25312 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/evaluator.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.553057 lmms_eval-0.1.1/lmms_eval/filters/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     1516 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/filters/__init__.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      631 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/filters/decontamination.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     1759 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/filters/extraction.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     1584 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/filters/selection.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     1512 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/filters/transformation.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)    14819 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/logging_utils.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.553057 lmms_eval-0.1.1/lmms_eval/models/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      419 2024-03-08 15:14:28.000000 lmms_eval-0.1.1/lmms_eval/models/__init__.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)    12571 2024-03-08 15:14:28.000000 lmms_eval-0.1.1/lmms_eval/models/fuyu.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     5407 2024-03-08 15:14:28.000000 lmms_eval-0.1.1/lmms_eval/models/gpt4v.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     9664 2024-03-08 15:14:28.000000 lmms_eval-0.1.1/lmms_eval/models/instructblip.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)    19551 2024-03-14 06:28:25.000000 lmms_eval-0.1.1/lmms_eval/models/llava.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     9771 2024-03-08 15:14:28.000000 lmms_eval-0.1.1/lmms_eval/models/minicpm_v.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.553057 lmms_eval-0.1.1/lmms_eval/models/model_utils/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)        0 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/models/model_utils/__init__.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.553057 lmms_eval-0.1.1/lmms_eval/models/model_utils/qwen/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)    14392 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/models/model_utils/qwen/qwen_generate_utils.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)    13182 2024-03-08 15:14:28.000000 lmms_eval-0.1.1/lmms_eval/models/qwen_vl.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.553057 lmms_eval-0.1.1/lmms_eval/tasks/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     5453 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/__init__.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.553057 lmms_eval-0.1.1/lmms_eval/tasks/__pycache__/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     7690 2024-03-08 12:50:58.000000 lmms_eval-0.1.1/lmms_eval/tasks/__pycache__/__init__.cpython-311.pyc
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.553057 lmms_eval-0.1.1/lmms_eval/tasks/_task_utils/
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.553057 lmms_eval-0.1.1/lmms_eval/tasks/_task_utils/__pycache__/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      753 2024-03-08 12:51:01.000000 lmms_eval-0.1.1/lmms_eval/tasks/_task_utils/__pycache__/file_utils.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     8354 2024-03-08 12:51:02.000000 lmms_eval-0.1.1/lmms_eval/tasks/_task_utils/__pycache__/vqa_eval_metric.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      227 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/_task_utils/file_utils.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)        0 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/_task_utils/gpt_eval_utils.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     6056 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/_task_utils/vqa_eval_metric.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.553057 lmms_eval-0.1.1/lmms_eval/tasks/ai2d/
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.557057 lmms_eval-0.1.1/lmms_eval/tasks/ai2d/__pycache__/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     2615 2024-03-08 12:51:02.000000 lmms_eval-0.1.1/lmms_eval/tasks/ai2d/__pycache__/utils.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      876 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/ai2d/ai2d.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     5098 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/ai2d/upload_ai2d.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     1271 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/ai2d/utils.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.557057 lmms_eval-0.1.1/lmms_eval/tasks/chartqa/
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.557057 lmms_eval-0.1.1/lmms_eval/tasks/chartqa/__pycache__/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     3340 2024-03-08 12:51:02.000000 lmms_eval-0.1.1/lmms_eval/tasks/chartqa/__pycache__/utils.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      844 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/chartqa/chartqa.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     5365 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/chartqa/upload_chartqa.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     2378 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/chartqa/utils.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.557057 lmms_eval-0.1.1/lmms_eval/tasks/cmmmu/
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.557057 lmms_eval-0.1.1/lmms_eval/tasks/cmmmu/__pycache__/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)    23315 2024-03-12 00:53:52.000000 lmms_eval-0.1.1/lmms_eval/tasks/cmmmu/__pycache__/utils.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)       44 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/cmmmu/_cmmmu.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      249 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/cmmmu/_default_template_cmmmu_yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      517 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/cmmmu/cmmmu_test.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      544 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/cmmmu/cmmmu_val.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)    17232 2024-03-08 15:14:28.000000 lmms_eval-0.1.1/lmms_eval/tasks/cmmmu/utils.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.557057 lmms_eval-0.1.1/lmms_eval/tasks/coco_cap/
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.557057 lmms_eval-0.1.1/lmms_eval/tasks/coco_cap/__pycache__/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     9135 2024-03-08 12:51:01.000000 lmms_eval-0.1.1/lmms_eval/tasks/coco_cap/__pycache__/utils.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)       69 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/coco_cap/coco2014_cap.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      764 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/coco_cap/coco2014_cap_test.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     1415 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/coco_cap/coco2014_cap_val.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)       69 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/coco_cap/coco2017_cap.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      748 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/coco_cap/coco2017_cap_test.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     1399 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/coco_cap/coco2017_cap_val.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      109 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/coco_cap/coco_cap.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     5273 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/coco_cap/utils.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.557057 lmms_eval-0.1.1/lmms_eval/tasks/docvqa/
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.557057 lmms_eval-0.1.1/lmms_eval/tasks/docvqa/__pycache__/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     2005 2024-03-08 12:51:02.000000 lmms_eval-0.1.1/lmms_eval/tasks/docvqa/__pycache__/utils.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      500 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/docvqa/_default_template_docvqa_yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)       46 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/docvqa/docvqa.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      263 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/docvqa/docvqa_test.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      160 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/docvqa/docvqa_val.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      992 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/docvqa/utils.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.557057 lmms_eval-0.1.1/lmms_eval/tasks/ferret/
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.557057 lmms_eval-0.1.1/lmms_eval/tasks/ferret/__pycache__/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)    10423 2024-03-08 12:51:02.000000 lmms_eval-0.1.1/lmms_eval/tasks/ferret/__pycache__/utils.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     1134 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/ferret/ferret.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     5228 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/ferret/rule.json
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     6956 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/ferret/utils.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.557057 lmms_eval-0.1.1/lmms_eval/tasks/flickr30k/
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.557057 lmms_eval-0.1.1/lmms_eval/tasks/flickr30k/__pycache__/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     7574 2024-03-08 12:51:02.000000 lmms_eval-0.1.1/lmms_eval/tasks/flickr30k/__pycache__/utils.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)       39 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/flickr30k/flickr30k.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     1403 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/flickr30k/flickr30k_test.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     4545 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/flickr30k/utils.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.557057 lmms_eval-0.1.1/lmms_eval/tasks/gqa/
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.557057 lmms_eval-0.1.1/lmms_eval/tasks/gqa/__pycache__/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     1162 2024-03-08 12:51:02.000000 lmms_eval-0.1.1/lmms_eval/tasks/gqa/__pycache__/utils.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      737 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/gqa/gqa.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      781 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/gqa/utils.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.557057 lmms_eval-0.1.1/lmms_eval/tasks/hallusion_bench/
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.557057 lmms_eval-0.1.1/lmms_eval/tasks/hallusion_bench/__pycache__/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     7903 2024-03-08 12:51:01.000000 lmms_eval-0.1.1/lmms_eval/tasks/hallusion_bench/__pycache__/evaluate_hb.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)    15596 2024-03-08 12:51:01.000000 lmms_eval-0.1.1/lmms_eval/tasks/hallusion_bench/__pycache__/utils.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     4862 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/hallusion_bench/evaluate_hb.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     1257 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/hallusion_bench/hallusion_bench_image.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)    12366 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/hallusion_bench/utils.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.557057 lmms_eval-0.1.1/lmms_eval/tasks/iconqa/
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.557057 lmms_eval-0.1.1/lmms_eval/tasks/iconqa/__pycache__/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     3467 2024-03-08 12:51:01.000000 lmms_eval-0.1.1/lmms_eval/tasks/iconqa/__pycache__/utils.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      816 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/iconqa/_default_template_docvqa_yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)       47 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/iconqa/iconqa.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)       75 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/iconqa/iconqa_test.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)       73 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/iconqa/iconqa_val.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     2162 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/iconqa/utils.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.557057 lmms_eval-0.1.1/lmms_eval/tasks/infovqa/
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.557057 lmms_eval-0.1.1/lmms_eval/tasks/infovqa/__pycache__/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     1936 2024-03-08 12:51:01.000000 lmms_eval-0.1.1/lmms_eval/tasks/infovqa/__pycache__/utils.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      423 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/infovqa/_default_template_infovqa_yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)       50 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/infovqa/infovqa.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      297 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/infovqa/infovqa_test.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      189 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/infovqa/infovqa_val.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      951 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/infovqa/utils.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.557057 lmms_eval-0.1.1/lmms_eval/tasks/llava-bench-coco/
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.557057 lmms_eval-0.1.1/lmms_eval/tasks/llava-bench-coco/__pycache__/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)    10528 2024-03-08 12:51:01.000000 lmms_eval-0.1.1/lmms_eval/tasks/llava-bench-coco/__pycache__/utils.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     1087 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/llava-bench-coco/llava-bench-coco.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     9098 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/llava-bench-coco/rule.json
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     6883 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/llava-bench-coco/utils.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.557057 lmms_eval-0.1.1/lmms_eval/tasks/llava-in-the-wild/
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.557057 lmms_eval-0.1.1/lmms_eval/tasks/llava-in-the-wild/__pycache__/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)    10433 2024-03-08 12:51:01.000000 lmms_eval-0.1.1/lmms_eval/tasks/llava-in-the-wild/__pycache__/utils.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     1115 2024-03-14 06:28:25.000000 lmms_eval-0.1.1/lmms_eval/tasks/llava-in-the-wild/llava-in-the-wild.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     9098 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/llava-in-the-wild/rule.json
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     6851 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/llava-in-the-wild/utils.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.561057 lmms_eval-0.1.1/lmms_eval/tasks/mathvista/
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.561057 lmms_eval-0.1.1/lmms_eval/tasks/mathvista/__pycache__/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)    20278 2024-03-08 12:51:02.000000 lmms_eval-0.1.1/lmms_eval/tasks/mathvista/__pycache__/mathvista_evals.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     8208 2024-03-08 12:51:02.000000 lmms_eval-0.1.1/lmms_eval/tasks/mathvista/__pycache__/utils.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      148 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/mathvista/mathvista.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)    18971 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/mathvista/mathvista_evals.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      775 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/mathvista/mathvista_test.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      789 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/mathvista/mathvista_testmini.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     5022 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/mathvista/utils.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.561057 lmms_eval-0.1.1/lmms_eval/tasks/mmbench/
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.561057 lmms_eval-0.1.1/lmms_eval/tasks/mmbench/__pycache__/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     3851 2024-03-12 02:56:32.000000 lmms_eval-0.1.1/lmms_eval/tasks/mmbench/__pycache__/cc_utils.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     5252 2024-03-12 02:52:32.000000 lmms_eval-0.1.1/lmms_eval/tasks/mmbench/__pycache__/cn_utils.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     5260 2024-03-12 02:52:32.000000 lmms_eval-0.1.1/lmms_eval/tasks/mmbench/__pycache__/en_utils.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     1870 2024-03-08 12:51:02.000000 lmms_eval-0.1.1/lmms_eval/tasks/mmbench/__pycache__/mmbench_evals.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     2285 2024-03-14 06:28:25.000000 lmms_eval-0.1.1/lmms_eval/tasks/mmbench/cc_utils.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     3081 2024-03-14 06:28:25.000000 lmms_eval-0.1.1/lmms_eval/tasks/mmbench/cn_utils.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     3081 2024-03-14 06:28:25.000000 lmms_eval-0.1.1/lmms_eval/tasks/mmbench/en_utils.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      116 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/mmbench/mmbench.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      896 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/mmbench/mmbench_cc.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      146 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/mmbench/mmbench_cn.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      876 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/mmbench/mmbench_cn_dev.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      887 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/mmbench/mmbench_cn_test.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      353 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/mmbench/mmbench_en.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      581 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/mmbench/mmbench_en_dev.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      582 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/mmbench/mmbench_en_test.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      684 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/mmbench/mmbench_evals.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.561057 lmms_eval-0.1.1/lmms_eval/tasks/mme/
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.561057 lmms_eval-0.1.1/lmms_eval/tasks/mme/__pycache__/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     5101 2024-03-08 12:51:02.000000 lmms_eval-0.1.1/lmms_eval/tasks/mme/__pycache__/utils.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     1105 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/mme/mme.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     3925 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/mme/utils.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.561057 lmms_eval-0.1.1/lmms_eval/tasks/mmmu/
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.561057 lmms_eval-0.1.1/lmms_eval/tasks/mmmu/__pycache__/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)    19955 2024-03-08 12:51:01.000000 lmms_eval-0.1.1/lmms_eval/tasks/mmmu/__pycache__/utils.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)       41 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/mmmu/mmmu.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      701 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/mmmu/mmmu_test.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      684 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/mmmu/mmmu_val.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)    16383 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/mmmu/utils.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.561057 lmms_eval-0.1.1/lmms_eval/tasks/mmvet/
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.561057 lmms_eval-0.1.1/lmms_eval/tasks/mmvet/__pycache__/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)    11881 2024-03-08 12:51:02.000000 lmms_eval-0.1.1/lmms_eval/tasks/mmvet/__pycache__/utils.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      768 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/mmvet/mmvet.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     9027 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/mmvet/utils.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.561057 lmms_eval-0.1.1/lmms_eval/tasks/multidocvqa/
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.561057 lmms_eval-0.1.1/lmms_eval/tasks/multidocvqa/__pycache__/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     8605 2024-03-08 12:51:02.000000 lmms_eval-0.1.1/lmms_eval/tasks/multidocvqa/__pycache__/utils.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)       62 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/multidocvqa/multidocvqa.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      648 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/multidocvqa/multidocvqa_test.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      750 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/multidocvqa/multidocvqa_val.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     3903 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/multidocvqa/utils.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.561057 lmms_eval-0.1.1/lmms_eval/tasks/nocaps/
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.561057 lmms_eval-0.1.1/lmms_eval/tasks/nocaps/__pycache__/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     8769 2024-03-08 12:51:01.000000 lmms_eval-0.1.1/lmms_eval/tasks/nocaps/__pycache__/utils.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      109 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/nocaps/_default_template_nocaps_yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)       51 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/nocaps/nocaps.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      792 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/nocaps/nocaps_test.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     1479 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/nocaps/nocaps_val.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     5255 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/nocaps/utils.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.561057 lmms_eval-0.1.1/lmms_eval/tasks/ok_vqa/
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.561057 lmms_eval-0.1.1/lmms_eval/tasks/ok_vqa/__pycache__/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     4152 2024-03-08 12:51:02.000000 lmms_eval-0.1.1/lmms_eval/tasks/ok_vqa/__pycache__/utils.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      768 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/ok_vqa/_default_template_vqa_yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      833 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/ok_vqa/_generate_config.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)       36 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/ok_vqa/_ok_vqa.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)       90 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/ok_vqa/ok_vqa_val2014.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     2233 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/ok_vqa/utils.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.561057 lmms_eval-0.1.1/lmms_eval/tasks/pope/
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.561057 lmms_eval-0.1.1/lmms_eval/tasks/pope/__pycache__/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     3692 2024-03-08 12:51:01.000000 lmms_eval-0.1.1/lmms_eval/tasks/pope/__pycache__/utils.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      982 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/pope/pope.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     2991 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/pope/utils.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.561057 lmms_eval-0.1.1/lmms_eval/tasks/refcoco/
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.565057 lmms_eval-0.1.1/lmms_eval/tasks/refcoco/__pycache__/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     7031 2024-03-08 12:51:02.000000 lmms_eval-0.1.1/lmms_eval/tasks/refcoco/__pycache__/utils.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     1161 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/refcoco/_default_template_bbox_yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     1160 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/refcoco/_default_template_seg_yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      951 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/refcoco/_generate_config.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      179 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/refcoco/_refcoco.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)       98 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/refcoco/refcoco_bbox_test.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      100 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/refcoco/refcoco_bbox_testA.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      100 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/refcoco/refcoco_bbox_testB.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)       96 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/refcoco/refcoco_bbox_val.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)       95 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/refcoco/refcoco_seg_test.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)       97 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/refcoco/refcoco_seg_testA.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)       97 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/refcoco/refcoco_seg_testB.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)       93 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/refcoco/refcoco_seg_val.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     4122 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/refcoco/utils.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.565057 lmms_eval-0.1.1/lmms_eval/tasks/refcoco+/
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.565057 lmms_eval-0.1.1/lmms_eval/tasks/refcoco+/__pycache__/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     7032 2024-03-08 12:51:02.000000 lmms_eval-0.1.1/lmms_eval/tasks/refcoco+/__pycache__/utils.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     1165 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/refcoco+/_default_template_bbox_yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     1164 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/refcoco+/_default_template_seg_yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      939 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/refcoco+/_generate_config.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      147 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/refcoco+/_refcoco.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      102 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/refcoco+/refcoco+_bbox_testA.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      102 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/refcoco+/refcoco+_bbox_testB.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)       98 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/refcoco+/refcoco+_bbox_val.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)       99 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/refcoco+/refcoco+_seg_testA.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)       99 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/refcoco+/refcoco+_seg_testB.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)       95 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/refcoco+/refcoco+_seg_val.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     4122 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/refcoco+/utils.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.565057 lmms_eval-0.1.1/lmms_eval/tasks/refcocog/
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.565057 lmms_eval-0.1.1/lmms_eval/tasks/refcocog/__pycache__/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     7032 2024-03-08 12:51:02.000000 lmms_eval-0.1.1/lmms_eval/tasks/refcocog/__pycache__/utils.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     1162 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/refcocog/_default_template_bbox_yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     1161 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/refcocog/_default_template_seg_yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      919 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/refcocog/_generate_config.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      102 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/refcocog/_refcoco.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      100 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/refcocog/refcocog_bbox_test.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)       98 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/refcocog/refcocog_bbox_val.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)       97 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/refcocog/refcocog_seg_test.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)       95 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/refcocog/refcocog_seg_val.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     4122 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/refcocog/utils.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.565057 lmms_eval-0.1.1/lmms_eval/tasks/scienceqa/
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.565057 lmms_eval-0.1.1/lmms_eval/tasks/scienceqa/__pycache__/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     3153 2024-03-08 12:51:02.000000 lmms_eval-0.1.1/lmms_eval/tasks/scienceqa/__pycache__/utils.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      871 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/scienceqa/scienceqa.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)       59 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/scienceqa/scienceqa_full.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      871 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/scienceqa/scienceqa_img.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     1729 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/scienceqa/utils.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.565057 lmms_eval-0.1.1/lmms_eval/tasks/seedbench/
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.565057 lmms_eval-0.1.1/lmms_eval/tasks/seedbench/__pycache__/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     3612 2024-03-08 12:51:02.000000 lmms_eval-0.1.1/lmms_eval/tasks/seedbench/__pycache__/utils.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      936 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/seedbench/seedbench.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      528 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/seedbench/seedbench_ppl.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     1820 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/seedbench/utils.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.565057 lmms_eval-0.1.1/lmms_eval/tasks/seedbench_2/
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.565057 lmms_eval-0.1.1/lmms_eval/tasks/seedbench_2/__pycache__/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     3999 2024-03-08 12:51:01.000000 lmms_eval-0.1.1/lmms_eval/tasks/seedbench_2/__pycache__/utils.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     1716 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/seedbench_2/seedbench_2.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     2188 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/seedbench_2/utils.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.565057 lmms_eval-0.1.1/lmms_eval/tasks/stvqa/
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.565057 lmms_eval-0.1.1/lmms_eval/tasks/stvqa/__pycache__/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     1881 2024-03-08 12:51:02.000000 lmms_eval-0.1.1/lmms_eval/tasks/stvqa/__pycache__/utils.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      574 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/stvqa/stvqa.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      858 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/stvqa/utils.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.565057 lmms_eval-0.1.1/lmms_eval/tasks/textcaps/
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.565057 lmms_eval-0.1.1/lmms_eval/tasks/textcaps/__pycache__/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     8649 2024-03-08 12:51:02.000000 lmms_eval-0.1.1/lmms_eval/tasks/textcaps/__pycache__/utils.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      107 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/textcaps/_default_template_textcaps_yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)       57 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/textcaps/textcaps.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      796 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/textcaps/textcaps_test.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     1539 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/textcaps/textcaps_train.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     1504 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/textcaps/textcaps_val.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     5050 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/textcaps/utils.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.565057 lmms_eval-0.1.1/lmms_eval/tasks/textvqa/
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.565057 lmms_eval-0.1.1/lmms_eval/tasks/textvqa/__pycache__/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     4397 2024-03-08 12:51:02.000000 lmms_eval-0.1.1/lmms_eval/tasks/textvqa/__pycache__/utils.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      494 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/textvqa/_default_template_textvqa_yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)       49 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/textvqa/_textvqa.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      201 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/textvqa/textvqa_test.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      330 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/textvqa/textvqa_val.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     2362 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/textvqa/utils.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.565057 lmms_eval-0.1.1/lmms_eval/tasks/vizwiz_vqa/
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.565057 lmms_eval-0.1.1/lmms_eval/tasks/vizwiz_vqa/__pycache__/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     4259 2024-03-08 12:51:02.000000 lmms_eval-0.1.1/lmms_eval/tasks/vizwiz_vqa/__pycache__/utils.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      537 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/vizwiz_vqa/_default_template_vqa_yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      873 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/vizwiz_vqa/_generate_config.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)       58 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/vizwiz_vqa/_vizwiz_vqa.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     2290 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/vizwiz_vqa/utils.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      415 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/vizwiz_vqa/vizwiz_vqa_test.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      348 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/vizwiz_vqa/vizwiz_vqa_val.yaml
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.565057 lmms_eval-0.1.1/lmms_eval/tasks/vqav2/
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.565057 lmms_eval-0.1.1/lmms_eval/tasks/vqav2/__pycache__/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     5331 2024-03-08 12:51:02.000000 lmms_eval-0.1.1/lmms_eval/tasks/vqav2/__pycache__/utils.cpython-311.pyc
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      407 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/vqav2/_default_template_vqav2_yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)       43 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/vqav2/_vqav2.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     3031 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/vqav2/utils.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      257 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/vqav2/vqav2_test.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      275 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/tasks/vqav2/vqav2_val.yaml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)    28990 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/lmms_eval/utils.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.569057 lmms_eval-0.1.1/lmms_eval.egg-info/
--rw-r--r--   0 fypu      (1003) fypu      (1004)    16936 2024-03-14 06:39:03.000000 lmms_eval-0.1.1/lmms_eval.egg-info/PKG-INFO
--rw-rw-r--   0 fypu      (1003) fypu      (1004)    10614 2024-03-14 06:39:03.000000 lmms_eval-0.1.1/lmms_eval.egg-info/SOURCES.txt
--rw-rw-r--   0 fypu      (1003) fypu      (1004)        1 2024-03-14 06:39:03.000000 lmms_eval-0.1.1/lmms_eval.egg-info/dependency_links.txt
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      106 2024-03-14 06:39:03.000000 lmms_eval-0.1.1/lmms_eval.egg-info/entry_points.txt
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      431 2024-03-14 06:39:03.000000 lmms_eval-0.1.1/lmms_eval.egg-info/requires.txt
--rw-rw-r--   0 fypu      (1003) fypu      (1004)       10 2024-03-14 06:39:03.000000 lmms_eval-0.1.1/lmms_eval.egg-info/top_level.txt
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.569057 lmms_eval-0.1.1/miscs/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)        0 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/miscs/llava_result_check.md
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      490 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/miscs/repr_scripts.sh
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     3653 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/miscs/repr_torch_envs.txt
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     9457 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/miscs/scienceqa_id.txt
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      865 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/miscs/script.sh
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      963 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/miscs/test_llava.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      153 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/miscs/test_scienceqa.py
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     1653 2024-03-14 06:37:41.000000 lmms_eval-0.1.1/pyproject.toml
--rw-rw-r--   0 fypu      (1003) fypu      (1004)       38 2024-03-14 06:39:03.569057 lmms_eval-0.1.1/setup.cfg
--rw-rw-r--   0 fypu      (1003) fypu      (1004)      105 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/setup.py
-drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-03-14 06:39:03.569057 lmms_eval-0.1.1/tools/
--rw-rw-r--   0 fypu      (1003) fypu      (1004)     3242 2024-03-08 12:43:44.000000 lmms_eval-0.1.1/tools/make_hf_dataset.ipynb
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.883436 lmms_eval-0.1.2/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.863435 lmms_eval-0.1.2/.github/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      272 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/.github/issue_template.md
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      284 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/.github/pull_request_template.md
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.863435 lmms_eval-0.1.2/.github/workflows/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      386 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/.github/workflows/black.yml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      340 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/.gitignore
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      125 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 fypu      (1003) fypu      (1004)    17471 2024-04-16 16:41:59.883436 lmms_eval-0.1.2/PKG-INFO
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)    16003 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/README.md
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.863435 lmms_eval-0.1.2/docs/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      449 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/docs/README.md
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     2701 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/docs/commands.md
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     5277 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/docs/model_guide.md
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     6819 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/docs/task_guide.md
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      345 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/example_eval.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      740 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/llava_repr_requirements.txt
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.863435 lmms_eval-0.1.2/lmms_eval/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)        0 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/__init__.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)    13586 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/__main__.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.863435 lmms_eval-0.1.2/lmms_eval/api/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)        0 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/api/__init__.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     2025 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/api/filter.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      914 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/api/instance.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)    12174 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/api/metrics.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     7308 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/api/model.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     3896 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/api/registry.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     3548 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/api/samplers.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)    49329 2024-04-16 16:40:09.000000 lmms_eval-0.1.2/lmms_eval/api/task.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)    25312 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/evaluator.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.867435 lmms_eval-0.1.2/lmms_eval/filters/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     1585 2024-04-16 16:40:09.000000 lmms_eval-0.1.2/lmms_eval/filters/__init__.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      631 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/filters/decontamination.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     7614 2024-04-16 16:40:09.000000 lmms_eval-0.1.2/lmms_eval/filters/extraction.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     1584 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/filters/selection.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     1512 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/filters/transformation.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)    14819 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/logging_utils.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.867435 lmms_eval-0.1.2/lmms_eval/models/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      446 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/models/__init__.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)    12571 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/models/fuyu.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     5521 2024-04-16 16:40:09.000000 lmms_eval-0.1.2/lmms_eval/models/gpt4v.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     9664 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/models/instructblip.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)    20092 2024-04-16 16:40:09.000000 lmms_eval-0.1.2/lmms_eval/models/llava.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)    16125 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/models/llava_hf.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     9771 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/models/minicpm_v.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.867435 lmms_eval-0.1.2/lmms_eval/models/model_utils/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)        0 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/models/model_utils/__init__.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.867435 lmms_eval-0.1.2/lmms_eval/models/model_utils/qwen/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)    14392 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/models/model_utils/qwen/qwen_generate_utils.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)    13182 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/models/qwen_vl.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.867435 lmms_eval-0.1.2/lmms_eval/tasks/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     5453 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/__init__.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.867435 lmms_eval-0.1.2/lmms_eval/tasks/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     7690 2024-04-15 17:52:11.000000 lmms_eval-0.1.2/lmms_eval/tasks/__pycache__/__init__.cpython-311.pyc
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.867435 lmms_eval-0.1.2/lmms_eval/tasks/_task_utils/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.867435 lmms_eval-0.1.2/lmms_eval/tasks/_task_utils/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      777 2024-04-15 17:52:14.000000 lmms_eval-0.1.2/lmms_eval/tasks/_task_utils/__pycache__/file_utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     8354 2024-04-15 17:52:15.000000 lmms_eval-0.1.2/lmms_eval/tasks/_task_utils/__pycache__/vqa_eval_metric.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      244 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/_task_utils/file_utils.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)        0 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/_task_utils/gpt_eval_utils.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     6056 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/_task_utils/vqa_eval_metric.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.867435 lmms_eval-0.1.2/lmms_eval/tasks/ai2d/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.867435 lmms_eval-0.1.2/lmms_eval/tasks/ai2d/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     2615 2024-04-15 17:52:15.000000 lmms_eval-0.1.2/lmms_eval/tasks/ai2d/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      876 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/ai2d/ai2d.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     5098 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/ai2d/upload_ai2d.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     1271 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/ai2d/utils.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.867435 lmms_eval-0.1.2/lmms_eval/tasks/chartqa/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.867435 lmms_eval-0.1.2/lmms_eval/tasks/chartqa/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     3340 2024-04-15 17:52:15.000000 lmms_eval-0.1.2/lmms_eval/tasks/chartqa/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      844 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/chartqa/chartqa.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     5365 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/chartqa/upload_chartqa.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     2378 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/chartqa/utils.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.867435 lmms_eval-0.1.2/lmms_eval/tasks/cmmmu/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.867435 lmms_eval-0.1.2/lmms_eval/tasks/cmmmu/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)    23315 2024-04-15 17:52:14.000000 lmms_eval-0.1.2/lmms_eval/tasks/cmmmu/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)       44 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/cmmmu/_cmmmu.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      249 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/cmmmu/_default_template_cmmmu_yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      517 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/cmmmu/cmmmu_test.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      544 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/cmmmu/cmmmu_val.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)    17232 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/cmmmu/utils.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.867435 lmms_eval-0.1.2/lmms_eval/tasks/coco_cap/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.867435 lmms_eval-0.1.2/lmms_eval/tasks/coco_cap/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     9135 2024-04-15 17:52:14.000000 lmms_eval-0.1.2/lmms_eval/tasks/coco_cap/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)       69 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/coco_cap/coco2014_cap.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      764 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/coco_cap/coco2014_cap_test.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     1415 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/coco_cap/coco2014_cap_val.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)       69 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/coco_cap/coco2017_cap.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      748 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/coco_cap/coco2017_cap_test.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     1399 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/coco_cap/coco2017_cap_val.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      109 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/coco_cap/coco_cap.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     5273 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/coco_cap/utils.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.867435 lmms_eval-0.1.2/lmms_eval/tasks/docvqa/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.867435 lmms_eval-0.1.2/lmms_eval/tasks/docvqa/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     2005 2024-04-15 17:52:15.000000 lmms_eval-0.1.2/lmms_eval/tasks/docvqa/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      500 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/docvqa/_default_template_docvqa_yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)       46 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/docvqa/docvqa.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      263 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/docvqa/docvqa_test.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      160 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/docvqa/docvqa_val.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      992 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/docvqa/utils.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.867435 lmms_eval-0.1.2/lmms_eval/tasks/ferret/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.867435 lmms_eval-0.1.2/lmms_eval/tasks/ferret/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)    10423 2024-04-15 17:52:15.000000 lmms_eval-0.1.2/lmms_eval/tasks/ferret/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     1134 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/ferret/ferret.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     5228 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/ferret/rule.json
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     6956 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/ferret/utils.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.871435 lmms_eval-0.1.2/lmms_eval/tasks/flickr30k/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.871435 lmms_eval-0.1.2/lmms_eval/tasks/flickr30k/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     7574 2024-04-15 17:52:15.000000 lmms_eval-0.1.2/lmms_eval/tasks/flickr30k/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)       39 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/flickr30k/flickr30k.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     1403 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/flickr30k/flickr30k_test.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     4545 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/flickr30k/utils.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.871435 lmms_eval-0.1.2/lmms_eval/tasks/gqa/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.871435 lmms_eval-0.1.2/lmms_eval/tasks/gqa/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     1162 2024-04-15 17:52:15.000000 lmms_eval-0.1.2/lmms_eval/tasks/gqa/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      737 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/gqa/gqa.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      781 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/gqa/utils.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.871435 lmms_eval-0.1.2/lmms_eval/tasks/hallusion_bench/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.871435 lmms_eval-0.1.2/lmms_eval/tasks/hallusion_bench/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     7903 2024-04-15 17:52:14.000000 lmms_eval-0.1.2/lmms_eval/tasks/hallusion_bench/__pycache__/evaluate_hb.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)    15596 2024-04-15 17:52:14.000000 lmms_eval-0.1.2/lmms_eval/tasks/hallusion_bench/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     4862 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/hallusion_bench/evaluate_hb.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     1257 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/hallusion_bench/hallusion_bench_image.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)    12366 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/hallusion_bench/utils.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.871435 lmms_eval-0.1.2/lmms_eval/tasks/iconqa/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.871435 lmms_eval-0.1.2/lmms_eval/tasks/iconqa/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     3467 2024-04-15 17:52:14.000000 lmms_eval-0.1.2/lmms_eval/tasks/iconqa/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      816 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/iconqa/_default_template_docvqa_yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)       47 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/iconqa/iconqa.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)       75 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/iconqa/iconqa_test.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)       73 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/iconqa/iconqa_val.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     2162 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/iconqa/utils.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.871435 lmms_eval-0.1.2/lmms_eval/tasks/infovqa/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.871435 lmms_eval-0.1.2/lmms_eval/tasks/infovqa/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     1936 2024-04-15 17:52:14.000000 lmms_eval-0.1.2/lmms_eval/tasks/infovqa/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      423 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/infovqa/_default_template_infovqa_yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)       50 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/infovqa/infovqa.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      297 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/infovqa/infovqa_test.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      189 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/infovqa/infovqa_val.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      951 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/infovqa/utils.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.871435 lmms_eval-0.1.2/lmms_eval/tasks/llava-bench-coco/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.871435 lmms_eval-0.1.2/lmms_eval/tasks/llava-bench-coco/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)    10528 2024-04-15 17:52:14.000000 lmms_eval-0.1.2/lmms_eval/tasks/llava-bench-coco/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     1087 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/llava-bench-coco/llava-bench-coco.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     9098 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/llava-bench-coco/rule.json
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     6883 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/llava-bench-coco/utils.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.871435 lmms_eval-0.1.2/lmms_eval/tasks/llava-in-the-wild/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.871435 lmms_eval-0.1.2/lmms_eval/tasks/llava-in-the-wild/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)    10433 2024-04-15 17:52:14.000000 lmms_eval-0.1.2/lmms_eval/tasks/llava-in-the-wild/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     1115 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/llava-in-the-wild/llava-in-the-wild.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     9098 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/llava-in-the-wild/rule.json
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     6851 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/llava-in-the-wild/utils.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.871435 lmms_eval-0.1.2/lmms_eval/tasks/mathvista/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.871435 lmms_eval-0.1.2/lmms_eval/tasks/mathvista/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)    20278 2024-04-15 17:52:15.000000 lmms_eval-0.1.2/lmms_eval/tasks/mathvista/__pycache__/mathvista_evals.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     8208 2024-04-15 17:52:15.000000 lmms_eval-0.1.2/lmms_eval/tasks/mathvista/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      148 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/mathvista/mathvista.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)    18971 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/mathvista/mathvista_evals.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      775 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/mathvista/mathvista_test.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      789 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/mathvista/mathvista_testmini.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     5022 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/mathvista/utils.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.871435 lmms_eval-0.1.2/lmms_eval/tasks/mmbench/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.871435 lmms_eval-0.1.2/lmms_eval/tasks/mmbench/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     5722 2024-04-15 17:52:15.000000 lmms_eval-0.1.2/lmms_eval/tasks/mmbench/__pycache__/cc_utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     6869 2024-04-15 17:52:15.000000 lmms_eval-0.1.2/lmms_eval/tasks/mmbench/__pycache__/cn_utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     6909 2024-04-15 17:52:15.000000 lmms_eval-0.1.2/lmms_eval/tasks/mmbench/__pycache__/en_utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)    18219 2024-04-15 17:52:15.000000 lmms_eval-0.1.2/lmms_eval/tasks/mmbench/__pycache__/mmbench_evals.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      621 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/mmbench/_default_template_mmbench_cn_yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      678 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/mmbench/_default_template_mmbench_en_yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     3750 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/mmbench/cc_utils.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     4589 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/mmbench/cn_utils.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     4550 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/mmbench/en_utils.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      228 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/mmbench/mmbench.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      974 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/mmbench/mmbench_cc.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      190 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/mmbench/mmbench_cn.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      338 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/mmbench/mmbench_cn_dev.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      212 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/mmbench/mmbench_cn_test.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      175 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/mmbench/mmbench_en.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      346 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/mmbench/mmbench_en_dev.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      214 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/mmbench/mmbench_en_test.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)    12180 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/mmbench/mmbench_evals.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.871435 lmms_eval-0.1.2/lmms_eval/tasks/mme/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.871435 lmms_eval-0.1.2/lmms_eval/tasks/mme/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     5101 2024-04-15 17:52:15.000000 lmms_eval-0.1.2/lmms_eval/tasks/mme/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     1105 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/mme/mme.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     3925 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/mme/utils.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.875435 lmms_eval-0.1.2/lmms_eval/tasks/mmmu/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.875435 lmms_eval-0.1.2/lmms_eval/tasks/mmmu/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)    19955 2024-04-15 17:52:14.000000 lmms_eval-0.1.2/lmms_eval/tasks/mmmu/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)       41 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/mmmu/mmmu.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      701 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/mmmu/mmmu_test.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      684 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/mmmu/mmmu_val.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)    16383 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/mmmu/utils.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.875435 lmms_eval-0.1.2/lmms_eval/tasks/mmvet/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.875435 lmms_eval-0.1.2/lmms_eval/tasks/mmvet/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)    11881 2024-04-15 17:52:15.000000 lmms_eval-0.1.2/lmms_eval/tasks/mmvet/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      768 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/mmvet/mmvet.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     9027 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/mmvet/utils.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.875435 lmms_eval-0.1.2/lmms_eval/tasks/multidocvqa/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.875435 lmms_eval-0.1.2/lmms_eval/tasks/multidocvqa/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     8605 2024-04-15 17:52:15.000000 lmms_eval-0.1.2/lmms_eval/tasks/multidocvqa/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)       62 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/multidocvqa/multidocvqa.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      648 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/multidocvqa/multidocvqa_test.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      750 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/multidocvqa/multidocvqa_val.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     3903 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/multidocvqa/utils.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.875435 lmms_eval-0.1.2/lmms_eval/tasks/nocaps/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.875435 lmms_eval-0.1.2/lmms_eval/tasks/nocaps/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     8769 2024-04-15 17:52:14.000000 lmms_eval-0.1.2/lmms_eval/tasks/nocaps/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      109 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/nocaps/_default_template_nocaps_yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)       51 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/nocaps/nocaps.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      792 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/nocaps/nocaps_test.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     1479 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/nocaps/nocaps_val.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     5255 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/nocaps/utils.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.875435 lmms_eval-0.1.2/lmms_eval/tasks/ocrbench/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.875435 lmms_eval-0.1.2/lmms_eval/tasks/ocrbench/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     7180 2024-04-15 17:52:14.000000 lmms_eval-0.1.2/lmms_eval/tasks/ocrbench/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      569 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/ocrbench/ocrbench.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     2935 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/ocrbench/upload_ocrbench.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     5460 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/ocrbench/utils.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.875435 lmms_eval-0.1.2/lmms_eval/tasks/ok_vqa/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.875435 lmms_eval-0.1.2/lmms_eval/tasks/ok_vqa/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     4152 2024-04-15 17:52:15.000000 lmms_eval-0.1.2/lmms_eval/tasks/ok_vqa/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      768 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/ok_vqa/_default_template_vqa_yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      833 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/ok_vqa/_generate_config.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)       36 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/ok_vqa/_ok_vqa.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)       90 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/ok_vqa/ok_vqa_val2014.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     2233 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/ok_vqa/utils.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.875435 lmms_eval-0.1.2/lmms_eval/tasks/olympiadbench/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.875435 lmms_eval-0.1.2/lmms_eval/tasks/olympiadbench/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     4344 2024-04-15 17:52:14.000000 lmms_eval-0.1.2/lmms_eval/tasks/olympiadbench/__pycache__/cn_utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     4445 2024-04-15 17:52:15.000000 lmms_eval-0.1.2/lmms_eval/tasks/olympiadbench/__pycache__/en_utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)    14656 2024-04-15 17:52:14.000000 lmms_eval-0.1.2/lmms_eval/tasks/olympiadbench/__pycache__/olympiadbench_evals.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     5336 2024-03-25 16:26:45.000000 lmms_eval-0.1.2/lmms_eval/tasks/olympiadbench/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     2519 2024-04-16 16:40:09.000000 lmms_eval-0.1.2/lmms_eval/tasks/olympiadbench/cn_utils.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     2659 2024-04-16 16:40:09.000000 lmms_eval-0.1.2/lmms_eval/tasks/olympiadbench/en_utils.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      102 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/olympiadbench/olympiadbench.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)    12660 2024-04-16 16:40:09.000000 lmms_eval-0.1.2/lmms_eval/tasks/olympiadbench/olympiadbench_evals.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      691 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/olympiadbench/olympiadbench_test_cn.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      691 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/olympiadbench/olympiadbench_test_en.yaml
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.875435 lmms_eval-0.1.2/lmms_eval/tasks/pope/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.875435 lmms_eval-0.1.2/lmms_eval/tasks/pope/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     3692 2024-04-15 17:52:14.000000 lmms_eval-0.1.2/lmms_eval/tasks/pope/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      982 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/pope/pope.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     2991 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/pope/utils.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.875435 lmms_eval-0.1.2/lmms_eval/tasks/realworldqa/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.875435 lmms_eval-0.1.2/lmms_eval/tasks/realworldqa/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     6734 2024-04-15 17:52:15.000000 lmms_eval-0.1.2/lmms_eval/tasks/realworldqa/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      961 2024-04-16 16:40:09.000000 lmms_eval-0.1.2/lmms_eval/tasks/realworldqa/realworldqa.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     4775 2024-04-16 16:40:09.000000 lmms_eval-0.1.2/lmms_eval/tasks/realworldqa/utils.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.875435 lmms_eval-0.1.2/lmms_eval/tasks/refcoco/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.879435 lmms_eval-0.1.2/lmms_eval/tasks/refcoco/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     7031 2024-04-15 17:52:15.000000 lmms_eval-0.1.2/lmms_eval/tasks/refcoco/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     1161 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/refcoco/_default_template_bbox_yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     1160 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/refcoco/_default_template_seg_yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      951 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/refcoco/_generate_config.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      179 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/refcoco/_refcoco.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)       98 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/refcoco/refcoco_bbox_test.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      100 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/refcoco/refcoco_bbox_testA.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      100 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/refcoco/refcoco_bbox_testB.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)       96 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/refcoco/refcoco_bbox_val.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)       95 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/refcoco/refcoco_seg_test.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)       97 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/refcoco/refcoco_seg_testA.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)       97 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/refcoco/refcoco_seg_testB.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)       93 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/refcoco/refcoco_seg_val.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     4122 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/refcoco/utils.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.879435 lmms_eval-0.1.2/lmms_eval/tasks/refcoco+/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.879435 lmms_eval-0.1.2/lmms_eval/tasks/refcoco+/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     7032 2024-04-15 17:52:15.000000 lmms_eval-0.1.2/lmms_eval/tasks/refcoco+/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     1165 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/refcoco+/_default_template_bbox_yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     1164 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/refcoco+/_default_template_seg_yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      939 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/refcoco+/_generate_config.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      147 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/refcoco+/_refcoco.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      102 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/refcoco+/refcoco+_bbox_testA.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      102 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/refcoco+/refcoco+_bbox_testB.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)       98 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/refcoco+/refcoco+_bbox_val.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)       99 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/refcoco+/refcoco+_seg_testA.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)       99 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/refcoco+/refcoco+_seg_testB.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)       95 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/refcoco+/refcoco+_seg_val.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     4122 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/refcoco+/utils.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.879435 lmms_eval-0.1.2/lmms_eval/tasks/refcocog/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.879435 lmms_eval-0.1.2/lmms_eval/tasks/refcocog/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     7032 2024-04-15 17:52:15.000000 lmms_eval-0.1.2/lmms_eval/tasks/refcocog/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     1162 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/refcocog/_default_template_bbox_yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     1161 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/refcocog/_default_template_seg_yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      919 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/refcocog/_generate_config.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      102 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/refcocog/_refcoco.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      100 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/refcocog/refcocog_bbox_test.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)       98 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/refcocog/refcocog_bbox_val.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)       97 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/refcocog/refcocog_seg_test.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)       95 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/refcocog/refcocog_seg_val.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     4122 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/refcocog/utils.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.879435 lmms_eval-0.1.2/lmms_eval/tasks/scienceqa/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.879435 lmms_eval-0.1.2/lmms_eval/tasks/scienceqa/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     3153 2024-04-15 17:52:15.000000 lmms_eval-0.1.2/lmms_eval/tasks/scienceqa/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      871 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/scienceqa/scienceqa.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)       59 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/scienceqa/scienceqa_full.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      871 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/scienceqa/scienceqa_img.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     1729 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/scienceqa/utils.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.879435 lmms_eval-0.1.2/lmms_eval/tasks/seedbench/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.879435 lmms_eval-0.1.2/lmms_eval/tasks/seedbench/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     3612 2024-04-15 17:52:15.000000 lmms_eval-0.1.2/lmms_eval/tasks/seedbench/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      936 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/seedbench/seedbench.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      528 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/seedbench/seedbench_ppl.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     1820 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/seedbench/utils.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.879435 lmms_eval-0.1.2/lmms_eval/tasks/seedbench_2/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.879435 lmms_eval-0.1.2/lmms_eval/tasks/seedbench_2/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     3999 2024-04-15 17:52:14.000000 lmms_eval-0.1.2/lmms_eval/tasks/seedbench_2/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     1716 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/seedbench_2/seedbench_2.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     2188 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/seedbench_2/utils.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.879435 lmms_eval-0.1.2/lmms_eval/tasks/stvqa/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.879435 lmms_eval-0.1.2/lmms_eval/tasks/stvqa/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     1881 2024-04-15 17:52:15.000000 lmms_eval-0.1.2/lmms_eval/tasks/stvqa/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      574 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/stvqa/stvqa.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      858 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/stvqa/utils.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.879435 lmms_eval-0.1.2/lmms_eval/tasks/textcaps/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.879435 lmms_eval-0.1.2/lmms_eval/tasks/textcaps/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     8649 2024-04-15 17:52:15.000000 lmms_eval-0.1.2/lmms_eval/tasks/textcaps/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      107 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/textcaps/_default_template_textcaps_yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)       57 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/textcaps/textcaps.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      796 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/textcaps/textcaps_test.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     1539 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/textcaps/textcaps_train.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     1504 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/textcaps/textcaps_val.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     5050 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/textcaps/utils.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.879435 lmms_eval-0.1.2/lmms_eval/tasks/textvqa/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.879435 lmms_eval-0.1.2/lmms_eval/tasks/textvqa/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     4397 2024-04-15 17:52:15.000000 lmms_eval-0.1.2/lmms_eval/tasks/textvqa/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      494 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/textvqa/_default_template_textvqa_yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)       49 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/textvqa/_textvqa.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      201 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/textvqa/textvqa_test.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      330 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/textvqa/textvqa_val.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     2362 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/textvqa/utils.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.879435 lmms_eval-0.1.2/lmms_eval/tasks/vizwiz_vqa/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.879435 lmms_eval-0.1.2/lmms_eval/tasks/vizwiz_vqa/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     4259 2024-04-15 17:52:15.000000 lmms_eval-0.1.2/lmms_eval/tasks/vizwiz_vqa/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      537 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/vizwiz_vqa/_default_template_vqa_yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      873 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/vizwiz_vqa/_generate_config.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)       58 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/vizwiz_vqa/_vizwiz_vqa.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     2290 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/vizwiz_vqa/utils.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      415 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/vizwiz_vqa/vizwiz_vqa_test.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      348 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/vizwiz_vqa/vizwiz_vqa_val.yaml
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.879435 lmms_eval-0.1.2/lmms_eval/tasks/vqav2/
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.883436 lmms_eval-0.1.2/lmms_eval/tasks/vqav2/__pycache__/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     5331 2024-04-15 17:52:15.000000 lmms_eval-0.1.2/lmms_eval/tasks/vqav2/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      407 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/vqav2/_default_template_vqav2_yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)       43 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/vqav2/_vqav2.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     3031 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/vqav2/utils.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      257 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/vqav2/vqav2_test.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      275 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/tasks/vqav2/vqav2_val.yaml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)    29051 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/lmms_eval/utils.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.883436 lmms_eval-0.1.2/lmms_eval.egg-info/
+-rw-r--r--   0 fypu      (1003) fypu      (1004)    17471 2024-04-16 16:41:59.000000 lmms_eval-0.1.2/lmms_eval.egg-info/PKG-INFO
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)    11655 2024-04-16 16:41:59.000000 lmms_eval-0.1.2/lmms_eval.egg-info/SOURCES.txt
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)        1 2024-04-16 16:41:59.000000 lmms_eval-0.1.2/lmms_eval.egg-info/dependency_links.txt
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      106 2024-04-16 16:41:59.000000 lmms_eval-0.1.2/lmms_eval.egg-info/entry_points.txt
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      423 2024-04-16 16:41:59.000000 lmms_eval-0.1.2/lmms_eval.egg-info/requires.txt
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)       10 2024-04-16 16:41:59.000000 lmms_eval-0.1.2/lmms_eval.egg-info/top_level.txt
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.883436 lmms_eval-0.1.2/miscs/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)        0 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/miscs/llava_result_check.md
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      604 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/miscs/repr_scripts.sh
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     3653 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/miscs/repr_torch_envs.txt
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     9457 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/miscs/scienceqa_id.txt
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      865 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/miscs/script.sh
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      963 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/miscs/test_llava.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      153 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/miscs/test_scienceqa.py
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     1645 2024-04-16 16:40:52.000000 lmms_eval-0.1.2/pyproject.toml
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)       38 2024-04-16 16:41:59.883436 lmms_eval-0.1.2/setup.cfg
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)      105 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/setup.py
+drwxrwxr-x   0 fypu      (1003) fypu      (1004)        0 2024-04-16 16:41:59.883436 lmms_eval-0.1.2/tools/
+-rw-rw-r--   0 fypu      (1003) fypu      (1004)     3242 2024-04-15 17:51:32.000000 lmms_eval-0.1.2/tools/make_hf_dataset.ipynb
```

### Comparing `lmms_eval-0.1.1/PKG-INFO` & `lmms_eval-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6c6d 6d73  : 2.1.Name: lmms
 00000020: 5f65 7661 6c0a 5665 7273 696f 6e3a 2030  _eval.Version: 0
-00000030: 2e31 2e31 0a53 756d 6d61 7279 3a20 4120  .1.1.Summary: A 
+00000030: 2e31 2e32 0a53 756d 6d61 7279 3a20 4120  .1.2.Summary: A 
 00000040: 6672 616d 6577 6f72 6b20 666f 7220 6576  framework for ev
 00000050: 616c 7561 7469 6e67 206c 6172 6765 206d  aluating large m
 00000060: 756c 7469 2d6d 6f64 616c 6974 7920 6c61  ulti-modality la
 00000070: 6e67 7561 6765 206d 6f64 656c 730a 4175  nguage models.Au
 00000080: 7468 6f72 2d65 6d61 696c 3a20 4c4d 4d4d  thor-email: LMMM
 00000090: 732d 4c61 6220 4576 616c 7561 7469 6f6e  s-Lab Evaluation
 000000a0: 2054 6561 6d20 3c6c 6d6d 735f 6576 616c   Team <lmms_eval
@@ -61,999 +61,1032 @@
 000003c0: 312e 380a 5265 7175 6972 6573 2d44 6973  1.8.Requires-Dis
 000003d0: 743a 206f 7065 6e61 693e 3d31 2e30 2e30  t: openai>=1.0.0
 000003e0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
 000003f0: 7079 636f 636f 6576 616c 6361 700a 5265  pycocoevalcap.Re
 00000400: 7175 6972 6573 2d44 6973 743a 2074 7164  quires-Dist: tqd
 00000410: 6d2d 6d75 6c74 6970 726f 6365 7373 0a52  m-multiprocess.R
 00000420: 6571 7569 7265 732d 4469 7374 3a20 7472  equires-Dist: tr
-00000430: 616e 7366 6f72 6d65 7273 3d3d 342e 3337  ansformers==4.37
-00000440: 2e32 0a52 6571 7569 7265 732d 4469 7374  .2.Requires-Dist
-00000450: 3a20 7a73 7461 6e64 6172 640a 5265 7175  : zstandard.Requ
-00000460: 6972 6573 2d44 6973 743a 2070 696c 6c6f  ires-Dist: pillo
-00000470: 770a 5265 7175 6972 6573 2d44 6973 743a  w.Requires-Dist:
-00000480: 2070 7979 616d 6c0a 5265 7175 6972 6573   pyyaml.Requires
-00000490: 2d44 6973 743a 2073 796d 7079 0a52 6571  -Dist: sympy.Req
-000004a0: 7569 7265 732d 4469 7374 3a20 6d70 6d61  uires-Dist: mpma
-000004b0: 7468 0a52 6571 7569 7265 732d 4469 7374  th.Requires-Dist
-000004c0: 3a20 4a69 6e6a 6132 0a52 6571 7569 7265  : Jinja2.Require
-000004d0: 732d 4469 7374 3a20 6f70 656e 7079 786c  s-Dist: openpyxl
-000004e0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000004f0: 4c65 7665 6e73 6874 6569 6e0a 5265 7175  Levenshtein.Requ
-00000500: 6972 6573 2d44 6973 743a 2068 665f 7472  ires-Dist: hf_tr
-00000510: 616e 7366 6572 0a52 6571 7569 7265 732d  ansfer.Requires-
-00000520: 4469 7374 3a20 7465 6e61 6369 7479 0a52  Dist: tenacity.R
-00000530: 6571 7569 7265 732d 4469 7374 3a20 7761  equires-Dist: wa
-00000540: 6e64 623e 3d30 2e31 362e 300a 5265 7175  ndb>=0.16.0.Requ
-00000550: 6972 6573 2d44 6973 743a 2074 7261 6e73  ires-Dist: trans
-00000560: 666f 726d 6572 732d 7374 7265 616d 2d67  formers-stream-g
-00000570: 656e 6572 6174 6f72 0a52 6571 7569 7265  enerator.Require
-00000580: 732d 4469 7374 3a20 7469 6b74 6f6b 656e  s-Dist: tiktoken
-00000590: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000005a0: 7072 652d 636f 6d6d 6974 0a52 6571 7569  pre-commit.Requi
-000005b0: 7265 732d 4469 7374 3a20 7079 6461 6e74  res-Dist: pydant
-000005c0: 6963 0a0a 3c70 2061 6c69 676e 3d22 6365  ic..<p align="ce
-000005d0: 6e74 6572 2220 7769 6474 683d 2231 3030  nter" width="100
-000005e0: 2522 3e0a 3c69 6d67 2073 7263 3d22 6874  %">.<img src="ht
-000005f0: 7470 733a 2f2f 692e 706f 7374 696d 672e  tps://i.postimg.
-00000600: 6363 2f67 3051 5267 4d56 762f 5758 3230  cc/g0QRgMVv/WX20
-00000610: 3234 3032 3238 2d31 3133 3333 372d 3278  240228-113337-2x
-00000620: 2e70 6e67 2220 2077 6964 7468 3d22 3130  .png"  width="10
-00000630: 3025 2220 6865 6967 6874 3d22 3730 2522  0%" height="70%"
-00000640: 3e0a 3c2f 703e 0a0a 2320 5468 6520 4576  >.</p>..# The Ev
-00000650: 616c 7561 7469 6f6e 2053 7569 7465 206f  aluation Suite o
-00000660: 6620 4c61 7267 6520 4d75 6c74 696d 6f64  f Large Multimod
-00000670: 616c 204d 6f64 656c 7320 0a0a 3e20 4163  al Models ..> Ac
-00000680: 6365 6c65 7261 7469 6e67 2074 6865 2064  celerating the d
-00000690: 6576 656c 6f70 6d65 6e74 206f 6620 6c61  evelopment of la
-000006a0: 7267 6520 6d75 6c74 696d 6f64 616c 206d  rge multimodal m
-000006b0: 6f64 656c 7320 284c 4d4d 7329 2077 6974  odels (LMMs) wit
-000006c0: 6820 606c 6d6d 732d 6576 616c 600a 0af0  h `lmms-eval`...
-000006d0: 9f8f a020 5b48 6f6d 6570 6167 655d 2868  ... [Homepage](h
-000006e0: 7474 7073 3a2f 2f6c 6d6d 732d 6c61 622e  ttps://lmms-lab.
-000006f0: 6769 7468 7562 2e69 6f2f 2920 7c20 20f0  github.io/) |  .
-00000700: 9f8e 8920 5b42 6c6f 675d 2868 7474 7073  ... [Blog](https
-00000710: 3a2f 2f6c 6d6d 732d 6c61 622e 6769 7468  ://lmms-lab.gith
-00000720: 7562 2e69 6f2f 6c6d 6d73 2d65 7661 6c2d  ub.io/lmms-eval-
-00000730: 626c 6f67 2f6c 6d6d 732d 6576 616c 2d30  blog/lmms-eval-0
-00000740: 2e31 2f29 207c 20f0 9f93 9a20 5b44 6f63  .1/) | .... [Doc
-00000750: 756d 656e 7461 7469 6f6e 5d28 646f 6373  umentation](docs
-00000760: 2f52 4541 444d 452e 6d64 2920 7c20 f09f  /README.md) | ..
-00000770: a497 205b 4875 6767 696e 6766 6163 6520  .. [Huggingface 
-00000780: 4461 7461 7365 7473 5d28 6874 7470 733a  Datasets](https:
-00000790: 2f2f 6875 6767 696e 6766 6163 652e 636f  //huggingface.co
-000007a0: 2f6c 6d6d 732d 6c61 6229 0a0a 496e 2061  /lmms-lab)..In a
-000007b0: 6e20 6572 6120 7768 6572 6520 7065 6f70  n era where peop
-000007c0: 6c65 2070 7572 7375 6520 4147 4920 2841  le pursue AGI (A
-000007d0: 7274 6966 6963 6961 6c20 4765 6e65 7261  rtificial Genera
-000007e0: 6c20 496e 7465 6c6c 6967 656e 6365 2920  l Intelligence) 
-000007f0: 7769 7468 2074 6865 207a 6561 6c20 616b  with the zeal ak
-00000800: 696e 2074 6f20 3139 3630 7320 6d6f 6f6e  in to 1960s moon
-00000810: 206c 616e 6469 6e67 206d 6973 7369 6f6e   landing mission
-00000820: 2e20 0a45 7661 6c75 6174 696e 6720 7468  . .Evaluating th
-00000830: 6520 636f 7265 206f 6620 4147 492c 2074  e core of AGI, t
-00000840: 6865 206c 6172 6765 206c 616e 6775 6167  he large languag
-00000850: 6520 6d6f 6465 6c73 2028 4c4c 4d73 2920  e models (LLMs) 
-00000860: 616e 6420 6c61 7267 6520 6d75 6c74 696d  and large multim
-00000870: 6f64 616c 206d 6f64 656c 7320 284c 4d4d  odal models (LMM
-00000880: 7329 2077 6974 6820 756e 7072 6563 6564  s) with unpreced
-00000890: 656e 7465 6420 6361 7061 6269 6c69 7469  ented capabiliti
-000008a0: 6573 2074 6861 7420 6361 6e20 756e 6465  es that can unde
-000008b0: 7273 7461 6e64 2c20 6c65 6172 6e2c 2061  rstand, learn, a
-000008c0: 6e64 2069 6e74 6572 6163 7420 6163 726f  nd interact acro
-000008d0: 7373 2061 2062 726f 6164 2072 616e 6765  ss a broad range
-000008e0: 206f 6620 6875 6d61 6e20 7461 736b 732c   of human tasks,
-000008f0: 2068 6173 2062 6563 6f6d 6520 6120 7069   has become a pi
-00000900: 766f 7461 6c20 6368 616c 6c65 6e67 652e  votal challenge.
-00000910: 0a0a 546f 2073 7572 6d6f 756e 7420 7468  ..To surmount th
-00000920: 6973 2c20 6120 6272 6f61 6420 7370 6563  is, a broad spec
-00000930: 7472 756d 206f 6620 6576 616c 7561 7469  trum of evaluati
-00000940: 6f6e 2064 6174 6173 6574 7320 6973 2070  on datasets is p
-00000950: 726f 706f 7365 6420 616e 6420 7573 6564  roposed and used
-00000960: 2074 6f20 6173 7365 7373 206d 6f64 656c   to assess model
-00000970: 2063 6170 6162 696c 6974 6965 7320 6163   capabilities ac
-00000980: 726f 7373 2076 6172 696f 7573 2064 696d  ross various dim
-00000990: 656e 7369 6f6e 732c 2063 7265 6174 696e  ensions, creatin
-000009a0: 6720 6120 636f 6d70 7265 6865 6e73 6976  g a comprehensiv
-000009b0: 6520 6361 7061 6269 6c69 7479 2063 6861  e capability cha
-000009c0: 7274 2074 6861 7420 7265 7665 616c 7320  rt that reveals 
-000009d0: 7468 6520 7472 7565 2070 6572 666f 726d  the true perform
-000009e0: 616e 6365 206f 6620 6d6f 6465 6c73 2e20  ance of models. 
-000009f0: 486f 7765 7665 722c 2065 7661 6c75 6174  However, evaluat
-00000a00: 696f 6e20 6f66 206d 6f64 656c 7320 6861  ion of models ha
-00000a10: 7320 6265 636f 6d65 2071 7569 7465 2068  s become quite h
-00000a20: 6172 6420 7369 6e63 6520 7468 6572 6520  ard since there 
-00000a30: 6172 6520 636f 756e 746c 6573 7320 6576  are countless ev
-00000a40: 616c 7561 7469 6f6e 2062 656e 6368 6d61  aluation benchma
-00000a50: 726b 7320 616e 6420 6461 7461 7365 7473  rks and datasets
-00000a60: 206f 7267 616e 697a 6564 2069 6e20 7661   organized in va
-00000a70: 7269 6f75 7320 7761 7973 2c20 7363 6174  rious ways, scat
-00000a80: 7465 7265 6420 6163 726f 7373 2074 6865  tered across the
-00000a90: 2069 6e74 6572 6e65 742c 2073 6c65 6570   internet, sleep
-00000aa0: 696e 6720 696e 2073 6f6d 6562 6f64 7927  ing in somebody'
-00000ab0: 7320 476f 6f67 6c65 2044 7269 7665 2c20  s Google Drive, 
-00000ac0: 4472 6f70 626f 782c 2061 6e64 206f 7468  Dropbox, and oth
-00000ad0: 6572 2077 6562 7369 7465 7320 686f 7374  er websites host
-00000ae0: 6564 2062 7920 7363 686f 6f6c 7320 6f72  ed by schools or
-00000af0: 2072 6573 6561 7263 6820 6c61 6273 2e0a   research labs..
-00000b00: 0a49 6e20 7468 6520 6669 656c 6420 6f66  .In the field of
-00000b10: 206c 616e 6775 6167 6520 6d6f 6465 6c73   language models
-00000b20: 2c20 7468 6572 6520 6861 7320 6265 656e  , there has been
-00000b30: 2061 2076 616c 7561 626c 6520 7072 6563   a valuable prec
-00000b40: 6564 656e 7420 7365 7420 6279 2074 6865  edent set by the
-00000b50: 2077 6f72 6b20 6f66 205b 6c6d 2d65 7661   work of [lm-eva
-00000b60: 6c75 6174 696f 6e2d 6861 726e 6573 735d  luation-harness]
-00000b70: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000b80: 636f 6d2f 456c 6575 7468 6572 4149 2f6c  com/EleutherAI/l
-00000b90: 6d2d 6576 616c 7561 7469 6f6e 2d68 6172  m-evaluation-har
-00000ba0: 6e65 7373 292e 2054 6865 7920 6f66 6665  ness). They offe
-00000bb0: 7220 696e 7465 6772 6174 6564 2064 6174  r integrated dat
-00000bc0: 6120 616e 6420 6d6f 6465 6c20 696e 7465  a and model inte
-00000bd0: 7266 6163 6573 2c20 656e 6162 6c69 6e67  rfaces, enabling
-00000be0: 2072 6170 6964 2065 7661 6c75 6174 696f   rapid evaluatio
-00000bf0: 6e20 6f66 206c 616e 6775 6167 6520 6d6f  n of language mo
-00000c00: 6465 6c73 2061 6e64 2073 6572 7669 6e67  dels and serving
-00000c10: 2061 7320 7468 6520 6261 636b 656e 6420   as the backend 
-00000c20: 7375 7070 6f72 7420 6672 616d 6577 6f72  support framewor
-00000c30: 6b20 666f 7220 7468 6520 5b6f 7065 6e2d  k for the [open-
-00000c40: 6c6c 6d2d 6c65 6164 6572 626f 6172 645d  llm-leaderboard]
-00000c50: 2868 7474 7073 3a2f 2f68 7567 6769 6e67  (https://hugging
-00000c60: 6661 6365 2e63 6f2f 7370 6163 6573 2f48  face.co/spaces/H
-00000c70: 7567 6769 6e67 4661 6365 4834 2f6f 7065  uggingFaceH4/ope
-00000c80: 6e5f 6c6c 6d5f 6c65 6164 6572 626f 6172  n_llm_leaderboar
-00000c90: 6429 2c20 616e 6420 6861 7320 6772 6164  d), and has grad
-00000ca0: 7561 6c6c 7920 6265 636f 6d65 2074 6865  ually become the
-00000cb0: 2075 6e64 6572 6c79 696e 6720 6563 6f73   underlying ecos
-00000cc0: 7973 7465 6d20 6f66 2074 6865 2065 7261  ystem of the era
-00000cd0: 206f 6620 666f 756e 6461 7469 6f6e 206d   of foundation m
-00000ce0: 6f64 656c 732e 0a0a 486f 7765 7665 722c  odels...However,
-00000cf0: 2074 686f 7567 6820 7468 6572 6520 6172   though there ar
-00000d00: 6520 6d61 6e79 206e 6577 2065 7661 6c75  e many new evalu
-00000d10: 6174 696f 6e20 6461 7461 7365 7473 2061  ation datasets a
-00000d20: 7265 2072 6563 656e 746c 7920 7072 6f70  re recently prop
-00000d30: 6f73 6564 2c20 7468 6520 6566 6669 6369  osed, the effici
-00000d40: 656e 7420 6576 616c 7561 7469 6f6e 2070  ent evaluation p
-00000d50: 6970 656c 696e 6520 6f66 204c 4d4d 2069  ipeline of LMM i
-00000d60: 7320 7374 696c 6c20 696e 2069 7473 2069  s still in its i
-00000d70: 6e66 616e 6379 2c20 616e 6420 7468 6572  nfancy, and ther
-00000d80: 6520 6973 206e 6f20 756e 6966 6965 6420  e is no unified 
-00000d90: 6576 616c 7561 7469 6f6e 2066 7261 6d65  evaluation frame
-00000da0: 776f 726b 2074 6861 7420 6361 6e20 6265  work that can be
-00000db0: 2075 7365 6420 746f 2065 7661 6c75 6174   used to evaluat
-00000dc0: 6520 4c4d 4d20 6163 726f 7373 2061 2077  e LMM across a w
-00000dd0: 6964 6520 7261 6e67 6520 6f66 2064 6174  ide range of dat
-00000de0: 6173 6574 732e 2054 6f20 6164 6472 6573  asets. To addres
-00000df0: 7320 7468 6973 2063 6861 6c6c 656e 6765  s this challenge
-00000e00: 2c20 7765 2069 6e74 726f 6475 6365 202a  , we introduce *
-00000e10: 2a6c 6d6d 732d 6576 616c 2a2a 2c20 616e  *lmms-eval**, an
-00000e20: 2065 7661 6c75 6174 696f 6e20 6672 616d   evaluation fram
-00000e30: 6577 6f72 6b20 6d65 7469 6375 6c6f 7573  ework meticulous
-00000e40: 6c79 2063 7261 6674 6564 2066 6f72 2063  ly crafted for c
-00000e50: 6f6e 7369 7374 656e 7420 616e 6420 6566  onsistent and ef
-00000e60: 6669 6369 656e 7420 6576 616c 7561 7469  ficient evaluati
-00000e70: 6f6e 206f 6620 4c4d 4d2e 0a0a 5765 2068  on of LMM...We h
-00000e80: 756d 626c 7920 6f62 736f 7262 6564 2074  umbly obsorbed t
-00000e90: 6865 2065 7871 7569 7369 7465 2061 6e64  he exquisite and
-00000ea0: 2065 6666 6963 6965 6e74 2064 6573 6967   efficient desig
-00000eb0: 6e20 6f66 205b 6c6d 2d65 7661 6c75 6174  n of [lm-evaluat
-00000ec0: 696f 6e2d 6861 726e 6573 735d 2868 7474  ion-harness](htt
-00000ed0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000ee0: 456c 6575 7468 6572 4149 2f6c 6d2d 6576  EleutherAI/lm-ev
-00000ef0: 616c 7561 7469 6f6e 2d68 6172 6e65 7373  aluation-harness
-00000f00: 292e 2042 7569 6c64 696e 6720 7570 6f6e  ). Building upon
-00000f10: 2069 7473 2066 6f75 6e64 6174 696f 6e2c   its foundation,
-00000f20: 2077 6520 696d 706c 656d 656e 7465 6420   we implemented 
-00000f30: 6f75 7220 606c 6d6d 732d 6576 616c 6020  our `lmms-eval` 
-00000f40: 6672 616d 6577 6f72 6b20 7769 7468 2070  framework with p
-00000f50: 6572 666f 726d 616e 6365 206f 7074 696d  erformance optim
-00000f60: 697a 6174 696f 6e73 2073 7065 6369 6669  izations specifi
-00000f70: 6361 6c6c 7920 666f 7220 4c4d 4d73 2e0a  cally for LMMs..
-00000f80: 0a23 2320 4e65 6365 7373 6974 7920 6f66  .## Necessity of
-00000f90: 206c 6d6d 732d 6576 616c 0a0a 5765 2062   lmms-eval..We b
-00000fa0: 656c 6965 7665 206f 7572 2065 6666 6f72  elieve our effor
-00000fb0: 7420 636f 756c 6420 7072 6f76 6964 6520  t could provide 
-00000fc0: 616e 2065 6666 6963 6965 6e74 2069 6e74  an efficient int
-00000fd0: 6572 6661 6365 2066 6f72 2074 6865 2064  erface for the d
-00000fe0: 6574 6169 6c65 6420 636f 6d70 6172 6973  etailed comparis
-00000ff0: 6f6e 206f 6620 7075 626c 6963 6c79 2061  on of publicly a
-00001000: 7661 696c 6162 6c65 206d 6f64 656c 7320  vailable models 
-00001010: 746f 2064 6973 6365 726e 2074 6865 6972  to discern their
-00001020: 2073 7472 656e 6774 6873 2061 6e64 2077   strengths and w
-00001030: 6561 6b6e 6573 7365 732e 2049 7427 7320  eaknesses. It's 
-00001040: 616c 736f 2075 7365 6675 6c20 666f 7220  also useful for 
-00001050: 7265 7365 6172 6368 2069 6e73 7469 7475  research institu
-00001060: 7469 6f6e 7320 616e 6420 7072 6f64 7563  tions and produc
-00001070: 7469 6f6e 2d6f 7269 656e 7465 6420 636f  tion-oriented co
-00001080: 6d70 616e 6965 7320 746f 2061 6363 656c  mpanies to accel
-00001090: 6572 6174 6520 7468 6520 6465 7665 6c6f  erate the develo
-000010a0: 706d 656e 7420 6f66 206c 6172 6765 206d  pment of large m
-000010b0: 756c 7469 6d6f 6461 6c20 6d6f 6465 6c73  ultimodal models
-000010c0: 2e20 5769 7468 2074 6865 2060 6c6d 6d73  . With the `lmms
-000010d0: 2d65 7661 6c60 2c20 7765 2068 6176 6520  -eval`, we have 
-000010e0: 7369 676e 6966 6963 616e 746c 7920 6163  significantly ac
-000010f0: 6365 6c65 7261 7465 6420 7468 6520 6c69  celerated the li
-00001100: 6665 6379 636c 6520 6f66 206d 6f64 656c  fecycle of model
-00001110: 2069 7465 7261 7469 6f6e 2e20 496e 7369   iteration. Insi
-00001120: 6465 2074 6865 204c 4c61 5641 2074 6561  de the LLaVA tea
-00001130: 6d2c 2074 6865 2075 7469 6c69 7a61 7469  m, the utilizati
-00001140: 6f6e 206f 6620 606c 6d6d 732d 6576 616c  on of `lmms-eval
-00001150: 6020 6c61 7267 656c 7920 696d 7072 6f76  ` largely improv
-00001160: 6573 2074 6865 2065 6666 6963 6965 6e63  es the efficienc
-00001170: 7920 6f66 2074 6865 206d 6f64 656c 2064  y of the model d
-00001180: 6576 656c 6f70 6d65 6e74 2063 7963 6c65  evelopment cycle
-00001190: 2c20 6173 2077 6520 6172 6520 6162 6c65  , as we are able
-000011a0: 2074 6f20 6576 616c 7561 7465 2077 6565   to evaluate wee
-000011b0: 6b6c 7920 7472 6169 6e65 6420 6875 6e64  kly trained hund
-000011c0: 7265 6473 206f 6620 6368 6563 6b70 6f69  reds of checkpoi
-000011d0: 6e74 7320 6f6e 2032 302d 3330 2064 6174  nts on 20-30 dat
-000011e0: 6173 6574 732c 2069 6465 6e74 6966 7969  asets, identifyi
-000011f0: 6e67 2074 6865 2073 7472 656e 6774 6873  ng the strengths
-00001200: 2061 6e64 2077 6561 6b6e 6573 7365 732c   and weaknesses,
-00001210: 2061 6e64 2074 6865 6e20 6d61 6b65 2074   and then make t
-00001220: 6172 6765 7465 6420 696d 7072 6f76 656d  argeted improvem
-00001230: 656e 7473 2e0a 0a23 2041 6e6e 6f75 6365  ents...# Annouce
-00001240: 6d65 6e74 0a0a 2323 2076 302e 312e 3020  ment..## v0.1.0 
-00001250: 5265 6c65 6173 6564 0a0a 5468 6520 6669  Released..The fi
-00001260: 7273 7420 7665 7273 696f 6e20 6f66 2074  rst version of t
-00001270: 6865 2060 6c6d 6d73 2d65 7661 6c60 2069  he `lmms-eval` i
-00001280: 7320 7265 6c65 6173 6564 2e20 5765 2061  s released. We a
-00001290: 7265 2077 6f72 6b69 6e67 206f 6e20 7072  re working on pr
-000012a0: 6f76 6964 696e 6720 616e 206f 6e65 2d63  oviding an one-c
-000012b0: 6f6d 6d61 6e64 2065 7661 6c75 6174 696f  ommand evaluatio
-000012c0: 6e20 7375 6974 6520 666f 7220 6163 6365  n suite for acce
-000012d0: 6c65 7261 7469 6e67 2074 6865 2064 6576  lerating the dev
-000012e0: 656c 6f70 6d65 6e74 206f 6620 4c4d 4d73  elopment of LMMs
-000012f0: 2e20 0a0a 3e20 496e 205b 4c4c 6156 4120  . ..> In [LLaVA 
-00001300: 4e65 7874 5d28 6874 7470 733a 2f2f 6c6c  Next](https://ll
-00001310: 6176 612d 766c 2e67 6974 6875 622e 696f  ava-vl.github.io
-00001320: 2f62 6c6f 672f 3230 3234 2d30 312d 3330  /blog/2024-01-30
-00001330: 2d6c 6c61 7661 2d6e 6578 742f 2920 6465  -llava-next/) de
-00001340: 7665 6c6f 706d 656e 742c 2077 6520 696e  velopment, we in
-00001350: 7465 726e 616c 6c79 2075 7469 6c69 7a65  ternally utilize
-00001360: 2074 6869 7320 7375 6974 6520 746f 2065   this suite to e
-00001370: 7661 6c75 6174 6520 7468 6520 6d75 6c74  valuate the mult
-00001380: 6970 6c65 2064 6966 6665 7265 6e74 206d  iple different m
-00001390: 6f64 656c 2076 6572 7369 6f6e 7320 6f6e  odel versions on
-000013a0: 2076 6172 696f 7573 2064 6174 6173 6574   various dataset
-000013b0: 732e 2049 7420 7369 676e 6966 6963 616e  s. It significan
-000013c0: 746c 7920 6163 6365 6c65 7261 7465 7320  tly accelerates 
-000013d0: 7468 6520 6d6f 6465 6c20 6465 7665 6c6f  the model develo
-000013e0: 706d 656e 7420 6379 636c 6520 666f 7220  pment cycle for 
-000013f0: 6974 2773 2065 6173 7920 696e 7465 6772  it's easy integr
-00001400: 6174 696f 6e20 616e 6420 6661 7374 2065  ation and fast e
-00001410: 7661 6c75 6174 696f 6e20 7370 6565 642e  valuation speed.
-00001420: 0a0a 5468 6520 6d61 696e 2066 6561 7475  ..The main featu
-00001430: 7265 2069 6e63 6c75 6465 733a 0a0a 3c70  re includes:..<p
-00001440: 2061 6c69 676e 3d22 6365 6e74 6572 2220   align="center" 
-00001450: 7769 6474 683d 2231 3030 2522 3e0a 3c69  width="100%">.<i
-00001460: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00001470: 692e 706f 7374 696d 672e 6363 2f73 677a  i.postimg.cc/sgz
-00001480: 4e6d 4a78 372f 7465 6173 6572 2e70 6e67  NmJx7/teaser.png
-00001490: 2220 2077 6964 7468 3d22 3130 3025 2220  "  width="100%" 
-000014a0: 6865 6967 6874 3d22 3830 2522 3e0a 3c2f  height="80%">.</
-000014b0: 703e 0a0a 2323 2320 4f6e 652d 636f 6d6d  p>..### One-comm
-000014c0: 616e 6420 6576 616c 7561 7469 6f6e 2c20  and evaluation, 
-000014d0: 7769 7468 2064 6574 6169 6c65 6420 6c6f  with detailed lo
-000014e0: 6773 2061 6e64 2073 616d 706c 6573 2e0a  gs and samples..
-000014f0: 596f 7520 6361 6e20 6576 616c 7561 7465  You can evaluate
-00001500: 2074 6865 206d 6f64 656c 7320 6f6e 206d   the models on m
-00001510: 756c 7469 706c 6520 6461 7461 7365 7473  ultiple datasets
-00001520: 2077 6974 6820 6120 7369 6e67 6c65 2063   with a single c
-00001530: 6f6d 6d61 6e64 2e20 4e6f 206d 6f64 656c  ommand. No model
-00001540: 2f64 6174 6120 7072 6570 6172 6174 696f  /data preparatio
-00001550: 6e20 6973 206e 6565 6465 642c 206a 7573  n is needed, jus
-00001560: 7420 6f6e 6520 636f 6d6d 616e 6420 6c69  t one command li
-00001570: 6e65 2c20 6665 7720 6d69 6e75 7465 732c  ne, few minutes,
-00001580: 2061 6e64 2067 6574 2074 6865 2072 6573   and get the res
-00001590: 756c 7473 2e20 4e6f 7420 6a75 7374 2061  ults. Not just a
-000015a0: 2072 6573 756c 7420 6e75 6d62 6572 2c20   result number, 
-000015b0: 6275 7420 616c 736f 2074 6865 2064 6574  but also the det
-000015c0: 6169 6c65 6420 6c6f 6773 2061 6e64 2073  ailed logs and s
-000015d0: 616d 706c 6573 2c20 696e 636c 7564 696e  amples, includin
-000015e0: 6720 7468 6520 6d6f 6465 6c20 6172 6773  g the model args
-000015f0: 2c20 696e 7075 7420 7175 6573 7469 6f6e  , input question
-00001600: 2c20 6d6f 6465 6c20 7265 7370 6f6e 7365  , model response
-00001610: 2c20 616e 6420 6772 6f75 6e64 2074 7275  , and ground tru
-00001620: 7468 2061 6e73 7765 722e 0a0a 6060 6070  th answer...```p
-00001630: 7974 686f 6e0a 2320 4576 616c 7561 7469  ython.# Evaluati
-00001640: 6e67 204c 4c61 5641 206f 6e20 6d75 6c74  ng LLaVA on mult
-00001650: 6970 6c65 2064 6174 6173 6574 730a 6163  iple datasets.ac
-00001660: 6365 6c65 7261 7465 206c 6175 6e63 6820  celerate launch 
-00001670: 2d2d 6e75 6d5f 7072 6f63 6573 7365 733d  --num_processes=
-00001680: 3820 2d6d 206c 6d6d 735f 6576 616c 202d  8 -m lmms_eval -
-00001690: 2d6d 6f64 656c 206c 6c61 7661 2020 202d  -model llava   -
-000016a0: 2d6d 6f64 656c 5f61 7267 7320 7072 6574  -model_args pret
-000016b0: 7261 696e 6564 3d22 6c69 7568 616f 7469  rained="liuhaoti
-000016c0: 616e 2f6c 6c61 7661 2d76 312e 352d 3762  an/llava-v1.5-7b
-000016d0: 2220 2020 2d2d 7461 736b 7320 6d6d 652c  "   --tasks mme,
-000016e0: 6d6d 6265 6e63 685f 656e 202d 2d62 6174  mmbench_en --bat
-000016f0: 6368 5f73 697a 6520 3120 2d2d 6c6f 675f  ch_size 1 --log_
-00001700: 7361 6d70 6c65 7320 2d2d 6c6f 675f 7361  samples --log_sa
-00001710: 6d70 6c65 735f 7375 6666 6978 206c 6c61  mples_suffix lla
-00001720: 7661 5f76 312e 355f 6d6d 655f 6d6d 6265  va_v1.5_mme_mmbe
-00001730: 6e63 6865 6e20 2d2d 6f75 7470 7574 5f70  nchen --output_p
-00001740: 6174 6820 2e2f 6c6f 6773 2f20 230a 6060  ath ./logs/ #.``
-00001750: 600a 0a23 2323 2041 6363 656c 6572 6174  `..### Accelerat
-00001760: 6f72 2073 7570 706f 7274 2061 6e64 2054  or support and T
-00001770: 6173 6b73 2067 726f 7570 696e 672e 0a57  asks grouping..W
-00001780: 6520 7375 7070 6f72 7420 7468 6520 7573  e support the us
-00001790: 6167 6520 6f66 2060 6163 6365 6c65 7261  age of `accelera
-000017a0: 7465 6020 746f 2077 7261 7020 7468 6520  te` to wrap the 
-000017b0: 6d6f 6465 6c20 666f 7220 6469 7374 7269  model for distri
-000017c0: 6275 7465 6420 6576 616c 7561 7469 6f6e  buted evaluation
-000017d0: 2c20 7375 7070 6f72 7469 6e67 206d 756c  , supporting mul
-000017e0: 7469 2d67 7075 2061 6e64 2074 656e 736f  ti-gpu and tenso
-000017f0: 7220 7061 7261 6c6c 656c 6973 6d2e 2057  r parallelism. W
-00001800: 6974 6820 2a2a 5461 736b 2047 726f 7570  ith **Task Group
-00001810: 696e 672a 2a2c 2061 6c6c 2069 6e73 7461  ing**, all insta
-00001820: 6e63 6573 2066 726f 6d20 616c 6c20 7461  nces from all ta
-00001830: 736b 7320 6172 6520 6772 6f75 7065 6420  sks are grouped 
-00001840: 616e 6420 6576 616c 7561 7465 6420 696e  and evaluated in
-00001850: 2070 6172 616c 6c65 6c2c 2077 6869 6368   parallel, which
-00001860: 2073 6967 6e69 6669 6361 6e74 6c79 2069   significantly i
-00001870: 6d70 726f 7665 7320 7468 6520 7468 726f  mproves the thro
-00001880: 7567 6870 7574 206f 6620 7468 6520 6576  ughput of the ev
-00001890: 616c 7561 7469 6f6e 2e20 4166 7465 7220  aluation. After 
-000018a0: 6576 616c 7561 7469 6f6e 2c20 616c 6c20  evaluation, all 
-000018b0: 696e 7374 616e 6365 7320 6172 6520 7365  instances are se
-000018c0: 6e74 2074 6f20 706f 7374 7072 6f63 6573  nt to postproces
-000018d0: 7369 6e67 206d 6f64 756c 6520 666f 7220  sing module for 
-000018e0: 6d65 7472 6963 2063 616c 6375 6174 696f  metric calcuatio
-000018f0: 6e73 2061 6e64 2070 6f74 656e 7469 616c  ns and potential
-00001900: 2047 5054 342d 6576 616c 2071 7565 7269   GPT4-eval queri
-00001910: 6573 2e0a 0a42 656c 6f77 2061 7265 2074  es...Below are t
-00001920: 6865 2074 6f74 616c 2072 756e 7469 6d65  he total runtime
-00001930: 206f 6e20 6469 6666 6572 656e 7420 6461   on different da
-00001940: 7461 7365 7473 2075 7369 6e67 2034 2078  tasets using 4 x
-00001950: 2041 3130 3020 3430 472e 0a0a 7c20 4461   A100 40G...| Da
-00001960: 7461 7365 7420 2823 6e75 6d29 2020 2020  taset (#num)    
-00001970: 2020 2020 2020 7c20 4c4c 6156 412d 7631        | LLaVA-v1
-00001980: 2e35 2d37 6220 2020 2020 207c 204c 4c61  .5-7b      | LLa
-00001990: 5641 2d76 312e 352d 3133 6220 2020 2020  VA-v1.5-13b     
-000019a0: 7c0a 7c20 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d  |.| :-----------
-000019b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c20 3a2d  ----------- | :-
-000019c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000019d0: 207c 203a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   | :------------
-000019e0: 2d2d 2d2d 2d20 7c0a 7c20 6d6d 6520 2832  ----- |.| mme (2
-000019f0: 3337 3429 2020 2020 2020 2020 2020 2020  374)            
-00001a00: 2020 7c20 3220 6d69 6e73 2034 3320 7365    | 2 mins 43 se
-00001a10: 636f 6e64 7320 207c 2033 206d 696e 7320  conds  | 3 mins 
-00001a20: 3237 2073 6563 6f6e 6473 2020 7c0a 7c20  27 seconds  |.| 
-00001a30: 6771 6120 2831 3235 3738 2920 2020 2020  gqa (12578)     
-00001a40: 2020 2020 2020 2020 7c20 3130 206d 696e          | 10 min
-00001a50: 7320 3433 2073 6563 6f6e 6473 207c 2031  s 43 seconds | 1
-00001a60: 3420 6d69 6e73 2032 3320 7365 636f 6e64  4 mins 23 second
-00001a70: 7320 7c0a 7c20 7363 6965 6e63 6571 615f  s |.| scienceqa_
-00001a80: 696d 6720 2832 3031 3729 2020 2020 7c20  img (2017)    | 
-00001a90: 3120 6d69 6e73 2035 3820 7365 636f 6e64  1 mins 58 second
-00001aa0: 7320 207c 2032 206d 696e 7320 3532 2073  s  | 2 mins 52 s
-00001ab0: 6563 6f6e 6473 2020 7c0a 7c20 6169 3264  econds  |.| ai2d
-00001ac0: 2028 3330 3838 2920 2020 2020 2020 2020   (3088)         
-00001ad0: 2020 2020 7c20 3320 6d69 6e73 2031 3720      | 3 mins 17 
-00001ae0: 7365 636f 6e64 7320 207c 2034 206d 696e  seconds  | 4 min
-00001af0: 7320 3132 2073 6563 6f6e 6473 2020 7c0a  s 12 seconds  |.
-00001b00: 7c20 636f 636f 3230 3137 5f63 6170 5f76  | coco2017_cap_v
-00001b10: 616c 2028 3530 3030 2920 7c20 3134 206d  al (5000) | 14 m
-00001b20: 696e 7320 3133 2073 6563 6f6e 6473 207c  ins 13 seconds |
-00001b30: 2031 3920 6d69 6e73 2035 3820 7365 636f   19 mins 58 seco
-00001b40: 6e64 7320 7c0a 0a23 2323 2041 6c6c 2d49  nds |..### All-I
-00001b50: 6e2d 4f6e 6520 4846 2064 6174 6173 6574  n-One HF dataset
-00001b60: 2068 7562 732e 0a0a 5765 2061 7265 2068   hubs...We are h
-00001b70: 6f73 7469 6e67 206d 6f72 6520 7468 616e  osting more than
-00001b80: 2034 3020 2861 6e64 2069 6e63 7265 6173   40 (and increas
-00001b90: 696e 6729 2064 6174 6173 6574 7320 6f6e  ing) datasets on
-00001ba0: 205b 6875 6767 696e 6766 6163 652f 6c6d   [huggingface/lm
-00001bb0: 6d73 2d6c 6162 5d28 6874 7470 733a 2f2f  ms-lab](https://
-00001bc0: 6875 6767 696e 6766 6163 652e 636f 2f6c  huggingface.co/l
-00001bd0: 6d6d 732d 6c61 6229 2c20 7765 2063 6172  mms-lab), we car
-00001be0: 6566 756c 6c79 2063 6f6e 7665 7274 6564  efully converted
-00001bf0: 2074 6865 7365 2064 6174 6173 6574 7320   these datasets 
-00001c00: 6672 6f6d 206f 7269 6769 6e61 6c20 736f  from original so
-00001c10: 7572 6365 7320 616e 6420 696e 636c 7564  urces and includ
-00001c20: 6564 2061 6c6c 2076 6172 6961 6e74 732c  ed all variants,
-00001c30: 2076 6572 7369 6f6e 7320 616e 6420 7370   versions and sp
-00001c40: 6c69 7473 2e20 4e6f 7720 7468 6579 2063  lits. Now they c
-00001c50: 616e 2062 6520 6469 7265 6374 6c79 2061  an be directly a
-00001c60: 6363 6573 7365 6420 7769 7468 6f75 7420  ccessed without 
-00001c70: 616e 7920 6275 7264 656e 206f 6620 6461  any burden of da
-00001c80: 7461 2070 7265 7072 6f63 6573 7369 6e67  ta preprocessing
-00001c90: 2e20 5468 6579 2061 6c73 6f20 7365 7276  . They also serv
-00001ca0: 6520 666f 7220 7468 6520 7075 7270 6f73  e for the purpos
-00001cb0: 6520 6f66 2076 6973 7561 6c69 7a69 6e67  e of visualizing
-00001cc0: 2074 6865 2064 6174 6120 616e 6420 6772   the data and gr
-00001cd0: 6173 7069 6e67 2074 6865 2073 656e 7365  asping the sense
-00001ce0: 206f 6620 6576 616c 7561 7469 6f6e 2074   of evaluation t
-00001cf0: 6173 6b73 2064 6973 7472 6962 7574 696f  asks distributio
-00001d00: 6e2e 0a0a 3c70 2061 6c69 676e 3d22 6365  n...<p align="ce
-00001d10: 6e74 6572 2220 7769 6474 683d 2231 3030  nter" width="100
-00001d20: 2522 3e0a 3c69 6d67 2073 7263 3d22 6874  %">.<img src="ht
-00001d30: 7470 733a 2f2f 692e 706f 7374 696d 672e  tps://i.postimg.
-00001d40: 6363 2f38 5058 4657 3973 6b2f 5758 3230  cc/8PXFW9sk/WX20
-00001d50: 3234 3032 3238 2d31 3233 3131 305f 3278  240228-123110_2x
-00001d60: 2e70 6e67 2220 2077 6964 7468 3d22 3130  .png"  width="10
-00001d70: 3025 2220 6865 6967 6874 3d22 3830 2522  0%" height="80%"
-00001d80: 3e0a 3c2f 703e 0a0a 2323 2320 4465 7461  >.</p>..### Deta
-00001d90: 696c 6564 204c 6f67 6769 6e67 2055 7469  iled Logging Uti
-00001da0: 6c69 7465 730a 0a57 6520 7072 6f76 6964  lites..We provid
-00001db0: 6520 6465 7461 696c 6564 206c 6f67 6769  e detailed loggi
-00001dc0: 6e67 2075 7469 6c69 7469 6573 2074 6f20  ng utilities to 
-00001dd0: 6865 6c70 2079 6f75 2075 6e64 6572 7374  help you underst
-00001de0: 616e 6420 7468 6520 6576 616c 7561 7469  and the evaluati
-00001df0: 6f6e 2070 726f 6365 7373 2061 6e64 2072  on process and r
-00001e00: 6573 756c 7473 2e20 5468 6520 6c6f 6773  esults. The logs
-00001e10: 2069 6e63 6c75 6465 2074 6865 206d 6f64   include the mod
-00001e20: 656c 2061 7267 732c 2067 656e 6572 6174  el args, generat
-00001e30: 696f 6e20 7061 7261 6d65 7465 7273 2c20  ion parameters, 
-00001e40: 696e 7075 7420 7175 6573 7469 6f6e 2c20  input question, 
-00001e50: 6d6f 6465 6c20 7265 7370 6f6e 7365 2c20  model response, 
-00001e60: 616e 6420 6772 6f75 6e64 2074 7275 7468  and ground truth
-00001e70: 2061 6e73 7765 722e 2059 6f75 2063 616e   answer. You can
-00001e80: 2061 6c73 6f20 7265 636f 7264 2065 7665   also record eve
-00001e90: 7279 2064 6574 6169 6c73 2061 6e64 2076  ry details and v
-00001ea0: 6973 7561 6c69 7a65 2074 6865 6d20 696e  isualize them in
-00001eb0: 7369 6465 2072 756e 7320 6f6e 2057 6569  side runs on Wei
-00001ec0: 6768 7473 2026 2042 6961 7365 732e 0a0a  ghts & Biases...
-00001ed0: 7b25 2069 6e63 6c75 6465 2066 6967 7572  {% include figur
-00001ee0: 652e 6c69 7175 6964 206c 6f61 6469 6e67  e.liquid loading
-00001ef0: 3d22 6561 6765 7222 2070 6174 683d 2261  ="eager" path="a
-00001f00: 7373 6574 732f 696d 672f 7761 6e64 625f  ssets/img/wandb_
-00001f10: 7461 626c 652e 706e 6722 2063 6c61 7373  table.png" class
-00001f20: 3d22 696d 672d 666c 7569 6420 726f 756e  ="img-fluid roun
-00001f30: 6465 6420 7a2d 6465 7074 682d 3122 207a  ded z-depth-1" z
-00001f40: 6f6f 6d61 626c 653d 7472 7565 2025 7d0a  oomable=true %}.
-00001f50: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
-00001f60: 7222 2077 6964 7468 3d22 3130 3025 223e  r" width="100%">
-00001f70: 0a3c 696d 6720 7372 633d 2268 7474 7073  .<img src="https
-00001f80: 3a2f 2f69 2e70 6f73 7469 6d67 2e63 632f  ://i.postimg.cc/
-00001f90: 5731 6331 7642 444a 2f57 6563 6861 742d  W1c1vBDJ/Wechat-
-00001fa0: 494d 4731 3939 332e 706e 6722 2020 7769  IMG1993.png"  wi
-00001fb0: 6474 683d 2231 3030 2522 2068 6569 6768  dth="100%" heigh
-00001fc0: 743d 2238 3025 223e 0a3c 2f70 3e0a 0a23  t="80%">.</p>..#
-00001fd0: 2049 6e73 7461 6c6c 6174 696f 6e0a 0a46   Installation..F
-00001fe0: 6f72 2066 6f72 6d61 6c20 7573 6167 652c  or formal usage,
-00001ff0: 2079 6f75 2063 616e 2069 6e73 7461 6c6c   you can install
-00002000: 2074 6865 2070 6163 6b61 6765 2066 726f   the package fro
-00002010: 6d20 5079 5049 2062 7920 7275 6e6e 696e  m PyPI by runnin
-00002020: 6720 7468 6520 666f 6c6c 6f77 696e 6720  g the following 
-00002030: 636f 6d6d 616e 643a 0a60 6060 6261 7368  command:.```bash
-00002040: 0a70 6970 2069 6e73 7461 6c6c 206c 6d6d  .pip install lmm
-00002050: 732d 6576 616c 0a60 6060 0a0a 466f 7220  s-eval.```..For 
-00002060: 6465 7665 6c6f 706d 656e 742c 2079 6f75  development, you
-00002070: 2063 616e 2069 6e73 7461 6c6c 2074 6865   can install the
-00002080: 2070 6163 6b61 6765 2062 7920 636c 6f6e   package by clon
-00002090: 696e 6720 7468 6520 7265 706f 7369 746f  ing the reposito
-000020a0: 7279 2061 6e64 2072 756e 6e69 6e67 2074  ry and running t
-000020b0: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6d  he following com
-000020c0: 6d61 6e64 3a0a 6060 6062 6173 680a 6769  mand:.```bash.gi
-000020d0: 7420 636c 6f6e 6520 6874 7470 733a 2f2f  t clone https://
-000020e0: 6769 7468 7562 2e63 6f6d 2f45 766f 6c76  github.com/Evolv
-000020f0: 696e 674c 4d4d 732d 4c61 622f 6c6d 6d73  ingLMMs-Lab/lmms
-00002100: 2d65 7661 6c0a 6364 206c 6d6d 732d 6576  -eval.cd lmms-ev
-00002110: 616c 0a70 6970 2069 6e73 7461 6c6c 202d  al.pip install -
-00002120: 6520 2e0a 6060 600a 0a49 6620 796f 7520  e ..```..If you 
-00002130: 7761 6e74 6564 2074 6f20 7465 7374 206c  wanted to test l
-00002140: 6c61 7661 2c20 796f 7520 7769 6c6c 2068  lava, you will h
-00002150: 6176 6520 746f 2063 6c6f 6e65 2074 6865  ave to clone the
-00002160: 6972 2072 6570 6f20 6672 6f6d 205b 4c4c  ir repo from [LL
-00002170: 6156 415d 2868 7474 7073 3a2f 2f67 6974  aVA](https://git
-00002180: 6875 622e 636f 6d2f 6861 6f74 6961 6e2d  hub.com/haotian-
-00002190: 6c69 752f 4c4c 6156 4129 2061 6e64 0a60  liu/LLaVA) and.`
-000021a0: 6060 0a67 6974 2063 6c6f 6e65 2068 7474  ``.git clone htt
-000021b0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000021c0: 6861 6f74 6961 6e2d 6c69 752f 4c4c 6156  haotian-liu/LLaV
-000021d0: 410a 6364 204c 4c61 5641 0a70 6970 2069  A.cd LLaVA.pip i
-000021e0: 6e73 7461 6c6c 202d 6520 2e0a 6060 600a  nstall -e ..```.
-000021f0: 0a59 6f75 2063 616e 2063 6865 636b 2074  .You can check t
-00002200: 6865 205b 656e 7669 726f 6e6d 656e 7420  he [environment 
-00002210: 696e 7374 616c 6c20 7363 7269 7074 5d28  install script](
-00002220: 6d69 7363 732f 7265 7072 5f73 6372 6970  miscs/repr_scrip
-00002230: 7473 2e73 6829 2061 6e64 205b 746f 7263  ts.sh) and [torc
-00002240: 6820 656e 7669 726f 6e6d 656e 7420 696e  h environment in
-00002250: 666f 5d28 6d69 7363 732f 7265 7072 5f74  fo](miscs/repr_t
-00002260: 6f72 6368 5f65 6e76 732e 7478 7429 2074  orch_envs.txt) t
-00002270: 6f20 2a2a 7265 7072 6f64 7563 6520 4c4c  o **reproduce LL
-00002280: 6156 412d 312e 3527 7320 7061 7065 7220  aVA-1.5's paper 
-00002290: 7265 7375 6c74 732a 2a2e 2057 6520 666f  results**. We fo
-000022a0: 756e 6420 746f 7263 682f 6375 6461 2076  und torch/cuda v
-000022b0: 6572 7369 6f6e 7320 6469 6666 6572 656e  ersions differen
-000022c0: 6365 2077 6f75 6c64 2063 6175 7365 2073  ce would cause s
-000022d0: 6d61 6c6c 2076 6172 6961 7469 6f6e 7320  mall variations 
-000022e0: 696e 2074 6865 2072 6573 756c 7473 2c20  in the results, 
-000022f0: 7765 2070 726f 7669 6465 2074 6865 205b  we provide the [
-00002300: 7265 7375 6c74 7320 6368 6563 6b5d 286d  results check](m
-00002310: 6973 6373 2f6c 6c61 7661 5f72 6573 756c  iscs/llava_resul
-00002320: 745f 6368 6563 6b2e 6d64 2920 7769 7468  t_check.md) with
-00002330: 2064 6966 6665 7265 6e74 2065 6e76 6972   different envir
-00002340: 6f6e 6d65 6e74 732e 0a0a 4966 2079 6f75  onments...If you
-00002350: 2077 616e 7420 746f 2074 6573 7420 6f6e   want to test on
-00002360: 2063 6170 7469 6f6e 2064 6174 6173 6574   caption dataset
-00002370: 2073 7563 6820 6173 2060 636f 636f 602c   such as `coco`,
-00002380: 2060 7265 6663 6f63 6f60 2c20 616e 6420   `refcoco`, and 
-00002390: 606e 6f63 6170 7360 2c20 796f 7520 7769  `nocaps`, you wi
-000023a0: 6c6c 206e 6565 6420 746f 2068 6176 6520  ll need to have 
-000023b0: 606a 6176 613d 3d31 2e38 2e30 2060 2074  `java==1.8.0 ` t
-000023c0: 6f20 6c65 7420 7079 636f 636f 6576 616c  o let pycocoeval
-000023d0: 2061 7069 2074 6f20 776f 726b 2e20 4966   api to work. If
-000023e0: 2079 6f75 2064 6f6e 2774 2068 6176 6520   you don't have 
-000023f0: 6974 2c20 796f 7520 6361 6e20 696e 7374  it, you can inst
-00002400: 616c 6c20 6279 2075 7369 6e67 2063 6f6e  all by using con
-00002410: 6461 0a60 6060 0a63 6f6e 6461 2069 6e73  da.```.conda ins
-00002420: 7461 6c6c 206f 7065 6e6a 646b 3d38 0a60  tall openjdk=8.`
-00002430: 6060 0a79 6f75 2063 616e 2074 6865 6e20  ``.you can then 
-00002440: 6368 6563 6b20 796f 7572 206a 6176 6120  check your java 
-00002450: 7665 7273 696f 6e20 6279 2060 6a61 7661  version by `java
-00002460: 202d 7665 7273 696f 6e60 200a 0a23 2055   -version` ..# U
-00002470: 7361 6765 0a60 6060 6261 7368 0a23 2045  sage.```bash.# E
-00002480: 7661 6c75 6174 696e 6720 4c4c 6156 4120  valuating LLaVA 
-00002490: 6f6e 204d 4d45 0a61 6363 656c 6572 6174  on MME.accelerat
-000024a0: 6520 6c61 756e 6368 202d 2d6e 756d 5f70  e launch --num_p
-000024b0: 726f 6365 7373 6573 3d38 202d 6d20 6c6d  rocesses=8 -m lm
-000024c0: 6d73 5f65 7661 6c20 2d2d 6d6f 6465 6c20  ms_eval --model 
-000024d0: 6c6c 6176 6120 2020 2d2d 6d6f 6465 6c5f  llava   --model_
-000024e0: 6172 6773 2070 7265 7472 6169 6e65 643d  args pretrained=
-000024f0: 226c 6975 6861 6f74 6961 6e2f 6c6c 6176  "liuhaotian/llav
-00002500: 612d 7631 2e35 2d37 6222 2020 202d 2d74  a-v1.5-7b"   --t
-00002510: 6173 6b73 206d 6d65 2020 2d2d 6261 7463  asks mme  --batc
-00002520: 685f 7369 7a65 2031 202d 2d6c 6f67 5f73  h_size 1 --log_s
-00002530: 616d 706c 6573 202d 2d6c 6f67 5f73 616d  amples --log_sam
-00002540: 706c 6573 5f73 7566 6669 7820 6c6c 6176  ples_suffix llav
-00002550: 615f 7631 2e35 5f6d 6d65 202d 2d6f 7574  a_v1.5_mme --out
-00002560: 7075 745f 7061 7468 202e 2f6c 6f67 732f  put_path ./logs/
-00002570: 200a 0a23 2045 7661 6c75 6174 696e 6720   ..# Evaluating 
-00002580: 4c4c 6156 4120 6f6e 206d 756c 7469 706c  LLaVA on multipl
-00002590: 6520 6461 7461 7365 7473 0a61 6363 656c  e datasets.accel
-000025a0: 6572 6174 6520 6c61 756e 6368 202d 2d6e  erate launch --n
-000025b0: 756d 5f70 726f 6365 7373 6573 3d38 202d  um_processes=8 -
-000025c0: 6d20 6c6d 6d73 5f65 7661 6c20 2d2d 6d6f  m lmms_eval --mo
-000025d0: 6465 6c20 6c6c 6176 6120 2020 2d2d 6d6f  del llava   --mo
-000025e0: 6465 6c5f 6172 6773 2070 7265 7472 6169  del_args pretrai
-000025f0: 6e65 643d 226c 6975 6861 6f74 6961 6e2f  ned="liuhaotian/
-00002600: 6c6c 6176 612d 7631 2e35 2d37 6222 2020  llava-v1.5-7b"  
-00002610: 202d 2d74 6173 6b73 206d 6d65 2c6d 6d62   --tasks mme,mmb
-00002620: 656e 6368 5f65 6e20 2d2d 6261 7463 685f  ench_en --batch_
-00002630: 7369 7a65 2031 202d 2d6c 6f67 5f73 616d  size 1 --log_sam
-00002640: 706c 6573 202d 2d6c 6f67 5f73 616d 706c  ples --log_sampl
-00002650: 6573 5f73 7566 6669 7820 6c6c 6176 615f  es_suffix llava_
-00002660: 7631 2e35 5f6d 6d65 5f6d 6d62 656e 6368  v1.5_mme_mmbench
-00002670: 656e 202d 2d6f 7574 7075 745f 7061 7468  en --output_path
-00002680: 202e 2f6c 6f67 732f 2023 0a0a 2320 466f   ./logs/ #..# Fo
-00002690: 7220 6f74 6865 7220 7661 7269 616e 7473  r other variants
-000026a0: 206c 6c61 7661 2e20 4e6f 7465 2074 6861   llava. Note tha
-000026b0: 7420 6063 6f6e 765f 7465 6d70 6c61 7465  t `conv_template
-000026c0: 6020 6973 2061 6e20 6172 6720 6f66 2074  ` is an arg of t
-000026d0: 6865 2069 6e69 7420 6675 6e63 7469 6f6e  he init function
-000026e0: 206f 6620 6c6c 6176 6120 696e 2060 6c6d   of llava in `lm
-000026f0: 6d73 5f65 7661 6c2f 6d6f 6465 6c73 2f6c  ms_eval/models/l
-00002700: 6c61 7661 2e70 7960 0a61 6363 656c 6572  lava.py`.acceler
-00002710: 6174 6520 6c61 756e 6368 202d 2d6e 756d  ate launch --num
-00002720: 5f70 726f 6365 7373 6573 3d38 202d 6d20  _processes=8 -m 
-00002730: 6c6d 6d73 5f65 7661 6c20 2d2d 6d6f 6465  lmms_eval --mode
-00002740: 6c20 6c6c 6176 6120 2020 2d2d 6d6f 6465  l llava   --mode
-00002750: 6c5f 6172 6773 2070 7265 7472 6169 6e65  l_args pretraine
-00002760: 643d 226c 6975 6861 6f74 6961 6e2f 6c6c  d="liuhaotian/ll
-00002770: 6176 612d 7631 2e36 2d6d 6973 7472 616c  ava-v1.6-mistral
-00002780: 2d37 622c 636f 6e76 5f74 656d 706c 6174  -7b,conv_templat
-00002790: 653d 6d69 7374 7261 6c5f 696e 7374 7275  e=mistral_instru
-000027a0: 6374 2220 2020 2d2d 7461 736b 7320 6d6d  ct"   --tasks mm
-000027b0: 652c 6d6d 6265 6e63 685f 656e 202d 2d62  e,mmbench_en --b
-000027c0: 6174 6368 5f73 697a 6520 3120 2d2d 6c6f  atch_size 1 --lo
-000027d0: 675f 7361 6d70 6c65 7320 2d2d 6c6f 675f  g_samples --log_
-000027e0: 7361 6d70 6c65 735f 7375 6666 6978 206c  samples_suffix l
-000027f0: 6c61 7661 5f76 312e 355f 6d6d 655f 6d6d  lava_v1.5_mme_mm
-00002800: 6265 6e63 6865 6e20 2d2d 6f75 7470 7574  benchen --output
-00002810: 5f70 6174 6820 2e2f 6c6f 6773 2f20 230a  _path ./logs/ #.
-00002820: 6163 6365 6c65 7261 7465 206c 6175 6e63  accelerate launc
-00002830: 6820 2d2d 6e75 6d5f 7072 6f63 6573 7365  h --num_processe
-00002840: 733d 3820 2d6d 206c 6d6d 735f 6576 616c  s=8 -m lmms_eval
-00002850: 202d 2d6d 6f64 656c 206c 6c61 7661 2020   --model llava  
-00002860: 202d 2d6d 6f64 656c 5f61 7267 7320 7072   --model_args pr
-00002870: 6574 7261 696e 6564 3d22 6c69 7568 616f  etrained="liuhao
-00002880: 7469 616e 2f6c 6c61 7661 2d76 312e 362d  tian/llava-v1.6-
-00002890: 3334 622c 636f 6e76 5f74 656d 706c 6174  34b,conv_templat
-000028a0: 653d 6d69 7374 7261 6c5f 6469 7265 6374  e=mistral_direct
-000028b0: 2220 2020 2d2d 7461 736b 7320 6d6d 652c  "   --tasks mme,
-000028c0: 6d6d 6265 6e63 685f 656e 202d 2d62 6174  mmbench_en --bat
-000028d0: 6368 5f73 697a 6520 3120 2d2d 6c6f 675f  ch_size 1 --log_
-000028e0: 7361 6d70 6c65 7320 2d2d 6c6f 675f 7361  samples --log_sa
-000028f0: 6d70 6c65 735f 7375 6666 6978 206c 6c61  mples_suffix lla
-00002900: 7661 5f76 312e 355f 6d6d 655f 6d6d 6265  va_v1.5_mme_mmbe
-00002910: 6e63 6865 6e20 2d2d 6f75 7470 7574 5f70  nchen --output_p
-00002920: 6174 6820 2e2f 6c6f 6773 2f20 230a 0a23  ath ./logs/ #..#
-00002930: 2046 726f 6d20 6120 7072 6564 6566 696e   From a predefin
-00002940: 6564 2063 6f6e 6669 6775 7261 7469 6f6e  ed configuration
-00002950: 2c20 7375 7070 6f72 7469 6e67 2065 7661  , supporting eva
-00002960: 6c75 6174 696f 6e20 6f66 206d 756c 7469  luation of multi
-00002970: 706c 6520 6d6f 6465 6c73 2061 6e64 2064  ple models and d
-00002980: 6174 6173 6574 730a 6163 6365 6c65 7261  atasets.accelera
-00002990: 7465 206c 6175 6e63 6820 2d2d 6e75 6d5f  te launch --num_
-000029a0: 7072 6f63 6573 7365 733d 3820 2d6d 206c  processes=8 -m l
-000029b0: 6d6d 735f 6576 616c 202d 2d63 6f6e 6669  mms_eval --confi
-000029c0: 6720 6578 616d 706c 655f 6576 616c 2e79  g example_eval.y
-000029d0: 616d 6c20 0a60 6060 0a0a 2320 4d6f 6465  aml .```..# Mode
-000029e0: 6c20 5265 7375 6c74 730a 0a41 7320 6465  l Results..As de
-000029f0: 6d6f 6e73 7472 6174 6564 2062 7920 7468  monstrated by th
-00002a00: 6520 6578 7465 6e73 6976 6520 7461 626c  e extensive tabl
-00002a10: 6520 6265 6c6f 772c 2077 6520 6169 6d20  e below, we aim 
-00002a20: 746f 2070 726f 7669 6465 2064 6574 6169  to provide detai
-00002a30: 6c65 6420 696e 666f 726d 6174 696f 6e20  led information 
-00002a40: 666f 7220 7265 6164 6572 7320 746f 2075  for readers to u
-00002a50: 6e64 6572 7374 616e 6420 7468 6520 6461  nderstand the da
-00002a60: 7461 7365 7473 2069 6e63 6c75 6465 6420  tasets included 
-00002a70: 696e 206c 6d6d 732d 6576 616c 2061 6e64  in lmms-eval and
-00002a80: 2073 6f6d 6520 7370 6563 6966 6963 2064   some specific d
-00002a90: 6574 6169 6c73 2061 626f 7574 2074 6865  etails about the
-00002aa0: 7365 2064 6174 6173 6574 7320 2877 6520  se datasets (we 
-00002ab0: 7265 6d61 696e 2067 7261 7465 6675 6c20  remain grateful 
-00002ac0: 666f 7220 616e 7920 636f 7272 6563 7469  for any correcti
-00002ad0: 6f6e 7320 7265 6164 6572 7320 6d61 7920  ons readers may 
-00002ae0: 6861 7665 2064 7572 696e 6720 6f75 7220  have during our 
-00002af0: 6576 616c 7561 7469 6f6e 2070 726f 6365  evaluation proce
-00002b00: 7373 292e 0a0a 5765 2070 726f 7669 6465  ss)...We provide
-00002b10: 2061 2047 6f6f 676c 6520 5368 6565 7420   a Google Sheet 
-00002b20: 666f 7220 7468 6520 6465 7461 696c 6564  for the detailed
-00002b30: 2072 6573 756c 7473 206f 6620 7468 6520   results of the 
-00002b40: 4c4c 6156 4120 7365 7269 6573 206d 6f64  LLaVA series mod
-00002b50: 656c 7320 6f6e 2064 6966 6665 7265 6e74  els on different
-00002b60: 2064 6174 6173 6574 732e 2059 6f75 2063   datasets. You c
-00002b70: 616e 2061 6363 6573 7320 7468 6520 7368  an access the sh
-00002b80: 6565 7420 5b68 6572 655d 2868 7474 7073  eet [here](https
-00002b90: 3a2f 2f64 6f63 732e 676f 6f67 6c65 2e63  ://docs.google.c
-00002ba0: 6f6d 2f73 7072 6561 6473 6865 6574 732f  om/spreadsheets/
-00002bb0: 642f 3161 3549 6d66 644b 4154 4449 3854  d/1a5ImfdKATDI8T
-00002bc0: 3743 7768 3665 482d 6245 736e 5146 7a61  7Cwh6eH-bEsnQFza
-00002bd0: 6e46 7261 4655 6763 5339 4b48 5763 2f65  nFraFUgcS9KHWc/e
-00002be0: 6469 743f 7573 703d 7368 6172 696e 6729  dit?usp=sharing)
-00002bf0: 2e20 4974 2773 2061 206c 6976 6520 7368  . It's a live sh
-00002c00: 6565 742c 2061 6e64 2077 6520 6172 6520  eet, and we are 
-00002c10: 7570 6461 7469 6e67 2069 7420 7769 7468  updating it with
-00002c20: 206e 6577 2072 6573 756c 7473 2e0a 0a3c   new results...<
-00002c30: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
-00002c40: 2077 6964 7468 3d22 3130 3025 223e 0a3c   width="100%">.<
-00002c50: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00002c60: 2f69 2e70 6f73 7469 6d67 2e63 632f 6a64  /i.postimg.cc/jd
-00002c70: 7734 3937 4e53 2f57 5832 3032 3430 3330  w497NS/WX2024030
-00002c80: 372d 3136 3235 3236 2d32 782e 706e 6722  7-162526-2x.png"
-00002c90: 2020 7769 6474 683d 2231 3030 2522 2068    width="100%" h
-00002ca0: 6569 6768 743d 2238 3025 223e 0a3c 2f70  eight="80%">.</p
-00002cb0: 3e0a 0a57 6520 616c 736f 2070 726f 7669  >..We also provi
-00002cc0: 6465 2074 6865 2072 6177 2064 6174 6120  de the raw data 
-00002cd0: 6578 706f 7274 6564 2066 726f 6d20 5765  exported from We
-00002ce0: 6967 6874 7320 2620 4269 6173 6573 2066  ights & Biases f
-00002cf0: 6f72 2074 6865 2064 6574 6169 6c65 6420  or the detailed 
-00002d00: 7265 7375 6c74 7320 6f66 2074 6865 204c  results of the L
-00002d10: 4c61 5641 2073 6572 6965 7320 6d6f 6465  LaVA series mode
-00002d20: 6c73 206f 6e20 6469 6666 6572 656e 7420  ls on different 
-00002d30: 6461 7461 7365 7473 2e20 596f 7520 6361  datasets. You ca
-00002d40: 6e20 6163 6365 7373 2074 6865 2072 6177  n access the raw
-00002d50: 2064 6174 6120 5b68 6572 655d 2868 7474   data [here](htt
-00002d60: 7073 3a2f 2f64 6f63 732e 676f 6f67 6c65  ps://docs.google
-00002d70: 2e63 6f6d 2f73 7072 6561 6473 6865 6574  .com/spreadsheet
-00002d80: 732f 642f 3141 7661 456d 7547 3463 7353  s/d/1AvaEmuG4csS
-00002d90: 6d58 6148 6a67 7534 6569 314b 424d 6d4e  mXaHjgu4ei1KBMmN
-00002da0: 4e57 3877 666c 4f44 5f6b 6b54 4464 7638  NW8wflOD_kkTDdv8
-00002db0: 2f65 6469 743f 7573 703d 7368 6172 696e  /edit?usp=sharin
-00002dc0: 6729 2e0a 0a3e 2044 6576 656c 6f70 6d65  g)...> Developme
-00002dd0: 6e74 2077 696c 6c20 6265 2063 6f6e 7469  nt will be conti
-00002de0: 6e75 696e 6720 6f6e 2074 6865 206d 6169  nuing on the mai
-00002df0: 6e20 6272 616e 6368 2c20 616e 6420 7765  n branch, and we
-00002e00: 2065 6e63 6f75 7261 6765 2079 6f75 2074   encourage you t
-00002e10: 6f20 6769 7665 2075 7320 6665 6564 6261  o give us feedba
-00002e20: 636b 206f 6e20 7768 6174 2066 6561 7475  ck on what featu
-00002e30: 7265 7320 6172 6520 6465 7369 7265 6420  res are desired 
-00002e40: 616e 6420 686f 7720 746f 2069 6d70 726f  and how to impro
-00002e50: 7665 2074 6865 206c 6962 7261 7279 2066  ve the library f
-00002e60: 7572 7468 6572 2c20 6f72 2061 736b 2071  urther, or ask q
-00002e70: 7565 7374 696f 6e73 2c20 6569 7468 6572  uestions, either
-00002e80: 2069 6e20 6973 7375 6573 206f 7220 5052   in issues or PR
-00002e90: 7320 6f6e 2047 6974 4875 622e 0a0a 0a23  s on GitHub....#
-00002ea0: 2320 5375 7070 6f72 7465 6420 6d6f 6465  # Supported mode
-00002eb0: 6c73 0a0a 2d20 4750 5434 5620 2841 5049  ls..- GPT4V (API
-00002ec0: 2c20 6f6e 6c79 2067 656e 6572 6174 696f  , only generatio
-00002ed0: 6e2d 6261 7365 6420 6576 616c 7561 7469  n-based evaluati
-00002ee0: 6f6e 290a 2d20 4c4c 6156 412d 7631 2e35  on).- LLaVA-v1.5
-00002ef0: 2f76 312e 362d 3742 2f31 3342 2f33 3442  /v1.6-7B/13B/34B
-00002f00: 2028 7070 6c2d 6261 7365 642c 2067 656e   (ppl-based, gen
-00002f10: 6572 6174 696f 6e2d 6261 7365 6429 0a2d  eration-based).-
-00002f20: 2051 7765 6e2d 564c 2073 6572 6965 7320   Qwen-VL series 
-00002f30: 2870 706c 2d62 6173 6564 2c20 6765 6e65  (ppl-based, gene
-00002f40: 7261 7469 6f6e 2d62 6173 6564 290a 2d20  ration-based).- 
-00002f50: 4675 7975 2073 6572 6965 7320 2870 706c  Fuyu series (ppl
-00002f60: 2d62 6173 6564 2c20 6765 6e65 7261 7469  -based, generati
-00002f70: 6f6e 2d62 6173 6564 290a 2d20 496e 7374  on-based).- Inst
-00002f80: 7275 6374 424c 4950 2073 6572 6965 7320  ructBLIP series 
-00002f90: 2867 656e 6572 6174 696f 6e2d 6261 7365  (generation-base
-00002fa0: 6429 0a0a 2323 2053 7570 706f 7274 6564  d)..## Supported
-00002fb0: 2064 6174 6173 6574 730a 3e20 2829 2069   datasets.> () i
-00002fc0: 6e64 6963 6174 6573 2074 6865 2074 6173  ndicates the tas
-00002fd0: 6b20 6e61 6d65 2069 6e20 7468 6520 6c6d  k name in the lm
-00002fe0: 6d73 5f65 7661 6c2e 2054 6865 2074 6173  ms_eval. The tas
-00002ff0: 6b20 6e61 6d65 2069 7320 616c 736f 2075  k name is also u
-00003000: 7365 6420 746f 2073 7065 6369 6679 2074  sed to specify t
-00003010: 6865 2064 6174 6173 6574 2069 6e20 7468  he dataset in th
-00003020: 6520 636f 6e66 6967 7572 6174 696f 6e20  e configuration 
-00003030: 6669 6c65 2e0a 0a2d 2041 4932 4420 2861  file...- AI2D (a
-00003040: 6932 6429 0a2d 2043 6861 7274 5141 2028  i2d).- ChartQA (
-00003050: 6368 6172 7471 6129 0a2d 2043 4d4d 4d55  chartqa).- CMMMU
-00003060: 2028 636d 6d6d 7529 0a20 202d 2043 4d4d   (cmmmu).  - CMM
-00003070: 4d55 2056 616c 6964 6174 696f 6e20 2863  MU Validation (c
-00003080: 6d6d 6d75 5f76 616c 290a 2020 2d20 434d  mmmu_val).  - CM
-00003090: 4d4d 5520 5465 7374 2028 636d 6d6d 755f  MMU Test (cmmmu_
-000030a0: 7465 7374 290a 2d20 434f 434f 2043 6170  test).- COCO Cap
-000030b0: 7469 6f6e 2028 636f 636f 5f63 6170 290a  tion (coco_cap).
-000030c0: 2020 2d20 434f 434f 2032 3031 3420 4361    - COCO 2014 Ca
-000030d0: 7074 696f 6e20 2863 6f63 6f32 3031 345f  ption (coco2014_
-000030e0: 6361 7029 0a20 2020 202d 2043 4f43 4f20  cap).    - COCO 
-000030f0: 3230 3134 2043 6170 7469 6f6e 2056 616c  2014 Caption Val
-00003100: 6964 6174 696f 6e20 2863 6f63 6f32 3031  idation (coco201
-00003110: 345f 6361 705f 7661 6c29 0a20 2020 202d  4_cap_val).    -
-00003120: 2043 4f43 4f20 3230 3134 2043 6170 7469   COCO 2014 Capti
-00003130: 6f6e 2054 6573 7420 2863 6f63 6f32 3031  on Test (coco201
-00003140: 345f 6361 705f 7465 7374 290a 2020 2d20  4_cap_test).  - 
-00003150: 434f 434f 2032 3031 3720 4361 7074 696f  COCO 2017 Captio
-00003160: 6e20 2863 6f63 6f32 3031 375f 6361 7029  n (coco2017_cap)
-00003170: 0a20 2020 202d 2043 4f43 4f20 3230 3137  .    - COCO 2017
-00003180: 2043 6170 7469 6f6e 204d 696e 6956 616c   Caption MiniVal
-00003190: 2028 636f 636f 3230 3137 5f63 6170 5f76   (coco2017_cap_v
-000031a0: 616c 290a 2020 2020 2d20 434f 434f 2032  al).    - COCO 2
-000031b0: 3031 3720 4361 7074 696f 6e20 4d69 6e69  017 Caption Mini
-000031c0: 5465 7374 2028 636f 636f 3230 3137 5f63  Test (coco2017_c
-000031d0: 6170 5f74 6573 7429 0a2d 2044 4f43 5651  ap_test).- DOCVQ
-000031e0: 4120 2864 6f63 7671 6129 0a20 202d 2044  A (docvqa).  - D
-000031f0: 4f43 5651 4120 5661 6c69 6461 7469 6f6e  OCVQA Validation
-00003200: 2028 646f 6376 7161 5f76 616c 290a 2020   (docvqa_val).  
-00003210: 2d20 444f 4356 5141 2054 6573 7420 2864  - DOCVQA Test (d
-00003220: 6f63 7671 615f 7465 7374 290a 2d20 4665  ocvqa_test).- Fe
-00003230: 7272 6574 2028 6665 7272 6574 290a 2d20  rret (ferret).- 
-00003240: 466c 6963 6b72 3330 4b20 2866 6c69 636b  Flickr30K (flick
-00003250: 7233 306b 290a 2020 2d20 4665 7272 6574  r30k).  - Ferret
-00003260: 2054 6573 7420 2866 6572 7265 745f 7465   Test (ferret_te
-00003270: 7374 290a 2d20 4751 4120 2867 7161 290a  st).- GQA (gqa).
-00003280: 2d20 4861 6c6c 7573 696f 6e42 656e 6368  - HallusionBench
-00003290: 6d61 726b 2028 6861 6c6c 7573 696f 6e5f  mark (hallusion_
-000032a0: 6265 6e63 685f 696d 6167 6529 0a2d 2049  bench_image).- I
-000032b0: 6e66 6f67 7261 7068 6963 2056 5141 2028  nfographic VQA (
-000032c0: 696e 666f 5f76 7161 290a 2020 2d20 496e  info_vqa).  - In
-000032d0: 666f 6772 6170 6869 6320 5651 4120 5661  fographic VQA Va
-000032e0: 6c69 6461 7469 6f6e 2028 696e 666f 5f76  lidation (info_v
-000032f0: 7161 5f76 616c 290a 2020 2d20 496e 666f  qa_val).  - Info
-00003300: 6772 6170 6869 6320 5651 4120 5465 7374  graphic VQA Test
-00003310: 2028 696e 666f 5f76 7161 5f74 6573 7429   (info_vqa_test)
-00003320: 0a2d 204c 4c61 5641 2d42 656e 6368 2028  .- LLaVA-Bench (
-00003330: 6c6c 6176 615f 696e 5f74 6865 5f77 696c  llava_in_the_wil
-00003340: 6429 0a2d 204c 4c61 5641 2d42 656e 6368  d).- LLaVA-Bench
-00003350: 2d43 4f43 4f20 286c 6c61 7661 5f62 656e  -COCO (llava_ben
-00003360: 6368 5f63 6f63 6f29 0a2d 204d 6174 6856  ch_coco).- MathV
-00003370: 6973 7461 2028 6d61 7468 7669 7374 6129  ista (mathvista)
-00003380: 0a20 202d 204d 6174 6856 6973 7461 2056  .  - MathVista V
-00003390: 616c 6964 6174 696f 6e20 286d 6174 6876  alidation (mathv
-000033a0: 6973 7461 5f74 6573 746d 696e 6929 0a20  ista_testmini). 
-000033b0: 202d 204d 6174 6856 6973 7461 2054 6573   - MathVista Tes
-000033c0: 7420 286d 6174 6876 6973 7461 5f74 6573  t (mathvista_tes
-000033d0: 7429 0a2d 204d 4d42 656e 6368 2028 6d6d  t).- MMBench (mm
-000033e0: 6265 6e63 6829 0a20 202d 204d 4d42 656e  bench).  - MMBen
-000033f0: 6368 2045 6e67 6c69 7368 2028 6d6d 6265  ch English (mmbe
-00003400: 6e63 685f 656e 290a 2020 2020 2d20 4d4d  nch_en).    - MM
-00003410: 4265 6e63 6820 456e 676c 6973 6820 4465  Bench English De
-00003420: 7620 286d 6d62 656e 6368 5f65 6e5f 6465  v (mmbench_en_de
-00003430: 7629 0a20 2020 202d 204d 4d42 656e 6368  v).    - MMBench
-00003440: 2045 6e67 6c69 7368 2054 6573 7420 286d   English Test (m
-00003450: 6d62 656e 6368 5f65 6e5f 7465 7374 290a  mbench_en_test).
-00003460: 2020 2d20 4d4d 4265 6e63 6820 4368 696e    - MMBench Chin
-00003470: 6573 6520 286d 6d62 656e 6368 5f63 6e29  ese (mmbench_cn)
-00003480: 0a20 2020 202d 204d 4d42 656e 6368 2043  .    - MMBench C
-00003490: 6869 6e65 7365 2044 6576 2028 6d6d 6265  hinese Dev (mmbe
-000034a0: 6e63 685f 636e 5f64 6576 290a 2020 2020  nch_cn_dev).    
-000034b0: 2d20 4d4d 4265 6e63 6820 4368 696e 6573  - MMBench Chines
-000034c0: 6520 5465 7374 2028 6d6d 6265 6e63 685f  e Test (mmbench_
-000034d0: 636e 5f74 6573 7429 0a2d 204d 4d45 2028  cn_test).- MME (
-000034e0: 6d6d 6529 0a2d 204d 4d4d 5520 286d 6d6d  mme).- MMMU (mmm
-000034f0: 7529 0a20 202d 204d 4d4d 5520 5661 6c69  u).  - MMMU Vali
-00003500: 6461 7469 6f6e 2028 6d6d 6d75 5f76 616c  dation (mmmu_val
-00003510: 290a 2020 2d20 4d4d 4d55 2054 6573 7420  ).  - MMMU Test 
-00003520: 286d 6d6d 755f 7465 7374 290a 2d20 4d4d  (mmmu_test).- MM
-00003530: 5665 7420 286d 6d76 6574 290a 2d20 4d75  Vet (mmvet).- Mu
-00003540: 6c74 692d 446f 6356 5141 2028 6d75 6c74  lti-DocVQA (mult
-00003550: 6964 6f63 7671 6129 0a20 202d 204d 756c  idocvqa).  - Mul
-00003560: 7469 2d44 6f63 5651 4120 5661 6c69 6461  ti-DocVQA Valida
-00003570: 7469 6f6e 2028 6d75 6c74 6964 6f63 7671  tion (multidocvq
-00003580: 615f 7661 6c29 0a20 202d 204d 756c 7469  a_val).  - Multi
-00003590: 2d44 6f63 5651 4120 5465 7374 2028 6d75  -DocVQA Test (mu
-000035a0: 6c74 6964 6f63 7671 615f 7465 7374 290a  ltidocvqa_test).
-000035b0: 2d20 4e6f 4361 7073 2028 6e6f 6361 7073  - NoCaps (nocaps
-000035c0: 290a 2020 2d20 4e6f 4361 7073 2056 616c  ).  - NoCaps Val
-000035d0: 6964 6174 696f 6e20 286e 6f63 6170 735f  idation (nocaps_
-000035e0: 7661 6c29 0a20 202d 204e 6f43 6170 7320  val).  - NoCaps 
-000035f0: 5465 7374 2028 6e6f 6361 7073 5f74 6573  Test (nocaps_tes
-00003600: 7429 0a2d 204f 4b56 5141 2028 6f6b 5f76  t).- OKVQA (ok_v
-00003610: 7161 290a 2020 2d20 4f4b 5651 4120 5661  qa).  - OKVQA Va
-00003620: 6c69 6461 7469 6f6e 2032 3031 3420 286f  lidation 2014 (o
-00003630: 6b5f 7671 615f 7661 6c32 3031 3429 0a2d  k_vqa_val2014).-
-00003640: 2050 4f50 4520 2870 6f70 6529 0a2d 2052   POPE (pope).- R
-00003650: 6566 434f 434f 2028 7265 6663 6f63 6f29  efCOCO (refcoco)
-00003660: 0a20 2020 202d 2072 6566 636f 636f 5f73  .    - refcoco_s
-00003670: 6567 5f74 6573 740a 2020 2020 2d20 7265  eg_test.    - re
-00003680: 6663 6f63 6f5f 7365 675f 7661 6c0a 2020  fcoco_seg_val.  
-00003690: 2020 2d20 7265 6663 6f63 6f5f 7365 675f    - refcoco_seg_
-000036a0: 7465 7374 410a 2020 2020 2d20 7265 6663  testA.    - refc
-000036b0: 6f63 6f5f 7365 675f 7465 7374 420a 2020  oco_seg_testB.  
-000036c0: 2020 2d20 7265 6663 6f63 6f5f 6262 6f78    - refcoco_bbox
-000036d0: 5f74 6573 740a 2020 2020 2d20 7265 6663  _test.    - refc
-000036e0: 6f63 6f5f 6262 6f78 5f76 616c 0a20 2020  oco_bbox_val.   
-000036f0: 202d 2072 6566 636f 636f 5f62 626f 785f   - refcoco_bbox_
-00003700: 7465 7374 410a 2020 2020 2d20 7265 6663  testA.    - refc
-00003710: 6f63 6f5f 6262 6f78 5f74 6573 7442 0a2d  oco_bbox_testB.-
-00003720: 2052 6566 434f 434f 2b20 2872 6566 636f   RefCOCO+ (refco
-00003730: 636f 2b29 0a20 2020 202d 2072 6566 636f  co+).    - refco
-00003740: 636f 2b5f 7365 670a 2020 2020 2020 2020  co+_seg.        
-00003750: 2d20 7265 6663 6f63 6f2b 5f73 6567 5f76  - refcoco+_seg_v
-00003760: 616c 0a20 2020 2020 2020 202d 2072 6566  al.        - ref
-00003770: 636f 636f 2b5f 7365 675f 7465 7374 410a  coco+_seg_testA.
-00003780: 2020 2020 2020 2020 2d20 7265 6663 6f63          - refcoc
-00003790: 6f2b 5f73 6567 5f74 6573 7442 0a20 2020  o+_seg_testB.   
-000037a0: 202d 2072 6566 636f 636f 2b5f 6262 6f78   - refcoco+_bbox
-000037b0: 0a20 2020 2020 2020 202d 2072 6566 636f  .        - refco
-000037c0: 636f 2b5f 6262 6f78 5f76 616c 0a20 2020  co+_bbox_val.   
-000037d0: 2020 2020 202d 2072 6566 636f 636f 2b5f       - refcoco+_
-000037e0: 6262 6f78 5f74 6573 7441 0a20 2020 2020  bbox_testA.     
-000037f0: 2020 202d 2072 6566 636f 636f 2b5f 6262     - refcoco+_bb
-00003800: 6f78 5f74 6573 7442 0a2d 2052 6566 434f  ox_testB.- RefCO
-00003810: 434f 6720 2872 6566 636f 636f 6729 0a20  COg (refcocog). 
-00003820: 2020 202d 2072 6566 636f 636f 675f 7365     - refcocog_se
-00003830: 675f 7465 7374 0a20 2020 202d 2072 6566  g_test.    - ref
-00003840: 636f 636f 675f 7365 675f 7661 6c0a 2020  cocog_seg_val.  
-00003850: 2020 2d20 7265 6663 6f63 6f67 5f62 626f    - refcocog_bbo
-00003860: 785f 7465 7374 0a20 2020 202d 2072 6566  x_test.    - ref
-00003870: 636f 636f 675f 6262 6f78 5f76 616c 0a2d  cocog_bbox_val.-
-00003880: 2053 6369 656e 6365 5141 2028 7363 6965   ScienceQA (scie
-00003890: 6e63 6571 615f 6675 6c6c 290a 2020 2d20  nceqa_full).  - 
-000038a0: 5363 6965 6e63 6551 4120 4675 6c6c 2028  ScienceQA Full (
-000038b0: 7363 6965 6e63 6571 6129 0a20 202d 2053  scienceqa).  - S
-000038c0: 6369 656e 6365 5141 2049 4d47 2028 7363  cienceQA IMG (sc
-000038d0: 6965 6e63 6571 615f 696d 6729 0a2d 2053  ienceqa_img).- S
-000038e0: 6565 6442 656e 6368 2028 7365 6564 6265  eedBench (seedbe
-000038f0: 6e63 6829 0a2d 2053 6565 6442 656e 6368  nch).- SeedBench
-00003900: 2032 2028 7365 6564 6265 6e63 685f 3229   2 (seedbench_2)
-00003910: 0a2d 2053 542d 5651 4120 2873 7476 7161  .- ST-VQA (stvqa
-00003920: 290a 2d20 5465 7874 4361 7073 2028 7465  ).- TextCaps (te
-00003930: 7874 6361 7073 290a 2020 2d20 5465 7874  xtcaps).  - Text
-00003940: 4361 7073 2056 616c 6964 6174 696f 6e20  Caps Validation 
-00003950: 2874 6578 7463 6170 735f 7661 6c29 0a20  (textcaps_val). 
-00003960: 202d 2054 6578 7443 6170 7320 5465 7374   - TextCaps Test
-00003970: 2028 7465 7874 6361 7073 5f74 6573 7429   (textcaps_test)
-00003980: 0a2d 2054 6578 7456 5141 2028 7465 7874  .- TextVQA (text
-00003990: 7671 6129 0a20 202d 2054 6578 7456 5141  vqa).  - TextVQA
-000039a0: 2056 616c 6964 6174 696f 6e20 2874 6578   Validation (tex
-000039b0: 7476 7161 5f76 616c 290a 2020 2d20 5465  tvqa_val).  - Te
-000039c0: 7874 5651 4120 5465 7374 2028 7465 7874  xtVQA Test (text
-000039d0: 7671 615f 7465 7374 290a 2d20 5669 7a57  vqa_test).- VizW
-000039e0: 697a 5651 4120 2876 697a 7769 7a5f 7671  izVQA (vizwiz_vq
-000039f0: 6129 0a20 202d 2056 697a 5769 7a56 5141  a).  - VizWizVQA
-00003a00: 2056 616c 6964 6174 696f 6e20 2876 697a   Validation (viz
-00003a10: 7769 7a5f 7671 615f 7661 6c29 0a20 202d  wiz_vqa_val).  -
-00003a20: 2056 697a 5769 7a56 5141 2054 6573 7420   VizWizVQA Test 
-00003a30: 2876 697a 7769 7a5f 7671 615f 7465 7374  (vizwiz_vqa_test
-00003a40: 290a 2d20 5651 4176 3220 2876 7161 7632  ).- VQAv2 (vqav2
-00003a50: 290a 2020 2d20 5651 4176 3220 5661 6c69  ).  - VQAv2 Vali
-00003a60: 6461 7469 6f6e 2028 7671 6176 325f 7661  dation (vqav2_va
-00003a70: 6c29 0a20 202d 2056 5141 7632 2054 6573  l).  - VQAv2 Tes
-00003a80: 7420 2876 7161 7632 5f74 6573 7429 0a0a  t (vqav2_test)..
-00003a90: 2323 2044 6174 6173 6574 7320 746f 2062  ## Datasets to b
-00003aa0: 6520 6164 6465 6420 616e 6420 7465 7374  e added and test
-00003ab0: 6564 0a2d 2054 616c 6c79 5141 2028 7461  ed.- TallyQA (ta
-00003ac0: 6c6c 7971 6129 0a2d 2056 5352 2028 7673  llyqa).- VSR (vs
-00003ad0: 7229 0a2d 2057 696e 6f67 726f 756e 6420  r).- Winoground 
-00003ae0: 2877 696e 6f67 726f 756e 6429 0a2d 204e  (winoground).- N
-00003af0: 4c56 5232 2028 6e6c 7672 3229 0a2d 2052  LVR2 (nlvr2).- R
-00003b00: 6176 656e 4951 2d54 6573 7420 2872 6176  avenIQ-Test (rav
-00003b10: 656e 6971 290a 2d20 4963 6f6e 5141 2028  eniq).- IconQA (
-00003b20: 6963 6f6e 7161 290a 2d20 5669 7374 4265  iconqa).- VistBe
-00003b30: 6e63 6820 2876 6973 7462 656e 6368 290a  nch (vistbench).
-00003b40: 0a23 2041 6464 2043 7573 746f 6d69 7a65  .# Add Customize
-00003b50: 6420 4d6f 6465 6c20 616e 6420 4461 7461  d Model and Data
-00003b60: 7365 740a 0a50 6c65 6173 6520 7265 6665  set..Please refe
-00003b70: 7220 746f 206f 7572 205b 646f 6375 6d65  r to our [docume
-00003b80: 6e74 6174 696f 6e5d 2864 6f63 732f 5245  ntation](docs/RE
-00003b90: 4144 4d45 2e6d 6429 2e0a 0a23 2041 636b  ADME.md)...# Ack
-00003ba0: 6e6f 776c 6564 6765 6d65 6e74 0a0a 6c6d  nowledgement..lm
-00003bb0: 6d73 5f65 7661 6c20 6973 2061 2066 6f72  ms_eval is a for
-00003bc0: 6b20 6f66 205b 6c6d 2d65 7661 6c2d 6861  k of [lm-eval-ha
-00003bd0: 726e 6573 735d 2868 7474 7073 3a2f 2f67  rness](https://g
-00003be0: 6974 6875 622e 636f 6d2f 456c 6575 7468  ithub.com/Eleuth
-00003bf0: 6572 4149 2f6c 6d2d 6576 616c 7561 7469  erAI/lm-evaluati
-00003c00: 6f6e 2d68 6172 6e65 7373 292e 2057 6520  on-harness). We 
-00003c10: 7265 636f 6d6d 656e 6420 796f 7520 746f  recommend you to
-00003c20: 2072 6561 6420 7468 726f 7567 6820 7468   read through th
-00003c30: 6520 5b64 6f63 7320 6f66 206c 6d2d 6576  e [docs of lm-ev
-00003c40: 616c 2d68 6172 6e65 7373 5d28 6874 7470  al-harness](http
-00003c50: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f45  s://github.com/E
-00003c60: 6c65 7574 6865 7241 492f 6c6d 2d65 7661  leutherAI/lm-eva
-00003c70: 6c75 6174 696f 6e2d 6861 726e 6573 732f  luation-harness/
-00003c80: 7472 6565 2f6d 6169 6e2f 646f 6373 2920  tree/main/docs) 
-00003c90: 666f 7220 7265 6c65 7661 6e74 2069 6e66  for relevant inf
-00003ca0: 6f72 6d61 7469 6f6e 2e20 0a0a 4265 6c6f  ormation. ..Belo
-00003cb0: 7720 6172 6520 7468 6520 6368 616e 6765  w are the change
-00003cc0: 7320 7765 206d 6164 6520 746f 2074 6865  s we made to the
-00003cd0: 206f 7269 6769 6e61 6c20 4150 493a 0a2d   original API:.-
-00003ce0: 2042 7569 6c64 2063 6f6e 7465 7874 206e   Build context n
-00003cf0: 6f77 206f 6e6c 7920 7061 7373 2069 6e20  ow only pass in 
-00003d00: 6964 7820 616e 6420 7072 6f63 6573 7320  idx and process 
-00003d10: 696d 6167 6520 616e 6420 646f 6320 6475  image and doc du
-00003d20: 7269 6e67 2074 6865 206d 6f64 656c 2072  ring the model r
-00003d30: 6573 706f 6e64 696e 6720 7068 6173 652e  esponding phase.
-00003d40: 2054 6869 7320 6973 2064 7565 2074 6f20   This is due to 
-00003d50: 7468 6520 6661 6374 2074 6861 7420 6461  the fact that da
-00003d60: 7461 7365 7420 6e6f 7720 636f 6e74 6169  taset now contai
-00003d70: 6e73 206c 6f74 7320 6f66 2069 6d61 6765  ns lots of image
-00003d80: 7320 616e 6420 7765 2063 616e 2774 2073  s and we can't s
-00003d90: 746f 7265 2074 6865 6d20 696e 2074 6865  tore them in the
-00003da0: 2064 6f63 206c 696b 6520 7468 6520 6f72   doc like the or
-00003db0: 6967 696e 616c 206c 6d2d 6576 616c 2d68  iginal lm-eval-h
-00003dc0: 6172 6e65 7373 206f 7468 6572 2077 6973  arness other wis
-00003dd0: 6520 7468 6520 6370 7520 6d65 6d6f 7279  e the cpu memory
-00003de0: 2077 6f75 6c64 2065 7870 6c6f 6465 2e0a   would explode..
-00003df0: 2d20 496e 7374 616e 6365 2e61 7267 7320  - Instance.args 
-00003e00: 286c 6d6d 735f 6576 616c 2f61 7069 2f69  (lmms_eval/api/i
-00003e10: 6e73 7461 6e63 652e 7079 2920 6e6f 7720  nstance.py) now 
-00003e20: 636f 6e74 6169 6e73 2061 206c 6973 7420  contains a list 
-00003e30: 6f66 2069 6d61 6765 7320 746f 2062 6520  of images to be 
-00003e40: 696e 7075 7474 6564 2074 6f20 6c6d 6d73  inputted to lmms
-00003e50: 2e0a 2d20 6c6d 2d65 7661 6c2d 6861 726e  ..- lm-eval-harn
-00003e60: 6573 7320 7375 7070 6f72 7473 2061 6c6c  ess supports all
-00003e70: 2048 4620 6c61 6e67 7561 6765 206d 6f64   HF language mod
-00003e80: 656c 7320 6173 2073 696e 676c 6520 6d6f  els as single mo
-00003e90: 6465 6c20 636c 6173 732e 2043 7572 7265  del class. Curre
-00003ea0: 6e74 6c79 2074 6869 7320 6973 206e 6f74  ntly this is not
-00003eb0: 2070 6f73 7369 626c 6520 6f66 206c 6d6d   possible of lmm
-00003ec0: 7320 6265 6361 7573 6520 7468 6520 696e  s because the in
-00003ed0: 7075 742f 6f75 7470 7574 2066 6f72 6d61  put/output forma
-00003ee0: 7420 6f66 206c 6d6d 7320 696e 2048 4620  t of lmms in HF 
-00003ef0: 6172 6520 6e6f 7420 7965 7420 756e 6966  are not yet unif
-00003f00: 6965 642e 2054 6865 7265 7266 6f72 652c  ied. Thererfore,
-00003f10: 2077 6520 6861 7665 2074 6f20 6372 6561   we have to crea
-00003f20: 7465 2061 206e 6577 2063 6c61 7373 2066  te a new class f
-00003f30: 6f72 2065 6163 6820 6c6d 6d73 206d 6f64  or each lmms mod
-00003f40: 656c 2e20 5468 6973 2069 7320 6e6f 7420  el. This is not 
-00003f50: 6964 6561 6c20 616e 6420 7765 2077 696c  ideal and we wil
-00003f60: 6c20 7472 7920 746f 2075 6e69 6679 2074  l try to unify t
-00003f70: 6865 6d20 696e 2074 6865 2066 7574 7572  hem in the futur
-00003f80: 652e 0a0a 5765 2061 6c73 6f20 7468 616e  e...We also than
-00003f90: 6b3a 0a2d 205b 5869 616e 6720 5975 655d  k:.- [Xiang Yue]
-00003fa0: 2868 7474 7073 3a2f 2f78 6961 6e67 7975  (https://xiangyu
-00003fb0: 6539 3630 372e 6769 7468 7562 2e69 6f2f  e9607.github.io/
-00003fc0: 292c 205b 4a69 6e67 6b61 6e67 2059 616e  ), [Jingkang Yan
-00003fd0: 675d 2868 7474 7073 3a2f 2f6a 696e 676b  g](https://jingk
-00003fe0: 616e 6735 302e 6769 7468 7562 2e69 6f2f  ang50.github.io/
-00003ff0: 292c 205b 446f 6e67 2047 756f 5d28 6874  ), [Dong Guo](ht
-00004000: 7470 733a 2f2f 7777 772e 6c69 6e6b 6564  tps://www.linked
-00004010: 696e 2e63 6f6d 2f69 6e2f 646f 6e67 6775  in.com/in/donggu
-00004020: 6f73 6574 2f29 2061 6e64 205b 5368 656e  oset/) and [Shen
-00004030: 6720 5368 656e 5d28 6874 7470 733a 2f2f  g Shen](https://
-00004040: 7369 6e63 6572 6173 732e 6769 7468 7562  sincerass.github
-00004050: 2e69 6f2f 2920 666f 7220 6561 726c 7920  .io/) for early 
-00004060: 6469 7363 7573 7369 6f6e 2061 6e64 2074  discussion and t
-00004070: 6573 7469 6e67 2e0a 0a23 2320 4369 7461  esting...## Cita
-00004080: 7469 6f6e 730a 0a60 6060 7368 656c 6c0a  tions..```shell.
-00004090: 406d 6973 637b 6c6d 6d73 5f65 7661 6c32  @misc{lmms_eval2
-000040a0: 3032 342c 0a20 2020 2074 6974 6c65 3d7b  024,.    title={
-000040b0: 4c4d 4d73 2d45 7661 6c3a 2041 6363 656c  LMMs-Eval: Accel
-000040c0: 6572 6174 696e 6720 7468 6520 4465 7665  erating the Deve
-000040d0: 6c6f 706d 656e 7420 6f66 204c 6172 6765  lopment of Large
-000040e0: 204d 756c 7469 6d6f 616c 204d 6f64 656c   Multimoal Model
-000040f0: 737d 2c0a 2020 2020 7572 6c3d 7b68 7474  s},.    url={htt
-00004100: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00004110: 4576 6f6c 7669 6e67 4c4d 4d73 2d4c 6162  EvolvingLMMs-Lab
-00004120: 2f6c 6d6d 732d 6576 616c 7d2c 0a20 2020  /lmms-eval},.   
-00004130: 2061 7574 686f 723d 7b42 6f20 4c69 2a2c   author={Bo Li*,
-00004140: 2050 6569 7975 616e 205a 6861 6e67 2a2c   Peiyuan Zhang*,
-00004150: 204b 6169 6368 656e 205a 6861 6e67 2a2c   Kaichen Zhang*,
-00004160: 2046 616e 7969 2050 752a 2c20 5869 6e72   Fanyi Pu*, Xinr
-00004170: 756e 2044 752c 2059 7568 616f 2044 6f6e  un Du, Yuhao Don
-00004180: 672c 2048 616f 7469 616e 204c 6975 2c20  g, Haotian Liu, 
-00004190: 5975 616e 6861 6e20 5a68 616e 672c 2047  Yuanhan Zhang, G
-000041a0: 6520 5a68 616e 672c 2043 6875 6e79 7561  e Zhang, Chunyua
-000041b0: 6e20 4c69 2061 6e64 205a 6977 6569 204c  n Li and Ziwei L
-000041c0: 6975 7d2c 0a20 2020 2070 7562 6c69 7368  iu},.    publish
-000041d0: 6572 2020 2020 3d20 7b5a 656e 6f64 6f7d  er    = {Zenodo}
-000041e0: 2c0a 2020 2020 7665 7273 696f 6e20 2020  ,.    version   
-000041f0: 2020 203d 207b 7630 2e31 2e30 7d2c 0a20     = {v0.1.0},. 
-00004200: 2020 206d 6f6e 7468 3d7b 4d61 7263 687d     month={March}
-00004210: 2c0a 2020 2020 7965 6172 3d7b 3230 3234  ,.    year={2024
-00004220: 7d0a 7d0a 6060 600a                      }.}.```.
+00000430: 616e 7366 6f72 6d65 7273 0a52 6571 7569  ansformers.Requi
+00000440: 7265 732d 4469 7374 3a20 7a73 7461 6e64  res-Dist: zstand
+00000450: 6172 640a 5265 7175 6972 6573 2d44 6973  ard.Requires-Dis
+00000460: 743a 2070 696c 6c6f 770a 5265 7175 6972  t: pillow.Requir
+00000470: 6573 2d44 6973 743a 2070 7979 616d 6c0a  es-Dist: pyyaml.
+00000480: 5265 7175 6972 6573 2d44 6973 743a 2073  Requires-Dist: s
+00000490: 796d 7079 0a52 6571 7569 7265 732d 4469  ympy.Requires-Di
+000004a0: 7374 3a20 6d70 6d61 7468 0a52 6571 7569  st: mpmath.Requi
+000004b0: 7265 732d 4469 7374 3a20 4a69 6e6a 6132  res-Dist: Jinja2
+000004c0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+000004d0: 6f70 656e 7079 786c 0a52 6571 7569 7265  openpyxl.Require
+000004e0: 732d 4469 7374 3a20 4c65 7665 6e73 6874  s-Dist: Levensht
+000004f0: 6569 6e0a 5265 7175 6972 6573 2d44 6973  ein.Requires-Dis
+00000500: 743a 2068 665f 7472 616e 7366 6572 0a52  t: hf_transfer.R
+00000510: 6571 7569 7265 732d 4469 7374 3a20 7465  equires-Dist: te
+00000520: 6e61 6369 7479 0a52 6571 7569 7265 732d  nacity.Requires-
+00000530: 4469 7374 3a20 7761 6e64 623e 3d30 2e31  Dist: wandb>=0.1
+00000540: 362e 300a 5265 7175 6972 6573 2d44 6973  6.0.Requires-Dis
+00000550: 743a 2074 7261 6e73 666f 726d 6572 732d  t: transformers-
+00000560: 7374 7265 616d 2d67 656e 6572 6174 6f72  stream-generator
+00000570: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000580: 7469 6b74 6f6b 656e 0a52 6571 7569 7265  tiktoken.Require
+00000590: 732d 4469 7374 3a20 7072 652d 636f 6d6d  s-Dist: pre-comm
+000005a0: 6974 0a52 6571 7569 7265 732d 4469 7374  it.Requires-Dist
+000005b0: 3a20 7079 6461 6e74 6963 0a0a 3c70 2061  : pydantic..<p a
+000005c0: 6c69 676e 3d22 6365 6e74 6572 2220 7769  lign="center" wi
+000005d0: 6474 683d 2231 3030 2522 3e0a 3c69 6d67  dth="100%">.<img
+000005e0: 2073 7263 3d22 6874 7470 733a 2f2f 692e   src="https://i.
+000005f0: 706f 7374 696d 672e 6363 2f67 3051 5267  postimg.cc/g0QRg
+00000600: 4d56 762f 5758 3230 3234 3032 3238 2d31  MVv/WX20240228-1
+00000610: 3133 3333 372d 3278 2e70 6e67 2220 2077  13337-2x.png"  w
+00000620: 6964 7468 3d22 3130 3025 2220 6865 6967  idth="100%" heig
+00000630: 6874 3d22 3730 2522 3e0a 3c2f 703e 0a0a  ht="70%">.</p>..
+00000640: 2320 5468 6520 4576 616c 7561 7469 6f6e  # The Evaluation
+00000650: 2053 7569 7465 206f 6620 4c61 7267 6520   Suite of Large 
+00000660: 4d75 6c74 696d 6f64 616c 204d 6f64 656c  Multimodal Model
+00000670: 7320 0a0a 3e20 4163 6365 6c65 7261 7469  s ..> Accelerati
+00000680: 6e67 2074 6865 2064 6576 656c 6f70 6d65  ng the developme
+00000690: 6e74 206f 6620 6c61 7267 6520 6d75 6c74  nt of large mult
+000006a0: 696d 6f64 616c 206d 6f64 656c 7320 284c  imodal models (L
+000006b0: 4d4d 7329 2077 6974 6820 606c 6d6d 732d  MMs) with `lmms-
+000006c0: 6576 616c 600a 0af0 9f8f a020 5b48 6f6d  eval`...... [Hom
+000006d0: 6570 6167 655d 2868 7474 7073 3a2f 2f6c  epage](https://l
+000006e0: 6d6d 732d 6c61 622e 6769 7468 7562 2e69  mms-lab.github.i
+000006f0: 6f2f 2920 7c20 20f0 9f8e 8920 5b42 6c6f  o/) |  .... [Blo
+00000700: 675d 2868 7474 7073 3a2f 2f6c 6d6d 732d  g](https://lmms-
+00000710: 6c61 622e 6769 7468 7562 2e69 6f2f 6c6d  lab.github.io/lm
+00000720: 6d73 2d65 7661 6c2d 626c 6f67 2f6c 6d6d  ms-eval-blog/lmm
+00000730: 732d 6576 616c 2d30 2e31 2f29 207c 20f0  s-eval-0.1/) | .
+00000740: 9f93 9a20 5b44 6f63 756d 656e 7461 7469  ... [Documentati
+00000750: 6f6e 5d28 646f 6373 2f52 4541 444d 452e  on](docs/README.
+00000760: 6d64 2920 7c20 f09f a497 205b 4875 6767  md) | .... [Hugg
+00000770: 696e 6766 6163 6520 4461 7461 7365 7473  ingface Datasets
+00000780: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
+00000790: 6766 6163 652e 636f 2f6c 6d6d 732d 6c61  gface.co/lmms-la
+000007a0: 6229 207c 203c 6120 6872 6566 3d22 6874  b) | <a href="ht
+000007b0: 7470 733a 2f2f 656d 6f6a 692e 6767 2f65  tps://emoji.gg/e
+000007c0: 6d6f 6a69 2f31 3638 342d 6469 7363 6f72  moji/1684-discor
+000007d0: 642d 7468 7265 6164 223e 3c69 6d67 2073  d-thread"><img s
+000007e0: 7263 3d22 6874 7470 733a 2f2f 6364 6e33  rc="https://cdn3
+000007f0: 2e65 6d6f 6a69 2e67 672f 656d 6f6a 6973  .emoji.gg/emojis
+00000800: 2f31 3638 342d 6469 7363 6f72 642d 7468  /1684-discord-th
+00000810: 7265 6164 2e70 6e67 2220 7769 6474 683d  read.png" width=
+00000820: 2231 3470 7822 2068 6569 6768 743d 2231  "14px" height="1
+00000830: 3470 7822 2061 6c74 3d22 4469 7363 6f72  4px" alt="Discor
+00000840: 645f 5468 7265 6164 223e 3c2f 613e 205b  d_Thread"></a> [
+00000850: 6469 7363 6f72 642f 6c6d 6d73 2d65 7661  discord/lmms-eva
+00000860: 6c5d 2868 7474 7073 3a2f 2f64 6973 636f  l](https://disco
+00000870: 7264 2e67 672f 7a64 6b77 4b55 7172 5079  rd.gg/zdkwKUqrPy
+00000880: 290a 0a0a 496e 2074 6f64 6179 2773 2077  )...In today's w
+00000890: 6f72 6c64 2c20 7765 2772 6520 6f6e 2061  orld, we're on a
+000008a0: 6e20 6578 6369 7469 6e67 206a 6f75 726e  n exciting journ
+000008b0: 6579 2074 6f77 6172 6420 6372 6561 7469  ey toward creati
+000008c0: 6e67 2041 7274 6966 6963 6961 6c20 4765  ng Artificial Ge
+000008d0: 6e65 7261 6c20 496e 7465 6c6c 6967 656e  neral Intelligen
+000008e0: 6365 2028 4147 4929 2c20 6d75 6368 206c  ce (AGI), much l
+000008f0: 696b 6520 7468 6520 656e 7468 7573 6961  ike the enthusia
+00000900: 736d 206f 6620 7468 6520 3139 3630 7320  sm of the 1960s 
+00000910: 6d6f 6f6e 206c 616e 6469 6e67 2e20 5468  moon landing. Th
+00000920: 6973 206a 6f75 726e 6579 2069 7320 706f  is journey is po
+00000930: 7765 7265 6420 6279 2061 6476 616e 6365  wered by advance
+00000940: 6420 6c61 7267 6520 6c61 6e67 7561 6765  d large language
+00000950: 206d 6f64 656c 7320 284c 4c4d 7329 2061   models (LLMs) a
+00000960: 6e64 206c 6172 6765 206d 756c 7469 6d6f  nd large multimo
+00000970: 6461 6c20 6d6f 6465 6c73 2028 4c4d 4d73  dal models (LMMs
+00000980: 292c 2077 6869 6368 2061 7265 2063 6f6d  ), which are com
+00000990: 706c 6578 2073 7973 7465 6d73 2063 6170  plex systems cap
+000009a0: 6162 6c65 206f 6620 756e 6465 7273 7461  able of understa
+000009b0: 6e64 696e 672c 206c 6561 726e 696e 672c  nding, learning,
+000009c0: 2061 6e64 2070 6572 666f 726d 696e 6720   and performing 
+000009d0: 6120 7769 6465 2076 6172 6965 7479 206f  a wide variety o
+000009e0: 6620 6875 6d61 6e20 7461 736b 732e 2054  f human tasks. T
+000009f0: 6865 7365 2061 6476 616e 6365 6d65 6e74  hese advancement
+00000a00: 7320 6272 696e 6720 7573 2063 6c6f 7365  s bring us close
+00000a10: 7220 746f 2061 6368 6965 7669 6e67 2041  r to achieving A
+00000a20: 4749 2e0a 0a54 6f20 6761 7567 6520 686f  GI...To gauge ho
+00000a30: 7720 6164 7661 6e63 6564 2074 6865 7365  w advanced these
+00000a40: 206d 6f64 656c 7320 6172 652c 2077 6520   models are, we 
+00000a50: 7573 6520 6120 7661 7269 6574 7920 6f66  use a variety of
+00000a60: 2065 7661 6c75 6174 696f 6e20 6265 6e63   evaluation benc
+00000a70: 686d 6172 6b73 2e20 5468 6573 6520 6265  hmarks. These be
+00000a80: 6e63 686d 6172 6b73 2061 7265 2074 6f6f  nchmarks are too
+00000a90: 6c73 2074 6861 7420 6865 6c70 2075 7320  ls that help us 
+00000aa0: 756e 6465 7273 7461 6e64 2074 6865 2063  understand the c
+00000ab0: 6170 6162 696c 6974 6965 7320 6f66 2074  apabilities of t
+00000ac0: 6865 7365 206d 6f64 656c 732c 2073 686f  hese models, sho
+00000ad0: 7769 6e67 2075 7320 686f 7720 636c 6f73  wing us how clos
+00000ae0: 6520 7765 2061 7265 2074 6f20 6163 6869  e we are to achi
+00000af0: 6576 696e 6720 4147 492e 2048 6f77 6576  eving AGI. Howev
+00000b00: 6572 2c20 6669 6e64 696e 6720 616e 6420  er, finding and 
+00000b10: 7573 696e 6720 7468 6573 6520 6265 6e63  using these benc
+00000b20: 686d 6172 6b73 2069 7320 6120 6269 6720  hmarks is a big 
+00000b30: 6368 616c 6c65 6e67 652e 2054 6865 206e  challenge. The n
+00000b40: 6563 6573 7361 7279 2062 656e 6368 6d61  ecessary benchma
+00000b50: 726b 7320 616e 6420 6461 7461 7365 7473  rks and datasets
+00000b60: 2061 7265 2073 7072 6561 6420 6f75 7420   are spread out 
+00000b70: 616e 6420 6869 6464 656e 2069 6e20 7661  and hidden in va
+00000b80: 7269 6f75 7320 706c 6163 6573 206c 696b  rious places lik
+00000b90: 6520 476f 6f67 6c65 2044 7269 7665 2c20  e Google Drive, 
+00000ba0: 4472 6f70 626f 782c 2061 6e64 2064 6966  Dropbox, and dif
+00000bb0: 6665 7265 6e74 2073 6368 6f6f 6c20 616e  ferent school an
+00000bc0: 6420 7265 7365 6172 6368 206c 6162 2077  d research lab w
+00000bd0: 6562 7369 7465 732e 2049 7420 6665 656c  ebsites. It feel
+00000be0: 7320 6c69 6b65 2077 6527 7265 206f 6e20  s like we're on 
+00000bf0: 6120 7472 6561 7375 7265 2068 756e 742c  a treasure hunt,
+00000c00: 2062 7574 2074 6865 206d 6170 7320 6172   but the maps ar
+00000c10: 6520 7363 6174 7465 7265 6420 6576 6572  e scattered ever
+00000c20: 7977 6865 7265 2e0a 0a49 6e20 7468 6520  ywhere...In the 
+00000c30: 6669 656c 6420 6f66 206c 616e 6775 6167  field of languag
+00000c40: 6520 6d6f 6465 6c73 2c20 7468 6572 6520  e models, there 
+00000c50: 6861 7320 6265 656e 2061 2076 616c 7561  has been a valua
+00000c60: 626c 6520 7072 6563 6564 656e 7420 7365  ble precedent se
+00000c70: 7420 6279 2074 6865 2077 6f72 6b20 6f66  t by the work of
+00000c80: 205b 6c6d 2d65 7661 6c75 6174 696f 6e2d   [lm-evaluation-
+00000c90: 6861 726e 6573 735d 2868 7474 7073 3a2f  harness](https:/
+00000ca0: 2f67 6974 6875 622e 636f 6d2f 456c 6575  /github.com/Eleu
+00000cb0: 7468 6572 4149 2f6c 6d2d 6576 616c 7561  therAI/lm-evalua
+00000cc0: 7469 6f6e 2d68 6172 6e65 7373 292e 2054  tion-harness). T
+00000cd0: 6865 7920 6f66 6665 7220 696e 7465 6772  hey offer integr
+00000ce0: 6174 6564 2064 6174 6120 616e 6420 6d6f  ated data and mo
+00000cf0: 6465 6c20 696e 7465 7266 6163 6573 2c20  del interfaces, 
+00000d00: 656e 6162 6c69 6e67 2072 6170 6964 2065  enabling rapid e
+00000d10: 7661 6c75 6174 696f 6e20 6f66 206c 616e  valuation of lan
+00000d20: 6775 6167 6520 6d6f 6465 6c73 2061 6e64  guage models and
+00000d30: 2073 6572 7669 6e67 2061 7320 7468 6520   serving as the 
+00000d40: 6261 636b 656e 6420 7375 7070 6f72 7420  backend support 
+00000d50: 6672 616d 6577 6f72 6b20 666f 7220 7468  framework for th
+00000d60: 6520 5b6f 7065 6e2d 6c6c 6d2d 6c65 6164  e [open-llm-lead
+00000d70: 6572 626f 6172 645d 2868 7474 7073 3a2f  erboard](https:/
+00000d80: 2f68 7567 6769 6e67 6661 6365 2e63 6f2f  /huggingface.co/
+00000d90: 7370 6163 6573 2f48 7567 6769 6e67 4661  spaces/HuggingFa
+00000da0: 6365 4834 2f6f 7065 6e5f 6c6c 6d5f 6c65  ceH4/open_llm_le
+00000db0: 6164 6572 626f 6172 6429 2c20 616e 6420  aderboard), and 
+00000dc0: 6861 7320 6772 6164 7561 6c6c 7920 6265  has gradually be
+00000dd0: 636f 6d65 2074 6865 2075 6e64 6572 6c79  come the underly
+00000de0: 696e 6720 6563 6f73 7973 7465 6d20 6f66  ing ecosystem of
+00000df0: 2074 6865 2065 7261 206f 6620 666f 756e   the era of foun
+00000e00: 6461 7469 6f6e 206d 6f64 656c 732e 0a0a  dation models...
+00000e10: 486f 7765 7665 722c 2074 686f 7567 6820  However, though 
+00000e20: 7468 6572 6520 6172 6520 6d61 6e79 206e  there are many n
+00000e30: 6577 2065 7661 6c75 6174 696f 6e20 6461  ew evaluation da
+00000e40: 7461 7365 7473 2061 7265 2072 6563 656e  tasets are recen
+00000e50: 746c 7920 7072 6f70 6f73 6564 2c20 7468  tly proposed, th
+00000e60: 6520 6566 6669 6369 656e 7420 6576 616c  e efficient eval
+00000e70: 7561 7469 6f6e 2070 6970 656c 696e 6520  uation pipeline 
+00000e80: 6f66 204c 4d4d 2069 7320 7374 696c 6c20  of LMM is still 
+00000e90: 696e 2069 7473 2069 6e66 616e 6379 2c20  in its infancy, 
+00000ea0: 616e 6420 7468 6572 6520 6973 206e 6f20  and there is no 
+00000eb0: 756e 6966 6965 6420 6576 616c 7561 7469  unified evaluati
+00000ec0: 6f6e 2066 7261 6d65 776f 726b 2074 6861  on framework tha
+00000ed0: 7420 6361 6e20 6265 2075 7365 6420 746f  t can be used to
+00000ee0: 2065 7661 6c75 6174 6520 4c4d 4d20 6163   evaluate LMM ac
+00000ef0: 726f 7373 2061 2077 6964 6520 7261 6e67  ross a wide rang
+00000f00: 6520 6f66 2064 6174 6173 6574 732e 2054  e of datasets. T
+00000f10: 6f20 6164 6472 6573 7320 7468 6973 2063  o address this c
+00000f20: 6861 6c6c 656e 6765 2c20 7765 2069 6e74  hallenge, we int
+00000f30: 726f 6475 6365 202a 2a6c 6d6d 732d 6576  roduce **lmms-ev
+00000f40: 616c 2a2a 2c20 616e 2065 7661 6c75 6174  al**, an evaluat
+00000f50: 696f 6e20 6672 616d 6577 6f72 6b20 6d65  ion framework me
+00000f60: 7469 6375 6c6f 7573 6c79 2063 7261 6674  ticulously craft
+00000f70: 6564 2066 6f72 2063 6f6e 7369 7374 656e  ed for consisten
+00000f80: 7420 616e 6420 6566 6669 6369 656e 7420  t and efficient 
+00000f90: 6576 616c 7561 7469 6f6e 206f 6620 4c4d  evaluation of LM
+00000fa0: 4d2e 0a0a 5765 2068 756d 626c 7920 6f62  M...We humbly ob
+00000fb0: 736f 7262 6564 2074 6865 2065 7871 7569  sorbed the exqui
+00000fc0: 7369 7465 2061 6e64 2065 6666 6963 6965  site and efficie
+00000fd0: 6e74 2064 6573 6967 6e20 6f66 205b 6c6d  nt design of [lm
+00000fe0: 2d65 7661 6c75 6174 696f 6e2d 6861 726e  -evaluation-harn
+00000ff0: 6573 735d 2868 7474 7073 3a2f 2f67 6974  ess](https://git
+00001000: 6875 622e 636f 6d2f 456c 6575 7468 6572  hub.com/Eleuther
+00001010: 4149 2f6c 6d2d 6576 616c 7561 7469 6f6e  AI/lm-evaluation
+00001020: 2d68 6172 6e65 7373 292e 2042 7569 6c64  -harness). Build
+00001030: 696e 6720 7570 6f6e 2069 7473 2066 6f75  ing upon its fou
+00001040: 6e64 6174 696f 6e2c 2077 6520 696d 706c  ndation, we impl
+00001050: 656d 656e 7465 6420 6f75 7220 606c 6d6d  emented our `lmm
+00001060: 732d 6576 616c 6020 6672 616d 6577 6f72  s-eval` framewor
+00001070: 6b20 7769 7468 2070 6572 666f 726d 616e  k with performan
+00001080: 6365 206f 7074 696d 697a 6174 696f 6e73  ce optimizations
+00001090: 2073 7065 6369 6669 6361 6c6c 7920 666f   specifically fo
+000010a0: 7220 4c4d 4d73 2e0a 0a23 2320 4e65 6365  r LMMs...## Nece
+000010b0: 7373 6974 7920 6f66 206c 6d6d 732d 6576  ssity of lmms-ev
+000010c0: 616c 0a0a 5765 2062 656c 6965 7665 206f  al..We believe o
+000010d0: 7572 2065 6666 6f72 7420 636f 756c 6420  ur effort could 
+000010e0: 7072 6f76 6964 6520 616e 2065 6666 6963  provide an effic
+000010f0: 6965 6e74 2069 6e74 6572 6661 6365 2066  ient interface f
+00001100: 6f72 2074 6865 2064 6574 6169 6c65 6420  or the detailed 
+00001110: 636f 6d70 6172 6973 6f6e 206f 6620 7075  comparison of pu
+00001120: 626c 6963 6c79 2061 7661 696c 6162 6c65  blicly available
+00001130: 206d 6f64 656c 7320 746f 2064 6973 6365   models to disce
+00001140: 726e 2074 6865 6972 2073 7472 656e 6774  rn their strengt
+00001150: 6873 2061 6e64 2077 6561 6b6e 6573 7365  hs and weaknesse
+00001160: 732e 2049 7427 7320 616c 736f 2075 7365  s. It's also use
+00001170: 6675 6c20 666f 7220 7265 7365 6172 6368  ful for research
+00001180: 2069 6e73 7469 7475 7469 6f6e 7320 616e   institutions an
+00001190: 6420 7072 6f64 7563 7469 6f6e 2d6f 7269  d production-ori
+000011a0: 656e 7465 6420 636f 6d70 616e 6965 7320  ented companies 
+000011b0: 746f 2061 6363 656c 6572 6174 6520 7468  to accelerate th
+000011c0: 6520 6465 7665 6c6f 706d 656e 7420 6f66  e development of
+000011d0: 206c 6172 6765 206d 756c 7469 6d6f 6461   large multimoda
+000011e0: 6c20 6d6f 6465 6c73 2e20 5769 7468 2074  l models. With t
+000011f0: 6865 2060 6c6d 6d73 2d65 7661 6c60 2c20  he `lmms-eval`, 
+00001200: 7765 2068 6176 6520 7369 676e 6966 6963  we have signific
+00001210: 616e 746c 7920 6163 6365 6c65 7261 7465  antly accelerate
+00001220: 6420 7468 6520 6c69 6665 6379 636c 6520  d the lifecycle 
+00001230: 6f66 206d 6f64 656c 2069 7465 7261 7469  of model iterati
+00001240: 6f6e 2e20 496e 7369 6465 2074 6865 204c  on. Inside the L
+00001250: 4c61 5641 2074 6561 6d2c 2074 6865 2075  LaVA team, the u
+00001260: 7469 6c69 7a61 7469 6f6e 206f 6620 606c  tilization of `l
+00001270: 6d6d 732d 6576 616c 6020 6c61 7267 656c  mms-eval` largel
+00001280: 7920 696d 7072 6f76 6573 2074 6865 2065  y improves the e
+00001290: 6666 6963 6965 6e63 7920 6f66 2074 6865  fficiency of the
+000012a0: 206d 6f64 656c 2064 6576 656c 6f70 6d65   model developme
+000012b0: 6e74 2063 7963 6c65 2c20 6173 2077 6520  nt cycle, as we 
+000012c0: 6172 6520 6162 6c65 2074 6f20 6576 616c  are able to eval
+000012d0: 7561 7465 2077 6565 6b6c 7920 7472 6169  uate weekly trai
+000012e0: 6e65 6420 6875 6e64 7265 6473 206f 6620  ned hundreds of 
+000012f0: 6368 6563 6b70 6f69 6e74 7320 6f6e 2032  checkpoints on 2
+00001300: 302d 3330 2064 6174 6173 6574 732c 2069  0-30 datasets, i
+00001310: 6465 6e74 6966 7969 6e67 2074 6865 2073  dentifying the s
+00001320: 7472 656e 6774 6873 2061 6e64 2077 6561  trengths and wea
+00001330: 6b6e 6573 7365 732c 2061 6e64 2074 6865  knesses, and the
+00001340: 6e20 6d61 6b65 2074 6172 6765 7465 6420  n make targeted 
+00001350: 696d 7072 6f76 656d 656e 7473 2e0a 0a23  improvements...#
+00001360: 2041 6e6e 6f75 6365 6d65 6e74 0a0a 2323   Annoucement..##
+00001370: 2043 6f6e 7472 6962 7574 696f 6e20 4775   Contribution Gu
+00001380: 6964 616e 6365 0a0a 5765 2776 6520 6164  idance..We've ad
+00001390: 6465 6420 6775 6964 616e 6365 206f 6e20  ded guidance on 
+000013a0: 636f 6e74 7269 6275 7469 6e67 206e 6577  contributing new
+000013b0: 2064 6174 6173 6574 7320 616e 6420 6d6f   datasets and mo
+000013c0: 6465 6c73 2e20 506c 6561 7365 2072 6566  dels. Please ref
+000013d0: 6572 2074 6f20 6f75 7220 5b64 6f63 756d  er to our [docum
+000013e0: 656e 7461 7469 6f6e 5d28 646f 6373 2f52  entation](docs/R
+000013f0: 4541 444d 452e 6d64 292e 2049 6620 796f  EADME.md). If yo
+00001400: 7520 6e65 6564 2061 7373 6973 7461 6e63  u need assistanc
+00001410: 652c 2079 6f75 2063 616e 2063 6f6e 7461  e, you can conta
+00001420: 6374 2075 7320 7669 6120 5b64 6973 636f  ct us via [disco
+00001430: 7264 2f6c 6d6d 732d 6576 616c 5d28 6874  rd/lmms-eval](ht
+00001440: 7470 733a 2f2f 6469 7363 6f72 642e 6767  tps://discord.gg
+00001450: 2f65 6241 4d47 5373 5329 2e0a 0a23 2320  /ebAMGSsS)...## 
+00001460: 7630 2e31 2e30 2052 656c 6561 7365 640a  v0.1.0 Released.
+00001470: 0a54 6865 2066 6972 7374 2076 6572 7369  .The first versi
+00001480: 6f6e 206f 6620 7468 6520 606c 6d6d 732d  on of the `lmms-
+00001490: 6576 616c 6020 6973 2072 656c 6561 7365  eval` is release
+000014a0: 642e 2057 6520 6172 6520 776f 726b 696e  d. We are workin
+000014b0: 6720 6f6e 2070 726f 7669 6469 6e67 2061  g on providing a
+000014c0: 6e20 6f6e 652d 636f 6d6d 616e 6420 6576  n one-command ev
+000014d0: 616c 7561 7469 6f6e 2073 7569 7465 2066  aluation suite f
+000014e0: 6f72 2061 6363 656c 6572 6174 696e 6720  or accelerating 
+000014f0: 7468 6520 6465 7665 6c6f 706d 656e 7420  the development 
+00001500: 6f66 204c 4d4d 732e 200a 0a3e 2049 6e20  of LMMs. ..> In 
+00001510: 5b4c 4c61 5641 204e 6578 745d 2868 7474  [LLaVA Next](htt
+00001520: 7073 3a2f 2f6c 6c61 7661 2d76 6c2e 6769  ps://llava-vl.gi
+00001530: 7468 7562 2e69 6f2f 626c 6f67 2f32 3032  thub.io/blog/202
+00001540: 342d 3031 2d33 302d 6c6c 6176 612d 6e65  4-01-30-llava-ne
+00001550: 7874 2f29 2064 6576 656c 6f70 6d65 6e74  xt/) development
+00001560: 2c20 7765 2069 6e74 6572 6e61 6c6c 7920  , we internally 
+00001570: 7574 696c 697a 6520 7468 6973 2073 7569  utilize this sui
+00001580: 7465 2074 6f20 6576 616c 7561 7465 2074  te to evaluate t
+00001590: 6865 206d 756c 7469 706c 6520 6469 6666  he multiple diff
+000015a0: 6572 656e 7420 6d6f 6465 6c20 7665 7273  erent model vers
+000015b0: 696f 6e73 206f 6e20 7661 7269 6f75 7320  ions on various 
+000015c0: 6461 7461 7365 7473 2e20 4974 2073 6967  datasets. It sig
+000015d0: 6e69 6669 6361 6e74 6c79 2061 6363 656c  nificantly accel
+000015e0: 6572 6174 6573 2074 6865 206d 6f64 656c  erates the model
+000015f0: 2064 6576 656c 6f70 6d65 6e74 2063 7963   development cyc
+00001600: 6c65 2066 6f72 2069 7427 7320 6561 7379  le for it's easy
+00001610: 2069 6e74 6567 7261 7469 6f6e 2061 6e64   integration and
+00001620: 2066 6173 7420 6576 616c 7561 7469 6f6e   fast evaluation
+00001630: 2073 7065 6564 2e0a 0a54 6865 206d 6169   speed...The mai
+00001640: 6e20 6665 6174 7572 6520 696e 636c 7564  n feature includ
+00001650: 6573 3a0a 0a3c 7020 616c 6967 6e3d 2263  es:..<p align="c
+00001660: 656e 7465 7222 2077 6964 7468 3d22 3130  enter" width="10
+00001670: 3025 223e 0a3c 696d 6720 7372 633d 2268  0%">.<img src="h
+00001680: 7474 7073 3a2f 2f69 2e70 6f73 7469 6d67  ttps://i.postimg
+00001690: 2e63 632f 7367 7a4e 6d4a 7837 2f74 6561  .cc/sgzNmJx7/tea
+000016a0: 7365 722e 706e 6722 2020 7769 6474 683d  ser.png"  width=
+000016b0: 2231 3030 2522 2068 6569 6768 743d 2238  "100%" height="8
+000016c0: 3025 223e 0a3c 2f70 3e0a 0a23 2323 204f  0%">.</p>..### O
+000016d0: 6e65 2d63 6f6d 6d61 6e64 2065 7661 6c75  ne-command evalu
+000016e0: 6174 696f 6e2c 2077 6974 6820 6465 7461  ation, with deta
+000016f0: 696c 6564 206c 6f67 7320 616e 6420 7361  iled logs and sa
+00001700: 6d70 6c65 732e 0a59 6f75 2063 616e 2065  mples..You can e
+00001710: 7661 6c75 6174 6520 7468 6520 6d6f 6465  valuate the mode
+00001720: 6c73 206f 6e20 6d75 6c74 6970 6c65 2064  ls on multiple d
+00001730: 6174 6173 6574 7320 7769 7468 2061 2073  atasets with a s
+00001740: 696e 676c 6520 636f 6d6d 616e 642e 204e  ingle command. N
+00001750: 6f20 6d6f 6465 6c2f 6461 7461 2070 7265  o model/data pre
+00001760: 7061 7261 7469 6f6e 2069 7320 6e65 6564  paration is need
+00001770: 6564 2c20 6a75 7374 206f 6e65 2063 6f6d  ed, just one com
+00001780: 6d61 6e64 206c 696e 652c 2066 6577 206d  mand line, few m
+00001790: 696e 7574 6573 2c20 616e 6420 6765 7420  inutes, and get 
+000017a0: 7468 6520 7265 7375 6c74 732e 204e 6f74  the results. Not
+000017b0: 206a 7573 7420 6120 7265 7375 6c74 206e   just a result n
+000017c0: 756d 6265 722c 2062 7574 2061 6c73 6f20  umber, but also 
+000017d0: 7468 6520 6465 7461 696c 6564 206c 6f67  the detailed log
+000017e0: 7320 616e 6420 7361 6d70 6c65 732c 2069  s and samples, i
+000017f0: 6e63 6c75 6469 6e67 2074 6865 206d 6f64  ncluding the mod
+00001800: 656c 2061 7267 732c 2069 6e70 7574 2071  el args, input q
+00001810: 7565 7374 696f 6e2c 206d 6f64 656c 2072  uestion, model r
+00001820: 6573 706f 6e73 652c 2061 6e64 2067 726f  esponse, and gro
+00001830: 756e 6420 7472 7574 6820 616e 7377 6572  und truth answer
+00001840: 2e0a 0a60 6060 7079 7468 6f6e 0a23 2045  ...```python.# E
+00001850: 7661 6c75 6174 696e 6720 4c4c 6156 4120  valuating LLaVA 
+00001860: 6f6e 206d 756c 7469 706c 6520 6461 7461  on multiple data
+00001870: 7365 7473 0a61 6363 656c 6572 6174 6520  sets.accelerate 
+00001880: 6c61 756e 6368 202d 2d6e 756d 5f70 726f  launch --num_pro
+00001890: 6365 7373 6573 3d38 202d 6d20 6c6d 6d73  cesses=8 -m lmms
+000018a0: 5f65 7661 6c20 2d2d 6d6f 6465 6c20 6c6c  _eval --model ll
+000018b0: 6176 6120 2020 2d2d 6d6f 6465 6c5f 6172  ava   --model_ar
+000018c0: 6773 2070 7265 7472 6169 6e65 643d 226c  gs pretrained="l
+000018d0: 6975 6861 6f74 6961 6e2f 6c6c 6176 612d  iuhaotian/llava-
+000018e0: 7631 2e35 2d37 6222 2020 202d 2d74 6173  v1.5-7b"   --tas
+000018f0: 6b73 206d 6d65 2c6d 6d62 656e 6368 5f65  ks mme,mmbench_e
+00001900: 6e20 2d2d 6261 7463 685f 7369 7a65 2031  n --batch_size 1
+00001910: 202d 2d6c 6f67 5f73 616d 706c 6573 202d   --log_samples -
+00001920: 2d6c 6f67 5f73 616d 706c 6573 5f73 7566  -log_samples_suf
+00001930: 6669 7820 6c6c 6176 615f 7631 2e35 5f6d  fix llava_v1.5_m
+00001940: 6d65 5f6d 6d62 656e 6368 656e 202d 2d6f  me_mmbenchen --o
+00001950: 7574 7075 745f 7061 7468 202e 2f6c 6f67  utput_path ./log
+00001960: 732f 2023 0a60 6060 0a0a 2323 2320 4163  s/ #.```..### Ac
+00001970: 6365 6c65 7261 746f 7220 7375 7070 6f72  celerator suppor
+00001980: 7420 616e 6420 5461 736b 7320 6772 6f75  t and Tasks grou
+00001990: 7069 6e67 2e0a 5765 2073 7570 706f 7274  ping..We support
+000019a0: 2074 6865 2075 7361 6765 206f 6620 6061   the usage of `a
+000019b0: 6363 656c 6572 6174 6560 2074 6f20 7772  ccelerate` to wr
+000019c0: 6170 2074 6865 206d 6f64 656c 2066 6f72  ap the model for
+000019d0: 2064 6973 7472 6962 7574 6564 2065 7661   distributed eva
+000019e0: 6c75 6174 696f 6e2c 2073 7570 706f 7274  luation, support
+000019f0: 696e 6720 6d75 6c74 692d 6770 7520 616e  ing multi-gpu an
+00001a00: 6420 7465 6e73 6f72 2070 6172 616c 6c65  d tensor paralle
+00001a10: 6c69 736d 2e20 5769 7468 202a 2a54 6173  lism. With **Tas
+00001a20: 6b20 4772 6f75 7069 6e67 2a2a 2c20 616c  k Grouping**, al
+00001a30: 6c20 696e 7374 616e 6365 7320 6672 6f6d  l instances from
+00001a40: 2061 6c6c 2074 6173 6b73 2061 7265 2067   all tasks are g
+00001a50: 726f 7570 6564 2061 6e64 2065 7661 6c75  rouped and evalu
+00001a60: 6174 6564 2069 6e20 7061 7261 6c6c 656c  ated in parallel
+00001a70: 2c20 7768 6963 6820 7369 676e 6966 6963  , which signific
+00001a80: 616e 746c 7920 696d 7072 6f76 6573 2074  antly improves t
+00001a90: 6865 2074 6872 6f75 6768 7075 7420 6f66  he throughput of
+00001aa0: 2074 6865 2065 7661 6c75 6174 696f 6e2e   the evaluation.
+00001ab0: 2041 6674 6572 2065 7661 6c75 6174 696f   After evaluatio
+00001ac0: 6e2c 2061 6c6c 2069 6e73 7461 6e63 6573  n, all instances
+00001ad0: 2061 7265 2073 656e 7420 746f 2070 6f73   are sent to pos
+00001ae0: 7470 726f 6365 7373 696e 6720 6d6f 6475  tprocessing modu
+00001af0: 6c65 2066 6f72 206d 6574 7269 6320 6361  le for metric ca
+00001b00: 6c63 7561 7469 6f6e 7320 616e 6420 706f  lcuations and po
+00001b10: 7465 6e74 6961 6c20 4750 5434 2d65 7661  tential GPT4-eva
+00001b20: 6c20 7175 6572 6965 732e 0a0a 4265 6c6f  l queries...Belo
+00001b30: 7720 6172 6520 7468 6520 746f 7461 6c20  w are the total 
+00001b40: 7275 6e74 696d 6520 6f6e 2064 6966 6665  runtime on diffe
+00001b50: 7265 6e74 2064 6174 6173 6574 7320 7573  rent datasets us
+00001b60: 696e 6720 3420 7820 4131 3030 2034 3047  ing 4 x A100 40G
+00001b70: 2e0a 0a7c 2044 6174 6173 6574 2028 236e  ...| Dataset (#n
+00001b80: 756d 2920 2020 2020 2020 2020 207c 204c  um)          | L
+00001b90: 4c61 5641 2d76 312e 352d 3762 2020 2020  LaVA-v1.5-7b    
+00001ba0: 2020 7c20 4c4c 6156 412d 7631 2e35 2d31    | LLaVA-v1.5-1
+00001bb0: 3362 2020 2020 207c 0a7c 203a 2d2d 2d2d  3b     |.| :----
+00001bc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001bd0: 2d2d 207c 203a 2d2d 2d2d 2d2d 2d2d 2d2d  -- | :----------
+00001be0: 2d2d 2d2d 2d2d 2d20 7c20 3a2d 2d2d 2d2d  ------- | :-----
+00001bf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c 0a7c  ------------ |.|
+00001c00: 206d 6d65 2028 3233 3734 2920 2020 2020   mme (2374)     
+00001c10: 2020 2020 2020 2020 207c 2032 206d 696e           | 2 min
+00001c20: 7320 3433 2073 6563 6f6e 6473 2020 7c20  s 43 seconds  | 
+00001c30: 3320 6d69 6e73 2032 3720 7365 636f 6e64  3 mins 27 second
+00001c40: 7320 207c 0a7c 2067 7161 2028 3132 3537  s  |.| gqa (1257
+00001c50: 3829 2020 2020 2020 2020 2020 2020 207c  8)             |
+00001c60: 2031 3020 6d69 6e73 2034 3320 7365 636f   10 mins 43 seco
+00001c70: 6e64 7320 7c20 3134 206d 696e 7320 3233  nds | 14 mins 23
+00001c80: 2073 6563 6f6e 6473 207c 0a7c 2073 6369   seconds |.| sci
+00001c90: 656e 6365 7161 5f69 6d67 2028 3230 3137  enceqa_img (2017
+00001ca0: 2920 2020 207c 2031 206d 696e 7320 3538  )    | 1 mins 58
+00001cb0: 2073 6563 6f6e 6473 2020 7c20 3220 6d69   seconds  | 2 mi
+00001cc0: 6e73 2035 3220 7365 636f 6e64 7320 207c  ns 52 seconds  |
+00001cd0: 0a7c 2061 6932 6420 2833 3038 3829 2020  .| ai2d (3088)  
+00001ce0: 2020 2020 2020 2020 2020 207c 2033 206d             | 3 m
+00001cf0: 696e 7320 3137 2073 6563 6f6e 6473 2020  ins 17 seconds  
+00001d00: 7c20 3420 6d69 6e73 2031 3220 7365 636f  | 4 mins 12 seco
+00001d10: 6e64 7320 207c 0a7c 2063 6f63 6f32 3031  nds  |.| coco201
+00001d20: 375f 6361 705f 7661 6c20 2835 3030 3029  7_cap_val (5000)
+00001d30: 207c 2031 3420 6d69 6e73 2031 3320 7365   | 14 mins 13 se
+00001d40: 636f 6e64 7320 7c20 3139 206d 696e 7320  conds | 19 mins 
+00001d50: 3538 2073 6563 6f6e 6473 207c 0a0a 2323  58 seconds |..##
+00001d60: 2320 416c 6c2d 496e 2d4f 6e65 2048 4620  # All-In-One HF 
+00001d70: 6461 7461 7365 7420 6875 6273 2e0a 0a57  dataset hubs...W
+00001d80: 6520 6172 6520 686f 7374 696e 6720 6d6f  e are hosting mo
+00001d90: 7265 2074 6861 6e20 3430 2028 616e 6420  re than 40 (and 
+00001da0: 696e 6372 6561 7369 6e67 2920 6461 7461  increasing) data
+00001db0: 7365 7473 206f 6e20 5b68 7567 6769 6e67  sets on [hugging
+00001dc0: 6661 6365 2f6c 6d6d 732d 6c61 625d 2868  face/lmms-lab](h
+00001dd0: 7474 7073 3a2f 2f68 7567 6769 6e67 6661  ttps://huggingfa
+00001de0: 6365 2e63 6f2f 6c6d 6d73 2d6c 6162 292c  ce.co/lmms-lab),
+00001df0: 2077 6520 6361 7265 6675 6c6c 7920 636f   we carefully co
+00001e00: 6e76 6572 7465 6420 7468 6573 6520 6461  nverted these da
+00001e10: 7461 7365 7473 2066 726f 6d20 6f72 6967  tasets from orig
+00001e20: 696e 616c 2073 6f75 7263 6573 2061 6e64  inal sources and
+00001e30: 2069 6e63 6c75 6465 6420 616c 6c20 7661   included all va
+00001e40: 7269 616e 7473 2c20 7665 7273 696f 6e73  riants, versions
+00001e50: 2061 6e64 2073 706c 6974 732e 204e 6f77   and splits. Now
+00001e60: 2074 6865 7920 6361 6e20 6265 2064 6972   they can be dir
+00001e70: 6563 746c 7920 6163 6365 7373 6564 2077  ectly accessed w
+00001e80: 6974 686f 7574 2061 6e79 2062 7572 6465  ithout any burde
+00001e90: 6e20 6f66 2064 6174 6120 7072 6570 726f  n of data prepro
+00001ea0: 6365 7373 696e 672e 2054 6865 7920 616c  cessing. They al
+00001eb0: 736f 2073 6572 7665 2066 6f72 2074 6865  so serve for the
+00001ec0: 2070 7572 706f 7365 206f 6620 7669 7375   purpose of visu
+00001ed0: 616c 697a 696e 6720 7468 6520 6461 7461  alizing the data
+00001ee0: 2061 6e64 2067 7261 7370 696e 6720 7468   and grasping th
+00001ef0: 6520 7365 6e73 6520 6f66 2065 7661 6c75  e sense of evalu
+00001f00: 6174 696f 6e20 7461 736b 7320 6469 7374  ation tasks dist
+00001f10: 7269 6275 7469 6f6e 2e0a 0a3c 7020 616c  ribution...<p al
+00001f20: 6967 6e3d 2263 656e 7465 7222 2077 6964  ign="center" wid
+00001f30: 7468 3d22 3130 3025 223e 0a3c 696d 6720  th="100%">.<img 
+00001f40: 7372 633d 2268 7474 7073 3a2f 2f69 2e70  src="https://i.p
+00001f50: 6f73 7469 6d67 2e63 632f 3850 5846 5739  ostimg.cc/8PXFW9
+00001f60: 736b 2f57 5832 3032 3430 3232 382d 3132  sk/WX20240228-12
+00001f70: 3331 3130 5f32 782e 706e 6722 2020 7769  3110_2x.png"  wi
+00001f80: 6474 683d 2231 3030 2522 2068 6569 6768  dth="100%" heigh
+00001f90: 743d 2238 3025 223e 0a3c 2f70 3e0a 0a23  t="80%">.</p>..#
+00001fa0: 2323 2044 6574 6169 6c65 6420 4c6f 6767  ## Detailed Logg
+00001fb0: 696e 6720 5574 696c 6974 6573 0a0a 5765  ing Utilites..We
+00001fc0: 2070 726f 7669 6465 2064 6574 6169 6c65   provide detaile
+00001fd0: 6420 6c6f 6767 696e 6720 7574 696c 6974  d logging utilit
+00001fe0: 6965 7320 746f 2068 656c 7020 796f 7520  ies to help you 
+00001ff0: 756e 6465 7273 7461 6e64 2074 6865 2065  understand the e
+00002000: 7661 6c75 6174 696f 6e20 7072 6f63 6573  valuation proces
+00002010: 7320 616e 6420 7265 7375 6c74 732e 2054  s and results. T
+00002020: 6865 206c 6f67 7320 696e 636c 7564 6520  he logs include 
+00002030: 7468 6520 6d6f 6465 6c20 6172 6773 2c20  the model args, 
+00002040: 6765 6e65 7261 7469 6f6e 2070 6172 616d  generation param
+00002050: 6574 6572 732c 2069 6e70 7574 2071 7565  eters, input que
+00002060: 7374 696f 6e2c 206d 6f64 656c 2072 6573  stion, model res
+00002070: 706f 6e73 652c 2061 6e64 2067 726f 756e  ponse, and groun
+00002080: 6420 7472 7574 6820 616e 7377 6572 2e20  d truth answer. 
+00002090: 596f 7520 6361 6e20 616c 736f 2072 6563  You can also rec
+000020a0: 6f72 6420 6576 6572 7920 6465 7461 696c  ord every detail
+000020b0: 7320 616e 6420 7669 7375 616c 697a 6520  s and visualize 
+000020c0: 7468 656d 2069 6e73 6964 6520 7275 6e73  them inside runs
+000020d0: 206f 6e20 5765 6967 6874 7320 2620 4269   on Weights & Bi
+000020e0: 6173 6573 2e0a 0a7b 2520 696e 636c 7564  ases...{% includ
+000020f0: 6520 6669 6775 7265 2e6c 6971 7569 6420  e figure.liquid 
+00002100: 6c6f 6164 696e 673d 2265 6167 6572 2220  loading="eager" 
+00002110: 7061 7468 3d22 6173 7365 7473 2f69 6d67  path="assets/img
+00002120: 2f77 616e 6462 5f74 6162 6c65 2e70 6e67  /wandb_table.png
+00002130: 2220 636c 6173 733d 2269 6d67 2d66 6c75  " class="img-flu
+00002140: 6964 2072 6f75 6e64 6564 207a 2d64 6570  id rounded z-dep
+00002150: 7468 2d31 2220 7a6f 6f6d 6162 6c65 3d74  th-1" zoomable=t
+00002160: 7275 6520 257d 0a0a 3c70 2061 6c69 676e  rue %}..<p align
+00002170: 3d22 6365 6e74 6572 2220 7769 6474 683d  ="center" width=
+00002180: 2231 3030 2522 3e0a 3c69 6d67 2073 7263  "100%">.<img src
+00002190: 3d22 6874 7470 733a 2f2f 692e 706f 7374  ="https://i.post
+000021a0: 696d 672e 6363 2f57 3163 3176 4244 4a2f  img.cc/W1c1vBDJ/
+000021b0: 5765 6368 6174 2d49 4d47 3139 3933 2e70  Wechat-IMG1993.p
+000021c0: 6e67 2220 2077 6964 7468 3d22 3130 3025  ng"  width="100%
+000021d0: 2220 6865 6967 6874 3d22 3830 2522 3e0a  " height="80%">.
+000021e0: 3c2f 703e 0a0a 2320 496e 7374 616c 6c61  </p>..# Installa
+000021f0: 7469 6f6e 0a0a 466f 7220 666f 726d 616c  tion..For formal
+00002200: 2075 7361 6765 2c20 796f 7520 6361 6e20   usage, you can 
+00002210: 696e 7374 616c 6c20 7468 6520 7061 636b  install the pack
+00002220: 6167 6520 6672 6f6d 2050 7950 4920 6279  age from PyPI by
+00002230: 2072 756e 6e69 6e67 2074 6865 2066 6f6c   running the fol
+00002240: 6c6f 7769 6e67 2063 6f6d 6d61 6e64 3a0a  lowing command:.
+00002250: 6060 6062 6173 680a 7069 7020 696e 7374  ```bash.pip inst
+00002260: 616c 6c20 6c6d 6d73 2d65 7661 6c0a 6060  all lmms-eval.``
+00002270: 600a 0a46 6f72 2064 6576 656c 6f70 6d65  `..For developme
+00002280: 6e74 2c20 796f 7520 6361 6e20 696e 7374  nt, you can inst
+00002290: 616c 6c20 7468 6520 7061 636b 6167 6520  all the package 
+000022a0: 6279 2063 6c6f 6e69 6e67 2074 6865 2072  by cloning the r
+000022b0: 6570 6f73 6974 6f72 7920 616e 6420 7275  epository and ru
+000022c0: 6e6e 696e 6720 7468 6520 666f 6c6c 6f77  nning the follow
+000022d0: 696e 6720 636f 6d6d 616e 643a 0a60 6060  ing command:.```
+000022e0: 6261 7368 0a67 6974 2063 6c6f 6e65 2068  bash.git clone h
+000022f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00002300: 6d2f 4576 6f6c 7669 6e67 4c4d 4d73 2d4c  m/EvolvingLMMs-L
+00002310: 6162 2f6c 6d6d 732d 6576 616c 0a63 6420  ab/lmms-eval.cd 
+00002320: 6c6d 6d73 2d65 7661 6c0a 7069 7020 696e  lmms-eval.pip in
+00002330: 7374 616c 6c20 2d65 202e 0a60 6060 0a0a  stall -e ..```..
+00002340: 4966 2079 6f75 2077 616e 7465 6420 746f  If you wanted to
+00002350: 2074 6573 7420 6c6c 6176 612c 2079 6f75   test llava, you
+00002360: 2077 696c 6c20 6861 7665 2074 6f20 636c   will have to cl
+00002370: 6f6e 6520 7468 6569 7220 7265 706f 2066  one their repo f
+00002380: 726f 6d20 5b4c 4c61 5641 5d28 6874 7470  rom [LLaVA](http
+00002390: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f68  s://github.com/h
+000023a0: 616f 7469 616e 2d6c 6975 2f4c 4c61 5641  aotian-liu/LLaVA
+000023b0: 2920 616e 640a 6060 600a 6769 7420 636c  ) and.```.git cl
+000023c0: 6f6e 6520 6874 7470 733a 2f2f 6769 7468  one https://gith
+000023d0: 7562 2e63 6f6d 2f68 616f 7469 616e 2d6c  ub.com/haotian-l
+000023e0: 6975 2f4c 4c61 5641 0a63 6420 4c4c 6156  iu/LLaVA.cd LLaV
+000023f0: 410a 7069 7020 696e 7374 616c 6c20 2d65  A.pip install -e
+00002400: 202e 0a60 6060 0a0a 596f 7520 6361 6e20   ..```..You can 
+00002410: 6368 6563 6b20 7468 6520 5b65 6e76 6972  check the [envir
+00002420: 6f6e 6d65 6e74 2069 6e73 7461 6c6c 2073  onment install s
+00002430: 6372 6970 745d 286d 6973 6373 2f72 6570  cript](miscs/rep
+00002440: 725f 7363 7269 7074 732e 7368 2920 616e  r_scripts.sh) an
+00002450: 6420 5b74 6f72 6368 2065 6e76 6972 6f6e  d [torch environ
+00002460: 6d65 6e74 2069 6e66 6f5d 286d 6973 6373  ment info](miscs
+00002470: 2f72 6570 725f 746f 7263 685f 656e 7673  /repr_torch_envs
+00002480: 2e74 7874 2920 746f 202a 2a72 6570 726f  .txt) to **repro
+00002490: 6475 6365 204c 4c61 5641 2d31 2e35 2773  duce LLaVA-1.5's
+000024a0: 2070 6170 6572 2072 6573 756c 7473 2a2a   paper results**
+000024b0: 2e20 5765 2066 6f75 6e64 2074 6f72 6368  . We found torch
+000024c0: 2f63 7564 6120 7665 7273 696f 6e73 2064  /cuda versions d
+000024d0: 6966 6665 7265 6e63 6520 776f 756c 6420  ifference would 
+000024e0: 6361 7573 6520 736d 616c 6c20 7661 7269  cause small vari
+000024f0: 6174 696f 6e73 2069 6e20 7468 6520 7265  ations in the re
+00002500: 7375 6c74 732c 2077 6520 7072 6f76 6964  sults, we provid
+00002510: 6520 7468 6520 5b72 6573 756c 7473 2063  e the [results c
+00002520: 6865 636b 5d28 6d69 7363 732f 6c6c 6176  heck](miscs/llav
+00002530: 615f 7265 7375 6c74 5f63 6865 636b 2e6d  a_result_check.m
+00002540: 6429 2077 6974 6820 6469 6666 6572 656e  d) with differen
+00002550: 7420 656e 7669 726f 6e6d 656e 7473 2e0a  t environments..
+00002560: 0a49 6620 796f 7520 7761 6e74 2074 6f20  .If you want to 
+00002570: 7465 7374 206f 6e20 6361 7074 696f 6e20  test on caption 
+00002580: 6461 7461 7365 7420 7375 6368 2061 7320  dataset such as 
+00002590: 6063 6f63 6f60 2c20 6072 6566 636f 636f  `coco`, `refcoco
+000025a0: 602c 2061 6e64 2060 6e6f 6361 7073 602c  `, and `nocaps`,
+000025b0: 2079 6f75 2077 696c 6c20 6e65 6564 2074   you will need t
+000025c0: 6f20 6861 7665 2060 6a61 7661 3d3d 312e  o have `java==1.
+000025d0: 382e 3020 6020 746f 206c 6574 2070 7963  8.0 ` to let pyc
+000025e0: 6f63 6f65 7661 6c20 6170 6920 746f 2077  ocoeval api to w
+000025f0: 6f72 6b2e 2049 6620 796f 7520 646f 6e27  ork. If you don'
+00002600: 7420 6861 7665 2069 742c 2079 6f75 2063  t have it, you c
+00002610: 616e 2069 6e73 7461 6c6c 2062 7920 7573  an install by us
+00002620: 696e 6720 636f 6e64 610a 6060 600a 636f  ing conda.```.co
+00002630: 6e64 6120 696e 7374 616c 6c20 6f70 656e  nda install open
+00002640: 6a64 6b3d 380a 6060 600a 796f 7520 6361  jdk=8.```.you ca
+00002650: 6e20 7468 656e 2063 6865 636b 2079 6f75  n then check you
+00002660: 7220 6a61 7661 2076 6572 7369 6f6e 2062  r java version b
+00002670: 7920 606a 6176 6120 2d76 6572 7369 6f6e  y `java -version
+00002680: 6020 0a0a 2320 5573 6167 650a 6060 6062  ` ..# Usage.```b
+00002690: 6173 680a 2320 4576 616c 7561 7469 6e67  ash.# Evaluating
+000026a0: 204c 4c61 5641 206f 6e20 4d4d 450a 6163   LLaVA on MME.ac
+000026b0: 6365 6c65 7261 7465 206c 6175 6e63 6820  celerate launch 
+000026c0: 2d2d 6e75 6d5f 7072 6f63 6573 7365 733d  --num_processes=
+000026d0: 3820 2d6d 206c 6d6d 735f 6576 616c 202d  8 -m lmms_eval -
+000026e0: 2d6d 6f64 656c 206c 6c61 7661 2020 202d  -model llava   -
+000026f0: 2d6d 6f64 656c 5f61 7267 7320 7072 6574  -model_args pret
+00002700: 7261 696e 6564 3d22 6c69 7568 616f 7469  rained="liuhaoti
+00002710: 616e 2f6c 6c61 7661 2d76 312e 352d 3762  an/llava-v1.5-7b
+00002720: 2220 2020 2d2d 7461 736b 7320 6d6d 6520  "   --tasks mme 
+00002730: 202d 2d62 6174 6368 5f73 697a 6520 3120   --batch_size 1 
+00002740: 2d2d 6c6f 675f 7361 6d70 6c65 7320 2d2d  --log_samples --
+00002750: 6c6f 675f 7361 6d70 6c65 735f 7375 6666  log_samples_suff
+00002760: 6978 206c 6c61 7661 5f76 312e 355f 6d6d  ix llava_v1.5_mm
+00002770: 6520 2d2d 6f75 7470 7574 5f70 6174 6820  e --output_path 
+00002780: 2e2f 6c6f 6773 2f20 0a0a 2320 4576 616c  ./logs/ ..# Eval
+00002790: 7561 7469 6e67 204c 4c61 5641 206f 6e20  uating LLaVA on 
+000027a0: 6d75 6c74 6970 6c65 2064 6174 6173 6574  multiple dataset
+000027b0: 730a 6163 6365 6c65 7261 7465 206c 6175  s.accelerate lau
+000027c0: 6e63 6820 2d2d 6e75 6d5f 7072 6f63 6573  nch --num_proces
+000027d0: 7365 733d 3820 2d6d 206c 6d6d 735f 6576  ses=8 -m lmms_ev
+000027e0: 616c 202d 2d6d 6f64 656c 206c 6c61 7661  al --model llava
+000027f0: 2020 202d 2d6d 6f64 656c 5f61 7267 7320     --model_args 
+00002800: 7072 6574 7261 696e 6564 3d22 6c69 7568  pretrained="liuh
+00002810: 616f 7469 616e 2f6c 6c61 7661 2d76 312e  aotian/llava-v1.
+00002820: 352d 3762 2220 2020 2d2d 7461 736b 7320  5-7b"   --tasks 
+00002830: 6d6d 652c 6d6d 6265 6e63 685f 656e 202d  mme,mmbench_en -
+00002840: 2d62 6174 6368 5f73 697a 6520 3120 2d2d  -batch_size 1 --
+00002850: 6c6f 675f 7361 6d70 6c65 7320 2d2d 6c6f  log_samples --lo
+00002860: 675f 7361 6d70 6c65 735f 7375 6666 6978  g_samples_suffix
+00002870: 206c 6c61 7661 5f76 312e 355f 6d6d 655f   llava_v1.5_mme_
+00002880: 6d6d 6265 6e63 6865 6e20 2d2d 6f75 7470  mmbenchen --outp
+00002890: 7574 5f70 6174 6820 2e2f 6c6f 6773 2f20  ut_path ./logs/ 
+000028a0: 230a 0a23 2046 6f72 206f 7468 6572 2076  #..# For other v
+000028b0: 6172 6961 6e74 7320 6c6c 6176 612e 204e  ariants llava. N
+000028c0: 6f74 6520 7468 6174 2060 636f 6e76 5f74  ote that `conv_t
+000028d0: 656d 706c 6174 6560 2069 7320 616e 2061  emplate` is an a
+000028e0: 7267 206f 6620 7468 6520 696e 6974 2066  rg of the init f
+000028f0: 756e 6374 696f 6e20 6f66 206c 6c61 7661  unction of llava
+00002900: 2069 6e20 606c 6d6d 735f 6576 616c 2f6d   in `lmms_eval/m
+00002910: 6f64 656c 732f 6c6c 6176 612e 7079 600a  odels/llava.py`.
+00002920: 6163 6365 6c65 7261 7465 206c 6175 6e63  accelerate launc
+00002930: 6820 2d2d 6e75 6d5f 7072 6f63 6573 7365  h --num_processe
+00002940: 733d 3820 2d6d 206c 6d6d 735f 6576 616c  s=8 -m lmms_eval
+00002950: 202d 2d6d 6f64 656c 206c 6c61 7661 2020   --model llava  
+00002960: 202d 2d6d 6f64 656c 5f61 7267 7320 7072   --model_args pr
+00002970: 6574 7261 696e 6564 3d22 6c69 7568 616f  etrained="liuhao
+00002980: 7469 616e 2f6c 6c61 7661 2d76 312e 362d  tian/llava-v1.6-
+00002990: 6d69 7374 7261 6c2d 3762 2c63 6f6e 765f  mistral-7b,conv_
+000029a0: 7465 6d70 6c61 7465 3d6d 6973 7472 616c  template=mistral
+000029b0: 5f69 6e73 7472 7563 7422 2020 202d 2d74  _instruct"   --t
+000029c0: 6173 6b73 206d 6d65 2c6d 6d62 656e 6368  asks mme,mmbench
+000029d0: 5f65 6e20 2d2d 6261 7463 685f 7369 7a65  _en --batch_size
+000029e0: 2031 202d 2d6c 6f67 5f73 616d 706c 6573   1 --log_samples
+000029f0: 202d 2d6c 6f67 5f73 616d 706c 6573 5f73   --log_samples_s
+00002a00: 7566 6669 7820 6c6c 6176 615f 7631 2e35  uffix llava_v1.5
+00002a10: 5f6d 6d65 5f6d 6d62 656e 6368 656e 202d  _mme_mmbenchen -
+00002a20: 2d6f 7574 7075 745f 7061 7468 202e 2f6c  -output_path ./l
+00002a30: 6f67 732f 2023 0a61 6363 656c 6572 6174  ogs/ #.accelerat
+00002a40: 6520 6c61 756e 6368 202d 2d6e 756d 5f70  e launch --num_p
+00002a50: 726f 6365 7373 6573 3d38 202d 6d20 6c6d  rocesses=8 -m lm
+00002a60: 6d73 5f65 7661 6c20 2d2d 6d6f 6465 6c20  ms_eval --model 
+00002a70: 6c6c 6176 6120 2020 2d2d 6d6f 6465 6c5f  llava   --model_
+00002a80: 6172 6773 2070 7265 7472 6169 6e65 643d  args pretrained=
+00002a90: 226c 6975 6861 6f74 6961 6e2f 6c6c 6176  "liuhaotian/llav
+00002aa0: 612d 7631 2e36 2d33 3462 2c63 6f6e 765f  a-v1.6-34b,conv_
+00002ab0: 7465 6d70 6c61 7465 3d6d 6973 7472 616c  template=mistral
+00002ac0: 5f64 6972 6563 7422 2020 202d 2d74 6173  _direct"   --tas
+00002ad0: 6b73 206d 6d65 2c6d 6d62 656e 6368 5f65  ks mme,mmbench_e
+00002ae0: 6e20 2d2d 6261 7463 685f 7369 7a65 2031  n --batch_size 1
+00002af0: 202d 2d6c 6f67 5f73 616d 706c 6573 202d   --log_samples -
+00002b00: 2d6c 6f67 5f73 616d 706c 6573 5f73 7566  -log_samples_suf
+00002b10: 6669 7820 6c6c 6176 615f 7631 2e35 5f6d  fix llava_v1.5_m
+00002b20: 6d65 5f6d 6d62 656e 6368 656e 202d 2d6f  me_mmbenchen --o
+00002b30: 7574 7075 745f 7061 7468 202e 2f6c 6f67  utput_path ./log
+00002b40: 732f 2023 0a0a 2320 4672 6f6d 2061 2070  s/ #..# From a p
+00002b50: 7265 6465 6669 6e65 6420 636f 6e66 6967  redefined config
+00002b60: 7572 6174 696f 6e2c 2073 7570 706f 7274  uration, support
+00002b70: 696e 6720 6576 616c 7561 7469 6f6e 206f  ing evaluation o
+00002b80: 6620 6d75 6c74 6970 6c65 206d 6f64 656c  f multiple model
+00002b90: 7320 616e 6420 6461 7461 7365 7473 0a61  s and datasets.a
+00002ba0: 6363 656c 6572 6174 6520 6c61 756e 6368  ccelerate launch
+00002bb0: 202d 2d6e 756d 5f70 726f 6365 7373 6573   --num_processes
+00002bc0: 3d38 202d 6d20 6c6d 6d73 5f65 7661 6c20  =8 -m lmms_eval 
+00002bd0: 2d2d 636f 6e66 6967 2065 7861 6d70 6c65  --config example
+00002be0: 5f65 7661 6c2e 7961 6d6c 200a 6060 600a  _eval.yaml .```.
+00002bf0: 0a23 204d 6f64 656c 2052 6573 756c 7473  .# Model Results
+00002c00: 0a0a 4173 2064 656d 6f6e 7374 7261 7465  ..As demonstrate
+00002c10: 6420 6279 2074 6865 2065 7874 656e 7369  d by the extensi
+00002c20: 7665 2074 6162 6c65 2062 656c 6f77 2c20  ve table below, 
+00002c30: 7765 2061 696d 2074 6f20 7072 6f76 6964  we aim to provid
+00002c40: 6520 6465 7461 696c 6564 2069 6e66 6f72  e detailed infor
+00002c50: 6d61 7469 6f6e 2066 6f72 2072 6561 6465  mation for reade
+00002c60: 7273 2074 6f20 756e 6465 7273 7461 6e64  rs to understand
+00002c70: 2074 6865 2064 6174 6173 6574 7320 696e   the datasets in
+00002c80: 636c 7564 6564 2069 6e20 6c6d 6d73 2d65  cluded in lmms-e
+00002c90: 7661 6c20 616e 6420 736f 6d65 2073 7065  val and some spe
+00002ca0: 6369 6669 6320 6465 7461 696c 7320 6162  cific details ab
+00002cb0: 6f75 7420 7468 6573 6520 6461 7461 7365  out these datase
+00002cc0: 7473 2028 7765 2072 656d 6169 6e20 6772  ts (we remain gr
+00002cd0: 6174 6566 756c 2066 6f72 2061 6e79 2063  ateful for any c
+00002ce0: 6f72 7265 6374 696f 6e73 2072 6561 6465  orrections reade
+00002cf0: 7273 206d 6179 2068 6176 6520 6475 7269  rs may have duri
+00002d00: 6e67 206f 7572 2065 7661 6c75 6174 696f  ng our evaluatio
+00002d10: 6e20 7072 6f63 6573 7329 2e0a 0a57 6520  n process)...We 
+00002d20: 7072 6f76 6964 6520 6120 476f 6f67 6c65  provide a Google
+00002d30: 2053 6865 6574 2066 6f72 2074 6865 2064   Sheet for the d
+00002d40: 6574 6169 6c65 6420 7265 7375 6c74 7320  etailed results 
+00002d50: 6f66 2074 6865 204c 4c61 5641 2073 6572  of the LLaVA ser
+00002d60: 6965 7320 6d6f 6465 6c73 206f 6e20 6469  ies models on di
+00002d70: 6666 6572 656e 7420 6461 7461 7365 7473  fferent datasets
+00002d80: 2e20 596f 7520 6361 6e20 6163 6365 7373  . You can access
+00002d90: 2074 6865 2073 6865 6574 205b 6865 7265   the sheet [here
+00002da0: 5d28 6874 7470 733a 2f2f 646f 6373 2e67  ](https://docs.g
+00002db0: 6f6f 676c 652e 636f 6d2f 7370 7265 6164  oogle.com/spread
+00002dc0: 7368 6565 7473 2f64 2f31 6135 496d 6664  sheets/d/1a5Imfd
+00002dd0: 4b41 5444 4938 5437 4377 6836 6548 2d62  KATDI8T7Cwh6eH-b
+00002de0: 4573 6e51 467a 616e 4672 6146 5567 6353  EsnQFzanFraFUgcS
+00002df0: 394b 4857 632f 6564 6974 3f75 7370 3d73  9KHWc/edit?usp=s
+00002e00: 6861 7269 6e67 292e 2049 7427 7320 6120  haring). It's a 
+00002e10: 6c69 7665 2073 6865 6574 2c20 616e 6420  live sheet, and 
+00002e20: 7765 2061 7265 2075 7064 6174 696e 6720  we are updating 
+00002e30: 6974 2077 6974 6820 6e65 7720 7265 7375  it with new resu
+00002e40: 6c74 732e 0a0a 3c70 2061 6c69 676e 3d22  lts...<p align="
+00002e50: 6365 6e74 6572 2220 7769 6474 683d 2231  center" width="1
+00002e60: 3030 2522 3e0a 3c69 6d67 2073 7263 3d22  00%">.<img src="
+00002e70: 6874 7470 733a 2f2f 692e 706f 7374 696d  https://i.postim
+00002e80: 672e 6363 2f6a 6477 3439 374e 532f 5758  g.cc/jdw497NS/WX
+00002e90: 3230 3234 3033 3037 2d31 3632 3532 362d  20240307-162526-
+00002ea0: 3278 2e70 6e67 2220 2077 6964 7468 3d22  2x.png"  width="
+00002eb0: 3130 3025 2220 6865 6967 6874 3d22 3830  100%" height="80
+00002ec0: 2522 3e0a 3c2f 703e 0a0a 5765 2061 6c73  %">.</p>..We als
+00002ed0: 6f20 7072 6f76 6964 6520 7468 6520 7261  o provide the ra
+00002ee0: 7720 6461 7461 2065 7870 6f72 7465 6420  w data exported 
+00002ef0: 6672 6f6d 2057 6569 6768 7473 2026 2042  from Weights & B
+00002f00: 6961 7365 7320 666f 7220 7468 6520 6465  iases for the de
+00002f10: 7461 696c 6564 2072 6573 756c 7473 206f  tailed results o
+00002f20: 6620 7468 6520 4c4c 6156 4120 7365 7269  f the LLaVA seri
+00002f30: 6573 206d 6f64 656c 7320 6f6e 2064 6966  es models on dif
+00002f40: 6665 7265 6e74 2064 6174 6173 6574 732e  ferent datasets.
+00002f50: 2059 6f75 2063 616e 2061 6363 6573 7320   You can access 
+00002f60: 7468 6520 7261 7720 6461 7461 205b 6865  the raw data [he
+00002f70: 7265 5d28 6874 7470 733a 2f2f 646f 6373  re](https://docs
+00002f80: 2e67 6f6f 676c 652e 636f 6d2f 7370 7265  .google.com/spre
+00002f90: 6164 7368 6565 7473 2f64 2f31 4176 6145  adsheets/d/1AvaE
+00002fa0: 6d75 4734 6373 536d 5861 486a 6775 3465  muG4csSmXaHjgu4e
+00002fb0: 6931 4b42 4d6d 4e4e 5738 7766 6c4f 445f  i1KBMmNNW8wflOD_
+00002fc0: 6b6b 5444 6476 382f 6564 6974 3f75 7370  kkTDdv8/edit?usp
+00002fd0: 3d73 6861 7269 6e67 292e 0a0a 3e20 4465  =sharing)...> De
+00002fe0: 7665 6c6f 706d 656e 7420 7769 6c6c 2062  velopment will b
+00002ff0: 6520 636f 6e74 696e 7569 6e67 206f 6e20  e continuing on 
+00003000: 7468 6520 6d61 696e 2062 7261 6e63 682c  the main branch,
+00003010: 2061 6e64 2077 6520 656e 636f 7572 6167   and we encourag
+00003020: 6520 796f 7520 746f 2067 6976 6520 7573  e you to give us
+00003030: 2066 6565 6462 6163 6b20 6f6e 2077 6861   feedback on wha
+00003040: 7420 6665 6174 7572 6573 2061 7265 2064  t features are d
+00003050: 6573 6972 6564 2061 6e64 2068 6f77 2074  esired and how t
+00003060: 6f20 696d 7072 6f76 6520 7468 6520 6c69  o improve the li
+00003070: 6272 6172 7920 6675 7274 6865 722c 206f  brary further, o
+00003080: 7220 6173 6b20 7175 6573 7469 6f6e 732c  r ask questions,
+00003090: 2065 6974 6865 7220 696e 2069 7373 7565   either in issue
+000030a0: 7320 6f72 2050 5273 206f 6e20 4769 7448  s or PRs on GitH
+000030b0: 7562 2e0a 0a0a 2323 2053 7570 706f 7274  ub....## Support
+000030c0: 6564 206d 6f64 656c 730a 0a2d 2047 5054  ed models..- GPT
+000030d0: 3456 2028 4150 492c 206f 6e6c 7920 6765  4V (API, only ge
+000030e0: 6e65 7261 7469 6f6e 2d62 6173 6564 2065  neration-based e
+000030f0: 7661 6c75 6174 696f 6e29 0a2d 204c 4c61  valuation).- LLa
+00003100: 5641 2d76 312e 352f 7631 2e36 2d37 422f  VA-v1.5/v1.6-7B/
+00003110: 3133 422f 3334 4220 2870 706c 2d62 6173  13B/34B (ppl-bas
+00003120: 6564 2c20 6765 6e65 7261 7469 6f6e 2d62  ed, generation-b
+00003130: 6173 6564 290a 2d20 5177 656e 2d56 4c20  ased).- Qwen-VL 
+00003140: 7365 7269 6573 2028 7070 6c2d 6261 7365  series (ppl-base
+00003150: 642c 2067 656e 6572 6174 696f 6e2d 6261  d, generation-ba
+00003160: 7365 6429 0a2d 2046 7579 7520 7365 7269  sed).- Fuyu seri
+00003170: 6573 2028 7070 6c2d 6261 7365 642c 2067  es (ppl-based, g
+00003180: 656e 6572 6174 696f 6e2d 6261 7365 6429  eneration-based)
+00003190: 0a2d 2049 6e73 7472 7563 7442 4c49 5020  .- InstructBLIP 
+000031a0: 7365 7269 6573 2028 6765 6e65 7261 7469  series (generati
+000031b0: 6f6e 2d62 6173 6564 290a 0a23 2320 5375  on-based)..## Su
+000031c0: 7070 6f72 7465 6420 6461 7461 7365 7473  pported datasets
+000031d0: 0a3e 2028 2920 696e 6469 6361 7465 7320  .> () indicates 
+000031e0: 7468 6520 7461 736b 206e 616d 6520 696e  the task name in
+000031f0: 2074 6865 206c 6d6d 735f 6576 616c 2e20   the lmms_eval. 
+00003200: 5468 6520 7461 736b 206e 616d 6520 6973  The task name is
+00003210: 2061 6c73 6f20 7573 6564 2074 6f20 7370   also used to sp
+00003220: 6563 6966 7920 7468 6520 6461 7461 7365  ecify the datase
+00003230: 7420 696e 2074 6865 2063 6f6e 6669 6775  t in the configu
+00003240: 7261 7469 6f6e 2066 696c 652e 0a0a 2d20  ration file...- 
+00003250: 4149 3244 2028 6169 3264 290a 2d20 4368  AI2D (ai2d).- Ch
+00003260: 6172 7451 4120 2863 6861 7274 7161 290a  artQA (chartqa).
+00003270: 2d20 434d 4d4d 5520 2863 6d6d 6d75 290a  - CMMMU (cmmmu).
+00003280: 2020 2d20 434d 4d4d 5520 5661 6c69 6461    - CMMMU Valida
+00003290: 7469 6f6e 2028 636d 6d6d 755f 7661 6c29  tion (cmmmu_val)
+000032a0: 0a20 202d 2043 4d4d 4d55 2054 6573 7420  .  - CMMMU Test 
+000032b0: 2863 6d6d 6d75 5f74 6573 7429 0a2d 2043  (cmmmu_test).- C
+000032c0: 4f43 4f20 4361 7074 696f 6e20 2863 6f63  OCO Caption (coc
+000032d0: 6f5f 6361 7029 0a20 202d 2043 4f43 4f20  o_cap).  - COCO 
+000032e0: 3230 3134 2043 6170 7469 6f6e 2028 636f  2014 Caption (co
+000032f0: 636f 3230 3134 5f63 6170 290a 2020 2020  co2014_cap).    
+00003300: 2d20 434f 434f 2032 3031 3420 4361 7074  - COCO 2014 Capt
+00003310: 696f 6e20 5661 6c69 6461 7469 6f6e 2028  ion Validation (
+00003320: 636f 636f 3230 3134 5f63 6170 5f76 616c  coco2014_cap_val
+00003330: 290a 2020 2020 2d20 434f 434f 2032 3031  ).    - COCO 201
+00003340: 3420 4361 7074 696f 6e20 5465 7374 2028  4 Caption Test (
+00003350: 636f 636f 3230 3134 5f63 6170 5f74 6573  coco2014_cap_tes
+00003360: 7429 0a20 202d 2043 4f43 4f20 3230 3137  t).  - COCO 2017
+00003370: 2043 6170 7469 6f6e 2028 636f 636f 3230   Caption (coco20
+00003380: 3137 5f63 6170 290a 2020 2020 2d20 434f  17_cap).    - CO
+00003390: 434f 2032 3031 3720 4361 7074 696f 6e20  CO 2017 Caption 
+000033a0: 4d69 6e69 5661 6c20 2863 6f63 6f32 3031  MiniVal (coco201
+000033b0: 375f 6361 705f 7661 6c29 0a20 2020 202d  7_cap_val).    -
+000033c0: 2043 4f43 4f20 3230 3137 2043 6170 7469   COCO 2017 Capti
+000033d0: 6f6e 204d 696e 6954 6573 7420 2863 6f63  on MiniTest (coc
+000033e0: 6f32 3031 375f 6361 705f 7465 7374 290a  o2017_cap_test).
+000033f0: 2d20 444f 4356 5141 2028 646f 6376 7161  - DOCVQA (docvqa
+00003400: 290a 2020 2d20 444f 4356 5141 2056 616c  ).  - DOCVQA Val
+00003410: 6964 6174 696f 6e20 2864 6f63 7671 615f  idation (docvqa_
+00003420: 7661 6c29 0a20 202d 2044 4f43 5651 4120  val).  - DOCVQA 
+00003430: 5465 7374 2028 646f 6376 7161 5f74 6573  Test (docvqa_tes
+00003440: 7429 0a2d 2046 6572 7265 7420 2866 6572  t).- Ferret (fer
+00003450: 7265 7429 0a2d 2046 6c69 636b 7233 304b  ret).- Flickr30K
+00003460: 2028 666c 6963 6b72 3330 6b29 0a20 202d   (flickr30k).  -
+00003470: 2046 6572 7265 7420 5465 7374 2028 6665   Ferret Test (fe
+00003480: 7272 6574 5f74 6573 7429 0a2d 2047 5141  rret_test).- GQA
+00003490: 2028 6771 6129 0a2d 2048 616c 6c75 7369   (gqa).- Hallusi
+000034a0: 6f6e 4265 6e63 686d 6172 6b20 2868 616c  onBenchmark (hal
+000034b0: 6c75 7369 6f6e 5f62 656e 6368 5f69 6d61  lusion_bench_ima
+000034c0: 6765 290a 2d20 496e 666f 6772 6170 6869  ge).- Infographi
+000034d0: 6320 5651 4120 2869 6e66 6f5f 7671 6129  c VQA (info_vqa)
+000034e0: 0a20 202d 2049 6e66 6f67 7261 7068 6963  .  - Infographic
+000034f0: 2056 5141 2056 616c 6964 6174 696f 6e20   VQA Validation 
+00003500: 2869 6e66 6f5f 7671 615f 7661 6c29 0a20  (info_vqa_val). 
+00003510: 202d 2049 6e66 6f67 7261 7068 6963 2056   - Infographic V
+00003520: 5141 2054 6573 7420 2869 6e66 6f5f 7671  QA Test (info_vq
+00003530: 615f 7465 7374 290a 2d20 4c4c 6156 412d  a_test).- LLaVA-
+00003540: 4265 6e63 6820 286c 6c61 7661 5f69 6e5f  Bench (llava_in_
+00003550: 7468 655f 7769 6c64 290a 2d20 4c4c 6156  the_wild).- LLaV
+00003560: 412d 4265 6e63 682d 434f 434f 2028 6c6c  A-Bench-COCO (ll
+00003570: 6176 615f 6265 6e63 685f 636f 636f 290a  ava_bench_coco).
+00003580: 2d20 4d61 7468 5669 7374 6120 286d 6174  - MathVista (mat
+00003590: 6876 6973 7461 290a 2020 2d20 4d61 7468  hvista).  - Math
+000035a0: 5669 7374 6120 5661 6c69 6461 7469 6f6e  Vista Validation
+000035b0: 2028 6d61 7468 7669 7374 615f 7465 7374   (mathvista_test
+000035c0: 6d69 6e69 290a 2020 2d20 4d61 7468 5669  mini).  - MathVi
+000035d0: 7374 6120 5465 7374 2028 6d61 7468 7669  sta Test (mathvi
+000035e0: 7374 615f 7465 7374 290a 2d20 4d4d 4265  sta_test).- MMBe
+000035f0: 6e63 6820 286d 6d62 656e 6368 290a 2020  nch (mmbench).  
+00003600: 2d20 4d4d 4265 6e63 6820 456e 676c 6973  - MMBench Englis
+00003610: 6820 286d 6d62 656e 6368 5f65 6e29 0a20  h (mmbench_en). 
+00003620: 2020 202d 204d 4d42 656e 6368 2045 6e67     - MMBench Eng
+00003630: 6c69 7368 2044 6576 2028 6d6d 6265 6e63  lish Dev (mmbenc
+00003640: 685f 656e 5f64 6576 290a 2020 2020 2d20  h_en_dev).    - 
+00003650: 4d4d 4265 6e63 6820 456e 676c 6973 6820  MMBench English 
+00003660: 5465 7374 2028 6d6d 6265 6e63 685f 656e  Test (mmbench_en
+00003670: 5f74 6573 7429 0a20 202d 204d 4d42 656e  _test).  - MMBen
+00003680: 6368 2043 6869 6e65 7365 2028 6d6d 6265  ch Chinese (mmbe
+00003690: 6e63 685f 636e 290a 2020 2020 2d20 4d4d  nch_cn).    - MM
+000036a0: 4265 6e63 6820 4368 696e 6573 6520 4465  Bench Chinese De
+000036b0: 7620 286d 6d62 656e 6368 5f63 6e5f 6465  v (mmbench_cn_de
+000036c0: 7629 0a20 2020 202d 204d 4d42 656e 6368  v).    - MMBench
+000036d0: 2043 6869 6e65 7365 2054 6573 7420 286d   Chinese Test (m
+000036e0: 6d62 656e 6368 5f63 6e5f 7465 7374 290a  mbench_cn_test).
+000036f0: 2d20 4d4d 4520 286d 6d65 290a 2d20 4d4d  - MME (mme).- MM
+00003700: 4d55 2028 6d6d 6d75 290a 2020 2d20 4d4d  MU (mmmu).  - MM
+00003710: 4d55 2056 616c 6964 6174 696f 6e20 286d  MU Validation (m
+00003720: 6d6d 755f 7661 6c29 0a20 202d 204d 4d4d  mmu_val).  - MMM
+00003730: 5520 5465 7374 2028 6d6d 6d75 5f74 6573  U Test (mmmu_tes
+00003740: 7429 0a2d 204d 4d56 6574 2028 6d6d 7665  t).- MMVet (mmve
+00003750: 7429 0a2d 204d 756c 7469 2d44 6f63 5651  t).- Multi-DocVQ
+00003760: 4120 286d 756c 7469 646f 6376 7161 290a  A (multidocvqa).
+00003770: 2020 2d20 4d75 6c74 692d 446f 6356 5141    - Multi-DocVQA
+00003780: 2056 616c 6964 6174 696f 6e20 286d 756c   Validation (mul
+00003790: 7469 646f 6376 7161 5f76 616c 290a 2020  tidocvqa_val).  
+000037a0: 2d20 4d75 6c74 692d 446f 6356 5141 2054  - Multi-DocVQA T
+000037b0: 6573 7420 286d 756c 7469 646f 6376 7161  est (multidocvqa
+000037c0: 5f74 6573 7429 0a2d 204e 6f43 6170 7320  _test).- NoCaps 
+000037d0: 286e 6f63 6170 7329 0a20 202d 204e 6f43  (nocaps).  - NoC
+000037e0: 6170 7320 5661 6c69 6461 7469 6f6e 2028  aps Validation (
+000037f0: 6e6f 6361 7073 5f76 616c 290a 2020 2d20  nocaps_val).  - 
+00003800: 4e6f 4361 7073 2054 6573 7420 286e 6f63  NoCaps Test (noc
+00003810: 6170 735f 7465 7374 290a 2d20 4f4b 5651  aps_test).- OKVQ
+00003820: 4120 286f 6b5f 7671 6129 0a20 202d 204f  A (ok_vqa).  - O
+00003830: 4b56 5141 2056 616c 6964 6174 696f 6e20  KVQA Validation 
+00003840: 3230 3134 2028 6f6b 5f76 7161 5f76 616c  2014 (ok_vqa_val
+00003850: 3230 3134 290a 2d20 504f 5045 2028 706f  2014).- POPE (po
+00003860: 7065 290a 2d20 5265 6643 4f43 4f20 2872  pe).- RefCOCO (r
+00003870: 6566 636f 636f 290a 2020 2020 2d20 7265  efcoco).    - re
+00003880: 6663 6f63 6f5f 7365 675f 7465 7374 0a20  fcoco_seg_test. 
+00003890: 2020 202d 2072 6566 636f 636f 5f73 6567     - refcoco_seg
+000038a0: 5f76 616c 0a20 2020 202d 2072 6566 636f  _val.    - refco
+000038b0: 636f 5f73 6567 5f74 6573 7441 0a20 2020  co_seg_testA.   
+000038c0: 202d 2072 6566 636f 636f 5f73 6567 5f74   - refcoco_seg_t
+000038d0: 6573 7442 0a20 2020 202d 2072 6566 636f  estB.    - refco
+000038e0: 636f 5f62 626f 785f 7465 7374 0a20 2020  co_bbox_test.   
+000038f0: 202d 2072 6566 636f 636f 5f62 626f 785f   - refcoco_bbox_
+00003900: 7661 6c0a 2020 2020 2d20 7265 6663 6f63  val.    - refcoc
+00003910: 6f5f 6262 6f78 5f74 6573 7441 0a20 2020  o_bbox_testA.   
+00003920: 202d 2072 6566 636f 636f 5f62 626f 785f   - refcoco_bbox_
+00003930: 7465 7374 420a 2d20 5265 6643 4f43 4f2b  testB.- RefCOCO+
+00003940: 2028 7265 6663 6f63 6f2b 290a 2020 2020   (refcoco+).    
+00003950: 2d20 7265 6663 6f63 6f2b 5f73 6567 0a20  - refcoco+_seg. 
+00003960: 2020 2020 2020 202d 2072 6566 636f 636f         - refcoco
+00003970: 2b5f 7365 675f 7661 6c0a 2020 2020 2020  +_seg_val.      
+00003980: 2020 2d20 7265 6663 6f63 6f2b 5f73 6567    - refcoco+_seg
+00003990: 5f74 6573 7441 0a20 2020 2020 2020 202d  _testA.        -
+000039a0: 2072 6566 636f 636f 2b5f 7365 675f 7465   refcoco+_seg_te
+000039b0: 7374 420a 2020 2020 2d20 7265 6663 6f63  stB.    - refcoc
+000039c0: 6f2b 5f62 626f 780a 2020 2020 2020 2020  o+_bbox.        
+000039d0: 2d20 7265 6663 6f63 6f2b 5f62 626f 785f  - refcoco+_bbox_
+000039e0: 7661 6c0a 2020 2020 2020 2020 2d20 7265  val.        - re
+000039f0: 6663 6f63 6f2b 5f62 626f 785f 7465 7374  fcoco+_bbox_test
+00003a00: 410a 2020 2020 2020 2020 2d20 7265 6663  A.        - refc
+00003a10: 6f63 6f2b 5f62 626f 785f 7465 7374 420a  oco+_bbox_testB.
+00003a20: 2d20 5265 6643 4f43 4f67 2028 7265 6663  - RefCOCOg (refc
+00003a30: 6f63 6f67 290a 2020 2020 2d20 7265 6663  ocog).    - refc
+00003a40: 6f63 6f67 5f73 6567 5f74 6573 740a 2020  ocog_seg_test.  
+00003a50: 2020 2d20 7265 6663 6f63 6f67 5f73 6567    - refcocog_seg
+00003a60: 5f76 616c 0a20 2020 202d 2072 6566 636f  _val.    - refco
+00003a70: 636f 675f 6262 6f78 5f74 6573 740a 2020  cog_bbox_test.  
+00003a80: 2020 2d20 7265 6663 6f63 6f67 5f62 626f    - refcocog_bbo
+00003a90: 785f 7661 6c0a 2d20 5363 6965 6e63 6551  x_val.- ScienceQ
+00003aa0: 4120 2873 6369 656e 6365 7161 5f66 756c  A (scienceqa_ful
+00003ab0: 6c29 0a20 202d 2053 6369 656e 6365 5141  l).  - ScienceQA
+00003ac0: 2046 756c 6c20 2873 6369 656e 6365 7161   Full (scienceqa
+00003ad0: 290a 2020 2d20 5363 6965 6e63 6551 4120  ).  - ScienceQA 
+00003ae0: 494d 4720 2873 6369 656e 6365 7161 5f69  IMG (scienceqa_i
+00003af0: 6d67 290a 2d20 5365 6564 4265 6e63 6820  mg).- SeedBench 
+00003b00: 2873 6565 6462 656e 6368 290a 2d20 5365  (seedbench).- Se
+00003b10: 6564 4265 6e63 6820 3220 2873 6565 6462  edBench 2 (seedb
+00003b20: 656e 6368 5f32 290a 2d20 5354 2d56 5141  ench_2).- ST-VQA
+00003b30: 2028 7374 7671 6129 0a2d 2054 6578 7443   (stvqa).- TextC
+00003b40: 6170 7320 2874 6578 7463 6170 7329 0a20  aps (textcaps). 
+00003b50: 202d 2054 6578 7443 6170 7320 5661 6c69   - TextCaps Vali
+00003b60: 6461 7469 6f6e 2028 7465 7874 6361 7073  dation (textcaps
+00003b70: 5f76 616c 290a 2020 2d20 5465 7874 4361  _val).  - TextCa
+00003b80: 7073 2054 6573 7420 2874 6578 7463 6170  ps Test (textcap
+00003b90: 735f 7465 7374 290a 2d20 5465 7874 5651  s_test).- TextVQ
+00003ba0: 4120 2874 6578 7476 7161 290a 2020 2d20  A (textvqa).  - 
+00003bb0: 5465 7874 5651 4120 5661 6c69 6461 7469  TextVQA Validati
+00003bc0: 6f6e 2028 7465 7874 7671 615f 7661 6c29  on (textvqa_val)
+00003bd0: 0a20 202d 2054 6578 7456 5141 2054 6573  .  - TextVQA Tes
+00003be0: 7420 2874 6578 7476 7161 5f74 6573 7429  t (textvqa_test)
+00003bf0: 0a2d 2056 697a 5769 7a56 5141 2028 7669  .- VizWizVQA (vi
+00003c00: 7a77 697a 5f76 7161 290a 2020 2d20 5669  zwiz_vqa).  - Vi
+00003c10: 7a57 697a 5651 4120 5661 6c69 6461 7469  zWizVQA Validati
+00003c20: 6f6e 2028 7669 7a77 697a 5f76 7161 5f76  on (vizwiz_vqa_v
+00003c30: 616c 290a 2020 2d20 5669 7a57 697a 5651  al).  - VizWizVQ
+00003c40: 4120 5465 7374 2028 7669 7a77 697a 5f76  A Test (vizwiz_v
+00003c50: 7161 5f74 6573 7429 0a2d 2056 5141 7632  qa_test).- VQAv2
+00003c60: 2028 7671 6176 3229 0a20 202d 2056 5141   (vqav2).  - VQA
+00003c70: 7632 2056 616c 6964 6174 696f 6e20 2876  v2 Validation (v
+00003c80: 7161 7632 5f76 616c 290a 2020 2d20 5651  qav2_val).  - VQ
+00003c90: 4176 3220 5465 7374 2028 7671 6176 325f  Av2 Test (vqav2_
+00003ca0: 7465 7374 290a 0a23 2320 4461 7461 7365  test)..## Datase
+00003cb0: 7473 2074 6f20 6265 2061 6464 6564 2061  ts to be added a
+00003cc0: 6e64 2074 6573 7465 640a 2d20 5461 6c6c  nd tested.- Tall
+00003cd0: 7951 4120 2874 616c 6c79 7161 290a 2d20  yQA (tallyqa).- 
+00003ce0: 5653 5220 2876 7372 290a 2d20 5769 6e6f  VSR (vsr).- Wino
+00003cf0: 6772 6f75 6e64 2028 7769 6e6f 6772 6f75  ground (winogrou
+00003d00: 6e64 290a 2d20 4e4c 5652 3220 286e 6c76  nd).- NLVR2 (nlv
+00003d10: 7232 290a 2d20 5261 7665 6e49 512d 5465  r2).- RavenIQ-Te
+00003d20: 7374 2028 7261 7665 6e69 7129 0a2d 2049  st (raveniq).- I
+00003d30: 636f 6e51 4120 2869 636f 6e71 6129 0a2d  conQA (iconqa).-
+00003d40: 2056 6973 7442 656e 6368 2028 7669 7374   VistBench (vist
+00003d50: 6265 6e63 6829 0a0a 2320 4164 6420 4375  bench)..# Add Cu
+00003d60: 7374 6f6d 697a 6564 204d 6f64 656c 2061  stomized Model a
+00003d70: 6e64 2044 6174 6173 6574 0a0a 506c 6561  nd Dataset..Plea
+00003d80: 7365 2072 6566 6572 2074 6f20 6f75 7220  se refer to our 
+00003d90: 5b64 6f63 756d 656e 7461 7469 6f6e 5d28  [documentation](
+00003da0: 646f 6373 2f52 4541 444d 452e 6d64 292e  docs/README.md).
+00003db0: 0a0a 2320 4163 6b6e 6f77 6c65 6467 656d  ..# Acknowledgem
+00003dc0: 656e 740a 0a6c 6d6d 735f 6576 616c 2069  ent..lmms_eval i
+00003dd0: 7320 6120 666f 726b 206f 6620 5b6c 6d2d  s a fork of [lm-
+00003de0: 6576 616c 2d68 6172 6e65 7373 5d28 6874  eval-harness](ht
+00003df0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00003e00: 2f45 6c65 7574 6865 7241 492f 6c6d 2d65  /EleutherAI/lm-e
+00003e10: 7661 6c75 6174 696f 6e2d 6861 726e 6573  valuation-harnes
+00003e20: 7329 2e20 5765 2072 6563 6f6d 6d65 6e64  s). We recommend
+00003e30: 2079 6f75 2074 6f20 7265 6164 2074 6872   you to read thr
+00003e40: 6f75 6768 2074 6865 205b 646f 6373 206f  ough the [docs o
+00003e50: 6620 6c6d 2d65 7661 6c2d 6861 726e 6573  f lm-eval-harnes
+00003e60: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
+00003e70: 622e 636f 6d2f 456c 6575 7468 6572 4149  b.com/EleutherAI
+00003e80: 2f6c 6d2d 6576 616c 7561 7469 6f6e 2d68  /lm-evaluation-h
+00003e90: 6172 6e65 7373 2f74 7265 652f 6d61 696e  arness/tree/main
+00003ea0: 2f64 6f63 7329 2066 6f72 2072 656c 6576  /docs) for relev
+00003eb0: 616e 7420 696e 666f 726d 6174 696f 6e2e  ant information.
+00003ec0: 200a 0a42 656c 6f77 2061 7265 2074 6865   ..Below are the
+00003ed0: 2063 6861 6e67 6573 2077 6520 6d61 6465   changes we made
+00003ee0: 2074 6f20 7468 6520 6f72 6967 696e 616c   to the original
+00003ef0: 2041 5049 3a0a 2d20 4275 696c 6420 636f   API:.- Build co
+00003f00: 6e74 6578 7420 6e6f 7720 6f6e 6c79 2070  ntext now only p
+00003f10: 6173 7320 696e 2069 6478 2061 6e64 2070  ass in idx and p
+00003f20: 726f 6365 7373 2069 6d61 6765 2061 6e64  rocess image and
+00003f30: 2064 6f63 2064 7572 696e 6720 7468 6520   doc during the 
+00003f40: 6d6f 6465 6c20 7265 7370 6f6e 6469 6e67  model responding
+00003f50: 2070 6861 7365 2e20 5468 6973 2069 7320   phase. This is 
+00003f60: 6475 6520 746f 2074 6865 2066 6163 7420  due to the fact 
+00003f70: 7468 6174 2064 6174 6173 6574 206e 6f77  that dataset now
+00003f80: 2063 6f6e 7461 696e 7320 6c6f 7473 206f   contains lots o
+00003f90: 6620 696d 6167 6573 2061 6e64 2077 6520  f images and we 
+00003fa0: 6361 6e27 7420 7374 6f72 6520 7468 656d  can't store them
+00003fb0: 2069 6e20 7468 6520 646f 6320 6c69 6b65   in the doc like
+00003fc0: 2074 6865 206f 7269 6769 6e61 6c20 6c6d   the original lm
+00003fd0: 2d65 7661 6c2d 6861 726e 6573 7320 6f74  -eval-harness ot
+00003fe0: 6865 7220 7769 7365 2074 6865 2063 7075  her wise the cpu
+00003ff0: 206d 656d 6f72 7920 776f 756c 6420 6578   memory would ex
+00004000: 706c 6f64 652e 0a2d 2049 6e73 7461 6e63  plode..- Instanc
+00004010: 652e 6172 6773 2028 6c6d 6d73 5f65 7661  e.args (lmms_eva
+00004020: 6c2f 6170 692f 696e 7374 616e 6365 2e70  l/api/instance.p
+00004030: 7929 206e 6f77 2063 6f6e 7461 696e 7320  y) now contains 
+00004040: 6120 6c69 7374 206f 6620 696d 6167 6573  a list of images
+00004050: 2074 6f20 6265 2069 6e70 7574 7465 6420   to be inputted 
+00004060: 746f 206c 6d6d 732e 0a2d 206c 6d2d 6576  to lmms..- lm-ev
+00004070: 616c 2d68 6172 6e65 7373 2073 7570 706f  al-harness suppo
+00004080: 7274 7320 616c 6c20 4846 206c 616e 6775  rts all HF langu
+00004090: 6167 6520 6d6f 6465 6c73 2061 7320 7369  age models as si
+000040a0: 6e67 6c65 206d 6f64 656c 2063 6c61 7373  ngle model class
+000040b0: 2e20 4375 7272 656e 746c 7920 7468 6973  . Currently this
+000040c0: 2069 7320 6e6f 7420 706f 7373 6962 6c65   is not possible
+000040d0: 206f 6620 6c6d 6d73 2062 6563 6175 7365   of lmms because
+000040e0: 2074 6865 2069 6e70 7574 2f6f 7574 7075   the input/outpu
+000040f0: 7420 666f 726d 6174 206f 6620 6c6d 6d73  t format of lmms
+00004100: 2069 6e20 4846 2061 7265 206e 6f74 2079   in HF are not y
+00004110: 6574 2075 6e69 6669 6564 2e20 5468 6572  et unified. Ther
+00004120: 6572 666f 7265 2c20 7765 2068 6176 6520  erfore, we have 
+00004130: 746f 2063 7265 6174 6520 6120 6e65 7720  to create a new 
+00004140: 636c 6173 7320 666f 7220 6561 6368 206c  class for each l
+00004150: 6d6d 7320 6d6f 6465 6c2e 2054 6869 7320  mms model. This 
+00004160: 6973 206e 6f74 2069 6465 616c 2061 6e64  is not ideal and
+00004170: 2077 6520 7769 6c6c 2074 7279 2074 6f20   we will try to 
+00004180: 756e 6966 7920 7468 656d 2069 6e20 7468  unify them in th
+00004190: 6520 6675 7475 7265 2e0a 0a57 6520 616c  e future...We al
+000041a0: 736f 2074 6861 6e6b 3a0a 2d20 5b58 6961  so thank:.- [Xia
+000041b0: 6e67 2059 7565 5d28 6874 7470 733a 2f2f  ng Yue](https://
+000041c0: 7869 616e 6779 7565 3936 3037 2e67 6974  xiangyue9607.git
+000041d0: 6875 622e 696f 2f29 2c20 5b4a 696e 676b  hub.io/), [Jingk
+000041e0: 616e 6720 5961 6e67 5d28 6874 7470 733a  ang Yang](https:
+000041f0: 2f2f 6a69 6e67 6b61 6e67 3530 2e67 6974  //jingkang50.git
+00004200: 6875 622e 696f 2f29 2c20 5b44 6f6e 6720  hub.io/), [Dong 
+00004210: 4775 6f5d 2868 7474 7073 3a2f 2f77 7777  Guo](https://www
+00004220: 2e6c 696e 6b65 6469 6e2e 636f 6d2f 696e  .linkedin.com/in
+00004230: 2f64 6f6e 6767 756f 7365 742f 2920 616e  /dongguoset/) an
+00004240: 6420 5b53 6865 6e67 2053 6865 6e5d 2868  d [Sheng Shen](h
+00004250: 7474 7073 3a2f 2f73 696e 6365 7261 7373  ttps://sincerass
+00004260: 2e67 6974 6875 622e 696f 2f29 2066 6f72  .github.io/) for
+00004270: 2065 6172 6c79 2064 6973 6375 7373 696f   early discussio
+00004280: 6e20 616e 6420 7465 7374 696e 672e 0a0a  n and testing...
+00004290: 2323 2043 6974 6174 696f 6e73 0a0a 6060  ## Citations..``
+000042a0: 6073 6865 6c6c 0a40 6d69 7363 7b6c 6d6d  `shell.@misc{lmm
+000042b0: 735f 6576 616c 3230 3234 2c0a 2020 2020  s_eval2024,.    
+000042c0: 7469 746c 653d 7b4c 4d4d 732d 4576 616c  title={LMMs-Eval
+000042d0: 3a20 4163 6365 6c65 7261 7469 6e67 2074  : Accelerating t
+000042e0: 6865 2044 6576 656c 6f70 6d65 6e74 206f  he Development o
+000042f0: 6620 4c61 7267 6520 4d75 6c74 696d 6f61  f Large Multimoa
+00004300: 6c20 4d6f 6465 6c73 7d2c 0a20 2020 2075  l Models},.    u
+00004310: 726c 3d7b 6874 7470 733a 2f2f 6769 7468  rl={https://gith
+00004320: 7562 2e63 6f6d 2f45 766f 6c76 696e 674c  ub.com/EvolvingL
+00004330: 4d4d 732d 4c61 622f 6c6d 6d73 2d65 7661  MMs-Lab/lmms-eva
+00004340: 6c7d 2c0a 2020 2020 6175 7468 6f72 3d7b  l},.    author={
+00004350: 426f 204c 692a 2c20 5065 6979 7561 6e20  Bo Li*, Peiyuan 
+00004360: 5a68 616e 672a 2c20 4b61 6963 6865 6e20  Zhang*, Kaichen 
+00004370: 5a68 616e 672a 2c20 4661 6e79 6920 5075  Zhang*, Fanyi Pu
+00004380: 2a2c 2058 696e 7275 6e20 4475 2c20 5975  *, Xinrun Du, Yu
+00004390: 6861 6f20 446f 6e67 2c20 4861 6f74 6961  hao Dong, Haotia
+000043a0: 6e20 4c69 752c 2059 7561 6e68 616e 205a  n Liu, Yuanhan Z
+000043b0: 6861 6e67 2c20 4765 205a 6861 6e67 2c20  hang, Ge Zhang, 
+000043c0: 4368 756e 7975 616e 204c 6920 616e 6420  Chunyuan Li and 
+000043d0: 5a69 7765 6920 4c69 757d 2c0a 2020 2020  Ziwei Liu},.    
+000043e0: 7075 626c 6973 6865 7220 2020 203d 207b  publisher    = {
+000043f0: 5a65 6e6f 646f 7d2c 0a20 2020 2076 6572  Zenodo},.    ver
+00004400: 7369 6f6e 2020 2020 2020 3d20 7b76 302e  sion      = {v0.
+00004410: 312e 307d 2c0a 2020 2020 6d6f 6e74 683d  1.0},.    month=
+00004420: 7b4d 6172 6368 7d2c 0a20 2020 2079 6561  {March},.    yea
+00004430: 723d 7b32 3032 347d 0a7d 0a60 6060 0a    r={2024}.}.```.
```

### Comparing `lmms_eval-0.1.1/README.md` & `lmms_eval-0.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -24,944 +24,978 @@
 00000170: 2f6c 6d6d 732d 6576 616c 2d30 2e31 2f29  /lmms-eval-0.1/)
 00000180: 207c 20f0 9f93 9a20 5b44 6f63 756d 656e   | .... [Documen
 00000190: 7461 7469 6f6e 5d28 646f 6373 2f52 4541  tation](docs/REA
 000001a0: 444d 452e 6d64 2920 7c20 f09f a497 205b  DME.md) | .... [
 000001b0: 4875 6767 696e 6766 6163 6520 4461 7461  Huggingface Data
 000001c0: 7365 7473 5d28 6874 7470 733a 2f2f 6875  sets](https://hu
 000001d0: 6767 696e 6766 6163 652e 636f 2f6c 6d6d  ggingface.co/lmm
-000001e0: 732d 6c61 6229 0a0a 496e 2061 6e20 6572  s-lab)..In an er
-000001f0: 6120 7768 6572 6520 7065 6f70 6c65 2070  a where people p
-00000200: 7572 7375 6520 4147 4920 2841 7274 6966  ursue AGI (Artif
-00000210: 6963 6961 6c20 4765 6e65 7261 6c20 496e  icial General In
-00000220: 7465 6c6c 6967 656e 6365 2920 7769 7468  telligence) with
-00000230: 2074 6865 207a 6561 6c20 616b 696e 2074   the zeal akin t
-00000240: 6f20 3139 3630 7320 6d6f 6f6e 206c 616e  o 1960s moon lan
-00000250: 6469 6e67 206d 6973 7369 6f6e 2e20 0a45  ding mission. .E
-00000260: 7661 6c75 6174 696e 6720 7468 6520 636f  valuating the co
-00000270: 7265 206f 6620 4147 492c 2074 6865 206c  re of AGI, the l
-00000280: 6172 6765 206c 616e 6775 6167 6520 6d6f  arge language mo
-00000290: 6465 6c73 2028 4c4c 4d73 2920 616e 6420  dels (LLMs) and 
-000002a0: 6c61 7267 6520 6d75 6c74 696d 6f64 616c  large multimodal
-000002b0: 206d 6f64 656c 7320 284c 4d4d 7329 2077   models (LMMs) w
-000002c0: 6974 6820 756e 7072 6563 6564 656e 7465  ith unprecedente
-000002d0: 6420 6361 7061 6269 6c69 7469 6573 2074  d capabilities t
-000002e0: 6861 7420 6361 6e20 756e 6465 7273 7461  hat can understa
-000002f0: 6e64 2c20 6c65 6172 6e2c 2061 6e64 2069  nd, learn, and i
-00000300: 6e74 6572 6163 7420 6163 726f 7373 2061  nteract across a
-00000310: 2062 726f 6164 2072 616e 6765 206f 6620   broad range of 
-00000320: 6875 6d61 6e20 7461 736b 732c 2068 6173  human tasks, has
-00000330: 2062 6563 6f6d 6520 6120 7069 766f 7461   become a pivota
-00000340: 6c20 6368 616c 6c65 6e67 652e 0a0a 546f  l challenge...To
-00000350: 2073 7572 6d6f 756e 7420 7468 6973 2c20   surmount this, 
-00000360: 6120 6272 6f61 6420 7370 6563 7472 756d  a broad spectrum
-00000370: 206f 6620 6576 616c 7561 7469 6f6e 2064   of evaluation d
-00000380: 6174 6173 6574 7320 6973 2070 726f 706f  atasets is propo
-00000390: 7365 6420 616e 6420 7573 6564 2074 6f20  sed and used to 
-000003a0: 6173 7365 7373 206d 6f64 656c 2063 6170  assess model cap
-000003b0: 6162 696c 6974 6965 7320 6163 726f 7373  abilities across
-000003c0: 2076 6172 696f 7573 2064 696d 656e 7369   various dimensi
-000003d0: 6f6e 732c 2063 7265 6174 696e 6720 6120  ons, creating a 
-000003e0: 636f 6d70 7265 6865 6e73 6976 6520 6361  comprehensive ca
-000003f0: 7061 6269 6c69 7479 2063 6861 7274 2074  pability chart t
-00000400: 6861 7420 7265 7665 616c 7320 7468 6520  hat reveals the 
-00000410: 7472 7565 2070 6572 666f 726d 616e 6365  true performance
-00000420: 206f 6620 6d6f 6465 6c73 2e20 486f 7765   of models. Howe
-00000430: 7665 722c 2065 7661 6c75 6174 696f 6e20  ver, evaluation 
-00000440: 6f66 206d 6f64 656c 7320 6861 7320 6265  of models has be
-00000450: 636f 6d65 2071 7569 7465 2068 6172 6420  come quite hard 
-00000460: 7369 6e63 6520 7468 6572 6520 6172 6520  since there are 
-00000470: 636f 756e 746c 6573 7320 6576 616c 7561  countless evalua
-00000480: 7469 6f6e 2062 656e 6368 6d61 726b 7320  tion benchmarks 
-00000490: 616e 6420 6461 7461 7365 7473 206f 7267  and datasets org
-000004a0: 616e 697a 6564 2069 6e20 7661 7269 6f75  anized in variou
-000004b0: 7320 7761 7973 2c20 7363 6174 7465 7265  s ways, scattere
-000004c0: 6420 6163 726f 7373 2074 6865 2069 6e74  d across the int
-000004d0: 6572 6e65 742c 2073 6c65 6570 696e 6720  ernet, sleeping 
-000004e0: 696e 2073 6f6d 6562 6f64 7927 7320 476f  in somebody's Go
-000004f0: 6f67 6c65 2044 7269 7665 2c20 4472 6f70  ogle Drive, Drop
-00000500: 626f 782c 2061 6e64 206f 7468 6572 2077  box, and other w
-00000510: 6562 7369 7465 7320 686f 7374 6564 2062  ebsites hosted b
-00000520: 7920 7363 686f 6f6c 7320 6f72 2072 6573  y schools or res
-00000530: 6561 7263 6820 6c61 6273 2e0a 0a49 6e20  earch labs...In 
-00000540: 7468 6520 6669 656c 6420 6f66 206c 616e  the field of lan
-00000550: 6775 6167 6520 6d6f 6465 6c73 2c20 7468  guage models, th
-00000560: 6572 6520 6861 7320 6265 656e 2061 2076  ere has been a v
-00000570: 616c 7561 626c 6520 7072 6563 6564 656e  aluable preceden
-00000580: 7420 7365 7420 6279 2074 6865 2077 6f72  t set by the wor
-00000590: 6b20 6f66 205b 6c6d 2d65 7661 6c75 6174  k of [lm-evaluat
-000005a0: 696f 6e2d 6861 726e 6573 735d 2868 7474  ion-harness](htt
-000005b0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000005c0: 456c 6575 7468 6572 4149 2f6c 6d2d 6576  EleutherAI/lm-ev
-000005d0: 616c 7561 7469 6f6e 2d68 6172 6e65 7373  aluation-harness
-000005e0: 292e 2054 6865 7920 6f66 6665 7220 696e  ). They offer in
-000005f0: 7465 6772 6174 6564 2064 6174 6120 616e  tegrated data an
-00000600: 6420 6d6f 6465 6c20 696e 7465 7266 6163  d model interfac
-00000610: 6573 2c20 656e 6162 6c69 6e67 2072 6170  es, enabling rap
-00000620: 6964 2065 7661 6c75 6174 696f 6e20 6f66  id evaluation of
-00000630: 206c 616e 6775 6167 6520 6d6f 6465 6c73   language models
-00000640: 2061 6e64 2073 6572 7669 6e67 2061 7320   and serving as 
-00000650: 7468 6520 6261 636b 656e 6420 7375 7070  the backend supp
-00000660: 6f72 7420 6672 616d 6577 6f72 6b20 666f  ort framework fo
-00000670: 7220 7468 6520 5b6f 7065 6e2d 6c6c 6d2d  r the [open-llm-
-00000680: 6c65 6164 6572 626f 6172 645d 2868 7474  leaderboard](htt
-00000690: 7073 3a2f 2f68 7567 6769 6e67 6661 6365  ps://huggingface
-000006a0: 2e63 6f2f 7370 6163 6573 2f48 7567 6769  .co/spaces/Huggi
-000006b0: 6e67 4661 6365 4834 2f6f 7065 6e5f 6c6c  ngFaceH4/open_ll
-000006c0: 6d5f 6c65 6164 6572 626f 6172 6429 2c20  m_leaderboard), 
-000006d0: 616e 6420 6861 7320 6772 6164 7561 6c6c  and has graduall
-000006e0: 7920 6265 636f 6d65 2074 6865 2075 6e64  y become the und
-000006f0: 6572 6c79 696e 6720 6563 6f73 7973 7465  erlying ecosyste
-00000700: 6d20 6f66 2074 6865 2065 7261 206f 6620  m of the era of 
-00000710: 666f 756e 6461 7469 6f6e 206d 6f64 656c  foundation model
-00000720: 732e 0a0a 486f 7765 7665 722c 2074 686f  s...However, tho
-00000730: 7567 6820 7468 6572 6520 6172 6520 6d61  ugh there are ma
-00000740: 6e79 206e 6577 2065 7661 6c75 6174 696f  ny new evaluatio
-00000750: 6e20 6461 7461 7365 7473 2061 7265 2072  n datasets are r
-00000760: 6563 656e 746c 7920 7072 6f70 6f73 6564  ecently proposed
-00000770: 2c20 7468 6520 6566 6669 6369 656e 7420  , the efficient 
-00000780: 6576 616c 7561 7469 6f6e 2070 6970 656c  evaluation pipel
-00000790: 696e 6520 6f66 204c 4d4d 2069 7320 7374  ine of LMM is st
-000007a0: 696c 6c20 696e 2069 7473 2069 6e66 616e  ill in its infan
-000007b0: 6379 2c20 616e 6420 7468 6572 6520 6973  cy, and there is
-000007c0: 206e 6f20 756e 6966 6965 6420 6576 616c   no unified eval
-000007d0: 7561 7469 6f6e 2066 7261 6d65 776f 726b  uation framework
-000007e0: 2074 6861 7420 6361 6e20 6265 2075 7365   that can be use
-000007f0: 6420 746f 2065 7661 6c75 6174 6520 4c4d  d to evaluate LM
-00000800: 4d20 6163 726f 7373 2061 2077 6964 6520  M across a wide 
-00000810: 7261 6e67 6520 6f66 2064 6174 6173 6574  range of dataset
-00000820: 732e 2054 6f20 6164 6472 6573 7320 7468  s. To address th
-00000830: 6973 2063 6861 6c6c 656e 6765 2c20 7765  is challenge, we
-00000840: 2069 6e74 726f 6475 6365 202a 2a6c 6d6d   introduce **lmm
-00000850: 732d 6576 616c 2a2a 2c20 616e 2065 7661  s-eval**, an eva
-00000860: 6c75 6174 696f 6e20 6672 616d 6577 6f72  luation framewor
-00000870: 6b20 6d65 7469 6375 6c6f 7573 6c79 2063  k meticulously c
-00000880: 7261 6674 6564 2066 6f72 2063 6f6e 7369  rafted for consi
-00000890: 7374 656e 7420 616e 6420 6566 6669 6369  stent and effici
-000008a0: 656e 7420 6576 616c 7561 7469 6f6e 206f  ent evaluation o
-000008b0: 6620 4c4d 4d2e 0a0a 5765 2068 756d 626c  f LMM...We humbl
-000008c0: 7920 6f62 736f 7262 6564 2074 6865 2065  y obsorbed the e
-000008d0: 7871 7569 7369 7465 2061 6e64 2065 6666  xquisite and eff
-000008e0: 6963 6965 6e74 2064 6573 6967 6e20 6f66  icient design of
-000008f0: 205b 6c6d 2d65 7661 6c75 6174 696f 6e2d   [lm-evaluation-
-00000900: 6861 726e 6573 735d 2868 7474 7073 3a2f  harness](https:/
-00000910: 2f67 6974 6875 622e 636f 6d2f 456c 6575  /github.com/Eleu
-00000920: 7468 6572 4149 2f6c 6d2d 6576 616c 7561  therAI/lm-evalua
-00000930: 7469 6f6e 2d68 6172 6e65 7373 292e 2042  tion-harness). B
-00000940: 7569 6c64 696e 6720 7570 6f6e 2069 7473  uilding upon its
-00000950: 2066 6f75 6e64 6174 696f 6e2c 2077 6520   foundation, we 
-00000960: 696d 706c 656d 656e 7465 6420 6f75 7220  implemented our 
-00000970: 606c 6d6d 732d 6576 616c 6020 6672 616d  `lmms-eval` fram
-00000980: 6577 6f72 6b20 7769 7468 2070 6572 666f  ework with perfo
-00000990: 726d 616e 6365 206f 7074 696d 697a 6174  rmance optimizat
-000009a0: 696f 6e73 2073 7065 6369 6669 6361 6c6c  ions specificall
-000009b0: 7920 666f 7220 4c4d 4d73 2e0a 0a23 2320  y for LMMs...## 
-000009c0: 4e65 6365 7373 6974 7920 6f66 206c 6d6d  Necessity of lmm
-000009d0: 732d 6576 616c 0a0a 5765 2062 656c 6965  s-eval..We belie
-000009e0: 7665 206f 7572 2065 6666 6f72 7420 636f  ve our effort co
-000009f0: 756c 6420 7072 6f76 6964 6520 616e 2065  uld provide an e
-00000a00: 6666 6963 6965 6e74 2069 6e74 6572 6661  fficient interfa
-00000a10: 6365 2066 6f72 2074 6865 2064 6574 6169  ce for the detai
-00000a20: 6c65 6420 636f 6d70 6172 6973 6f6e 206f  led comparison o
-00000a30: 6620 7075 626c 6963 6c79 2061 7661 696c  f publicly avail
-00000a40: 6162 6c65 206d 6f64 656c 7320 746f 2064  able models to d
-00000a50: 6973 6365 726e 2074 6865 6972 2073 7472  iscern their str
-00000a60: 656e 6774 6873 2061 6e64 2077 6561 6b6e  engths and weakn
-00000a70: 6573 7365 732e 2049 7427 7320 616c 736f  esses. It's also
-00000a80: 2075 7365 6675 6c20 666f 7220 7265 7365   useful for rese
-00000a90: 6172 6368 2069 6e73 7469 7475 7469 6f6e  arch institution
-00000aa0: 7320 616e 6420 7072 6f64 7563 7469 6f6e  s and production
-00000ab0: 2d6f 7269 656e 7465 6420 636f 6d70 616e  -oriented compan
-00000ac0: 6965 7320 746f 2061 6363 656c 6572 6174  ies to accelerat
-00000ad0: 6520 7468 6520 6465 7665 6c6f 706d 656e  e the developmen
-00000ae0: 7420 6f66 206c 6172 6765 206d 756c 7469  t of large multi
-00000af0: 6d6f 6461 6c20 6d6f 6465 6c73 2e20 5769  modal models. Wi
-00000b00: 7468 2074 6865 2060 6c6d 6d73 2d65 7661  th the `lmms-eva
-00000b10: 6c60 2c20 7765 2068 6176 6520 7369 676e  l`, we have sign
-00000b20: 6966 6963 616e 746c 7920 6163 6365 6c65  ificantly accele
-00000b30: 7261 7465 6420 7468 6520 6c69 6665 6379  rated the lifecy
-00000b40: 636c 6520 6f66 206d 6f64 656c 2069 7465  cle of model ite
-00000b50: 7261 7469 6f6e 2e20 496e 7369 6465 2074  ration. Inside t
-00000b60: 6865 204c 4c61 5641 2074 6561 6d2c 2074  he LLaVA team, t
-00000b70: 6865 2075 7469 6c69 7a61 7469 6f6e 206f  he utilization o
-00000b80: 6620 606c 6d6d 732d 6576 616c 6020 6c61  f `lmms-eval` la
-00000b90: 7267 656c 7920 696d 7072 6f76 6573 2074  rgely improves t
-00000ba0: 6865 2065 6666 6963 6965 6e63 7920 6f66  he efficiency of
-00000bb0: 2074 6865 206d 6f64 656c 2064 6576 656c   the model devel
-00000bc0: 6f70 6d65 6e74 2063 7963 6c65 2c20 6173  opment cycle, as
-00000bd0: 2077 6520 6172 6520 6162 6c65 2074 6f20   we are able to 
-00000be0: 6576 616c 7561 7465 2077 6565 6b6c 7920  evaluate weekly 
-00000bf0: 7472 6169 6e65 6420 6875 6e64 7265 6473  trained hundreds
-00000c00: 206f 6620 6368 6563 6b70 6f69 6e74 7320   of checkpoints 
-00000c10: 6f6e 2032 302d 3330 2064 6174 6173 6574  on 20-30 dataset
-00000c20: 732c 2069 6465 6e74 6966 7969 6e67 2074  s, identifying t
-00000c30: 6865 2073 7472 656e 6774 6873 2061 6e64  he strengths and
-00000c40: 2077 6561 6b6e 6573 7365 732c 2061 6e64   weaknesses, and
-00000c50: 2074 6865 6e20 6d61 6b65 2074 6172 6765   then make targe
-00000c60: 7465 6420 696d 7072 6f76 656d 656e 7473  ted improvements
-00000c70: 2e0a 0a23 2041 6e6e 6f75 6365 6d65 6e74  ...# Annoucement
-00000c80: 0a0a 2323 2076 302e 312e 3020 5265 6c65  ..## v0.1.0 Rele
-00000c90: 6173 6564 0a0a 5468 6520 6669 7273 7420  ased..The first 
-00000ca0: 7665 7273 696f 6e20 6f66 2074 6865 2060  version of the `
-00000cb0: 6c6d 6d73 2d65 7661 6c60 2069 7320 7265  lmms-eval` is re
-00000cc0: 6c65 6173 6564 2e20 5765 2061 7265 2077  leased. We are w
-00000cd0: 6f72 6b69 6e67 206f 6e20 7072 6f76 6964  orking on provid
-00000ce0: 696e 6720 616e 206f 6e65 2d63 6f6d 6d61  ing an one-comma
-00000cf0: 6e64 2065 7661 6c75 6174 696f 6e20 7375  nd evaluation su
-00000d00: 6974 6520 666f 7220 6163 6365 6c65 7261  ite for accelera
-00000d10: 7469 6e67 2074 6865 2064 6576 656c 6f70  ting the develop
-00000d20: 6d65 6e74 206f 6620 4c4d 4d73 2e20 0a0a  ment of LMMs. ..
-00000d30: 3e20 496e 205b 4c4c 6156 4120 4e65 7874  > In [LLaVA Next
-00000d40: 5d28 6874 7470 733a 2f2f 6c6c 6176 612d  ](https://llava-
-00000d50: 766c 2e67 6974 6875 622e 696f 2f62 6c6f  vl.github.io/blo
-00000d60: 672f 3230 3234 2d30 312d 3330 2d6c 6c61  g/2024-01-30-lla
-00000d70: 7661 2d6e 6578 742f 2920 6465 7665 6c6f  va-next/) develo
-00000d80: 706d 656e 742c 2077 6520 696e 7465 726e  pment, we intern
-00000d90: 616c 6c79 2075 7469 6c69 7a65 2074 6869  ally utilize thi
-00000da0: 7320 7375 6974 6520 746f 2065 7661 6c75  s suite to evalu
-00000db0: 6174 6520 7468 6520 6d75 6c74 6970 6c65  ate the multiple
-00000dc0: 2064 6966 6665 7265 6e74 206d 6f64 656c   different model
-00000dd0: 2076 6572 7369 6f6e 7320 6f6e 2076 6172   versions on var
-00000de0: 696f 7573 2064 6174 6173 6574 732e 2049  ious datasets. I
-00000df0: 7420 7369 676e 6966 6963 616e 746c 7920  t significantly 
-00000e00: 6163 6365 6c65 7261 7465 7320 7468 6520  accelerates the 
-00000e10: 6d6f 6465 6c20 6465 7665 6c6f 706d 656e  model developmen
-00000e20: 7420 6379 636c 6520 666f 7220 6974 2773  t cycle for it's
-00000e30: 2065 6173 7920 696e 7465 6772 6174 696f   easy integratio
-00000e40: 6e20 616e 6420 6661 7374 2065 7661 6c75  n and fast evalu
-00000e50: 6174 696f 6e20 7370 6565 642e 0a0a 5468  ation speed...Th
-00000e60: 6520 6d61 696e 2066 6561 7475 7265 2069  e main feature i
-00000e70: 6e63 6c75 6465 733a 0a0a 3c70 2061 6c69  ncludes:..<p ali
-00000e80: 676e 3d22 6365 6e74 6572 2220 7769 6474  gn="center" widt
-00000e90: 683d 2231 3030 2522 3e0a 3c69 6d67 2073  h="100%">.<img s
-00000ea0: 7263 3d22 6874 7470 733a 2f2f 692e 706f  rc="https://i.po
-00000eb0: 7374 696d 672e 6363 2f73 677a 4e6d 4a78  stimg.cc/sgzNmJx
-00000ec0: 372f 7465 6173 6572 2e70 6e67 2220 2077  7/teaser.png"  w
-00000ed0: 6964 7468 3d22 3130 3025 2220 6865 6967  idth="100%" heig
-00000ee0: 6874 3d22 3830 2522 3e0a 3c2f 703e 0a0a  ht="80%">.</p>..
-00000ef0: 2323 2320 4f6e 652d 636f 6d6d 616e 6420  ### One-command 
-00000f00: 6576 616c 7561 7469 6f6e 2c20 7769 7468  evaluation, with
-00000f10: 2064 6574 6169 6c65 6420 6c6f 6773 2061   detailed logs a
-00000f20: 6e64 2073 616d 706c 6573 2e0a 596f 7520  nd samples..You 
-00000f30: 6361 6e20 6576 616c 7561 7465 2074 6865  can evaluate the
-00000f40: 206d 6f64 656c 7320 6f6e 206d 756c 7469   models on multi
-00000f50: 706c 6520 6461 7461 7365 7473 2077 6974  ple datasets wit
-00000f60: 6820 6120 7369 6e67 6c65 2063 6f6d 6d61  h a single comma
-00000f70: 6e64 2e20 4e6f 206d 6f64 656c 2f64 6174  nd. No model/dat
-00000f80: 6120 7072 6570 6172 6174 696f 6e20 6973  a preparation is
-00000f90: 206e 6565 6465 642c 206a 7573 7420 6f6e   needed, just on
-00000fa0: 6520 636f 6d6d 616e 6420 6c69 6e65 2c20  e command line, 
-00000fb0: 6665 7720 6d69 6e75 7465 732c 2061 6e64  few minutes, and
-00000fc0: 2067 6574 2074 6865 2072 6573 756c 7473   get the results
-00000fd0: 2e20 4e6f 7420 6a75 7374 2061 2072 6573  . Not just a res
-00000fe0: 756c 7420 6e75 6d62 6572 2c20 6275 7420  ult number, but 
-00000ff0: 616c 736f 2074 6865 2064 6574 6169 6c65  also the detaile
-00001000: 6420 6c6f 6773 2061 6e64 2073 616d 706c  d logs and sampl
-00001010: 6573 2c20 696e 636c 7564 696e 6720 7468  es, including th
-00001020: 6520 6d6f 6465 6c20 6172 6773 2c20 696e  e model args, in
-00001030: 7075 7420 7175 6573 7469 6f6e 2c20 6d6f  put question, mo
-00001040: 6465 6c20 7265 7370 6f6e 7365 2c20 616e  del response, an
-00001050: 6420 6772 6f75 6e64 2074 7275 7468 2061  d ground truth a
-00001060: 6e73 7765 722e 0a0a 6060 6070 7974 686f  nswer...```pytho
-00001070: 6e0a 2320 4576 616c 7561 7469 6e67 204c  n.# Evaluating L
-00001080: 4c61 5641 206f 6e20 6d75 6c74 6970 6c65  LaVA on multiple
-00001090: 2064 6174 6173 6574 730a 6163 6365 6c65   datasets.accele
-000010a0: 7261 7465 206c 6175 6e63 6820 2d2d 6e75  rate launch --nu
-000010b0: 6d5f 7072 6f63 6573 7365 733d 3820 2d6d  m_processes=8 -m
-000010c0: 206c 6d6d 735f 6576 616c 202d 2d6d 6f64   lmms_eval --mod
-000010d0: 656c 206c 6c61 7661 2020 202d 2d6d 6f64  el llava   --mod
-000010e0: 656c 5f61 7267 7320 7072 6574 7261 696e  el_args pretrain
-000010f0: 6564 3d22 6c69 7568 616f 7469 616e 2f6c  ed="liuhaotian/l
-00001100: 6c61 7661 2d76 312e 352d 3762 2220 2020  lava-v1.5-7b"   
-00001110: 2d2d 7461 736b 7320 6d6d 652c 6d6d 6265  --tasks mme,mmbe
-00001120: 6e63 685f 656e 202d 2d62 6174 6368 5f73  nch_en --batch_s
-00001130: 697a 6520 3120 2d2d 6c6f 675f 7361 6d70  ize 1 --log_samp
-00001140: 6c65 7320 2d2d 6c6f 675f 7361 6d70 6c65  les --log_sample
-00001150: 735f 7375 6666 6978 206c 6c61 7661 5f76  s_suffix llava_v
-00001160: 312e 355f 6d6d 655f 6d6d 6265 6e63 6865  1.5_mme_mmbenche
-00001170: 6e20 2d2d 6f75 7470 7574 5f70 6174 6820  n --output_path 
-00001180: 2e2f 6c6f 6773 2f20 230a 6060 600a 0a23  ./logs/ #.```..#
-00001190: 2323 2041 6363 656c 6572 6174 6f72 2073  ## Accelerator s
-000011a0: 7570 706f 7274 2061 6e64 2054 6173 6b73  upport and Tasks
-000011b0: 2067 726f 7570 696e 672e 0a57 6520 7375   grouping..We su
-000011c0: 7070 6f72 7420 7468 6520 7573 6167 6520  pport the usage 
-000011d0: 6f66 2060 6163 6365 6c65 7261 7465 6020  of `accelerate` 
-000011e0: 746f 2077 7261 7020 7468 6520 6d6f 6465  to wrap the mode
-000011f0: 6c20 666f 7220 6469 7374 7269 6275 7465  l for distribute
-00001200: 6420 6576 616c 7561 7469 6f6e 2c20 7375  d evaluation, su
-00001210: 7070 6f72 7469 6e67 206d 756c 7469 2d67  pporting multi-g
-00001220: 7075 2061 6e64 2074 656e 736f 7220 7061  pu and tensor pa
-00001230: 7261 6c6c 656c 6973 6d2e 2057 6974 6820  rallelism. With 
-00001240: 2a2a 5461 736b 2047 726f 7570 696e 672a  **Task Grouping*
-00001250: 2a2c 2061 6c6c 2069 6e73 7461 6e63 6573  *, all instances
-00001260: 2066 726f 6d20 616c 6c20 7461 736b 7320   from all tasks 
-00001270: 6172 6520 6772 6f75 7065 6420 616e 6420  are grouped and 
-00001280: 6576 616c 7561 7465 6420 696e 2070 6172  evaluated in par
-00001290: 616c 6c65 6c2c 2077 6869 6368 2073 6967  allel, which sig
-000012a0: 6e69 6669 6361 6e74 6c79 2069 6d70 726f  nificantly impro
-000012b0: 7665 7320 7468 6520 7468 726f 7567 6870  ves the throughp
-000012c0: 7574 206f 6620 7468 6520 6576 616c 7561  ut of the evalua
-000012d0: 7469 6f6e 2e20 4166 7465 7220 6576 616c  tion. After eval
-000012e0: 7561 7469 6f6e 2c20 616c 6c20 696e 7374  uation, all inst
-000012f0: 616e 6365 7320 6172 6520 7365 6e74 2074  ances are sent t
-00001300: 6f20 706f 7374 7072 6f63 6573 7369 6e67  o postprocessing
-00001310: 206d 6f64 756c 6520 666f 7220 6d65 7472   module for metr
-00001320: 6963 2063 616c 6375 6174 696f 6e73 2061  ic calcuations a
-00001330: 6e64 2070 6f74 656e 7469 616c 2047 5054  nd potential GPT
-00001340: 342d 6576 616c 2071 7565 7269 6573 2e0a  4-eval queries..
-00001350: 0a42 656c 6f77 2061 7265 2074 6865 2074  .Below are the t
-00001360: 6f74 616c 2072 756e 7469 6d65 206f 6e20  otal runtime on 
-00001370: 6469 6666 6572 656e 7420 6461 7461 7365  different datase
-00001380: 7473 2075 7369 6e67 2034 2078 2041 3130  ts using 4 x A10
-00001390: 3020 3430 472e 0a0a 7c20 4461 7461 7365  0 40G...| Datase
-000013a0: 7420 2823 6e75 6d29 2020 2020 2020 2020  t (#num)        
-000013b0: 2020 7c20 4c4c 6156 412d 7631 2e35 2d37    | LLaVA-v1.5-7
-000013c0: 6220 2020 2020 207c 204c 4c61 5641 2d76  b      | LLaVA-v
-000013d0: 312e 352d 3133 6220 2020 2020 7c0a 7c20  1.5-13b     |.| 
-000013e0: 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :---------------
-000013f0: 2d2d 2d2d 2d2d 2d20 7c20 3a2d 2d2d 2d2d  ------- | :-----
-00001400: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c 203a  ------------ | :
-00001410: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001420: 2d20 7c0a 7c20 6d6d 6520 2832 3337 3429  - |.| mme (2374)
-00001430: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00001440: 3220 6d69 6e73 2034 3320 7365 636f 6e64  2 mins 43 second
-00001450: 7320 207c 2033 206d 696e 7320 3237 2073  s  | 3 mins 27 s
-00001460: 6563 6f6e 6473 2020 7c0a 7c20 6771 6120  econds  |.| gqa 
-00001470: 2831 3235 3738 2920 2020 2020 2020 2020  (12578)         
-00001480: 2020 2020 7c20 3130 206d 696e 7320 3433      | 10 mins 43
-00001490: 2073 6563 6f6e 6473 207c 2031 3420 6d69   seconds | 14 mi
-000014a0: 6e73 2032 3320 7365 636f 6e64 7320 7c0a  ns 23 seconds |.
-000014b0: 7c20 7363 6965 6e63 6571 615f 696d 6720  | scienceqa_img 
-000014c0: 2832 3031 3729 2020 2020 7c20 3120 6d69  (2017)    | 1 mi
-000014d0: 6e73 2035 3820 7365 636f 6e64 7320 207c  ns 58 seconds  |
-000014e0: 2032 206d 696e 7320 3532 2073 6563 6f6e   2 mins 52 secon
-000014f0: 6473 2020 7c0a 7c20 6169 3264 2028 3330  ds  |.| ai2d (30
-00001500: 3838 2920 2020 2020 2020 2020 2020 2020  88)             
-00001510: 7c20 3320 6d69 6e73 2031 3720 7365 636f  | 3 mins 17 seco
-00001520: 6e64 7320 207c 2034 206d 696e 7320 3132  nds  | 4 mins 12
-00001530: 2073 6563 6f6e 6473 2020 7c0a 7c20 636f   seconds  |.| co
-00001540: 636f 3230 3137 5f63 6170 5f76 616c 2028  co2017_cap_val (
-00001550: 3530 3030 2920 7c20 3134 206d 696e 7320  5000) | 14 mins 
-00001560: 3133 2073 6563 6f6e 6473 207c 2031 3920  13 seconds | 19 
-00001570: 6d69 6e73 2035 3820 7365 636f 6e64 7320  mins 58 seconds 
-00001580: 7c0a 0a23 2323 2041 6c6c 2d49 6e2d 4f6e  |..### All-In-On
-00001590: 6520 4846 2064 6174 6173 6574 2068 7562  e HF dataset hub
-000015a0: 732e 0a0a 5765 2061 7265 2068 6f73 7469  s...We are hosti
-000015b0: 6e67 206d 6f72 6520 7468 616e 2034 3020  ng more than 40 
-000015c0: 2861 6e64 2069 6e63 7265 6173 696e 6729  (and increasing)
-000015d0: 2064 6174 6173 6574 7320 6f6e 205b 6875   datasets on [hu
-000015e0: 6767 696e 6766 6163 652f 6c6d 6d73 2d6c  ggingface/lmms-l
-000015f0: 6162 5d28 6874 7470 733a 2f2f 6875 6767  ab](https://hugg
-00001600: 696e 6766 6163 652e 636f 2f6c 6d6d 732d  ingface.co/lmms-
-00001610: 6c61 6229 2c20 7765 2063 6172 6566 756c  lab), we careful
-00001620: 6c79 2063 6f6e 7665 7274 6564 2074 6865  ly converted the
-00001630: 7365 2064 6174 6173 6574 7320 6672 6f6d  se datasets from
-00001640: 206f 7269 6769 6e61 6c20 736f 7572 6365   original source
-00001650: 7320 616e 6420 696e 636c 7564 6564 2061  s and included a
-00001660: 6c6c 2076 6172 6961 6e74 732c 2076 6572  ll variants, ver
-00001670: 7369 6f6e 7320 616e 6420 7370 6c69 7473  sions and splits
-00001680: 2e20 4e6f 7720 7468 6579 2063 616e 2062  . Now they can b
-00001690: 6520 6469 7265 6374 6c79 2061 6363 6573  e directly acces
-000016a0: 7365 6420 7769 7468 6f75 7420 616e 7920  sed without any 
-000016b0: 6275 7264 656e 206f 6620 6461 7461 2070  burden of data p
-000016c0: 7265 7072 6f63 6573 7369 6e67 2e20 5468  reprocessing. Th
-000016d0: 6579 2061 6c73 6f20 7365 7276 6520 666f  ey also serve fo
-000016e0: 7220 7468 6520 7075 7270 6f73 6520 6f66  r the purpose of
-000016f0: 2076 6973 7561 6c69 7a69 6e67 2074 6865   visualizing the
-00001700: 2064 6174 6120 616e 6420 6772 6173 7069   data and graspi
-00001710: 6e67 2074 6865 2073 656e 7365 206f 6620  ng the sense of 
-00001720: 6576 616c 7561 7469 6f6e 2074 6173 6b73  evaluation tasks
-00001730: 2064 6973 7472 6962 7574 696f 6e2e 0a0a   distribution...
-00001740: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
-00001750: 2220 7769 6474 683d 2231 3030 2522 3e0a  " width="100%">.
-00001760: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00001770: 2f2f 692e 706f 7374 696d 672e 6363 2f38  //i.postimg.cc/8
-00001780: 5058 4657 3973 6b2f 5758 3230 3234 3032  PXFW9sk/WX202402
-00001790: 3238 2d31 3233 3131 305f 3278 2e70 6e67  28-123110_2x.png
-000017a0: 2220 2077 6964 7468 3d22 3130 3025 2220  "  width="100%" 
-000017b0: 6865 6967 6874 3d22 3830 2522 3e0a 3c2f  height="80%">.</
-000017c0: 703e 0a0a 2323 2320 4465 7461 696c 6564  p>..### Detailed
-000017d0: 204c 6f67 6769 6e67 2055 7469 6c69 7465   Logging Utilite
-000017e0: 730a 0a57 6520 7072 6f76 6964 6520 6465  s..We provide de
-000017f0: 7461 696c 6564 206c 6f67 6769 6e67 2075  tailed logging u
-00001800: 7469 6c69 7469 6573 2074 6f20 6865 6c70  tilities to help
-00001810: 2079 6f75 2075 6e64 6572 7374 616e 6420   you understand 
-00001820: 7468 6520 6576 616c 7561 7469 6f6e 2070  the evaluation p
-00001830: 726f 6365 7373 2061 6e64 2072 6573 756c  rocess and resul
-00001840: 7473 2e20 5468 6520 6c6f 6773 2069 6e63  ts. The logs inc
-00001850: 6c75 6465 2074 6865 206d 6f64 656c 2061  lude the model a
-00001860: 7267 732c 2067 656e 6572 6174 696f 6e20  rgs, generation 
-00001870: 7061 7261 6d65 7465 7273 2c20 696e 7075  parameters, inpu
-00001880: 7420 7175 6573 7469 6f6e 2c20 6d6f 6465  t question, mode
-00001890: 6c20 7265 7370 6f6e 7365 2c20 616e 6420  l response, and 
-000018a0: 6772 6f75 6e64 2074 7275 7468 2061 6e73  ground truth ans
-000018b0: 7765 722e 2059 6f75 2063 616e 2061 6c73  wer. You can als
-000018c0: 6f20 7265 636f 7264 2065 7665 7279 2064  o record every d
-000018d0: 6574 6169 6c73 2061 6e64 2076 6973 7561  etails and visua
-000018e0: 6c69 7a65 2074 6865 6d20 696e 7369 6465  lize them inside
-000018f0: 2072 756e 7320 6f6e 2057 6569 6768 7473   runs on Weights
-00001900: 2026 2042 6961 7365 732e 0a0a 7b25 2069   & Biases...{% i
-00001910: 6e63 6c75 6465 2066 6967 7572 652e 6c69  nclude figure.li
-00001920: 7175 6964 206c 6f61 6469 6e67 3d22 6561  quid loading="ea
-00001930: 6765 7222 2070 6174 683d 2261 7373 6574  ger" path="asset
-00001940: 732f 696d 672f 7761 6e64 625f 7461 626c  s/img/wandb_tabl
-00001950: 652e 706e 6722 2063 6c61 7373 3d22 696d  e.png" class="im
-00001960: 672d 666c 7569 6420 726f 756e 6465 6420  g-fluid rounded 
-00001970: 7a2d 6465 7074 682d 3122 207a 6f6f 6d61  z-depth-1" zooma
-00001980: 626c 653d 7472 7565 2025 7d0a 0a3c 7020  ble=true %}..<p 
-00001990: 616c 6967 6e3d 2263 656e 7465 7222 2077  align="center" w
-000019a0: 6964 7468 3d22 3130 3025 223e 0a3c 696d  idth="100%">.<im
-000019b0: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
-000019c0: 2e70 6f73 7469 6d67 2e63 632f 5731 6331  .postimg.cc/W1c1
-000019d0: 7642 444a 2f57 6563 6861 742d 494d 4731  vBDJ/Wechat-IMG1
-000019e0: 3939 332e 706e 6722 2020 7769 6474 683d  993.png"  width=
-000019f0: 2231 3030 2522 2068 6569 6768 743d 2238  "100%" height="8
-00001a00: 3025 223e 0a3c 2f70 3e0a 0a23 2049 6e73  0%">.</p>..# Ins
-00001a10: 7461 6c6c 6174 696f 6e0a 0a46 6f72 2066  tallation..For f
-00001a20: 6f72 6d61 6c20 7573 6167 652c 2079 6f75  ormal usage, you
-00001a30: 2063 616e 2069 6e73 7461 6c6c 2074 6865   can install the
-00001a40: 2070 6163 6b61 6765 2066 726f 6d20 5079   package from Py
-00001a50: 5049 2062 7920 7275 6e6e 696e 6720 7468  PI by running th
-00001a60: 6520 666f 6c6c 6f77 696e 6720 636f 6d6d  e following comm
-00001a70: 616e 643a 0a60 6060 6261 7368 0a70 6970  and:.```bash.pip
-00001a80: 2069 6e73 7461 6c6c 206c 6d6d 732d 6576   install lmms-ev
-00001a90: 616c 0a60 6060 0a0a 466f 7220 6465 7665  al.```..For deve
-00001aa0: 6c6f 706d 656e 742c 2079 6f75 2063 616e  lopment, you can
-00001ab0: 2069 6e73 7461 6c6c 2074 6865 2070 6163   install the pac
-00001ac0: 6b61 6765 2062 7920 636c 6f6e 696e 6720  kage by cloning 
-00001ad0: 7468 6520 7265 706f 7369 746f 7279 2061  the repository a
-00001ae0: 6e64 2072 756e 6e69 6e67 2074 6865 2066  nd running the f
-00001af0: 6f6c 6c6f 7769 6e67 2063 6f6d 6d61 6e64  ollowing command
-00001b00: 3a0a 6060 6062 6173 680a 6769 7420 636c  :.```bash.git cl
-00001b10: 6f6e 6520 6874 7470 733a 2f2f 6769 7468  one https://gith
-00001b20: 7562 2e63 6f6d 2f45 766f 6c76 696e 674c  ub.com/EvolvingL
-00001b30: 4d4d 732d 4c61 622f 6c6d 6d73 2d65 7661  MMs-Lab/lmms-eva
-00001b40: 6c0a 6364 206c 6d6d 732d 6576 616c 0a70  l.cd lmms-eval.p
-00001b50: 6970 2069 6e73 7461 6c6c 202d 6520 2e0a  ip install -e ..
-00001b60: 6060 600a 0a49 6620 796f 7520 7761 6e74  ```..If you want
-00001b70: 6564 2074 6f20 7465 7374 206c 6c61 7661  ed to test llava
-00001b80: 2c20 796f 7520 7769 6c6c 2068 6176 6520  , you will have 
-00001b90: 746f 2063 6c6f 6e65 2074 6865 6972 2072  to clone their r
-00001ba0: 6570 6f20 6672 6f6d 205b 4c4c 6156 415d  epo from [LLaVA]
-00001bb0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00001bc0: 636f 6d2f 6861 6f74 6961 6e2d 6c69 752f  com/haotian-liu/
-00001bd0: 4c4c 6156 4129 2061 6e64 0a60 6060 0a67  LLaVA) and.```.g
-00001be0: 6974 2063 6c6f 6e65 2068 7474 7073 3a2f  it clone https:/
-00001bf0: 2f67 6974 6875 622e 636f 6d2f 6861 6f74  /github.com/haot
-00001c00: 6961 6e2d 6c69 752f 4c4c 6156 410a 6364  ian-liu/LLaVA.cd
-00001c10: 204c 4c61 5641 0a70 6970 2069 6e73 7461   LLaVA.pip insta
-00001c20: 6c6c 202d 6520 2e0a 6060 600a 0a59 6f75  ll -e ..```..You
-00001c30: 2063 616e 2063 6865 636b 2074 6865 205b   can check the [
-00001c40: 656e 7669 726f 6e6d 656e 7420 696e 7374  environment inst
-00001c50: 616c 6c20 7363 7269 7074 5d28 6d69 7363  all script](misc
-00001c60: 732f 7265 7072 5f73 6372 6970 7473 2e73  s/repr_scripts.s
-00001c70: 6829 2061 6e64 205b 746f 7263 6820 656e  h) and [torch en
-00001c80: 7669 726f 6e6d 656e 7420 696e 666f 5d28  vironment info](
-00001c90: 6d69 7363 732f 7265 7072 5f74 6f72 6368  miscs/repr_torch
-00001ca0: 5f65 6e76 732e 7478 7429 2074 6f20 2a2a  _envs.txt) to **
-00001cb0: 7265 7072 6f64 7563 6520 4c4c 6156 412d  reproduce LLaVA-
-00001cc0: 312e 3527 7320 7061 7065 7220 7265 7375  1.5's paper resu
-00001cd0: 6c74 732a 2a2e 2057 6520 666f 756e 6420  lts**. We found 
-00001ce0: 746f 7263 682f 6375 6461 2076 6572 7369  torch/cuda versi
-00001cf0: 6f6e 7320 6469 6666 6572 656e 6365 2077  ons difference w
-00001d00: 6f75 6c64 2063 6175 7365 2073 6d61 6c6c  ould cause small
-00001d10: 2076 6172 6961 7469 6f6e 7320 696e 2074   variations in t
-00001d20: 6865 2072 6573 756c 7473 2c20 7765 2070  he results, we p
-00001d30: 726f 7669 6465 2074 6865 205b 7265 7375  rovide the [resu
-00001d40: 6c74 7320 6368 6563 6b5d 286d 6973 6373  lts check](miscs
-00001d50: 2f6c 6c61 7661 5f72 6573 756c 745f 6368  /llava_result_ch
-00001d60: 6563 6b2e 6d64 2920 7769 7468 2064 6966  eck.md) with dif
-00001d70: 6665 7265 6e74 2065 6e76 6972 6f6e 6d65  ferent environme
-00001d80: 6e74 732e 0a0a 4966 2079 6f75 2077 616e  nts...If you wan
-00001d90: 7420 746f 2074 6573 7420 6f6e 2063 6170  t to test on cap
-00001da0: 7469 6f6e 2064 6174 6173 6574 2073 7563  tion dataset suc
-00001db0: 6820 6173 2060 636f 636f 602c 2060 7265  h as `coco`, `re
-00001dc0: 6663 6f63 6f60 2c20 616e 6420 606e 6f63  fcoco`, and `noc
-00001dd0: 6170 7360 2c20 796f 7520 7769 6c6c 206e  aps`, you will n
-00001de0: 6565 6420 746f 2068 6176 6520 606a 6176  eed to have `jav
-00001df0: 613d 3d31 2e38 2e30 2060 2074 6f20 6c65  a==1.8.0 ` to le
-00001e00: 7420 7079 636f 636f 6576 616c 2061 7069  t pycocoeval api
-00001e10: 2074 6f20 776f 726b 2e20 4966 2079 6f75   to work. If you
-00001e20: 2064 6f6e 2774 2068 6176 6520 6974 2c20   don't have it, 
-00001e30: 796f 7520 6361 6e20 696e 7374 616c 6c20  you can install 
-00001e40: 6279 2075 7369 6e67 2063 6f6e 6461 0a60  by using conda.`
-00001e50: 6060 0a63 6f6e 6461 2069 6e73 7461 6c6c  ``.conda install
-00001e60: 206f 7065 6e6a 646b 3d38 0a60 6060 0a79   openjdk=8.```.y
-00001e70: 6f75 2063 616e 2074 6865 6e20 6368 6563  ou can then chec
-00001e80: 6b20 796f 7572 206a 6176 6120 7665 7273  k your java vers
-00001e90: 696f 6e20 6279 2060 6a61 7661 202d 7665  ion by `java -ve
-00001ea0: 7273 696f 6e60 200a 0a23 2055 7361 6765  rsion` ..# Usage
-00001eb0: 0a60 6060 6261 7368 0a23 2045 7661 6c75  .```bash.# Evalu
-00001ec0: 6174 696e 6720 4c4c 6156 4120 6f6e 204d  ating LLaVA on M
-00001ed0: 4d45 0a61 6363 656c 6572 6174 6520 6c61  ME.accelerate la
-00001ee0: 756e 6368 202d 2d6e 756d 5f70 726f 6365  unch --num_proce
-00001ef0: 7373 6573 3d38 202d 6d20 6c6d 6d73 5f65  sses=8 -m lmms_e
-00001f00: 7661 6c20 2d2d 6d6f 6465 6c20 6c6c 6176  val --model llav
-00001f10: 6120 2020 2d2d 6d6f 6465 6c5f 6172 6773  a   --model_args
-00001f20: 2070 7265 7472 6169 6e65 643d 226c 6975   pretrained="liu
-00001f30: 6861 6f74 6961 6e2f 6c6c 6176 612d 7631  haotian/llava-v1
-00001f40: 2e35 2d37 6222 2020 202d 2d74 6173 6b73  .5-7b"   --tasks
-00001f50: 206d 6d65 2020 2d2d 6261 7463 685f 7369   mme  --batch_si
-00001f60: 7a65 2031 202d 2d6c 6f67 5f73 616d 706c  ze 1 --log_sampl
-00001f70: 6573 202d 2d6c 6f67 5f73 616d 706c 6573  es --log_samples
-00001f80: 5f73 7566 6669 7820 6c6c 6176 615f 7631  _suffix llava_v1
-00001f90: 2e35 5f6d 6d65 202d 2d6f 7574 7075 745f  .5_mme --output_
-00001fa0: 7061 7468 202e 2f6c 6f67 732f 200a 0a23  path ./logs/ ..#
-00001fb0: 2045 7661 6c75 6174 696e 6720 4c4c 6156   Evaluating LLaV
-00001fc0: 4120 6f6e 206d 756c 7469 706c 6520 6461  A on multiple da
-00001fd0: 7461 7365 7473 0a61 6363 656c 6572 6174  tasets.accelerat
-00001fe0: 6520 6c61 756e 6368 202d 2d6e 756d 5f70  e launch --num_p
-00001ff0: 726f 6365 7373 6573 3d38 202d 6d20 6c6d  rocesses=8 -m lm
-00002000: 6d73 5f65 7661 6c20 2d2d 6d6f 6465 6c20  ms_eval --model 
-00002010: 6c6c 6176 6120 2020 2d2d 6d6f 6465 6c5f  llava   --model_
-00002020: 6172 6773 2070 7265 7472 6169 6e65 643d  args pretrained=
-00002030: 226c 6975 6861 6f74 6961 6e2f 6c6c 6176  "liuhaotian/llav
-00002040: 612d 7631 2e35 2d37 6222 2020 202d 2d74  a-v1.5-7b"   --t
-00002050: 6173 6b73 206d 6d65 2c6d 6d62 656e 6368  asks mme,mmbench
-00002060: 5f65 6e20 2d2d 6261 7463 685f 7369 7a65  _en --batch_size
-00002070: 2031 202d 2d6c 6f67 5f73 616d 706c 6573   1 --log_samples
-00002080: 202d 2d6c 6f67 5f73 616d 706c 6573 5f73   --log_samples_s
-00002090: 7566 6669 7820 6c6c 6176 615f 7631 2e35  uffix llava_v1.5
-000020a0: 5f6d 6d65 5f6d 6d62 656e 6368 656e 202d  _mme_mmbenchen -
-000020b0: 2d6f 7574 7075 745f 7061 7468 202e 2f6c  -output_path ./l
-000020c0: 6f67 732f 2023 0a0a 2320 466f 7220 6f74  ogs/ #..# For ot
-000020d0: 6865 7220 7661 7269 616e 7473 206c 6c61  her variants lla
-000020e0: 7661 2e20 4e6f 7465 2074 6861 7420 6063  va. Note that `c
-000020f0: 6f6e 765f 7465 6d70 6c61 7465 6020 6973  onv_template` is
-00002100: 2061 6e20 6172 6720 6f66 2074 6865 2069   an arg of the i
-00002110: 6e69 7420 6675 6e63 7469 6f6e 206f 6620  nit function of 
-00002120: 6c6c 6176 6120 696e 2060 6c6d 6d73 5f65  llava in `lmms_e
-00002130: 7661 6c2f 6d6f 6465 6c73 2f6c 6c61 7661  val/models/llava
-00002140: 2e70 7960 0a61 6363 656c 6572 6174 6520  .py`.accelerate 
-00002150: 6c61 756e 6368 202d 2d6e 756d 5f70 726f  launch --num_pro
-00002160: 6365 7373 6573 3d38 202d 6d20 6c6d 6d73  cesses=8 -m lmms
-00002170: 5f65 7661 6c20 2d2d 6d6f 6465 6c20 6c6c  _eval --model ll
-00002180: 6176 6120 2020 2d2d 6d6f 6465 6c5f 6172  ava   --model_ar
-00002190: 6773 2070 7265 7472 6169 6e65 643d 226c  gs pretrained="l
-000021a0: 6975 6861 6f74 6961 6e2f 6c6c 6176 612d  iuhaotian/llava-
-000021b0: 7631 2e36 2d6d 6973 7472 616c 2d37 622c  v1.6-mistral-7b,
-000021c0: 636f 6e76 5f74 656d 706c 6174 653d 6d69  conv_template=mi
-000021d0: 7374 7261 6c5f 696e 7374 7275 6374 2220  stral_instruct" 
-000021e0: 2020 2d2d 7461 736b 7320 6d6d 652c 6d6d    --tasks mme,mm
-000021f0: 6265 6e63 685f 656e 202d 2d62 6174 6368  bench_en --batch
-00002200: 5f73 697a 6520 3120 2d2d 6c6f 675f 7361  _size 1 --log_sa
-00002210: 6d70 6c65 7320 2d2d 6c6f 675f 7361 6d70  mples --log_samp
-00002220: 6c65 735f 7375 6666 6978 206c 6c61 7661  les_suffix llava
-00002230: 5f76 312e 355f 6d6d 655f 6d6d 6265 6e63  _v1.5_mme_mmbenc
-00002240: 6865 6e20 2d2d 6f75 7470 7574 5f70 6174  hen --output_pat
-00002250: 6820 2e2f 6c6f 6773 2f20 230a 6163 6365  h ./logs/ #.acce
-00002260: 6c65 7261 7465 206c 6175 6e63 6820 2d2d  lerate launch --
-00002270: 6e75 6d5f 7072 6f63 6573 7365 733d 3820  num_processes=8 
-00002280: 2d6d 206c 6d6d 735f 6576 616c 202d 2d6d  -m lmms_eval --m
-00002290: 6f64 656c 206c 6c61 7661 2020 202d 2d6d  odel llava   --m
-000022a0: 6f64 656c 5f61 7267 7320 7072 6574 7261  odel_args pretra
-000022b0: 696e 6564 3d22 6c69 7568 616f 7469 616e  ined="liuhaotian
-000022c0: 2f6c 6c61 7661 2d76 312e 362d 3334 622c  /llava-v1.6-34b,
-000022d0: 636f 6e76 5f74 656d 706c 6174 653d 6d69  conv_template=mi
-000022e0: 7374 7261 6c5f 6469 7265 6374 2220 2020  stral_direct"   
-000022f0: 2d2d 7461 736b 7320 6d6d 652c 6d6d 6265  --tasks mme,mmbe
-00002300: 6e63 685f 656e 202d 2d62 6174 6368 5f73  nch_en --batch_s
-00002310: 697a 6520 3120 2d2d 6c6f 675f 7361 6d70  ize 1 --log_samp
-00002320: 6c65 7320 2d2d 6c6f 675f 7361 6d70 6c65  les --log_sample
-00002330: 735f 7375 6666 6978 206c 6c61 7661 5f76  s_suffix llava_v
-00002340: 312e 355f 6d6d 655f 6d6d 6265 6e63 6865  1.5_mme_mmbenche
-00002350: 6e20 2d2d 6f75 7470 7574 5f70 6174 6820  n --output_path 
-00002360: 2e2f 6c6f 6773 2f20 230a 0a23 2046 726f  ./logs/ #..# Fro
-00002370: 6d20 6120 7072 6564 6566 696e 6564 2063  m a predefined c
-00002380: 6f6e 6669 6775 7261 7469 6f6e 2c20 7375  onfiguration, su
-00002390: 7070 6f72 7469 6e67 2065 7661 6c75 6174  pporting evaluat
-000023a0: 696f 6e20 6f66 206d 756c 7469 706c 6520  ion of multiple 
-000023b0: 6d6f 6465 6c73 2061 6e64 2064 6174 6173  models and datas
-000023c0: 6574 730a 6163 6365 6c65 7261 7465 206c  ets.accelerate l
-000023d0: 6175 6e63 6820 2d2d 6e75 6d5f 7072 6f63  aunch --num_proc
-000023e0: 6573 7365 733d 3820 2d6d 206c 6d6d 735f  esses=8 -m lmms_
-000023f0: 6576 616c 202d 2d63 6f6e 6669 6720 6578  eval --config ex
-00002400: 616d 706c 655f 6576 616c 2e79 616d 6c20  ample_eval.yaml 
-00002410: 0a60 6060 0a0a 2320 4d6f 6465 6c20 5265  .```..# Model Re
-00002420: 7375 6c74 730a 0a41 7320 6465 6d6f 6e73  sults..As demons
-00002430: 7472 6174 6564 2062 7920 7468 6520 6578  trated by the ex
-00002440: 7465 6e73 6976 6520 7461 626c 6520 6265  tensive table be
-00002450: 6c6f 772c 2077 6520 6169 6d20 746f 2070  low, we aim to p
-00002460: 726f 7669 6465 2064 6574 6169 6c65 6420  rovide detailed 
-00002470: 696e 666f 726d 6174 696f 6e20 666f 7220  information for 
-00002480: 7265 6164 6572 7320 746f 2075 6e64 6572  readers to under
-00002490: 7374 616e 6420 7468 6520 6461 7461 7365  stand the datase
-000024a0: 7473 2069 6e63 6c75 6465 6420 696e 206c  ts included in l
-000024b0: 6d6d 732d 6576 616c 2061 6e64 2073 6f6d  mms-eval and som
-000024c0: 6520 7370 6563 6966 6963 2064 6574 6169  e specific detai
-000024d0: 6c73 2061 626f 7574 2074 6865 7365 2064  ls about these d
-000024e0: 6174 6173 6574 7320 2877 6520 7265 6d61  atasets (we rema
-000024f0: 696e 2067 7261 7465 6675 6c20 666f 7220  in grateful for 
-00002500: 616e 7920 636f 7272 6563 7469 6f6e 7320  any corrections 
-00002510: 7265 6164 6572 7320 6d61 7920 6861 7665  readers may have
-00002520: 2064 7572 696e 6720 6f75 7220 6576 616c   during our eval
-00002530: 7561 7469 6f6e 2070 726f 6365 7373 292e  uation process).
-00002540: 0a0a 5765 2070 726f 7669 6465 2061 2047  ..We provide a G
-00002550: 6f6f 676c 6520 5368 6565 7420 666f 7220  oogle Sheet for 
-00002560: 7468 6520 6465 7461 696c 6564 2072 6573  the detailed res
-00002570: 756c 7473 206f 6620 7468 6520 4c4c 6156  ults of the LLaV
-00002580: 4120 7365 7269 6573 206d 6f64 656c 7320  A series models 
-00002590: 6f6e 2064 6966 6665 7265 6e74 2064 6174  on different dat
-000025a0: 6173 6574 732e 2059 6f75 2063 616e 2061  asets. You can a
-000025b0: 6363 6573 7320 7468 6520 7368 6565 7420  ccess the sheet 
-000025c0: 5b68 6572 655d 2868 7474 7073 3a2f 2f64  [here](https://d
-000025d0: 6f63 732e 676f 6f67 6c65 2e63 6f6d 2f73  ocs.google.com/s
-000025e0: 7072 6561 6473 6865 6574 732f 642f 3161  preadsheets/d/1a
-000025f0: 3549 6d66 644b 4154 4449 3854 3743 7768  5ImfdKATDI8T7Cwh
-00002600: 3665 482d 6245 736e 5146 7a61 6e46 7261  6eH-bEsnQFzanFra
-00002610: 4655 6763 5339 4b48 5763 2f65 6469 743f  FUgcS9KHWc/edit?
-00002620: 7573 703d 7368 6172 696e 6729 2e20 4974  usp=sharing). It
-00002630: 2773 2061 206c 6976 6520 7368 6565 742c  's a live sheet,
-00002640: 2061 6e64 2077 6520 6172 6520 7570 6461   and we are upda
-00002650: 7469 6e67 2069 7420 7769 7468 206e 6577  ting it with new
-00002660: 2072 6573 756c 7473 2e0a 0a3c 7020 616c   results...<p al
-00002670: 6967 6e3d 2263 656e 7465 7222 2077 6964  ign="center" wid
-00002680: 7468 3d22 3130 3025 223e 0a3c 696d 6720  th="100%">.<img 
-00002690: 7372 633d 2268 7474 7073 3a2f 2f69 2e70  src="https://i.p
-000026a0: 6f73 7469 6d67 2e63 632f 6a64 7734 3937  ostimg.cc/jdw497
-000026b0: 4e53 2f57 5832 3032 3430 3330 372d 3136  NS/WX20240307-16
-000026c0: 3235 3236 2d32 782e 706e 6722 2020 7769  2526-2x.png"  wi
-000026d0: 6474 683d 2231 3030 2522 2068 6569 6768  dth="100%" heigh
-000026e0: 743d 2238 3025 223e 0a3c 2f70 3e0a 0a57  t="80%">.</p>..W
-000026f0: 6520 616c 736f 2070 726f 7669 6465 2074  e also provide t
-00002700: 6865 2072 6177 2064 6174 6120 6578 706f  he raw data expo
-00002710: 7274 6564 2066 726f 6d20 5765 6967 6874  rted from Weight
-00002720: 7320 2620 4269 6173 6573 2066 6f72 2074  s & Biases for t
-00002730: 6865 2064 6574 6169 6c65 6420 7265 7375  he detailed resu
-00002740: 6c74 7320 6f66 2074 6865 204c 4c61 5641  lts of the LLaVA
-00002750: 2073 6572 6965 7320 6d6f 6465 6c73 206f   series models o
-00002760: 6e20 6469 6666 6572 656e 7420 6461 7461  n different data
-00002770: 7365 7473 2e20 596f 7520 6361 6e20 6163  sets. You can ac
-00002780: 6365 7373 2074 6865 2072 6177 2064 6174  cess the raw dat
-00002790: 6120 5b68 6572 655d 2868 7474 7073 3a2f  a [here](https:/
-000027a0: 2f64 6f63 732e 676f 6f67 6c65 2e63 6f6d  /docs.google.com
-000027b0: 2f73 7072 6561 6473 6865 6574 732f 642f  /spreadsheets/d/
-000027c0: 3141 7661 456d 7547 3463 7353 6d58 6148  1AvaEmuG4csSmXaH
-000027d0: 6a67 7534 6569 314b 424d 6d4e 4e57 3877  jgu4ei1KBMmNNW8w
-000027e0: 666c 4f44 5f6b 6b54 4464 7638 2f65 6469  flOD_kkTDdv8/edi
-000027f0: 743f 7573 703d 7368 6172 696e 6729 2e0a  t?usp=sharing)..
-00002800: 0a3e 2044 6576 656c 6f70 6d65 6e74 2077  .> Development w
-00002810: 696c 6c20 6265 2063 6f6e 7469 6e75 696e  ill be continuin
-00002820: 6720 6f6e 2074 6865 206d 6169 6e20 6272  g on the main br
-00002830: 616e 6368 2c20 616e 6420 7765 2065 6e63  anch, and we enc
-00002840: 6f75 7261 6765 2079 6f75 2074 6f20 6769  ourage you to gi
-00002850: 7665 2075 7320 6665 6564 6261 636b 206f  ve us feedback o
-00002860: 6e20 7768 6174 2066 6561 7475 7265 7320  n what features 
-00002870: 6172 6520 6465 7369 7265 6420 616e 6420  are desired and 
-00002880: 686f 7720 746f 2069 6d70 726f 7665 2074  how to improve t
-00002890: 6865 206c 6962 7261 7279 2066 7572 7468  he library furth
-000028a0: 6572 2c20 6f72 2061 736b 2071 7565 7374  er, or ask quest
-000028b0: 696f 6e73 2c20 6569 7468 6572 2069 6e20  ions, either in 
-000028c0: 6973 7375 6573 206f 7220 5052 7320 6f6e  issues or PRs on
-000028d0: 2047 6974 4875 622e 0a0a 0a23 2320 5375   GitHub....## Su
-000028e0: 7070 6f72 7465 6420 6d6f 6465 6c73 0a0a  pported models..
-000028f0: 2d20 4750 5434 5620 2841 5049 2c20 6f6e  - GPT4V (API, on
-00002900: 6c79 2067 656e 6572 6174 696f 6e2d 6261  ly generation-ba
-00002910: 7365 6420 6576 616c 7561 7469 6f6e 290a  sed evaluation).
-00002920: 2d20 4c4c 6156 412d 7631 2e35 2f76 312e  - LLaVA-v1.5/v1.
-00002930: 362d 3742 2f31 3342 2f33 3442 2028 7070  6-7B/13B/34B (pp
-00002940: 6c2d 6261 7365 642c 2067 656e 6572 6174  l-based, generat
-00002950: 696f 6e2d 6261 7365 6429 0a2d 2051 7765  ion-based).- Qwe
-00002960: 6e2d 564c 2073 6572 6965 7320 2870 706c  n-VL series (ppl
-00002970: 2d62 6173 6564 2c20 6765 6e65 7261 7469  -based, generati
-00002980: 6f6e 2d62 6173 6564 290a 2d20 4675 7975  on-based).- Fuyu
-00002990: 2073 6572 6965 7320 2870 706c 2d62 6173   series (ppl-bas
-000029a0: 6564 2c20 6765 6e65 7261 7469 6f6e 2d62  ed, generation-b
-000029b0: 6173 6564 290a 2d20 496e 7374 7275 6374  ased).- Instruct
-000029c0: 424c 4950 2073 6572 6965 7320 2867 656e  BLIP series (gen
-000029d0: 6572 6174 696f 6e2d 6261 7365 6429 0a0a  eration-based)..
-000029e0: 2323 2053 7570 706f 7274 6564 2064 6174  ## Supported dat
-000029f0: 6173 6574 730a 3e20 2829 2069 6e64 6963  asets.> () indic
-00002a00: 6174 6573 2074 6865 2074 6173 6b20 6e61  ates the task na
-00002a10: 6d65 2069 6e20 7468 6520 6c6d 6d73 5f65  me in the lmms_e
-00002a20: 7661 6c2e 2054 6865 2074 6173 6b20 6e61  val. The task na
-00002a30: 6d65 2069 7320 616c 736f 2075 7365 6420  me is also used 
-00002a40: 746f 2073 7065 6369 6679 2074 6865 2064  to specify the d
-00002a50: 6174 6173 6574 2069 6e20 7468 6520 636f  ataset in the co
-00002a60: 6e66 6967 7572 6174 696f 6e20 6669 6c65  nfiguration file
-00002a70: 2e0a 0a2d 2041 4932 4420 2861 6932 6429  ...- AI2D (ai2d)
-00002a80: 0a2d 2043 6861 7274 5141 2028 6368 6172  .- ChartQA (char
-00002a90: 7471 6129 0a2d 2043 4d4d 4d55 2028 636d  tqa).- CMMMU (cm
-00002aa0: 6d6d 7529 0a20 202d 2043 4d4d 4d55 2056  mmu).  - CMMMU V
-00002ab0: 616c 6964 6174 696f 6e20 2863 6d6d 6d75  alidation (cmmmu
-00002ac0: 5f76 616c 290a 2020 2d20 434d 4d4d 5520  _val).  - CMMMU 
-00002ad0: 5465 7374 2028 636d 6d6d 755f 7465 7374  Test (cmmmu_test
-00002ae0: 290a 2d20 434f 434f 2043 6170 7469 6f6e  ).- COCO Caption
-00002af0: 2028 636f 636f 5f63 6170 290a 2020 2d20   (coco_cap).  - 
-00002b00: 434f 434f 2032 3031 3420 4361 7074 696f  COCO 2014 Captio
-00002b10: 6e20 2863 6f63 6f32 3031 345f 6361 7029  n (coco2014_cap)
-00002b20: 0a20 2020 202d 2043 4f43 4f20 3230 3134  .    - COCO 2014
-00002b30: 2043 6170 7469 6f6e 2056 616c 6964 6174   Caption Validat
-00002b40: 696f 6e20 2863 6f63 6f32 3031 345f 6361  ion (coco2014_ca
-00002b50: 705f 7661 6c29 0a20 2020 202d 2043 4f43  p_val).    - COC
-00002b60: 4f20 3230 3134 2043 6170 7469 6f6e 2054  O 2014 Caption T
-00002b70: 6573 7420 2863 6f63 6f32 3031 345f 6361  est (coco2014_ca
-00002b80: 705f 7465 7374 290a 2020 2d20 434f 434f  p_test).  - COCO
-00002b90: 2032 3031 3720 4361 7074 696f 6e20 2863   2017 Caption (c
-00002ba0: 6f63 6f32 3031 375f 6361 7029 0a20 2020  oco2017_cap).   
-00002bb0: 202d 2043 4f43 4f20 3230 3137 2043 6170   - COCO 2017 Cap
-00002bc0: 7469 6f6e 204d 696e 6956 616c 2028 636f  tion MiniVal (co
-00002bd0: 636f 3230 3137 5f63 6170 5f76 616c 290a  co2017_cap_val).
-00002be0: 2020 2020 2d20 434f 434f 2032 3031 3720      - COCO 2017 
-00002bf0: 4361 7074 696f 6e20 4d69 6e69 5465 7374  Caption MiniTest
-00002c00: 2028 636f 636f 3230 3137 5f63 6170 5f74   (coco2017_cap_t
-00002c10: 6573 7429 0a2d 2044 4f43 5651 4120 2864  est).- DOCVQA (d
-00002c20: 6f63 7671 6129 0a20 202d 2044 4f43 5651  ocvqa).  - DOCVQ
-00002c30: 4120 5661 6c69 6461 7469 6f6e 2028 646f  A Validation (do
-00002c40: 6376 7161 5f76 616c 290a 2020 2d20 444f  cvqa_val).  - DO
-00002c50: 4356 5141 2054 6573 7420 2864 6f63 7671  CVQA Test (docvq
-00002c60: 615f 7465 7374 290a 2d20 4665 7272 6574  a_test).- Ferret
-00002c70: 2028 6665 7272 6574 290a 2d20 466c 6963   (ferret).- Flic
-00002c80: 6b72 3330 4b20 2866 6c69 636b 7233 306b  kr30K (flickr30k
-00002c90: 290a 2020 2d20 4665 7272 6574 2054 6573  ).  - Ferret Tes
-00002ca0: 7420 2866 6572 7265 745f 7465 7374 290a  t (ferret_test).
-00002cb0: 2d20 4751 4120 2867 7161 290a 2d20 4861  - GQA (gqa).- Ha
-00002cc0: 6c6c 7573 696f 6e42 656e 6368 6d61 726b  llusionBenchmark
-00002cd0: 2028 6861 6c6c 7573 696f 6e5f 6265 6e63   (hallusion_benc
-00002ce0: 685f 696d 6167 6529 0a2d 2049 6e66 6f67  h_image).- Infog
-00002cf0: 7261 7068 6963 2056 5141 2028 696e 666f  raphic VQA (info
-00002d00: 5f76 7161 290a 2020 2d20 496e 666f 6772  _vqa).  - Infogr
-00002d10: 6170 6869 6320 5651 4120 5661 6c69 6461  aphic VQA Valida
-00002d20: 7469 6f6e 2028 696e 666f 5f76 7161 5f76  tion (info_vqa_v
-00002d30: 616c 290a 2020 2d20 496e 666f 6772 6170  al).  - Infograp
-00002d40: 6869 6320 5651 4120 5465 7374 2028 696e  hic VQA Test (in
-00002d50: 666f 5f76 7161 5f74 6573 7429 0a2d 204c  fo_vqa_test).- L
-00002d60: 4c61 5641 2d42 656e 6368 2028 6c6c 6176  LaVA-Bench (llav
-00002d70: 615f 696e 5f74 6865 5f77 696c 6429 0a2d  a_in_the_wild).-
-00002d80: 204c 4c61 5641 2d42 656e 6368 2d43 4f43   LLaVA-Bench-COC
-00002d90: 4f20 286c 6c61 7661 5f62 656e 6368 5f63  O (llava_bench_c
-00002da0: 6f63 6f29 0a2d 204d 6174 6856 6973 7461  oco).- MathVista
-00002db0: 2028 6d61 7468 7669 7374 6129 0a20 202d   (mathvista).  -
-00002dc0: 204d 6174 6856 6973 7461 2056 616c 6964   MathVista Valid
-00002dd0: 6174 696f 6e20 286d 6174 6876 6973 7461  ation (mathvista
-00002de0: 5f74 6573 746d 696e 6929 0a20 202d 204d  _testmini).  - M
-00002df0: 6174 6856 6973 7461 2054 6573 7420 286d  athVista Test (m
-00002e00: 6174 6876 6973 7461 5f74 6573 7429 0a2d  athvista_test).-
-00002e10: 204d 4d42 656e 6368 2028 6d6d 6265 6e63   MMBench (mmbenc
-00002e20: 6829 0a20 202d 204d 4d42 656e 6368 2045  h).  - MMBench E
-00002e30: 6e67 6c69 7368 2028 6d6d 6265 6e63 685f  nglish (mmbench_
-00002e40: 656e 290a 2020 2020 2d20 4d4d 4265 6e63  en).    - MMBenc
-00002e50: 6820 456e 676c 6973 6820 4465 7620 286d  h English Dev (m
-00002e60: 6d62 656e 6368 5f65 6e5f 6465 7629 0a20  mbench_en_dev). 
-00002e70: 2020 202d 204d 4d42 656e 6368 2045 6e67     - MMBench Eng
-00002e80: 6c69 7368 2054 6573 7420 286d 6d62 656e  lish Test (mmben
-00002e90: 6368 5f65 6e5f 7465 7374 290a 2020 2d20  ch_en_test).  - 
-00002ea0: 4d4d 4265 6e63 6820 4368 696e 6573 6520  MMBench Chinese 
-00002eb0: 286d 6d62 656e 6368 5f63 6e29 0a20 2020  (mmbench_cn).   
-00002ec0: 202d 204d 4d42 656e 6368 2043 6869 6e65   - MMBench Chine
-00002ed0: 7365 2044 6576 2028 6d6d 6265 6e63 685f  se Dev (mmbench_
-00002ee0: 636e 5f64 6576 290a 2020 2020 2d20 4d4d  cn_dev).    - MM
-00002ef0: 4265 6e63 6820 4368 696e 6573 6520 5465  Bench Chinese Te
-00002f00: 7374 2028 6d6d 6265 6e63 685f 636e 5f74  st (mmbench_cn_t
-00002f10: 6573 7429 0a2d 204d 4d45 2028 6d6d 6529  est).- MME (mme)
-00002f20: 0a2d 204d 4d4d 5520 286d 6d6d 7529 0a20  .- MMMU (mmmu). 
-00002f30: 202d 204d 4d4d 5520 5661 6c69 6461 7469   - MMMU Validati
-00002f40: 6f6e 2028 6d6d 6d75 5f76 616c 290a 2020  on (mmmu_val).  
-00002f50: 2d20 4d4d 4d55 2054 6573 7420 286d 6d6d  - MMMU Test (mmm
-00002f60: 755f 7465 7374 290a 2d20 4d4d 5665 7420  u_test).- MMVet 
-00002f70: 286d 6d76 6574 290a 2d20 4d75 6c74 692d  (mmvet).- Multi-
-00002f80: 446f 6356 5141 2028 6d75 6c74 6964 6f63  DocVQA (multidoc
-00002f90: 7671 6129 0a20 202d 204d 756c 7469 2d44  vqa).  - Multi-D
-00002fa0: 6f63 5651 4120 5661 6c69 6461 7469 6f6e  ocVQA Validation
-00002fb0: 2028 6d75 6c74 6964 6f63 7671 615f 7661   (multidocvqa_va
-00002fc0: 6c29 0a20 202d 204d 756c 7469 2d44 6f63  l).  - Multi-Doc
-00002fd0: 5651 4120 5465 7374 2028 6d75 6c74 6964  VQA Test (multid
-00002fe0: 6f63 7671 615f 7465 7374 290a 2d20 4e6f  ocvqa_test).- No
-00002ff0: 4361 7073 2028 6e6f 6361 7073 290a 2020  Caps (nocaps).  
-00003000: 2d20 4e6f 4361 7073 2056 616c 6964 6174  - NoCaps Validat
-00003010: 696f 6e20 286e 6f63 6170 735f 7661 6c29  ion (nocaps_val)
-00003020: 0a20 202d 204e 6f43 6170 7320 5465 7374  .  - NoCaps Test
-00003030: 2028 6e6f 6361 7073 5f74 6573 7429 0a2d   (nocaps_test).-
-00003040: 204f 4b56 5141 2028 6f6b 5f76 7161 290a   OKVQA (ok_vqa).
-00003050: 2020 2d20 4f4b 5651 4120 5661 6c69 6461    - OKVQA Valida
-00003060: 7469 6f6e 2032 3031 3420 286f 6b5f 7671  tion 2014 (ok_vq
-00003070: 615f 7661 6c32 3031 3429 0a2d 2050 4f50  a_val2014).- POP
-00003080: 4520 2870 6f70 6529 0a2d 2052 6566 434f  E (pope).- RefCO
-00003090: 434f 2028 7265 6663 6f63 6f29 0a20 2020  CO (refcoco).   
-000030a0: 202d 2072 6566 636f 636f 5f73 6567 5f74   - refcoco_seg_t
-000030b0: 6573 740a 2020 2020 2d20 7265 6663 6f63  est.    - refcoc
-000030c0: 6f5f 7365 675f 7661 6c0a 2020 2020 2d20  o_seg_val.    - 
-000030d0: 7265 6663 6f63 6f5f 7365 675f 7465 7374  refcoco_seg_test
-000030e0: 410a 2020 2020 2d20 7265 6663 6f63 6f5f  A.    - refcoco_
-000030f0: 7365 675f 7465 7374 420a 2020 2020 2d20  seg_testB.    - 
-00003100: 7265 6663 6f63 6f5f 6262 6f78 5f74 6573  refcoco_bbox_tes
-00003110: 740a 2020 2020 2d20 7265 6663 6f63 6f5f  t.    - refcoco_
-00003120: 6262 6f78 5f76 616c 0a20 2020 202d 2072  bbox_val.    - r
-00003130: 6566 636f 636f 5f62 626f 785f 7465 7374  efcoco_bbox_test
-00003140: 410a 2020 2020 2d20 7265 6663 6f63 6f5f  A.    - refcoco_
-00003150: 6262 6f78 5f74 6573 7442 0a2d 2052 6566  bbox_testB.- Ref
-00003160: 434f 434f 2b20 2872 6566 636f 636f 2b29  COCO+ (refcoco+)
-00003170: 0a20 2020 202d 2072 6566 636f 636f 2b5f  .    - refcoco+_
-00003180: 7365 670a 2020 2020 2020 2020 2d20 7265  seg.        - re
-00003190: 6663 6f63 6f2b 5f73 6567 5f76 616c 0a20  fcoco+_seg_val. 
-000031a0: 2020 2020 2020 202d 2072 6566 636f 636f         - refcoco
-000031b0: 2b5f 7365 675f 7465 7374 410a 2020 2020  +_seg_testA.    
-000031c0: 2020 2020 2d20 7265 6663 6f63 6f2b 5f73      - refcoco+_s
-000031d0: 6567 5f74 6573 7442 0a20 2020 202d 2072  eg_testB.    - r
-000031e0: 6566 636f 636f 2b5f 6262 6f78 0a20 2020  efcoco+_bbox.   
-000031f0: 2020 2020 202d 2072 6566 636f 636f 2b5f       - refcoco+_
-00003200: 6262 6f78 5f76 616c 0a20 2020 2020 2020  bbox_val.       
-00003210: 202d 2072 6566 636f 636f 2b5f 6262 6f78   - refcoco+_bbox
-00003220: 5f74 6573 7441 0a20 2020 2020 2020 202d  _testA.        -
-00003230: 2072 6566 636f 636f 2b5f 6262 6f78 5f74   refcoco+_bbox_t
-00003240: 6573 7442 0a2d 2052 6566 434f 434f 6720  estB.- RefCOCOg 
-00003250: 2872 6566 636f 636f 6729 0a20 2020 202d  (refcocog).    -
-00003260: 2072 6566 636f 636f 675f 7365 675f 7465   refcocog_seg_te
-00003270: 7374 0a20 2020 202d 2072 6566 636f 636f  st.    - refcoco
-00003280: 675f 7365 675f 7661 6c0a 2020 2020 2d20  g_seg_val.    - 
-00003290: 7265 6663 6f63 6f67 5f62 626f 785f 7465  refcocog_bbox_te
-000032a0: 7374 0a20 2020 202d 2072 6566 636f 636f  st.    - refcoco
-000032b0: 675f 6262 6f78 5f76 616c 0a2d 2053 6369  g_bbox_val.- Sci
-000032c0: 656e 6365 5141 2028 7363 6965 6e63 6571  enceQA (scienceq
-000032d0: 615f 6675 6c6c 290a 2020 2d20 5363 6965  a_full).  - Scie
-000032e0: 6e63 6551 4120 4675 6c6c 2028 7363 6965  nceQA Full (scie
-000032f0: 6e63 6571 6129 0a20 202d 2053 6369 656e  nceqa).  - Scien
-00003300: 6365 5141 2049 4d47 2028 7363 6965 6e63  ceQA IMG (scienc
-00003310: 6571 615f 696d 6729 0a2d 2053 6565 6442  eqa_img).- SeedB
-00003320: 656e 6368 2028 7365 6564 6265 6e63 6829  ench (seedbench)
-00003330: 0a2d 2053 6565 6442 656e 6368 2032 2028  .- SeedBench 2 (
-00003340: 7365 6564 6265 6e63 685f 3229 0a2d 2053  seedbench_2).- S
-00003350: 542d 5651 4120 2873 7476 7161 290a 2d20  T-VQA (stvqa).- 
-00003360: 5465 7874 4361 7073 2028 7465 7874 6361  TextCaps (textca
-00003370: 7073 290a 2020 2d20 5465 7874 4361 7073  ps).  - TextCaps
-00003380: 2056 616c 6964 6174 696f 6e20 2874 6578   Validation (tex
-00003390: 7463 6170 735f 7661 6c29 0a20 202d 2054  tcaps_val).  - T
-000033a0: 6578 7443 6170 7320 5465 7374 2028 7465  extCaps Test (te
-000033b0: 7874 6361 7073 5f74 6573 7429 0a2d 2054  xtcaps_test).- T
-000033c0: 6578 7456 5141 2028 7465 7874 7671 6129  extVQA (textvqa)
-000033d0: 0a20 202d 2054 6578 7456 5141 2056 616c  .  - TextVQA Val
-000033e0: 6964 6174 696f 6e20 2874 6578 7476 7161  idation (textvqa
-000033f0: 5f76 616c 290a 2020 2d20 5465 7874 5651  _val).  - TextVQ
-00003400: 4120 5465 7374 2028 7465 7874 7671 615f  A Test (textvqa_
-00003410: 7465 7374 290a 2d20 5669 7a57 697a 5651  test).- VizWizVQ
-00003420: 4120 2876 697a 7769 7a5f 7671 6129 0a20  A (vizwiz_vqa). 
-00003430: 202d 2056 697a 5769 7a56 5141 2056 616c   - VizWizVQA Val
-00003440: 6964 6174 696f 6e20 2876 697a 7769 7a5f  idation (vizwiz_
-00003450: 7671 615f 7661 6c29 0a20 202d 2056 697a  vqa_val).  - Viz
-00003460: 5769 7a56 5141 2054 6573 7420 2876 697a  WizVQA Test (viz
-00003470: 7769 7a5f 7671 615f 7465 7374 290a 2d20  wiz_vqa_test).- 
-00003480: 5651 4176 3220 2876 7161 7632 290a 2020  VQAv2 (vqav2).  
-00003490: 2d20 5651 4176 3220 5661 6c69 6461 7469  - VQAv2 Validati
-000034a0: 6f6e 2028 7671 6176 325f 7661 6c29 0a20  on (vqav2_val). 
-000034b0: 202d 2056 5141 7632 2054 6573 7420 2876   - VQAv2 Test (v
-000034c0: 7161 7632 5f74 6573 7429 0a0a 2323 2044  qav2_test)..## D
-000034d0: 6174 6173 6574 7320 746f 2062 6520 6164  atasets to be ad
-000034e0: 6465 6420 616e 6420 7465 7374 6564 0a2d  ded and tested.-
-000034f0: 2054 616c 6c79 5141 2028 7461 6c6c 7971   TallyQA (tallyq
-00003500: 6129 0a2d 2056 5352 2028 7673 7229 0a2d  a).- VSR (vsr).-
-00003510: 2057 696e 6f67 726f 756e 6420 2877 696e   Winoground (win
-00003520: 6f67 726f 756e 6429 0a2d 204e 4c56 5232  oground).- NLVR2
-00003530: 2028 6e6c 7672 3229 0a2d 2052 6176 656e   (nlvr2).- Raven
-00003540: 4951 2d54 6573 7420 2872 6176 656e 6971  IQ-Test (raveniq
-00003550: 290a 2d20 4963 6f6e 5141 2028 6963 6f6e  ).- IconQA (icon
-00003560: 7161 290a 2d20 5669 7374 4265 6e63 6820  qa).- VistBench 
-00003570: 2876 6973 7462 656e 6368 290a 0a23 2041  (vistbench)..# A
-00003580: 6464 2043 7573 746f 6d69 7a65 6420 4d6f  dd Customized Mo
-00003590: 6465 6c20 616e 6420 4461 7461 7365 740a  del and Dataset.
-000035a0: 0a50 6c65 6173 6520 7265 6665 7220 746f  .Please refer to
-000035b0: 206f 7572 205b 646f 6375 6d65 6e74 6174   our [documentat
-000035c0: 696f 6e5d 2864 6f63 732f 5245 4144 4d45  ion](docs/README
-000035d0: 2e6d 6429 2e0a 0a23 2041 636b 6e6f 776c  .md)...# Acknowl
-000035e0: 6564 6765 6d65 6e74 0a0a 6c6d 6d73 5f65  edgement..lmms_e
-000035f0: 7661 6c20 6973 2061 2066 6f72 6b20 6f66  val is a fork of
-00003600: 205b 6c6d 2d65 7661 6c2d 6861 726e 6573   [lm-eval-harnes
-00003610: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
-00003620: 622e 636f 6d2f 456c 6575 7468 6572 4149  b.com/EleutherAI
-00003630: 2f6c 6d2d 6576 616c 7561 7469 6f6e 2d68  /lm-evaluation-h
-00003640: 6172 6e65 7373 292e 2057 6520 7265 636f  arness). We reco
-00003650: 6d6d 656e 6420 796f 7520 746f 2072 6561  mmend you to rea
-00003660: 6420 7468 726f 7567 6820 7468 6520 5b64  d through the [d
-00003670: 6f63 7320 6f66 206c 6d2d 6576 616c 2d68  ocs of lm-eval-h
-00003680: 6172 6e65 7373 5d28 6874 7470 733a 2f2f  arness](https://
-00003690: 6769 7468 7562 2e63 6f6d 2f45 6c65 7574  github.com/Eleut
-000036a0: 6865 7241 492f 6c6d 2d65 7661 6c75 6174  herAI/lm-evaluat
-000036b0: 696f 6e2d 6861 726e 6573 732f 7472 6565  ion-harness/tree
-000036c0: 2f6d 6169 6e2f 646f 6373 2920 666f 7220  /main/docs) for 
-000036d0: 7265 6c65 7661 6e74 2069 6e66 6f72 6d61  relevant informa
-000036e0: 7469 6f6e 2e20 0a0a 4265 6c6f 7720 6172  tion. ..Below ar
-000036f0: 6520 7468 6520 6368 616e 6765 7320 7765  e the changes we
-00003700: 206d 6164 6520 746f 2074 6865 206f 7269   made to the ori
-00003710: 6769 6e61 6c20 4150 493a 0a2d 2042 7569  ginal API:.- Bui
-00003720: 6c64 2063 6f6e 7465 7874 206e 6f77 206f  ld context now o
-00003730: 6e6c 7920 7061 7373 2069 6e20 6964 7820  nly pass in idx 
-00003740: 616e 6420 7072 6f63 6573 7320 696d 6167  and process imag
-00003750: 6520 616e 6420 646f 6320 6475 7269 6e67  e and doc during
-00003760: 2074 6865 206d 6f64 656c 2072 6573 706f   the model respo
-00003770: 6e64 696e 6720 7068 6173 652e 2054 6869  nding phase. Thi
-00003780: 7320 6973 2064 7565 2074 6f20 7468 6520  s is due to the 
-00003790: 6661 6374 2074 6861 7420 6461 7461 7365  fact that datase
-000037a0: 7420 6e6f 7720 636f 6e74 6169 6e73 206c  t now contains l
-000037b0: 6f74 7320 6f66 2069 6d61 6765 7320 616e  ots of images an
-000037c0: 6420 7765 2063 616e 2774 2073 746f 7265  d we can't store
-000037d0: 2074 6865 6d20 696e 2074 6865 2064 6f63   them in the doc
-000037e0: 206c 696b 6520 7468 6520 6f72 6967 696e   like the origin
-000037f0: 616c 206c 6d2d 6576 616c 2d68 6172 6e65  al lm-eval-harne
-00003800: 7373 206f 7468 6572 2077 6973 6520 7468  ss other wise th
-00003810: 6520 6370 7520 6d65 6d6f 7279 2077 6f75  e cpu memory wou
-00003820: 6c64 2065 7870 6c6f 6465 2e0a 2d20 496e  ld explode..- In
-00003830: 7374 616e 6365 2e61 7267 7320 286c 6d6d  stance.args (lmm
-00003840: 735f 6576 616c 2f61 7069 2f69 6e73 7461  s_eval/api/insta
-00003850: 6e63 652e 7079 2920 6e6f 7720 636f 6e74  nce.py) now cont
-00003860: 6169 6e73 2061 206c 6973 7420 6f66 2069  ains a list of i
-00003870: 6d61 6765 7320 746f 2062 6520 696e 7075  mages to be inpu
-00003880: 7474 6564 2074 6f20 6c6d 6d73 2e0a 2d20  tted to lmms..- 
-00003890: 6c6d 2d65 7661 6c2d 6861 726e 6573 7320  lm-eval-harness 
-000038a0: 7375 7070 6f72 7473 2061 6c6c 2048 4620  supports all HF 
-000038b0: 6c61 6e67 7561 6765 206d 6f64 656c 7320  language models 
-000038c0: 6173 2073 696e 676c 6520 6d6f 6465 6c20  as single model 
-000038d0: 636c 6173 732e 2043 7572 7265 6e74 6c79  class. Currently
-000038e0: 2074 6869 7320 6973 206e 6f74 2070 6f73   this is not pos
-000038f0: 7369 626c 6520 6f66 206c 6d6d 7320 6265  sible of lmms be
-00003900: 6361 7573 6520 7468 6520 696e 7075 742f  cause the input/
-00003910: 6f75 7470 7574 2066 6f72 6d61 7420 6f66  output format of
-00003920: 206c 6d6d 7320 696e 2048 4620 6172 6520   lmms in HF are 
-00003930: 6e6f 7420 7965 7420 756e 6966 6965 642e  not yet unified.
-00003940: 2054 6865 7265 7266 6f72 652c 2077 6520   Thererfore, we 
-00003950: 6861 7665 2074 6f20 6372 6561 7465 2061  have to create a
-00003960: 206e 6577 2063 6c61 7373 2066 6f72 2065   new class for e
-00003970: 6163 6820 6c6d 6d73 206d 6f64 656c 2e20  ach lmms model. 
-00003980: 5468 6973 2069 7320 6e6f 7420 6964 6561  This is not idea
-00003990: 6c20 616e 6420 7765 2077 696c 6c20 7472  l and we will tr
-000039a0: 7920 746f 2075 6e69 6679 2074 6865 6d20  y to unify them 
-000039b0: 696e 2074 6865 2066 7574 7572 652e 0a0a  in the future...
-000039c0: 5765 2061 6c73 6f20 7468 616e 6b3a 0a2d  We also thank:.-
-000039d0: 205b 5869 616e 6720 5975 655d 2868 7474   [Xiang Yue](htt
-000039e0: 7073 3a2f 2f78 6961 6e67 7975 6539 3630  ps://xiangyue960
-000039f0: 372e 6769 7468 7562 2e69 6f2f 292c 205b  7.github.io/), [
-00003a00: 4a69 6e67 6b61 6e67 2059 616e 675d 2868  Jingkang Yang](h
-00003a10: 7474 7073 3a2f 2f6a 696e 676b 616e 6735  ttps://jingkang5
-00003a20: 302e 6769 7468 7562 2e69 6f2f 292c 205b  0.github.io/), [
-00003a30: 446f 6e67 2047 756f 5d28 6874 7470 733a  Dong Guo](https:
-00003a40: 2f2f 7777 772e 6c69 6e6b 6564 696e 2e63  //www.linkedin.c
-00003a50: 6f6d 2f69 6e2f 646f 6e67 6775 6f73 6574  om/in/dongguoset
-00003a60: 2f29 2061 6e64 205b 5368 656e 6720 5368  /) and [Sheng Sh
-00003a70: 656e 5d28 6874 7470 733a 2f2f 7369 6e63  en](https://sinc
-00003a80: 6572 6173 732e 6769 7468 7562 2e69 6f2f  erass.github.io/
-00003a90: 2920 666f 7220 6561 726c 7920 6469 7363  ) for early disc
-00003aa0: 7573 7369 6f6e 2061 6e64 2074 6573 7469  ussion and testi
-00003ab0: 6e67 2e0a 0a23 2320 4369 7461 7469 6f6e  ng...## Citation
-00003ac0: 730a 0a60 6060 7368 656c 6c0a 406d 6973  s..```shell.@mis
-00003ad0: 637b 6c6d 6d73 5f65 7661 6c32 3032 342c  c{lmms_eval2024,
-00003ae0: 0a20 2020 2074 6974 6c65 3d7b 4c4d 4d73  .    title={LMMs
-00003af0: 2d45 7661 6c3a 2041 6363 656c 6572 6174  -Eval: Accelerat
-00003b00: 696e 6720 7468 6520 4465 7665 6c6f 706d  ing the Developm
-00003b10: 656e 7420 6f66 204c 6172 6765 204d 756c  ent of Large Mul
-00003b20: 7469 6d6f 616c 204d 6f64 656c 737d 2c0a  timoal Models},.
-00003b30: 2020 2020 7572 6c3d 7b68 7474 7073 3a2f      url={https:/
-00003b40: 2f67 6974 6875 622e 636f 6d2f 4576 6f6c  /github.com/Evol
-00003b50: 7669 6e67 4c4d 4d73 2d4c 6162 2f6c 6d6d  vingLMMs-Lab/lmm
-00003b60: 732d 6576 616c 7d2c 0a20 2020 2061 7574  s-eval},.    aut
-00003b70: 686f 723d 7b42 6f20 4c69 2a2c 2050 6569  hor={Bo Li*, Pei
-00003b80: 7975 616e 205a 6861 6e67 2a2c 204b 6169  yuan Zhang*, Kai
-00003b90: 6368 656e 205a 6861 6e67 2a2c 2046 616e  chen Zhang*, Fan
-00003ba0: 7969 2050 752a 2c20 5869 6e72 756e 2044  yi Pu*, Xinrun D
-00003bb0: 752c 2059 7568 616f 2044 6f6e 672c 2048  u, Yuhao Dong, H
-00003bc0: 616f 7469 616e 204c 6975 2c20 5975 616e  aotian Liu, Yuan
-00003bd0: 6861 6e20 5a68 616e 672c 2047 6520 5a68  han Zhang, Ge Zh
-00003be0: 616e 672c 2043 6875 6e79 7561 6e20 4c69  ang, Chunyuan Li
-00003bf0: 2061 6e64 205a 6977 6569 204c 6975 7d2c   and Ziwei Liu},
-00003c00: 0a20 2020 2070 7562 6c69 7368 6572 2020  .    publisher  
-00003c10: 2020 3d20 7b5a 656e 6f64 6f7d 2c0a 2020    = {Zenodo},.  
-00003c20: 2020 7665 7273 696f 6e20 2020 2020 203d    version      =
-00003c30: 207b 7630 2e31 2e30 7d2c 0a20 2020 206d   {v0.1.0},.    m
-00003c40: 6f6e 7468 3d7b 4d61 7263 687d 2c0a 2020  onth={March},.  
-00003c50: 2020 7965 6172 3d7b 3230 3234 7d0a 7d0a    year={2024}.}.
-00003c60: 6060 600a                                ```.
+000001e0: 732d 6c61 6229 207c 203c 6120 6872 6566  s-lab) | <a href
+000001f0: 3d22 6874 7470 733a 2f2f 656d 6f6a 692e  ="https://emoji.
+00000200: 6767 2f65 6d6f 6a69 2f31 3638 342d 6469  gg/emoji/1684-di
+00000210: 7363 6f72 642d 7468 7265 6164 223e 3c69  scord-thread"><i
+00000220: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00000230: 6364 6e33 2e65 6d6f 6a69 2e67 672f 656d  cdn3.emoji.gg/em
+00000240: 6f6a 6973 2f31 3638 342d 6469 7363 6f72  ojis/1684-discor
+00000250: 642d 7468 7265 6164 2e70 6e67 2220 7769  d-thread.png" wi
+00000260: 6474 683d 2231 3470 7822 2068 6569 6768  dth="14px" heigh
+00000270: 743d 2231 3470 7822 2061 6c74 3d22 4469  t="14px" alt="Di
+00000280: 7363 6f72 645f 5468 7265 6164 223e 3c2f  scord_Thread"></
+00000290: 613e 205b 6469 7363 6f72 642f 6c6d 6d73  a> [discord/lmms
+000002a0: 2d65 7661 6c5d 2868 7474 7073 3a2f 2f64  -eval](https://d
+000002b0: 6973 636f 7264 2e67 672f 7a64 6b77 4b55  iscord.gg/zdkwKU
+000002c0: 7172 5079 290a 0a0a 496e 2074 6f64 6179  qrPy)...In today
+000002d0: 2773 2077 6f72 6c64 2c20 7765 2772 6520  's world, we're 
+000002e0: 6f6e 2061 6e20 6578 6369 7469 6e67 206a  on an exciting j
+000002f0: 6f75 726e 6579 2074 6f77 6172 6420 6372  ourney toward cr
+00000300: 6561 7469 6e67 2041 7274 6966 6963 6961  eating Artificia
+00000310: 6c20 4765 6e65 7261 6c20 496e 7465 6c6c  l General Intell
+00000320: 6967 656e 6365 2028 4147 4929 2c20 6d75  igence (AGI), mu
+00000330: 6368 206c 696b 6520 7468 6520 656e 7468  ch like the enth
+00000340: 7573 6961 736d 206f 6620 7468 6520 3139  usiasm of the 19
+00000350: 3630 7320 6d6f 6f6e 206c 616e 6469 6e67  60s moon landing
+00000360: 2e20 5468 6973 206a 6f75 726e 6579 2069  . This journey i
+00000370: 7320 706f 7765 7265 6420 6279 2061 6476  s powered by adv
+00000380: 616e 6365 6420 6c61 7267 6520 6c61 6e67  anced large lang
+00000390: 7561 6765 206d 6f64 656c 7320 284c 4c4d  uage models (LLM
+000003a0: 7329 2061 6e64 206c 6172 6765 206d 756c  s) and large mul
+000003b0: 7469 6d6f 6461 6c20 6d6f 6465 6c73 2028  timodal models (
+000003c0: 4c4d 4d73 292c 2077 6869 6368 2061 7265  LMMs), which are
+000003d0: 2063 6f6d 706c 6578 2073 7973 7465 6d73   complex systems
+000003e0: 2063 6170 6162 6c65 206f 6620 756e 6465   capable of unde
+000003f0: 7273 7461 6e64 696e 672c 206c 6561 726e  rstanding, learn
+00000400: 696e 672c 2061 6e64 2070 6572 666f 726d  ing, and perform
+00000410: 696e 6720 6120 7769 6465 2076 6172 6965  ing a wide varie
+00000420: 7479 206f 6620 6875 6d61 6e20 7461 736b  ty of human task
+00000430: 732e 2054 6865 7365 2061 6476 616e 6365  s. These advance
+00000440: 6d65 6e74 7320 6272 696e 6720 7573 2063  ments bring us c
+00000450: 6c6f 7365 7220 746f 2061 6368 6965 7669  loser to achievi
+00000460: 6e67 2041 4749 2e0a 0a54 6f20 6761 7567  ng AGI...To gaug
+00000470: 6520 686f 7720 6164 7661 6e63 6564 2074  e how advanced t
+00000480: 6865 7365 206d 6f64 656c 7320 6172 652c  hese models are,
+00000490: 2077 6520 7573 6520 6120 7661 7269 6574   we use a variet
+000004a0: 7920 6f66 2065 7661 6c75 6174 696f 6e20  y of evaluation 
+000004b0: 6265 6e63 686d 6172 6b73 2e20 5468 6573  benchmarks. Thes
+000004c0: 6520 6265 6e63 686d 6172 6b73 2061 7265  e benchmarks are
+000004d0: 2074 6f6f 6c73 2074 6861 7420 6865 6c70   tools that help
+000004e0: 2075 7320 756e 6465 7273 7461 6e64 2074   us understand t
+000004f0: 6865 2063 6170 6162 696c 6974 6965 7320  he capabilities 
+00000500: 6f66 2074 6865 7365 206d 6f64 656c 732c  of these models,
+00000510: 2073 686f 7769 6e67 2075 7320 686f 7720   showing us how 
+00000520: 636c 6f73 6520 7765 2061 7265 2074 6f20  close we are to 
+00000530: 6163 6869 6576 696e 6720 4147 492e 2048  achieving AGI. H
+00000540: 6f77 6576 6572 2c20 6669 6e64 696e 6720  owever, finding 
+00000550: 616e 6420 7573 696e 6720 7468 6573 6520  and using these 
+00000560: 6265 6e63 686d 6172 6b73 2069 7320 6120  benchmarks is a 
+00000570: 6269 6720 6368 616c 6c65 6e67 652e 2054  big challenge. T
+00000580: 6865 206e 6563 6573 7361 7279 2062 656e  he necessary ben
+00000590: 6368 6d61 726b 7320 616e 6420 6461 7461  chmarks and data
+000005a0: 7365 7473 2061 7265 2073 7072 6561 6420  sets are spread 
+000005b0: 6f75 7420 616e 6420 6869 6464 656e 2069  out and hidden i
+000005c0: 6e20 7661 7269 6f75 7320 706c 6163 6573  n various places
+000005d0: 206c 696b 6520 476f 6f67 6c65 2044 7269   like Google Dri
+000005e0: 7665 2c20 4472 6f70 626f 782c 2061 6e64  ve, Dropbox, and
+000005f0: 2064 6966 6665 7265 6e74 2073 6368 6f6f   different schoo
+00000600: 6c20 616e 6420 7265 7365 6172 6368 206c  l and research l
+00000610: 6162 2077 6562 7369 7465 732e 2049 7420  ab websites. It 
+00000620: 6665 656c 7320 6c69 6b65 2077 6527 7265  feels like we're
+00000630: 206f 6e20 6120 7472 6561 7375 7265 2068   on a treasure h
+00000640: 756e 742c 2062 7574 2074 6865 206d 6170  unt, but the map
+00000650: 7320 6172 6520 7363 6174 7465 7265 6420  s are scattered 
+00000660: 6576 6572 7977 6865 7265 2e0a 0a49 6e20  everywhere...In 
+00000670: 7468 6520 6669 656c 6420 6f66 206c 616e  the field of lan
+00000680: 6775 6167 6520 6d6f 6465 6c73 2c20 7468  guage models, th
+00000690: 6572 6520 6861 7320 6265 656e 2061 2076  ere has been a v
+000006a0: 616c 7561 626c 6520 7072 6563 6564 656e  aluable preceden
+000006b0: 7420 7365 7420 6279 2074 6865 2077 6f72  t set by the wor
+000006c0: 6b20 6f66 205b 6c6d 2d65 7661 6c75 6174  k of [lm-evaluat
+000006d0: 696f 6e2d 6861 726e 6573 735d 2868 7474  ion-harness](htt
+000006e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000006f0: 456c 6575 7468 6572 4149 2f6c 6d2d 6576  EleutherAI/lm-ev
+00000700: 616c 7561 7469 6f6e 2d68 6172 6e65 7373  aluation-harness
+00000710: 292e 2054 6865 7920 6f66 6665 7220 696e  ). They offer in
+00000720: 7465 6772 6174 6564 2064 6174 6120 616e  tegrated data an
+00000730: 6420 6d6f 6465 6c20 696e 7465 7266 6163  d model interfac
+00000740: 6573 2c20 656e 6162 6c69 6e67 2072 6170  es, enabling rap
+00000750: 6964 2065 7661 6c75 6174 696f 6e20 6f66  id evaluation of
+00000760: 206c 616e 6775 6167 6520 6d6f 6465 6c73   language models
+00000770: 2061 6e64 2073 6572 7669 6e67 2061 7320   and serving as 
+00000780: 7468 6520 6261 636b 656e 6420 7375 7070  the backend supp
+00000790: 6f72 7420 6672 616d 6577 6f72 6b20 666f  ort framework fo
+000007a0: 7220 7468 6520 5b6f 7065 6e2d 6c6c 6d2d  r the [open-llm-
+000007b0: 6c65 6164 6572 626f 6172 645d 2868 7474  leaderboard](htt
+000007c0: 7073 3a2f 2f68 7567 6769 6e67 6661 6365  ps://huggingface
+000007d0: 2e63 6f2f 7370 6163 6573 2f48 7567 6769  .co/spaces/Huggi
+000007e0: 6e67 4661 6365 4834 2f6f 7065 6e5f 6c6c  ngFaceH4/open_ll
+000007f0: 6d5f 6c65 6164 6572 626f 6172 6429 2c20  m_leaderboard), 
+00000800: 616e 6420 6861 7320 6772 6164 7561 6c6c  and has graduall
+00000810: 7920 6265 636f 6d65 2074 6865 2075 6e64  y become the und
+00000820: 6572 6c79 696e 6720 6563 6f73 7973 7465  erlying ecosyste
+00000830: 6d20 6f66 2074 6865 2065 7261 206f 6620  m of the era of 
+00000840: 666f 756e 6461 7469 6f6e 206d 6f64 656c  foundation model
+00000850: 732e 0a0a 486f 7765 7665 722c 2074 686f  s...However, tho
+00000860: 7567 6820 7468 6572 6520 6172 6520 6d61  ugh there are ma
+00000870: 6e79 206e 6577 2065 7661 6c75 6174 696f  ny new evaluatio
+00000880: 6e20 6461 7461 7365 7473 2061 7265 2072  n datasets are r
+00000890: 6563 656e 746c 7920 7072 6f70 6f73 6564  ecently proposed
+000008a0: 2c20 7468 6520 6566 6669 6369 656e 7420  , the efficient 
+000008b0: 6576 616c 7561 7469 6f6e 2070 6970 656c  evaluation pipel
+000008c0: 696e 6520 6f66 204c 4d4d 2069 7320 7374  ine of LMM is st
+000008d0: 696c 6c20 696e 2069 7473 2069 6e66 616e  ill in its infan
+000008e0: 6379 2c20 616e 6420 7468 6572 6520 6973  cy, and there is
+000008f0: 206e 6f20 756e 6966 6965 6420 6576 616c   no unified eval
+00000900: 7561 7469 6f6e 2066 7261 6d65 776f 726b  uation framework
+00000910: 2074 6861 7420 6361 6e20 6265 2075 7365   that can be use
+00000920: 6420 746f 2065 7661 6c75 6174 6520 4c4d  d to evaluate LM
+00000930: 4d20 6163 726f 7373 2061 2077 6964 6520  M across a wide 
+00000940: 7261 6e67 6520 6f66 2064 6174 6173 6574  range of dataset
+00000950: 732e 2054 6f20 6164 6472 6573 7320 7468  s. To address th
+00000960: 6973 2063 6861 6c6c 656e 6765 2c20 7765  is challenge, we
+00000970: 2069 6e74 726f 6475 6365 202a 2a6c 6d6d   introduce **lmm
+00000980: 732d 6576 616c 2a2a 2c20 616e 2065 7661  s-eval**, an eva
+00000990: 6c75 6174 696f 6e20 6672 616d 6577 6f72  luation framewor
+000009a0: 6b20 6d65 7469 6375 6c6f 7573 6c79 2063  k meticulously c
+000009b0: 7261 6674 6564 2066 6f72 2063 6f6e 7369  rafted for consi
+000009c0: 7374 656e 7420 616e 6420 6566 6669 6369  stent and effici
+000009d0: 656e 7420 6576 616c 7561 7469 6f6e 206f  ent evaluation o
+000009e0: 6620 4c4d 4d2e 0a0a 5765 2068 756d 626c  f LMM...We humbl
+000009f0: 7920 6f62 736f 7262 6564 2074 6865 2065  y obsorbed the e
+00000a00: 7871 7569 7369 7465 2061 6e64 2065 6666  xquisite and eff
+00000a10: 6963 6965 6e74 2064 6573 6967 6e20 6f66  icient design of
+00000a20: 205b 6c6d 2d65 7661 6c75 6174 696f 6e2d   [lm-evaluation-
+00000a30: 6861 726e 6573 735d 2868 7474 7073 3a2f  harness](https:/
+00000a40: 2f67 6974 6875 622e 636f 6d2f 456c 6575  /github.com/Eleu
+00000a50: 7468 6572 4149 2f6c 6d2d 6576 616c 7561  therAI/lm-evalua
+00000a60: 7469 6f6e 2d68 6172 6e65 7373 292e 2042  tion-harness). B
+00000a70: 7569 6c64 696e 6720 7570 6f6e 2069 7473  uilding upon its
+00000a80: 2066 6f75 6e64 6174 696f 6e2c 2077 6520   foundation, we 
+00000a90: 696d 706c 656d 656e 7465 6420 6f75 7220  implemented our 
+00000aa0: 606c 6d6d 732d 6576 616c 6020 6672 616d  `lmms-eval` fram
+00000ab0: 6577 6f72 6b20 7769 7468 2070 6572 666f  ework with perfo
+00000ac0: 726d 616e 6365 206f 7074 696d 697a 6174  rmance optimizat
+00000ad0: 696f 6e73 2073 7065 6369 6669 6361 6c6c  ions specificall
+00000ae0: 7920 666f 7220 4c4d 4d73 2e0a 0a23 2320  y for LMMs...## 
+00000af0: 4e65 6365 7373 6974 7920 6f66 206c 6d6d  Necessity of lmm
+00000b00: 732d 6576 616c 0a0a 5765 2062 656c 6965  s-eval..We belie
+00000b10: 7665 206f 7572 2065 6666 6f72 7420 636f  ve our effort co
+00000b20: 756c 6420 7072 6f76 6964 6520 616e 2065  uld provide an e
+00000b30: 6666 6963 6965 6e74 2069 6e74 6572 6661  fficient interfa
+00000b40: 6365 2066 6f72 2074 6865 2064 6574 6169  ce for the detai
+00000b50: 6c65 6420 636f 6d70 6172 6973 6f6e 206f  led comparison o
+00000b60: 6620 7075 626c 6963 6c79 2061 7661 696c  f publicly avail
+00000b70: 6162 6c65 206d 6f64 656c 7320 746f 2064  able models to d
+00000b80: 6973 6365 726e 2074 6865 6972 2073 7472  iscern their str
+00000b90: 656e 6774 6873 2061 6e64 2077 6561 6b6e  engths and weakn
+00000ba0: 6573 7365 732e 2049 7427 7320 616c 736f  esses. It's also
+00000bb0: 2075 7365 6675 6c20 666f 7220 7265 7365   useful for rese
+00000bc0: 6172 6368 2069 6e73 7469 7475 7469 6f6e  arch institution
+00000bd0: 7320 616e 6420 7072 6f64 7563 7469 6f6e  s and production
+00000be0: 2d6f 7269 656e 7465 6420 636f 6d70 616e  -oriented compan
+00000bf0: 6965 7320 746f 2061 6363 656c 6572 6174  ies to accelerat
+00000c00: 6520 7468 6520 6465 7665 6c6f 706d 656e  e the developmen
+00000c10: 7420 6f66 206c 6172 6765 206d 756c 7469  t of large multi
+00000c20: 6d6f 6461 6c20 6d6f 6465 6c73 2e20 5769  modal models. Wi
+00000c30: 7468 2074 6865 2060 6c6d 6d73 2d65 7661  th the `lmms-eva
+00000c40: 6c60 2c20 7765 2068 6176 6520 7369 676e  l`, we have sign
+00000c50: 6966 6963 616e 746c 7920 6163 6365 6c65  ificantly accele
+00000c60: 7261 7465 6420 7468 6520 6c69 6665 6379  rated the lifecy
+00000c70: 636c 6520 6f66 206d 6f64 656c 2069 7465  cle of model ite
+00000c80: 7261 7469 6f6e 2e20 496e 7369 6465 2074  ration. Inside t
+00000c90: 6865 204c 4c61 5641 2074 6561 6d2c 2074  he LLaVA team, t
+00000ca0: 6865 2075 7469 6c69 7a61 7469 6f6e 206f  he utilization o
+00000cb0: 6620 606c 6d6d 732d 6576 616c 6020 6c61  f `lmms-eval` la
+00000cc0: 7267 656c 7920 696d 7072 6f76 6573 2074  rgely improves t
+00000cd0: 6865 2065 6666 6963 6965 6e63 7920 6f66  he efficiency of
+00000ce0: 2074 6865 206d 6f64 656c 2064 6576 656c   the model devel
+00000cf0: 6f70 6d65 6e74 2063 7963 6c65 2c20 6173  opment cycle, as
+00000d00: 2077 6520 6172 6520 6162 6c65 2074 6f20   we are able to 
+00000d10: 6576 616c 7561 7465 2077 6565 6b6c 7920  evaluate weekly 
+00000d20: 7472 6169 6e65 6420 6875 6e64 7265 6473  trained hundreds
+00000d30: 206f 6620 6368 6563 6b70 6f69 6e74 7320   of checkpoints 
+00000d40: 6f6e 2032 302d 3330 2064 6174 6173 6574  on 20-30 dataset
+00000d50: 732c 2069 6465 6e74 6966 7969 6e67 2074  s, identifying t
+00000d60: 6865 2073 7472 656e 6774 6873 2061 6e64  he strengths and
+00000d70: 2077 6561 6b6e 6573 7365 732c 2061 6e64   weaknesses, and
+00000d80: 2074 6865 6e20 6d61 6b65 2074 6172 6765   then make targe
+00000d90: 7465 6420 696d 7072 6f76 656d 656e 7473  ted improvements
+00000da0: 2e0a 0a23 2041 6e6e 6f75 6365 6d65 6e74  ...# Annoucement
+00000db0: 0a0a 2323 2043 6f6e 7472 6962 7574 696f  ..## Contributio
+00000dc0: 6e20 4775 6964 616e 6365 0a0a 5765 2776  n Guidance..We'v
+00000dd0: 6520 6164 6465 6420 6775 6964 616e 6365  e added guidance
+00000de0: 206f 6e20 636f 6e74 7269 6275 7469 6e67   on contributing
+00000df0: 206e 6577 2064 6174 6173 6574 7320 616e   new datasets an
+00000e00: 6420 6d6f 6465 6c73 2e20 506c 6561 7365  d models. Please
+00000e10: 2072 6566 6572 2074 6f20 6f75 7220 5b64   refer to our [d
+00000e20: 6f63 756d 656e 7461 7469 6f6e 5d28 646f  ocumentation](do
+00000e30: 6373 2f52 4541 444d 452e 6d64 292e 2049  cs/README.md). I
+00000e40: 6620 796f 7520 6e65 6564 2061 7373 6973  f you need assis
+00000e50: 7461 6e63 652c 2079 6f75 2063 616e 2063  tance, you can c
+00000e60: 6f6e 7461 6374 2075 7320 7669 6120 5b64  ontact us via [d
+00000e70: 6973 636f 7264 2f6c 6d6d 732d 6576 616c  iscord/lmms-eval
+00000e80: 5d28 6874 7470 733a 2f2f 6469 7363 6f72  ](https://discor
+00000e90: 642e 6767 2f65 6241 4d47 5373 5329 2e0a  d.gg/ebAMGSsS)..
+00000ea0: 0a23 2320 7630 2e31 2e30 2052 656c 6561  .## v0.1.0 Relea
+00000eb0: 7365 640a 0a54 6865 2066 6972 7374 2076  sed..The first v
+00000ec0: 6572 7369 6f6e 206f 6620 7468 6520 606c  ersion of the `l
+00000ed0: 6d6d 732d 6576 616c 6020 6973 2072 656c  mms-eval` is rel
+00000ee0: 6561 7365 642e 2057 6520 6172 6520 776f  eased. We are wo
+00000ef0: 726b 696e 6720 6f6e 2070 726f 7669 6469  rking on providi
+00000f00: 6e67 2061 6e20 6f6e 652d 636f 6d6d 616e  ng an one-comman
+00000f10: 6420 6576 616c 7561 7469 6f6e 2073 7569  d evaluation sui
+00000f20: 7465 2066 6f72 2061 6363 656c 6572 6174  te for accelerat
+00000f30: 696e 6720 7468 6520 6465 7665 6c6f 706d  ing the developm
+00000f40: 656e 7420 6f66 204c 4d4d 732e 200a 0a3e  ent of LMMs. ..>
+00000f50: 2049 6e20 5b4c 4c61 5641 204e 6578 745d   In [LLaVA Next]
+00000f60: 2868 7474 7073 3a2f 2f6c 6c61 7661 2d76  (https://llava-v
+00000f70: 6c2e 6769 7468 7562 2e69 6f2f 626c 6f67  l.github.io/blog
+00000f80: 2f32 3032 342d 3031 2d33 302d 6c6c 6176  /2024-01-30-llav
+00000f90: 612d 6e65 7874 2f29 2064 6576 656c 6f70  a-next/) develop
+00000fa0: 6d65 6e74 2c20 7765 2069 6e74 6572 6e61  ment, we interna
+00000fb0: 6c6c 7920 7574 696c 697a 6520 7468 6973  lly utilize this
+00000fc0: 2073 7569 7465 2074 6f20 6576 616c 7561   suite to evalua
+00000fd0: 7465 2074 6865 206d 756c 7469 706c 6520  te the multiple 
+00000fe0: 6469 6666 6572 656e 7420 6d6f 6465 6c20  different model 
+00000ff0: 7665 7273 696f 6e73 206f 6e20 7661 7269  versions on vari
+00001000: 6f75 7320 6461 7461 7365 7473 2e20 4974  ous datasets. It
+00001010: 2073 6967 6e69 6669 6361 6e74 6c79 2061   significantly a
+00001020: 6363 656c 6572 6174 6573 2074 6865 206d  ccelerates the m
+00001030: 6f64 656c 2064 6576 656c 6f70 6d65 6e74  odel development
+00001040: 2063 7963 6c65 2066 6f72 2069 7427 7320   cycle for it's 
+00001050: 6561 7379 2069 6e74 6567 7261 7469 6f6e  easy integration
+00001060: 2061 6e64 2066 6173 7420 6576 616c 7561   and fast evalua
+00001070: 7469 6f6e 2073 7065 6564 2e0a 0a54 6865  tion speed...The
+00001080: 206d 6169 6e20 6665 6174 7572 6520 696e   main feature in
+00001090: 636c 7564 6573 3a0a 0a3c 7020 616c 6967  cludes:..<p alig
+000010a0: 6e3d 2263 656e 7465 7222 2077 6964 7468  n="center" width
+000010b0: 3d22 3130 3025 223e 0a3c 696d 6720 7372  ="100%">.<img sr
+000010c0: 633d 2268 7474 7073 3a2f 2f69 2e70 6f73  c="https://i.pos
+000010d0: 7469 6d67 2e63 632f 7367 7a4e 6d4a 7837  timg.cc/sgzNmJx7
+000010e0: 2f74 6561 7365 722e 706e 6722 2020 7769  /teaser.png"  wi
+000010f0: 6474 683d 2231 3030 2522 2068 6569 6768  dth="100%" heigh
+00001100: 743d 2238 3025 223e 0a3c 2f70 3e0a 0a23  t="80%">.</p>..#
+00001110: 2323 204f 6e65 2d63 6f6d 6d61 6e64 2065  ## One-command e
+00001120: 7661 6c75 6174 696f 6e2c 2077 6974 6820  valuation, with 
+00001130: 6465 7461 696c 6564 206c 6f67 7320 616e  detailed logs an
+00001140: 6420 7361 6d70 6c65 732e 0a59 6f75 2063  d samples..You c
+00001150: 616e 2065 7661 6c75 6174 6520 7468 6520  an evaluate the 
+00001160: 6d6f 6465 6c73 206f 6e20 6d75 6c74 6970  models on multip
+00001170: 6c65 2064 6174 6173 6574 7320 7769 7468  le datasets with
+00001180: 2061 2073 696e 676c 6520 636f 6d6d 616e   a single comman
+00001190: 642e 204e 6f20 6d6f 6465 6c2f 6461 7461  d. No model/data
+000011a0: 2070 7265 7061 7261 7469 6f6e 2069 7320   preparation is 
+000011b0: 6e65 6564 6564 2c20 6a75 7374 206f 6e65  needed, just one
+000011c0: 2063 6f6d 6d61 6e64 206c 696e 652c 2066   command line, f
+000011d0: 6577 206d 696e 7574 6573 2c20 616e 6420  ew minutes, and 
+000011e0: 6765 7420 7468 6520 7265 7375 6c74 732e  get the results.
+000011f0: 204e 6f74 206a 7573 7420 6120 7265 7375   Not just a resu
+00001200: 6c74 206e 756d 6265 722c 2062 7574 2061  lt number, but a
+00001210: 6c73 6f20 7468 6520 6465 7461 696c 6564  lso the detailed
+00001220: 206c 6f67 7320 616e 6420 7361 6d70 6c65   logs and sample
+00001230: 732c 2069 6e63 6c75 6469 6e67 2074 6865  s, including the
+00001240: 206d 6f64 656c 2061 7267 732c 2069 6e70   model args, inp
+00001250: 7574 2071 7565 7374 696f 6e2c 206d 6f64  ut question, mod
+00001260: 656c 2072 6573 706f 6e73 652c 2061 6e64  el response, and
+00001270: 2067 726f 756e 6420 7472 7574 6820 616e   ground truth an
+00001280: 7377 6572 2e0a 0a60 6060 7079 7468 6f6e  swer...```python
+00001290: 0a23 2045 7661 6c75 6174 696e 6720 4c4c  .# Evaluating LL
+000012a0: 6156 4120 6f6e 206d 756c 7469 706c 6520  aVA on multiple 
+000012b0: 6461 7461 7365 7473 0a61 6363 656c 6572  datasets.acceler
+000012c0: 6174 6520 6c61 756e 6368 202d 2d6e 756d  ate launch --num
+000012d0: 5f70 726f 6365 7373 6573 3d38 202d 6d20  _processes=8 -m 
+000012e0: 6c6d 6d73 5f65 7661 6c20 2d2d 6d6f 6465  lmms_eval --mode
+000012f0: 6c20 6c6c 6176 6120 2020 2d2d 6d6f 6465  l llava   --mode
+00001300: 6c5f 6172 6773 2070 7265 7472 6169 6e65  l_args pretraine
+00001310: 643d 226c 6975 6861 6f74 6961 6e2f 6c6c  d="liuhaotian/ll
+00001320: 6176 612d 7631 2e35 2d37 6222 2020 202d  ava-v1.5-7b"   -
+00001330: 2d74 6173 6b73 206d 6d65 2c6d 6d62 656e  -tasks mme,mmben
+00001340: 6368 5f65 6e20 2d2d 6261 7463 685f 7369  ch_en --batch_si
+00001350: 7a65 2031 202d 2d6c 6f67 5f73 616d 706c  ze 1 --log_sampl
+00001360: 6573 202d 2d6c 6f67 5f73 616d 706c 6573  es --log_samples
+00001370: 5f73 7566 6669 7820 6c6c 6176 615f 7631  _suffix llava_v1
+00001380: 2e35 5f6d 6d65 5f6d 6d62 656e 6368 656e  .5_mme_mmbenchen
+00001390: 202d 2d6f 7574 7075 745f 7061 7468 202e   --output_path .
+000013a0: 2f6c 6f67 732f 2023 0a60 6060 0a0a 2323  /logs/ #.```..##
+000013b0: 2320 4163 6365 6c65 7261 746f 7220 7375  # Accelerator su
+000013c0: 7070 6f72 7420 616e 6420 5461 736b 7320  pport and Tasks 
+000013d0: 6772 6f75 7069 6e67 2e0a 5765 2073 7570  grouping..We sup
+000013e0: 706f 7274 2074 6865 2075 7361 6765 206f  port the usage o
+000013f0: 6620 6061 6363 656c 6572 6174 6560 2074  f `accelerate` t
+00001400: 6f20 7772 6170 2074 6865 206d 6f64 656c  o wrap the model
+00001410: 2066 6f72 2064 6973 7472 6962 7574 6564   for distributed
+00001420: 2065 7661 6c75 6174 696f 6e2c 2073 7570   evaluation, sup
+00001430: 706f 7274 696e 6720 6d75 6c74 692d 6770  porting multi-gp
+00001440: 7520 616e 6420 7465 6e73 6f72 2070 6172  u and tensor par
+00001450: 616c 6c65 6c69 736d 2e20 5769 7468 202a  allelism. With *
+00001460: 2a54 6173 6b20 4772 6f75 7069 6e67 2a2a  *Task Grouping**
+00001470: 2c20 616c 6c20 696e 7374 616e 6365 7320  , all instances 
+00001480: 6672 6f6d 2061 6c6c 2074 6173 6b73 2061  from all tasks a
+00001490: 7265 2067 726f 7570 6564 2061 6e64 2065  re grouped and e
+000014a0: 7661 6c75 6174 6564 2069 6e20 7061 7261  valuated in para
+000014b0: 6c6c 656c 2c20 7768 6963 6820 7369 676e  llel, which sign
+000014c0: 6966 6963 616e 746c 7920 696d 7072 6f76  ificantly improv
+000014d0: 6573 2074 6865 2074 6872 6f75 6768 7075  es the throughpu
+000014e0: 7420 6f66 2074 6865 2065 7661 6c75 6174  t of the evaluat
+000014f0: 696f 6e2e 2041 6674 6572 2065 7661 6c75  ion. After evalu
+00001500: 6174 696f 6e2c 2061 6c6c 2069 6e73 7461  ation, all insta
+00001510: 6e63 6573 2061 7265 2073 656e 7420 746f  nces are sent to
+00001520: 2070 6f73 7470 726f 6365 7373 696e 6720   postprocessing 
+00001530: 6d6f 6475 6c65 2066 6f72 206d 6574 7269  module for metri
+00001540: 6320 6361 6c63 7561 7469 6f6e 7320 616e  c calcuations an
+00001550: 6420 706f 7465 6e74 6961 6c20 4750 5434  d potential GPT4
+00001560: 2d65 7661 6c20 7175 6572 6965 732e 0a0a  -eval queries...
+00001570: 4265 6c6f 7720 6172 6520 7468 6520 746f  Below are the to
+00001580: 7461 6c20 7275 6e74 696d 6520 6f6e 2064  tal runtime on d
+00001590: 6966 6665 7265 6e74 2064 6174 6173 6574  ifferent dataset
+000015a0: 7320 7573 696e 6720 3420 7820 4131 3030  s using 4 x A100
+000015b0: 2034 3047 2e0a 0a7c 2044 6174 6173 6574   40G...| Dataset
+000015c0: 2028 236e 756d 2920 2020 2020 2020 2020   (#num)         
+000015d0: 207c 204c 4c61 5641 2d76 312e 352d 3762   | LLaVA-v1.5-7b
+000015e0: 2020 2020 2020 7c20 4c4c 6156 412d 7631        | LLaVA-v1
+000015f0: 2e35 2d31 3362 2020 2020 207c 0a7c 203a  .5-13b     |.| :
+00001600: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001610: 2d2d 2d2d 2d2d 207c 203a 2d2d 2d2d 2d2d  ------ | :------
+00001620: 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c20 3a2d  ----------- | :-
+00001630: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001640: 207c 0a7c 206d 6d65 2028 3233 3734 2920   |.| mme (2374) 
+00001650: 2020 2020 2020 2020 2020 2020 207c 2032               | 2
+00001660: 206d 696e 7320 3433 2073 6563 6f6e 6473   mins 43 seconds
+00001670: 2020 7c20 3320 6d69 6e73 2032 3720 7365    | 3 mins 27 se
+00001680: 636f 6e64 7320 207c 0a7c 2067 7161 2028  conds  |.| gqa (
+00001690: 3132 3537 3829 2020 2020 2020 2020 2020  12578)          
+000016a0: 2020 207c 2031 3020 6d69 6e73 2034 3320     | 10 mins 43 
+000016b0: 7365 636f 6e64 7320 7c20 3134 206d 696e  seconds | 14 min
+000016c0: 7320 3233 2073 6563 6f6e 6473 207c 0a7c  s 23 seconds |.|
+000016d0: 2073 6369 656e 6365 7161 5f69 6d67 2028   scienceqa_img (
+000016e0: 3230 3137 2920 2020 207c 2031 206d 696e  2017)    | 1 min
+000016f0: 7320 3538 2073 6563 6f6e 6473 2020 7c20  s 58 seconds  | 
+00001700: 3220 6d69 6e73 2035 3220 7365 636f 6e64  2 mins 52 second
+00001710: 7320 207c 0a7c 2061 6932 6420 2833 3038  s  |.| ai2d (308
+00001720: 3829 2020 2020 2020 2020 2020 2020 207c  8)             |
+00001730: 2033 206d 696e 7320 3137 2073 6563 6f6e   3 mins 17 secon
+00001740: 6473 2020 7c20 3420 6d69 6e73 2031 3220  ds  | 4 mins 12 
+00001750: 7365 636f 6e64 7320 207c 0a7c 2063 6f63  seconds  |.| coc
+00001760: 6f32 3031 375f 6361 705f 7661 6c20 2835  o2017_cap_val (5
+00001770: 3030 3029 207c 2031 3420 6d69 6e73 2031  000) | 14 mins 1
+00001780: 3320 7365 636f 6e64 7320 7c20 3139 206d  3 seconds | 19 m
+00001790: 696e 7320 3538 2073 6563 6f6e 6473 207c  ins 58 seconds |
+000017a0: 0a0a 2323 2320 416c 6c2d 496e 2d4f 6e65  ..### All-In-One
+000017b0: 2048 4620 6461 7461 7365 7420 6875 6273   HF dataset hubs
+000017c0: 2e0a 0a57 6520 6172 6520 686f 7374 696e  ...We are hostin
+000017d0: 6720 6d6f 7265 2074 6861 6e20 3430 2028  g more than 40 (
+000017e0: 616e 6420 696e 6372 6561 7369 6e67 2920  and increasing) 
+000017f0: 6461 7461 7365 7473 206f 6e20 5b68 7567  datasets on [hug
+00001800: 6769 6e67 6661 6365 2f6c 6d6d 732d 6c61  gingface/lmms-la
+00001810: 625d 2868 7474 7073 3a2f 2f68 7567 6769  b](https://huggi
+00001820: 6e67 6661 6365 2e63 6f2f 6c6d 6d73 2d6c  ngface.co/lmms-l
+00001830: 6162 292c 2077 6520 6361 7265 6675 6c6c  ab), we carefull
+00001840: 7920 636f 6e76 6572 7465 6420 7468 6573  y converted thes
+00001850: 6520 6461 7461 7365 7473 2066 726f 6d20  e datasets from 
+00001860: 6f72 6967 696e 616c 2073 6f75 7263 6573  original sources
+00001870: 2061 6e64 2069 6e63 6c75 6465 6420 616c   and included al
+00001880: 6c20 7661 7269 616e 7473 2c20 7665 7273  l variants, vers
+00001890: 696f 6e73 2061 6e64 2073 706c 6974 732e  ions and splits.
+000018a0: 204e 6f77 2074 6865 7920 6361 6e20 6265   Now they can be
+000018b0: 2064 6972 6563 746c 7920 6163 6365 7373   directly access
+000018c0: 6564 2077 6974 686f 7574 2061 6e79 2062  ed without any b
+000018d0: 7572 6465 6e20 6f66 2064 6174 6120 7072  urden of data pr
+000018e0: 6570 726f 6365 7373 696e 672e 2054 6865  eprocessing. The
+000018f0: 7920 616c 736f 2073 6572 7665 2066 6f72  y also serve for
+00001900: 2074 6865 2070 7572 706f 7365 206f 6620   the purpose of 
+00001910: 7669 7375 616c 697a 696e 6720 7468 6520  visualizing the 
+00001920: 6461 7461 2061 6e64 2067 7261 7370 696e  data and graspin
+00001930: 6720 7468 6520 7365 6e73 6520 6f66 2065  g the sense of e
+00001940: 7661 6c75 6174 696f 6e20 7461 736b 7320  valuation tasks 
+00001950: 6469 7374 7269 6275 7469 6f6e 2e0a 0a3c  distribution...<
+00001960: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
+00001970: 2077 6964 7468 3d22 3130 3025 223e 0a3c   width="100%">.<
+00001980: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00001990: 2f69 2e70 6f73 7469 6d67 2e63 632f 3850  /i.postimg.cc/8P
+000019a0: 5846 5739 736b 2f57 5832 3032 3430 3232  XFW9sk/WX2024022
+000019b0: 382d 3132 3331 3130 5f32 782e 706e 6722  8-123110_2x.png"
+000019c0: 2020 7769 6474 683d 2231 3030 2522 2068    width="100%" h
+000019d0: 6569 6768 743d 2238 3025 223e 0a3c 2f70  eight="80%">.</p
+000019e0: 3e0a 0a23 2323 2044 6574 6169 6c65 6420  >..### Detailed 
+000019f0: 4c6f 6767 696e 6720 5574 696c 6974 6573  Logging Utilites
+00001a00: 0a0a 5765 2070 726f 7669 6465 2064 6574  ..We provide det
+00001a10: 6169 6c65 6420 6c6f 6767 696e 6720 7574  ailed logging ut
+00001a20: 696c 6974 6965 7320 746f 2068 656c 7020  ilities to help 
+00001a30: 796f 7520 756e 6465 7273 7461 6e64 2074  you understand t
+00001a40: 6865 2065 7661 6c75 6174 696f 6e20 7072  he evaluation pr
+00001a50: 6f63 6573 7320 616e 6420 7265 7375 6c74  ocess and result
+00001a60: 732e 2054 6865 206c 6f67 7320 696e 636c  s. The logs incl
+00001a70: 7564 6520 7468 6520 6d6f 6465 6c20 6172  ude the model ar
+00001a80: 6773 2c20 6765 6e65 7261 7469 6f6e 2070  gs, generation p
+00001a90: 6172 616d 6574 6572 732c 2069 6e70 7574  arameters, input
+00001aa0: 2071 7565 7374 696f 6e2c 206d 6f64 656c   question, model
+00001ab0: 2072 6573 706f 6e73 652c 2061 6e64 2067   response, and g
+00001ac0: 726f 756e 6420 7472 7574 6820 616e 7377  round truth answ
+00001ad0: 6572 2e20 596f 7520 6361 6e20 616c 736f  er. You can also
+00001ae0: 2072 6563 6f72 6420 6576 6572 7920 6465   record every de
+00001af0: 7461 696c 7320 616e 6420 7669 7375 616c  tails and visual
+00001b00: 697a 6520 7468 656d 2069 6e73 6964 6520  ize them inside 
+00001b10: 7275 6e73 206f 6e20 5765 6967 6874 7320  runs on Weights 
+00001b20: 2620 4269 6173 6573 2e0a 0a7b 2520 696e  & Biases...{% in
+00001b30: 636c 7564 6520 6669 6775 7265 2e6c 6971  clude figure.liq
+00001b40: 7569 6420 6c6f 6164 696e 673d 2265 6167  uid loading="eag
+00001b50: 6572 2220 7061 7468 3d22 6173 7365 7473  er" path="assets
+00001b60: 2f69 6d67 2f77 616e 6462 5f74 6162 6c65  /img/wandb_table
+00001b70: 2e70 6e67 2220 636c 6173 733d 2269 6d67  .png" class="img
+00001b80: 2d66 6c75 6964 2072 6f75 6e64 6564 207a  -fluid rounded z
+00001b90: 2d64 6570 7468 2d31 2220 7a6f 6f6d 6162  -depth-1" zoomab
+00001ba0: 6c65 3d74 7275 6520 257d 0a0a 3c70 2061  le=true %}..<p a
+00001bb0: 6c69 676e 3d22 6365 6e74 6572 2220 7769  lign="center" wi
+00001bc0: 6474 683d 2231 3030 2522 3e0a 3c69 6d67  dth="100%">.<img
+00001bd0: 2073 7263 3d22 6874 7470 733a 2f2f 692e   src="https://i.
+00001be0: 706f 7374 696d 672e 6363 2f57 3163 3176  postimg.cc/W1c1v
+00001bf0: 4244 4a2f 5765 6368 6174 2d49 4d47 3139  BDJ/Wechat-IMG19
+00001c00: 3933 2e70 6e67 2220 2077 6964 7468 3d22  93.png"  width="
+00001c10: 3130 3025 2220 6865 6967 6874 3d22 3830  100%" height="80
+00001c20: 2522 3e0a 3c2f 703e 0a0a 2320 496e 7374  %">.</p>..# Inst
+00001c30: 616c 6c61 7469 6f6e 0a0a 466f 7220 666f  allation..For fo
+00001c40: 726d 616c 2075 7361 6765 2c20 796f 7520  rmal usage, you 
+00001c50: 6361 6e20 696e 7374 616c 6c20 7468 6520  can install the 
+00001c60: 7061 636b 6167 6520 6672 6f6d 2050 7950  package from PyP
+00001c70: 4920 6279 2072 756e 6e69 6e67 2074 6865  I by running the
+00001c80: 2066 6f6c 6c6f 7769 6e67 2063 6f6d 6d61   following comma
+00001c90: 6e64 3a0a 6060 6062 6173 680a 7069 7020  nd:.```bash.pip 
+00001ca0: 696e 7374 616c 6c20 6c6d 6d73 2d65 7661  install lmms-eva
+00001cb0: 6c0a 6060 600a 0a46 6f72 2064 6576 656c  l.```..For devel
+00001cc0: 6f70 6d65 6e74 2c20 796f 7520 6361 6e20  opment, you can 
+00001cd0: 696e 7374 616c 6c20 7468 6520 7061 636b  install the pack
+00001ce0: 6167 6520 6279 2063 6c6f 6e69 6e67 2074  age by cloning t
+00001cf0: 6865 2072 6570 6f73 6974 6f72 7920 616e  he repository an
+00001d00: 6420 7275 6e6e 696e 6720 7468 6520 666f  d running the fo
+00001d10: 6c6c 6f77 696e 6720 636f 6d6d 616e 643a  llowing command:
+00001d20: 0a60 6060 6261 7368 0a67 6974 2063 6c6f  .```bash.git clo
+00001d30: 6e65 2068 7474 7073 3a2f 2f67 6974 6875  ne https://githu
+00001d40: 622e 636f 6d2f 4576 6f6c 7669 6e67 4c4d  b.com/EvolvingLM
+00001d50: 4d73 2d4c 6162 2f6c 6d6d 732d 6576 616c  Ms-Lab/lmms-eval
+00001d60: 0a63 6420 6c6d 6d73 2d65 7661 6c0a 7069  .cd lmms-eval.pi
+00001d70: 7020 696e 7374 616c 6c20 2d65 202e 0a60  p install -e ..`
+00001d80: 6060 0a0a 4966 2079 6f75 2077 616e 7465  ``..If you wante
+00001d90: 6420 746f 2074 6573 7420 6c6c 6176 612c  d to test llava,
+00001da0: 2079 6f75 2077 696c 6c20 6861 7665 2074   you will have t
+00001db0: 6f20 636c 6f6e 6520 7468 6569 7220 7265  o clone their re
+00001dc0: 706f 2066 726f 6d20 5b4c 4c61 5641 5d28  po from [LLaVA](
+00001dd0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001de0: 6f6d 2f68 616f 7469 616e 2d6c 6975 2f4c  om/haotian-liu/L
+00001df0: 4c61 5641 2920 616e 640a 6060 600a 6769  LaVA) and.```.gi
+00001e00: 7420 636c 6f6e 6520 6874 7470 733a 2f2f  t clone https://
+00001e10: 6769 7468 7562 2e63 6f6d 2f68 616f 7469  github.com/haoti
+00001e20: 616e 2d6c 6975 2f4c 4c61 5641 0a63 6420  an-liu/LLaVA.cd 
+00001e30: 4c4c 6156 410a 7069 7020 696e 7374 616c  LLaVA.pip instal
+00001e40: 6c20 2d65 202e 0a60 6060 0a0a 596f 7520  l -e ..```..You 
+00001e50: 6361 6e20 6368 6563 6b20 7468 6520 5b65  can check the [e
+00001e60: 6e76 6972 6f6e 6d65 6e74 2069 6e73 7461  nvironment insta
+00001e70: 6c6c 2073 6372 6970 745d 286d 6973 6373  ll script](miscs
+00001e80: 2f72 6570 725f 7363 7269 7074 732e 7368  /repr_scripts.sh
+00001e90: 2920 616e 6420 5b74 6f72 6368 2065 6e76  ) and [torch env
+00001ea0: 6972 6f6e 6d65 6e74 2069 6e66 6f5d 286d  ironment info](m
+00001eb0: 6973 6373 2f72 6570 725f 746f 7263 685f  iscs/repr_torch_
+00001ec0: 656e 7673 2e74 7874 2920 746f 202a 2a72  envs.txt) to **r
+00001ed0: 6570 726f 6475 6365 204c 4c61 5641 2d31  eproduce LLaVA-1
+00001ee0: 2e35 2773 2070 6170 6572 2072 6573 756c  .5's paper resul
+00001ef0: 7473 2a2a 2e20 5765 2066 6f75 6e64 2074  ts**. We found t
+00001f00: 6f72 6368 2f63 7564 6120 7665 7273 696f  orch/cuda versio
+00001f10: 6e73 2064 6966 6665 7265 6e63 6520 776f  ns difference wo
+00001f20: 756c 6420 6361 7573 6520 736d 616c 6c20  uld cause small 
+00001f30: 7661 7269 6174 696f 6e73 2069 6e20 7468  variations in th
+00001f40: 6520 7265 7375 6c74 732c 2077 6520 7072  e results, we pr
+00001f50: 6f76 6964 6520 7468 6520 5b72 6573 756c  ovide the [resul
+00001f60: 7473 2063 6865 636b 5d28 6d69 7363 732f  ts check](miscs/
+00001f70: 6c6c 6176 615f 7265 7375 6c74 5f63 6865  llava_result_che
+00001f80: 636b 2e6d 6429 2077 6974 6820 6469 6666  ck.md) with diff
+00001f90: 6572 656e 7420 656e 7669 726f 6e6d 656e  erent environmen
+00001fa0: 7473 2e0a 0a49 6620 796f 7520 7761 6e74  ts...If you want
+00001fb0: 2074 6f20 7465 7374 206f 6e20 6361 7074   to test on capt
+00001fc0: 696f 6e20 6461 7461 7365 7420 7375 6368  ion dataset such
+00001fd0: 2061 7320 6063 6f63 6f60 2c20 6072 6566   as `coco`, `ref
+00001fe0: 636f 636f 602c 2061 6e64 2060 6e6f 6361  coco`, and `noca
+00001ff0: 7073 602c 2079 6f75 2077 696c 6c20 6e65  ps`, you will ne
+00002000: 6564 2074 6f20 6861 7665 2060 6a61 7661  ed to have `java
+00002010: 3d3d 312e 382e 3020 6020 746f 206c 6574  ==1.8.0 ` to let
+00002020: 2070 7963 6f63 6f65 7661 6c20 6170 6920   pycocoeval api 
+00002030: 746f 2077 6f72 6b2e 2049 6620 796f 7520  to work. If you 
+00002040: 646f 6e27 7420 6861 7665 2069 742c 2079  don't have it, y
+00002050: 6f75 2063 616e 2069 6e73 7461 6c6c 2062  ou can install b
+00002060: 7920 7573 696e 6720 636f 6e64 610a 6060  y using conda.``
+00002070: 600a 636f 6e64 6120 696e 7374 616c 6c20  `.conda install 
+00002080: 6f70 656e 6a64 6b3d 380a 6060 600a 796f  openjdk=8.```.yo
+00002090: 7520 6361 6e20 7468 656e 2063 6865 636b  u can then check
+000020a0: 2079 6f75 7220 6a61 7661 2076 6572 7369   your java versi
+000020b0: 6f6e 2062 7920 606a 6176 6120 2d76 6572  on by `java -ver
+000020c0: 7369 6f6e 6020 0a0a 2320 5573 6167 650a  sion` ..# Usage.
+000020d0: 6060 6062 6173 680a 2320 4576 616c 7561  ```bash.# Evalua
+000020e0: 7469 6e67 204c 4c61 5641 206f 6e20 4d4d  ting LLaVA on MM
+000020f0: 450a 6163 6365 6c65 7261 7465 206c 6175  E.accelerate lau
+00002100: 6e63 6820 2d2d 6e75 6d5f 7072 6f63 6573  nch --num_proces
+00002110: 7365 733d 3820 2d6d 206c 6d6d 735f 6576  ses=8 -m lmms_ev
+00002120: 616c 202d 2d6d 6f64 656c 206c 6c61 7661  al --model llava
+00002130: 2020 202d 2d6d 6f64 656c 5f61 7267 7320     --model_args 
+00002140: 7072 6574 7261 696e 6564 3d22 6c69 7568  pretrained="liuh
+00002150: 616f 7469 616e 2f6c 6c61 7661 2d76 312e  aotian/llava-v1.
+00002160: 352d 3762 2220 2020 2d2d 7461 736b 7320  5-7b"   --tasks 
+00002170: 6d6d 6520 202d 2d62 6174 6368 5f73 697a  mme  --batch_siz
+00002180: 6520 3120 2d2d 6c6f 675f 7361 6d70 6c65  e 1 --log_sample
+00002190: 7320 2d2d 6c6f 675f 7361 6d70 6c65 735f  s --log_samples_
+000021a0: 7375 6666 6978 206c 6c61 7661 5f76 312e  suffix llava_v1.
+000021b0: 355f 6d6d 6520 2d2d 6f75 7470 7574 5f70  5_mme --output_p
+000021c0: 6174 6820 2e2f 6c6f 6773 2f20 0a0a 2320  ath ./logs/ ..# 
+000021d0: 4576 616c 7561 7469 6e67 204c 4c61 5641  Evaluating LLaVA
+000021e0: 206f 6e20 6d75 6c74 6970 6c65 2064 6174   on multiple dat
+000021f0: 6173 6574 730a 6163 6365 6c65 7261 7465  asets.accelerate
+00002200: 206c 6175 6e63 6820 2d2d 6e75 6d5f 7072   launch --num_pr
+00002210: 6f63 6573 7365 733d 3820 2d6d 206c 6d6d  ocesses=8 -m lmm
+00002220: 735f 6576 616c 202d 2d6d 6f64 656c 206c  s_eval --model l
+00002230: 6c61 7661 2020 202d 2d6d 6f64 656c 5f61  lava   --model_a
+00002240: 7267 7320 7072 6574 7261 696e 6564 3d22  rgs pretrained="
+00002250: 6c69 7568 616f 7469 616e 2f6c 6c61 7661  liuhaotian/llava
+00002260: 2d76 312e 352d 3762 2220 2020 2d2d 7461  -v1.5-7b"   --ta
+00002270: 736b 7320 6d6d 652c 6d6d 6265 6e63 685f  sks mme,mmbench_
+00002280: 656e 202d 2d62 6174 6368 5f73 697a 6520  en --batch_size 
+00002290: 3120 2d2d 6c6f 675f 7361 6d70 6c65 7320  1 --log_samples 
+000022a0: 2d2d 6c6f 675f 7361 6d70 6c65 735f 7375  --log_samples_su
+000022b0: 6666 6978 206c 6c61 7661 5f76 312e 355f  ffix llava_v1.5_
+000022c0: 6d6d 655f 6d6d 6265 6e63 6865 6e20 2d2d  mme_mmbenchen --
+000022d0: 6f75 7470 7574 5f70 6174 6820 2e2f 6c6f  output_path ./lo
+000022e0: 6773 2f20 230a 0a23 2046 6f72 206f 7468  gs/ #..# For oth
+000022f0: 6572 2076 6172 6961 6e74 7320 6c6c 6176  er variants llav
+00002300: 612e 204e 6f74 6520 7468 6174 2060 636f  a. Note that `co
+00002310: 6e76 5f74 656d 706c 6174 6560 2069 7320  nv_template` is 
+00002320: 616e 2061 7267 206f 6620 7468 6520 696e  an arg of the in
+00002330: 6974 2066 756e 6374 696f 6e20 6f66 206c  it function of l
+00002340: 6c61 7661 2069 6e20 606c 6d6d 735f 6576  lava in `lmms_ev
+00002350: 616c 2f6d 6f64 656c 732f 6c6c 6176 612e  al/models/llava.
+00002360: 7079 600a 6163 6365 6c65 7261 7465 206c  py`.accelerate l
+00002370: 6175 6e63 6820 2d2d 6e75 6d5f 7072 6f63  aunch --num_proc
+00002380: 6573 7365 733d 3820 2d6d 206c 6d6d 735f  esses=8 -m lmms_
+00002390: 6576 616c 202d 2d6d 6f64 656c 206c 6c61  eval --model lla
+000023a0: 7661 2020 202d 2d6d 6f64 656c 5f61 7267  va   --model_arg
+000023b0: 7320 7072 6574 7261 696e 6564 3d22 6c69  s pretrained="li
+000023c0: 7568 616f 7469 616e 2f6c 6c61 7661 2d76  uhaotian/llava-v
+000023d0: 312e 362d 6d69 7374 7261 6c2d 3762 2c63  1.6-mistral-7b,c
+000023e0: 6f6e 765f 7465 6d70 6c61 7465 3d6d 6973  onv_template=mis
+000023f0: 7472 616c 5f69 6e73 7472 7563 7422 2020  tral_instruct"  
+00002400: 202d 2d74 6173 6b73 206d 6d65 2c6d 6d62   --tasks mme,mmb
+00002410: 656e 6368 5f65 6e20 2d2d 6261 7463 685f  ench_en --batch_
+00002420: 7369 7a65 2031 202d 2d6c 6f67 5f73 616d  size 1 --log_sam
+00002430: 706c 6573 202d 2d6c 6f67 5f73 616d 706c  ples --log_sampl
+00002440: 6573 5f73 7566 6669 7820 6c6c 6176 615f  es_suffix llava_
+00002450: 7631 2e35 5f6d 6d65 5f6d 6d62 656e 6368  v1.5_mme_mmbench
+00002460: 656e 202d 2d6f 7574 7075 745f 7061 7468  en --output_path
+00002470: 202e 2f6c 6f67 732f 2023 0a61 6363 656c   ./logs/ #.accel
+00002480: 6572 6174 6520 6c61 756e 6368 202d 2d6e  erate launch --n
+00002490: 756d 5f70 726f 6365 7373 6573 3d38 202d  um_processes=8 -
+000024a0: 6d20 6c6d 6d73 5f65 7661 6c20 2d2d 6d6f  m lmms_eval --mo
+000024b0: 6465 6c20 6c6c 6176 6120 2020 2d2d 6d6f  del llava   --mo
+000024c0: 6465 6c5f 6172 6773 2070 7265 7472 6169  del_args pretrai
+000024d0: 6e65 643d 226c 6975 6861 6f74 6961 6e2f  ned="liuhaotian/
+000024e0: 6c6c 6176 612d 7631 2e36 2d33 3462 2c63  llava-v1.6-34b,c
+000024f0: 6f6e 765f 7465 6d70 6c61 7465 3d6d 6973  onv_template=mis
+00002500: 7472 616c 5f64 6972 6563 7422 2020 202d  tral_direct"   -
+00002510: 2d74 6173 6b73 206d 6d65 2c6d 6d62 656e  -tasks mme,mmben
+00002520: 6368 5f65 6e20 2d2d 6261 7463 685f 7369  ch_en --batch_si
+00002530: 7a65 2031 202d 2d6c 6f67 5f73 616d 706c  ze 1 --log_sampl
+00002540: 6573 202d 2d6c 6f67 5f73 616d 706c 6573  es --log_samples
+00002550: 5f73 7566 6669 7820 6c6c 6176 615f 7631  _suffix llava_v1
+00002560: 2e35 5f6d 6d65 5f6d 6d62 656e 6368 656e  .5_mme_mmbenchen
+00002570: 202d 2d6f 7574 7075 745f 7061 7468 202e   --output_path .
+00002580: 2f6c 6f67 732f 2023 0a0a 2320 4672 6f6d  /logs/ #..# From
+00002590: 2061 2070 7265 6465 6669 6e65 6420 636f   a predefined co
+000025a0: 6e66 6967 7572 6174 696f 6e2c 2073 7570  nfiguration, sup
+000025b0: 706f 7274 696e 6720 6576 616c 7561 7469  porting evaluati
+000025c0: 6f6e 206f 6620 6d75 6c74 6970 6c65 206d  on of multiple m
+000025d0: 6f64 656c 7320 616e 6420 6461 7461 7365  odels and datase
+000025e0: 7473 0a61 6363 656c 6572 6174 6520 6c61  ts.accelerate la
+000025f0: 756e 6368 202d 2d6e 756d 5f70 726f 6365  unch --num_proce
+00002600: 7373 6573 3d38 202d 6d20 6c6d 6d73 5f65  sses=8 -m lmms_e
+00002610: 7661 6c20 2d2d 636f 6e66 6967 2065 7861  val --config exa
+00002620: 6d70 6c65 5f65 7661 6c2e 7961 6d6c 200a  mple_eval.yaml .
+00002630: 6060 600a 0a23 204d 6f64 656c 2052 6573  ```..# Model Res
+00002640: 756c 7473 0a0a 4173 2064 656d 6f6e 7374  ults..As demonst
+00002650: 7261 7465 6420 6279 2074 6865 2065 7874  rated by the ext
+00002660: 656e 7369 7665 2074 6162 6c65 2062 656c  ensive table bel
+00002670: 6f77 2c20 7765 2061 696d 2074 6f20 7072  ow, we aim to pr
+00002680: 6f76 6964 6520 6465 7461 696c 6564 2069  ovide detailed i
+00002690: 6e66 6f72 6d61 7469 6f6e 2066 6f72 2072  nformation for r
+000026a0: 6561 6465 7273 2074 6f20 756e 6465 7273  eaders to unders
+000026b0: 7461 6e64 2074 6865 2064 6174 6173 6574  tand the dataset
+000026c0: 7320 696e 636c 7564 6564 2069 6e20 6c6d  s included in lm
+000026d0: 6d73 2d65 7661 6c20 616e 6420 736f 6d65  ms-eval and some
+000026e0: 2073 7065 6369 6669 6320 6465 7461 696c   specific detail
+000026f0: 7320 6162 6f75 7420 7468 6573 6520 6461  s about these da
+00002700: 7461 7365 7473 2028 7765 2072 656d 6169  tasets (we remai
+00002710: 6e20 6772 6174 6566 756c 2066 6f72 2061  n grateful for a
+00002720: 6e79 2063 6f72 7265 6374 696f 6e73 2072  ny corrections r
+00002730: 6561 6465 7273 206d 6179 2068 6176 6520  eaders may have 
+00002740: 6475 7269 6e67 206f 7572 2065 7661 6c75  during our evalu
+00002750: 6174 696f 6e20 7072 6f63 6573 7329 2e0a  ation process)..
+00002760: 0a57 6520 7072 6f76 6964 6520 6120 476f  .We provide a Go
+00002770: 6f67 6c65 2053 6865 6574 2066 6f72 2074  ogle Sheet for t
+00002780: 6865 2064 6574 6169 6c65 6420 7265 7375  he detailed resu
+00002790: 6c74 7320 6f66 2074 6865 204c 4c61 5641  lts of the LLaVA
+000027a0: 2073 6572 6965 7320 6d6f 6465 6c73 206f   series models o
+000027b0: 6e20 6469 6666 6572 656e 7420 6461 7461  n different data
+000027c0: 7365 7473 2e20 596f 7520 6361 6e20 6163  sets. You can ac
+000027d0: 6365 7373 2074 6865 2073 6865 6574 205b  cess the sheet [
+000027e0: 6865 7265 5d28 6874 7470 733a 2f2f 646f  here](https://do
+000027f0: 6373 2e67 6f6f 676c 652e 636f 6d2f 7370  cs.google.com/sp
+00002800: 7265 6164 7368 6565 7473 2f64 2f31 6135  readsheets/d/1a5
+00002810: 496d 6664 4b41 5444 4938 5437 4377 6836  ImfdKATDI8T7Cwh6
+00002820: 6548 2d62 4573 6e51 467a 616e 4672 6146  eH-bEsnQFzanFraF
+00002830: 5567 6353 394b 4857 632f 6564 6974 3f75  UgcS9KHWc/edit?u
+00002840: 7370 3d73 6861 7269 6e67 292e 2049 7427  sp=sharing). It'
+00002850: 7320 6120 6c69 7665 2073 6865 6574 2c20  s a live sheet, 
+00002860: 616e 6420 7765 2061 7265 2075 7064 6174  and we are updat
+00002870: 696e 6720 6974 2077 6974 6820 6e65 7720  ing it with new 
+00002880: 7265 7375 6c74 732e 0a0a 3c70 2061 6c69  results...<p ali
+00002890: 676e 3d22 6365 6e74 6572 2220 7769 6474  gn="center" widt
+000028a0: 683d 2231 3030 2522 3e0a 3c69 6d67 2073  h="100%">.<img s
+000028b0: 7263 3d22 6874 7470 733a 2f2f 692e 706f  rc="https://i.po
+000028c0: 7374 696d 672e 6363 2f6a 6477 3439 374e  stimg.cc/jdw497N
+000028d0: 532f 5758 3230 3234 3033 3037 2d31 3632  S/WX20240307-162
+000028e0: 3532 362d 3278 2e70 6e67 2220 2077 6964  526-2x.png"  wid
+000028f0: 7468 3d22 3130 3025 2220 6865 6967 6874  th="100%" height
+00002900: 3d22 3830 2522 3e0a 3c2f 703e 0a0a 5765  ="80%">.</p>..We
+00002910: 2061 6c73 6f20 7072 6f76 6964 6520 7468   also provide th
+00002920: 6520 7261 7720 6461 7461 2065 7870 6f72  e raw data expor
+00002930: 7465 6420 6672 6f6d 2057 6569 6768 7473  ted from Weights
+00002940: 2026 2042 6961 7365 7320 666f 7220 7468   & Biases for th
+00002950: 6520 6465 7461 696c 6564 2072 6573 756c  e detailed resul
+00002960: 7473 206f 6620 7468 6520 4c4c 6156 4120  ts of the LLaVA 
+00002970: 7365 7269 6573 206d 6f64 656c 7320 6f6e  series models on
+00002980: 2064 6966 6665 7265 6e74 2064 6174 6173   different datas
+00002990: 6574 732e 2059 6f75 2063 616e 2061 6363  ets. You can acc
+000029a0: 6573 7320 7468 6520 7261 7720 6461 7461  ess the raw data
+000029b0: 205b 6865 7265 5d28 6874 7470 733a 2f2f   [here](https://
+000029c0: 646f 6373 2e67 6f6f 676c 652e 636f 6d2f  docs.google.com/
+000029d0: 7370 7265 6164 7368 6565 7473 2f64 2f31  spreadsheets/d/1
+000029e0: 4176 6145 6d75 4734 6373 536d 5861 486a  AvaEmuG4csSmXaHj
+000029f0: 6775 3465 6931 4b42 4d6d 4e4e 5738 7766  gu4ei1KBMmNNW8wf
+00002a00: 6c4f 445f 6b6b 5444 6476 382f 6564 6974  lOD_kkTDdv8/edit
+00002a10: 3f75 7370 3d73 6861 7269 6e67 292e 0a0a  ?usp=sharing)...
+00002a20: 3e20 4465 7665 6c6f 706d 656e 7420 7769  > Development wi
+00002a30: 6c6c 2062 6520 636f 6e74 696e 7569 6e67  ll be continuing
+00002a40: 206f 6e20 7468 6520 6d61 696e 2062 7261   on the main bra
+00002a50: 6e63 682c 2061 6e64 2077 6520 656e 636f  nch, and we enco
+00002a60: 7572 6167 6520 796f 7520 746f 2067 6976  urage you to giv
+00002a70: 6520 7573 2066 6565 6462 6163 6b20 6f6e  e us feedback on
+00002a80: 2077 6861 7420 6665 6174 7572 6573 2061   what features a
+00002a90: 7265 2064 6573 6972 6564 2061 6e64 2068  re desired and h
+00002aa0: 6f77 2074 6f20 696d 7072 6f76 6520 7468  ow to improve th
+00002ab0: 6520 6c69 6272 6172 7920 6675 7274 6865  e library furthe
+00002ac0: 722c 206f 7220 6173 6b20 7175 6573 7469  r, or ask questi
+00002ad0: 6f6e 732c 2065 6974 6865 7220 696e 2069  ons, either in i
+00002ae0: 7373 7565 7320 6f72 2050 5273 206f 6e20  ssues or PRs on 
+00002af0: 4769 7448 7562 2e0a 0a0a 2323 2053 7570  GitHub....## Sup
+00002b00: 706f 7274 6564 206d 6f64 656c 730a 0a2d  ported models..-
+00002b10: 2047 5054 3456 2028 4150 492c 206f 6e6c   GPT4V (API, onl
+00002b20: 7920 6765 6e65 7261 7469 6f6e 2d62 6173  y generation-bas
+00002b30: 6564 2065 7661 6c75 6174 696f 6e29 0a2d  ed evaluation).-
+00002b40: 204c 4c61 5641 2d76 312e 352f 7631 2e36   LLaVA-v1.5/v1.6
+00002b50: 2d37 422f 3133 422f 3334 4220 2870 706c  -7B/13B/34B (ppl
+00002b60: 2d62 6173 6564 2c20 6765 6e65 7261 7469  -based, generati
+00002b70: 6f6e 2d62 6173 6564 290a 2d20 5177 656e  on-based).- Qwen
+00002b80: 2d56 4c20 7365 7269 6573 2028 7070 6c2d  -VL series (ppl-
+00002b90: 6261 7365 642c 2067 656e 6572 6174 696f  based, generatio
+00002ba0: 6e2d 6261 7365 6429 0a2d 2046 7579 7520  n-based).- Fuyu 
+00002bb0: 7365 7269 6573 2028 7070 6c2d 6261 7365  series (ppl-base
+00002bc0: 642c 2067 656e 6572 6174 696f 6e2d 6261  d, generation-ba
+00002bd0: 7365 6429 0a2d 2049 6e73 7472 7563 7442  sed).- InstructB
+00002be0: 4c49 5020 7365 7269 6573 2028 6765 6e65  LIP series (gene
+00002bf0: 7261 7469 6f6e 2d62 6173 6564 290a 0a23  ration-based)..#
+00002c00: 2320 5375 7070 6f72 7465 6420 6461 7461  # Supported data
+00002c10: 7365 7473 0a3e 2028 2920 696e 6469 6361  sets.> () indica
+00002c20: 7465 7320 7468 6520 7461 736b 206e 616d  tes the task nam
+00002c30: 6520 696e 2074 6865 206c 6d6d 735f 6576  e in the lmms_ev
+00002c40: 616c 2e20 5468 6520 7461 736b 206e 616d  al. The task nam
+00002c50: 6520 6973 2061 6c73 6f20 7573 6564 2074  e is also used t
+00002c60: 6f20 7370 6563 6966 7920 7468 6520 6461  o specify the da
+00002c70: 7461 7365 7420 696e 2074 6865 2063 6f6e  taset in the con
+00002c80: 6669 6775 7261 7469 6f6e 2066 696c 652e  figuration file.
+00002c90: 0a0a 2d20 4149 3244 2028 6169 3264 290a  ..- AI2D (ai2d).
+00002ca0: 2d20 4368 6172 7451 4120 2863 6861 7274  - ChartQA (chart
+00002cb0: 7161 290a 2d20 434d 4d4d 5520 2863 6d6d  qa).- CMMMU (cmm
+00002cc0: 6d75 290a 2020 2d20 434d 4d4d 5520 5661  mu).  - CMMMU Va
+00002cd0: 6c69 6461 7469 6f6e 2028 636d 6d6d 755f  lidation (cmmmu_
+00002ce0: 7661 6c29 0a20 202d 2043 4d4d 4d55 2054  val).  - CMMMU T
+00002cf0: 6573 7420 2863 6d6d 6d75 5f74 6573 7429  est (cmmmu_test)
+00002d00: 0a2d 2043 4f43 4f20 4361 7074 696f 6e20  .- COCO Caption 
+00002d10: 2863 6f63 6f5f 6361 7029 0a20 202d 2043  (coco_cap).  - C
+00002d20: 4f43 4f20 3230 3134 2043 6170 7469 6f6e  OCO 2014 Caption
+00002d30: 2028 636f 636f 3230 3134 5f63 6170 290a   (coco2014_cap).
+00002d40: 2020 2020 2d20 434f 434f 2032 3031 3420      - COCO 2014 
+00002d50: 4361 7074 696f 6e20 5661 6c69 6461 7469  Caption Validati
+00002d60: 6f6e 2028 636f 636f 3230 3134 5f63 6170  on (coco2014_cap
+00002d70: 5f76 616c 290a 2020 2020 2d20 434f 434f  _val).    - COCO
+00002d80: 2032 3031 3420 4361 7074 696f 6e20 5465   2014 Caption Te
+00002d90: 7374 2028 636f 636f 3230 3134 5f63 6170  st (coco2014_cap
+00002da0: 5f74 6573 7429 0a20 202d 2043 4f43 4f20  _test).  - COCO 
+00002db0: 3230 3137 2043 6170 7469 6f6e 2028 636f  2017 Caption (co
+00002dc0: 636f 3230 3137 5f63 6170 290a 2020 2020  co2017_cap).    
+00002dd0: 2d20 434f 434f 2032 3031 3720 4361 7074  - COCO 2017 Capt
+00002de0: 696f 6e20 4d69 6e69 5661 6c20 2863 6f63  ion MiniVal (coc
+00002df0: 6f32 3031 375f 6361 705f 7661 6c29 0a20  o2017_cap_val). 
+00002e00: 2020 202d 2043 4f43 4f20 3230 3137 2043     - COCO 2017 C
+00002e10: 6170 7469 6f6e 204d 696e 6954 6573 7420  aption MiniTest 
+00002e20: 2863 6f63 6f32 3031 375f 6361 705f 7465  (coco2017_cap_te
+00002e30: 7374 290a 2d20 444f 4356 5141 2028 646f  st).- DOCVQA (do
+00002e40: 6376 7161 290a 2020 2d20 444f 4356 5141  cvqa).  - DOCVQA
+00002e50: 2056 616c 6964 6174 696f 6e20 2864 6f63   Validation (doc
+00002e60: 7671 615f 7661 6c29 0a20 202d 2044 4f43  vqa_val).  - DOC
+00002e70: 5651 4120 5465 7374 2028 646f 6376 7161  VQA Test (docvqa
+00002e80: 5f74 6573 7429 0a2d 2046 6572 7265 7420  _test).- Ferret 
+00002e90: 2866 6572 7265 7429 0a2d 2046 6c69 636b  (ferret).- Flick
+00002ea0: 7233 304b 2028 666c 6963 6b72 3330 6b29  r30K (flickr30k)
+00002eb0: 0a20 202d 2046 6572 7265 7420 5465 7374  .  - Ferret Test
+00002ec0: 2028 6665 7272 6574 5f74 6573 7429 0a2d   (ferret_test).-
+00002ed0: 2047 5141 2028 6771 6129 0a2d 2048 616c   GQA (gqa).- Hal
+00002ee0: 6c75 7369 6f6e 4265 6e63 686d 6172 6b20  lusionBenchmark 
+00002ef0: 2868 616c 6c75 7369 6f6e 5f62 656e 6368  (hallusion_bench
+00002f00: 5f69 6d61 6765 290a 2d20 496e 666f 6772  _image).- Infogr
+00002f10: 6170 6869 6320 5651 4120 2869 6e66 6f5f  aphic VQA (info_
+00002f20: 7671 6129 0a20 202d 2049 6e66 6f67 7261  vqa).  - Infogra
+00002f30: 7068 6963 2056 5141 2056 616c 6964 6174  phic VQA Validat
+00002f40: 696f 6e20 2869 6e66 6f5f 7671 615f 7661  ion (info_vqa_va
+00002f50: 6c29 0a20 202d 2049 6e66 6f67 7261 7068  l).  - Infograph
+00002f60: 6963 2056 5141 2054 6573 7420 2869 6e66  ic VQA Test (inf
+00002f70: 6f5f 7671 615f 7465 7374 290a 2d20 4c4c  o_vqa_test).- LL
+00002f80: 6156 412d 4265 6e63 6820 286c 6c61 7661  aVA-Bench (llava
+00002f90: 5f69 6e5f 7468 655f 7769 6c64 290a 2d20  _in_the_wild).- 
+00002fa0: 4c4c 6156 412d 4265 6e63 682d 434f 434f  LLaVA-Bench-COCO
+00002fb0: 2028 6c6c 6176 615f 6265 6e63 685f 636f   (llava_bench_co
+00002fc0: 636f 290a 2d20 4d61 7468 5669 7374 6120  co).- MathVista 
+00002fd0: 286d 6174 6876 6973 7461 290a 2020 2d20  (mathvista).  - 
+00002fe0: 4d61 7468 5669 7374 6120 5661 6c69 6461  MathVista Valida
+00002ff0: 7469 6f6e 2028 6d61 7468 7669 7374 615f  tion (mathvista_
+00003000: 7465 7374 6d69 6e69 290a 2020 2d20 4d61  testmini).  - Ma
+00003010: 7468 5669 7374 6120 5465 7374 2028 6d61  thVista Test (ma
+00003020: 7468 7669 7374 615f 7465 7374 290a 2d20  thvista_test).- 
+00003030: 4d4d 4265 6e63 6820 286d 6d62 656e 6368  MMBench (mmbench
+00003040: 290a 2020 2d20 4d4d 4265 6e63 6820 456e  ).  - MMBench En
+00003050: 676c 6973 6820 286d 6d62 656e 6368 5f65  glish (mmbench_e
+00003060: 6e29 0a20 2020 202d 204d 4d42 656e 6368  n).    - MMBench
+00003070: 2045 6e67 6c69 7368 2044 6576 2028 6d6d   English Dev (mm
+00003080: 6265 6e63 685f 656e 5f64 6576 290a 2020  bench_en_dev).  
+00003090: 2020 2d20 4d4d 4265 6e63 6820 456e 676c    - MMBench Engl
+000030a0: 6973 6820 5465 7374 2028 6d6d 6265 6e63  ish Test (mmbenc
+000030b0: 685f 656e 5f74 6573 7429 0a20 202d 204d  h_en_test).  - M
+000030c0: 4d42 656e 6368 2043 6869 6e65 7365 2028  MBench Chinese (
+000030d0: 6d6d 6265 6e63 685f 636e 290a 2020 2020  mmbench_cn).    
+000030e0: 2d20 4d4d 4265 6e63 6820 4368 696e 6573  - MMBench Chines
+000030f0: 6520 4465 7620 286d 6d62 656e 6368 5f63  e Dev (mmbench_c
+00003100: 6e5f 6465 7629 0a20 2020 202d 204d 4d42  n_dev).    - MMB
+00003110: 656e 6368 2043 6869 6e65 7365 2054 6573  ench Chinese Tes
+00003120: 7420 286d 6d62 656e 6368 5f63 6e5f 7465  t (mmbench_cn_te
+00003130: 7374 290a 2d20 4d4d 4520 286d 6d65 290a  st).- MME (mme).
+00003140: 2d20 4d4d 4d55 2028 6d6d 6d75 290a 2020  - MMMU (mmmu).  
+00003150: 2d20 4d4d 4d55 2056 616c 6964 6174 696f  - MMMU Validatio
+00003160: 6e20 286d 6d6d 755f 7661 6c29 0a20 202d  n (mmmu_val).  -
+00003170: 204d 4d4d 5520 5465 7374 2028 6d6d 6d75   MMMU Test (mmmu
+00003180: 5f74 6573 7429 0a2d 204d 4d56 6574 2028  _test).- MMVet (
+00003190: 6d6d 7665 7429 0a2d 204d 756c 7469 2d44  mmvet).- Multi-D
+000031a0: 6f63 5651 4120 286d 756c 7469 646f 6376  ocVQA (multidocv
+000031b0: 7161 290a 2020 2d20 4d75 6c74 692d 446f  qa).  - Multi-Do
+000031c0: 6356 5141 2056 616c 6964 6174 696f 6e20  cVQA Validation 
+000031d0: 286d 756c 7469 646f 6376 7161 5f76 616c  (multidocvqa_val
+000031e0: 290a 2020 2d20 4d75 6c74 692d 446f 6356  ).  - Multi-DocV
+000031f0: 5141 2054 6573 7420 286d 756c 7469 646f  QA Test (multido
+00003200: 6376 7161 5f74 6573 7429 0a2d 204e 6f43  cvqa_test).- NoC
+00003210: 6170 7320 286e 6f63 6170 7329 0a20 202d  aps (nocaps).  -
+00003220: 204e 6f43 6170 7320 5661 6c69 6461 7469   NoCaps Validati
+00003230: 6f6e 2028 6e6f 6361 7073 5f76 616c 290a  on (nocaps_val).
+00003240: 2020 2d20 4e6f 4361 7073 2054 6573 7420    - NoCaps Test 
+00003250: 286e 6f63 6170 735f 7465 7374 290a 2d20  (nocaps_test).- 
+00003260: 4f4b 5651 4120 286f 6b5f 7671 6129 0a20  OKVQA (ok_vqa). 
+00003270: 202d 204f 4b56 5141 2056 616c 6964 6174   - OKVQA Validat
+00003280: 696f 6e20 3230 3134 2028 6f6b 5f76 7161  ion 2014 (ok_vqa
+00003290: 5f76 616c 3230 3134 290a 2d20 504f 5045  _val2014).- POPE
+000032a0: 2028 706f 7065 290a 2d20 5265 6643 4f43   (pope).- RefCOC
+000032b0: 4f20 2872 6566 636f 636f 290a 2020 2020  O (refcoco).    
+000032c0: 2d20 7265 6663 6f63 6f5f 7365 675f 7465  - refcoco_seg_te
+000032d0: 7374 0a20 2020 202d 2072 6566 636f 636f  st.    - refcoco
+000032e0: 5f73 6567 5f76 616c 0a20 2020 202d 2072  _seg_val.    - r
+000032f0: 6566 636f 636f 5f73 6567 5f74 6573 7441  efcoco_seg_testA
+00003300: 0a20 2020 202d 2072 6566 636f 636f 5f73  .    - refcoco_s
+00003310: 6567 5f74 6573 7442 0a20 2020 202d 2072  eg_testB.    - r
+00003320: 6566 636f 636f 5f62 626f 785f 7465 7374  efcoco_bbox_test
+00003330: 0a20 2020 202d 2072 6566 636f 636f 5f62  .    - refcoco_b
+00003340: 626f 785f 7661 6c0a 2020 2020 2d20 7265  box_val.    - re
+00003350: 6663 6f63 6f5f 6262 6f78 5f74 6573 7441  fcoco_bbox_testA
+00003360: 0a20 2020 202d 2072 6566 636f 636f 5f62  .    - refcoco_b
+00003370: 626f 785f 7465 7374 420a 2d20 5265 6643  box_testB.- RefC
+00003380: 4f43 4f2b 2028 7265 6663 6f63 6f2b 290a  OCO+ (refcoco+).
+00003390: 2020 2020 2d20 7265 6663 6f63 6f2b 5f73      - refcoco+_s
+000033a0: 6567 0a20 2020 2020 2020 202d 2072 6566  eg.        - ref
+000033b0: 636f 636f 2b5f 7365 675f 7661 6c0a 2020  coco+_seg_val.  
+000033c0: 2020 2020 2020 2d20 7265 6663 6f63 6f2b        - refcoco+
+000033d0: 5f73 6567 5f74 6573 7441 0a20 2020 2020  _seg_testA.     
+000033e0: 2020 202d 2072 6566 636f 636f 2b5f 7365     - refcoco+_se
+000033f0: 675f 7465 7374 420a 2020 2020 2d20 7265  g_testB.    - re
+00003400: 6663 6f63 6f2b 5f62 626f 780a 2020 2020  fcoco+_bbox.    
+00003410: 2020 2020 2d20 7265 6663 6f63 6f2b 5f62      - refcoco+_b
+00003420: 626f 785f 7661 6c0a 2020 2020 2020 2020  box_val.        
+00003430: 2d20 7265 6663 6f63 6f2b 5f62 626f 785f  - refcoco+_bbox_
+00003440: 7465 7374 410a 2020 2020 2020 2020 2d20  testA.        - 
+00003450: 7265 6663 6f63 6f2b 5f62 626f 785f 7465  refcoco+_bbox_te
+00003460: 7374 420a 2d20 5265 6643 4f43 4f67 2028  stB.- RefCOCOg (
+00003470: 7265 6663 6f63 6f67 290a 2020 2020 2d20  refcocog).    - 
+00003480: 7265 6663 6f63 6f67 5f73 6567 5f74 6573  refcocog_seg_tes
+00003490: 740a 2020 2020 2d20 7265 6663 6f63 6f67  t.    - refcocog
+000034a0: 5f73 6567 5f76 616c 0a20 2020 202d 2072  _seg_val.    - r
+000034b0: 6566 636f 636f 675f 6262 6f78 5f74 6573  efcocog_bbox_tes
+000034c0: 740a 2020 2020 2d20 7265 6663 6f63 6f67  t.    - refcocog
+000034d0: 5f62 626f 785f 7661 6c0a 2d20 5363 6965  _bbox_val.- Scie
+000034e0: 6e63 6551 4120 2873 6369 656e 6365 7161  nceQA (scienceqa
+000034f0: 5f66 756c 6c29 0a20 202d 2053 6369 656e  _full).  - Scien
+00003500: 6365 5141 2046 756c 6c20 2873 6369 656e  ceQA Full (scien
+00003510: 6365 7161 290a 2020 2d20 5363 6965 6e63  ceqa).  - Scienc
+00003520: 6551 4120 494d 4720 2873 6369 656e 6365  eQA IMG (science
+00003530: 7161 5f69 6d67 290a 2d20 5365 6564 4265  qa_img).- SeedBe
+00003540: 6e63 6820 2873 6565 6462 656e 6368 290a  nch (seedbench).
+00003550: 2d20 5365 6564 4265 6e63 6820 3220 2873  - SeedBench 2 (s
+00003560: 6565 6462 656e 6368 5f32 290a 2d20 5354  eedbench_2).- ST
+00003570: 2d56 5141 2028 7374 7671 6129 0a2d 2054  -VQA (stvqa).- T
+00003580: 6578 7443 6170 7320 2874 6578 7463 6170  extCaps (textcap
+00003590: 7329 0a20 202d 2054 6578 7443 6170 7320  s).  - TextCaps 
+000035a0: 5661 6c69 6461 7469 6f6e 2028 7465 7874  Validation (text
+000035b0: 6361 7073 5f76 616c 290a 2020 2d20 5465  caps_val).  - Te
+000035c0: 7874 4361 7073 2054 6573 7420 2874 6578  xtCaps Test (tex
+000035d0: 7463 6170 735f 7465 7374 290a 2d20 5465  tcaps_test).- Te
+000035e0: 7874 5651 4120 2874 6578 7476 7161 290a  xtVQA (textvqa).
+000035f0: 2020 2d20 5465 7874 5651 4120 5661 6c69    - TextVQA Vali
+00003600: 6461 7469 6f6e 2028 7465 7874 7671 615f  dation (textvqa_
+00003610: 7661 6c29 0a20 202d 2054 6578 7456 5141  val).  - TextVQA
+00003620: 2054 6573 7420 2874 6578 7476 7161 5f74   Test (textvqa_t
+00003630: 6573 7429 0a2d 2056 697a 5769 7a56 5141  est).- VizWizVQA
+00003640: 2028 7669 7a77 697a 5f76 7161 290a 2020   (vizwiz_vqa).  
+00003650: 2d20 5669 7a57 697a 5651 4120 5661 6c69  - VizWizVQA Vali
+00003660: 6461 7469 6f6e 2028 7669 7a77 697a 5f76  dation (vizwiz_v
+00003670: 7161 5f76 616c 290a 2020 2d20 5669 7a57  qa_val).  - VizW
+00003680: 697a 5651 4120 5465 7374 2028 7669 7a77  izVQA Test (vizw
+00003690: 697a 5f76 7161 5f74 6573 7429 0a2d 2056  iz_vqa_test).- V
+000036a0: 5141 7632 2028 7671 6176 3229 0a20 202d  QAv2 (vqav2).  -
+000036b0: 2056 5141 7632 2056 616c 6964 6174 696f   VQAv2 Validatio
+000036c0: 6e20 2876 7161 7632 5f76 616c 290a 2020  n (vqav2_val).  
+000036d0: 2d20 5651 4176 3220 5465 7374 2028 7671  - VQAv2 Test (vq
+000036e0: 6176 325f 7465 7374 290a 0a23 2320 4461  av2_test)..## Da
+000036f0: 7461 7365 7473 2074 6f20 6265 2061 6464  tasets to be add
+00003700: 6564 2061 6e64 2074 6573 7465 640a 2d20  ed and tested.- 
+00003710: 5461 6c6c 7951 4120 2874 616c 6c79 7161  TallyQA (tallyqa
+00003720: 290a 2d20 5653 5220 2876 7372 290a 2d20  ).- VSR (vsr).- 
+00003730: 5769 6e6f 6772 6f75 6e64 2028 7769 6e6f  Winoground (wino
+00003740: 6772 6f75 6e64 290a 2d20 4e4c 5652 3220  ground).- NLVR2 
+00003750: 286e 6c76 7232 290a 2d20 5261 7665 6e49  (nlvr2).- RavenI
+00003760: 512d 5465 7374 2028 7261 7665 6e69 7129  Q-Test (raveniq)
+00003770: 0a2d 2049 636f 6e51 4120 2869 636f 6e71  .- IconQA (iconq
+00003780: 6129 0a2d 2056 6973 7442 656e 6368 2028  a).- VistBench (
+00003790: 7669 7374 6265 6e63 6829 0a0a 2320 4164  vistbench)..# Ad
+000037a0: 6420 4375 7374 6f6d 697a 6564 204d 6f64  d Customized Mod
+000037b0: 656c 2061 6e64 2044 6174 6173 6574 0a0a  el and Dataset..
+000037c0: 506c 6561 7365 2072 6566 6572 2074 6f20  Please refer to 
+000037d0: 6f75 7220 5b64 6f63 756d 656e 7461 7469  our [documentati
+000037e0: 6f6e 5d28 646f 6373 2f52 4541 444d 452e  on](docs/README.
+000037f0: 6d64 292e 0a0a 2320 4163 6b6e 6f77 6c65  md)...# Acknowle
+00003800: 6467 656d 656e 740a 0a6c 6d6d 735f 6576  dgement..lmms_ev
+00003810: 616c 2069 7320 6120 666f 726b 206f 6620  al is a fork of 
+00003820: 5b6c 6d2d 6576 616c 2d68 6172 6e65 7373  [lm-eval-harness
+00003830: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00003840: 2e63 6f6d 2f45 6c65 7574 6865 7241 492f  .com/EleutherAI/
+00003850: 6c6d 2d65 7661 6c75 6174 696f 6e2d 6861  lm-evaluation-ha
+00003860: 726e 6573 7329 2e20 5765 2072 6563 6f6d  rness). We recom
+00003870: 6d65 6e64 2079 6f75 2074 6f20 7265 6164  mend you to read
+00003880: 2074 6872 6f75 6768 2074 6865 205b 646f   through the [do
+00003890: 6373 206f 6620 6c6d 2d65 7661 6c2d 6861  cs of lm-eval-ha
+000038a0: 726e 6573 735d 2868 7474 7073 3a2f 2f67  rness](https://g
+000038b0: 6974 6875 622e 636f 6d2f 456c 6575 7468  ithub.com/Eleuth
+000038c0: 6572 4149 2f6c 6d2d 6576 616c 7561 7469  erAI/lm-evaluati
+000038d0: 6f6e 2d68 6172 6e65 7373 2f74 7265 652f  on-harness/tree/
+000038e0: 6d61 696e 2f64 6f63 7329 2066 6f72 2072  main/docs) for r
+000038f0: 656c 6576 616e 7420 696e 666f 726d 6174  elevant informat
+00003900: 696f 6e2e 200a 0a42 656c 6f77 2061 7265  ion. ..Below are
+00003910: 2074 6865 2063 6861 6e67 6573 2077 6520   the changes we 
+00003920: 6d61 6465 2074 6f20 7468 6520 6f72 6967  made to the orig
+00003930: 696e 616c 2041 5049 3a0a 2d20 4275 696c  inal API:.- Buil
+00003940: 6420 636f 6e74 6578 7420 6e6f 7720 6f6e  d context now on
+00003950: 6c79 2070 6173 7320 696e 2069 6478 2061  ly pass in idx a
+00003960: 6e64 2070 726f 6365 7373 2069 6d61 6765  nd process image
+00003970: 2061 6e64 2064 6f63 2064 7572 696e 6720   and doc during 
+00003980: 7468 6520 6d6f 6465 6c20 7265 7370 6f6e  the model respon
+00003990: 6469 6e67 2070 6861 7365 2e20 5468 6973  ding phase. This
+000039a0: 2069 7320 6475 6520 746f 2074 6865 2066   is due to the f
+000039b0: 6163 7420 7468 6174 2064 6174 6173 6574  act that dataset
+000039c0: 206e 6f77 2063 6f6e 7461 696e 7320 6c6f   now contains lo
+000039d0: 7473 206f 6620 696d 6167 6573 2061 6e64  ts of images and
+000039e0: 2077 6520 6361 6e27 7420 7374 6f72 6520   we can't store 
+000039f0: 7468 656d 2069 6e20 7468 6520 646f 6320  them in the doc 
+00003a00: 6c69 6b65 2074 6865 206f 7269 6769 6e61  like the origina
+00003a10: 6c20 6c6d 2d65 7661 6c2d 6861 726e 6573  l lm-eval-harnes
+00003a20: 7320 6f74 6865 7220 7769 7365 2074 6865  s other wise the
+00003a30: 2063 7075 206d 656d 6f72 7920 776f 756c   cpu memory woul
+00003a40: 6420 6578 706c 6f64 652e 0a2d 2049 6e73  d explode..- Ins
+00003a50: 7461 6e63 652e 6172 6773 2028 6c6d 6d73  tance.args (lmms
+00003a60: 5f65 7661 6c2f 6170 692f 696e 7374 616e  _eval/api/instan
+00003a70: 6365 2e70 7929 206e 6f77 2063 6f6e 7461  ce.py) now conta
+00003a80: 696e 7320 6120 6c69 7374 206f 6620 696d  ins a list of im
+00003a90: 6167 6573 2074 6f20 6265 2069 6e70 7574  ages to be input
+00003aa0: 7465 6420 746f 206c 6d6d 732e 0a2d 206c  ted to lmms..- l
+00003ab0: 6d2d 6576 616c 2d68 6172 6e65 7373 2073  m-eval-harness s
+00003ac0: 7570 706f 7274 7320 616c 6c20 4846 206c  upports all HF l
+00003ad0: 616e 6775 6167 6520 6d6f 6465 6c73 2061  anguage models a
+00003ae0: 7320 7369 6e67 6c65 206d 6f64 656c 2063  s single model c
+00003af0: 6c61 7373 2e20 4375 7272 656e 746c 7920  lass. Currently 
+00003b00: 7468 6973 2069 7320 6e6f 7420 706f 7373  this is not poss
+00003b10: 6962 6c65 206f 6620 6c6d 6d73 2062 6563  ible of lmms bec
+00003b20: 6175 7365 2074 6865 2069 6e70 7574 2f6f  ause the input/o
+00003b30: 7574 7075 7420 666f 726d 6174 206f 6620  utput format of 
+00003b40: 6c6d 6d73 2069 6e20 4846 2061 7265 206e  lmms in HF are n
+00003b50: 6f74 2079 6574 2075 6e69 6669 6564 2e20  ot yet unified. 
+00003b60: 5468 6572 6572 666f 7265 2c20 7765 2068  Thererfore, we h
+00003b70: 6176 6520 746f 2063 7265 6174 6520 6120  ave to create a 
+00003b80: 6e65 7720 636c 6173 7320 666f 7220 6561  new class for ea
+00003b90: 6368 206c 6d6d 7320 6d6f 6465 6c2e 2054  ch lmms model. T
+00003ba0: 6869 7320 6973 206e 6f74 2069 6465 616c  his is not ideal
+00003bb0: 2061 6e64 2077 6520 7769 6c6c 2074 7279   and we will try
+00003bc0: 2074 6f20 756e 6966 7920 7468 656d 2069   to unify them i
+00003bd0: 6e20 7468 6520 6675 7475 7265 2e0a 0a57  n the future...W
+00003be0: 6520 616c 736f 2074 6861 6e6b 3a0a 2d20  e also thank:.- 
+00003bf0: 5b58 6961 6e67 2059 7565 5d28 6874 7470  [Xiang Yue](http
+00003c00: 733a 2f2f 7869 616e 6779 7565 3936 3037  s://xiangyue9607
+00003c10: 2e67 6974 6875 622e 696f 2f29 2c20 5b4a  .github.io/), [J
+00003c20: 696e 676b 616e 6720 5961 6e67 5d28 6874  ingkang Yang](ht
+00003c30: 7470 733a 2f2f 6a69 6e67 6b61 6e67 3530  tps://jingkang50
+00003c40: 2e67 6974 6875 622e 696f 2f29 2c20 5b44  .github.io/), [D
+00003c50: 6f6e 6720 4775 6f5d 2868 7474 7073 3a2f  ong Guo](https:/
+00003c60: 2f77 7777 2e6c 696e 6b65 6469 6e2e 636f  /www.linkedin.co
+00003c70: 6d2f 696e 2f64 6f6e 6767 756f 7365 742f  m/in/dongguoset/
+00003c80: 2920 616e 6420 5b53 6865 6e67 2053 6865  ) and [Sheng She
+00003c90: 6e5d 2868 7474 7073 3a2f 2f73 696e 6365  n](https://since
+00003ca0: 7261 7373 2e67 6974 6875 622e 696f 2f29  rass.github.io/)
+00003cb0: 2066 6f72 2065 6172 6c79 2064 6973 6375   for early discu
+00003cc0: 7373 696f 6e20 616e 6420 7465 7374 696e  ssion and testin
+00003cd0: 672e 0a0a 2323 2043 6974 6174 696f 6e73  g...## Citations
+00003ce0: 0a0a 6060 6073 6865 6c6c 0a40 6d69 7363  ..```shell.@misc
+00003cf0: 7b6c 6d6d 735f 6576 616c 3230 3234 2c0a  {lmms_eval2024,.
+00003d00: 2020 2020 7469 746c 653d 7b4c 4d4d 732d      title={LMMs-
+00003d10: 4576 616c 3a20 4163 6365 6c65 7261 7469  Eval: Accelerati
+00003d20: 6e67 2074 6865 2044 6576 656c 6f70 6d65  ng the Developme
+00003d30: 6e74 206f 6620 4c61 7267 6520 4d75 6c74  nt of Large Mult
+00003d40: 696d 6f61 6c20 4d6f 6465 6c73 7d2c 0a20  imoal Models},. 
+00003d50: 2020 2075 726c 3d7b 6874 7470 733a 2f2f     url={https://
+00003d60: 6769 7468 7562 2e63 6f6d 2f45 766f 6c76  github.com/Evolv
+00003d70: 696e 674c 4d4d 732d 4c61 622f 6c6d 6d73  ingLMMs-Lab/lmms
+00003d80: 2d65 7661 6c7d 2c0a 2020 2020 6175 7468  -eval},.    auth
+00003d90: 6f72 3d7b 426f 204c 692a 2c20 5065 6979  or={Bo Li*, Peiy
+00003da0: 7561 6e20 5a68 616e 672a 2c20 4b61 6963  uan Zhang*, Kaic
+00003db0: 6865 6e20 5a68 616e 672a 2c20 4661 6e79  hen Zhang*, Fany
+00003dc0: 6920 5075 2a2c 2058 696e 7275 6e20 4475  i Pu*, Xinrun Du
+00003dd0: 2c20 5975 6861 6f20 446f 6e67 2c20 4861  , Yuhao Dong, Ha
+00003de0: 6f74 6961 6e20 4c69 752c 2059 7561 6e68  otian Liu, Yuanh
+00003df0: 616e 205a 6861 6e67 2c20 4765 205a 6861  an Zhang, Ge Zha
+00003e00: 6e67 2c20 4368 756e 7975 616e 204c 6920  ng, Chunyuan Li 
+00003e10: 616e 6420 5a69 7765 6920 4c69 757d 2c0a  and Ziwei Liu},.
+00003e20: 2020 2020 7075 626c 6973 6865 7220 2020      publisher   
+00003e30: 203d 207b 5a65 6e6f 646f 7d2c 0a20 2020   = {Zenodo},.   
+00003e40: 2076 6572 7369 6f6e 2020 2020 2020 3d20   version      = 
+00003e50: 7b76 302e 312e 307d 2c0a 2020 2020 6d6f  {v0.1.0},.    mo
+00003e60: 6e74 683d 7b4d 6172 6368 7d2c 0a20 2020  nth={March},.   
+00003e70: 2079 6561 723d 7b32 3032 347d 0a7d 0a60   year={2024}.}.`
+00003e80: 6060 0a                                  ``.
```

### Comparing `lmms_eval-0.1.1/docs/commands.md` & `lmms_eval-0.1.2/docs/commands.md`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/docs/model_guide.md` & `lmms_eval-0.1.2/docs/model_guide.md`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/docs/task_guide.md` & `lmms_eval-0.1.2/docs/task_guide.md`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/__main__.py` & `lmms_eval-0.1.2/lmms_eval/__main__.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/api/filter.py` & `lmms_eval-0.1.2/lmms_eval/api/filter.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/api/instance.py` & `lmms_eval-0.1.2/lmms_eval/api/instance.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/api/metrics.py` & `lmms_eval-0.1.2/lmms_eval/api/metrics.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/api/model.py` & `lmms_eval-0.1.2/lmms_eval/api/model.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/api/registry.py` & `lmms_eval-0.1.2/lmms_eval/api/registry.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/api/samplers.py` & `lmms_eval-0.1.2/lmms_eval/api/samplers.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/api/task.py` & `lmms_eval-0.1.2/lmms_eval/api/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -674,14 +674,30 @@
                     self._higher_is_better[metric_name] = metric_config["higher_is_better"]
                 else:
                     eval_logger.warning(f"[Task: {self._config.task}] metric {metric_name} is defined, but higher_is_better is not. " f"using default " f"higher_is_better={is_higher_better(metric_name)}")
                     self._higher_is_better[metric_name] = is_higher_better(metric_name)
 
     @retry(stop=stop_after_attempt(5), wait=wait_fixed(2))
     def download(self, dataset_kwargs=None) -> None:
+        # If the dataset is a video dataset,
+        # Recursively search whether their is a zip and unzip it to the huggingface home
+        if dataset_kwargs is not None and "video" in dataset_kwargs and dataset_kwargs["video"]:
+            hf_home = os.environ["HF_HOME"]
+            cache_dir = dataset_kwargs["cache_dir"]
+            dataset_kwargs.pop("cache_dir")
+            cache_dir = os.path.join(hf_home, cache_dir)
+            cache_path = snapshot_download(repo_id=self.DATASET_PATH, repo_type="dataset")
+            zip_files = glob(os.path.join(cache_path, "**/*.zip"), recursive=True)
+            if not os.path.exists(cache_dir):
+                for zip_file in zip_files:
+                    shutil.unpack_archive(zip_file, cache_dir)
+            builder_script = dataset_kwargs["builder_script"]
+            self.DATASET_PATH = os.path.join(cache_path, builder_script)
+            dataset_kwargs.pop("video")
+            dataset_kwargs.pop("builder_script")
         download_config = DownloadConfig()
         download_config.max_retries = dataset_kwargs.get("max_retries", 3) if dataset_kwargs is not None else 3
         download_config.num_proc = dataset_kwargs.get("num_proc", 8) if dataset_kwargs is not None else 8
         self.dataset = datasets.load_dataset(
             path=self.DATASET_PATH,
             name=self.DATASET_NAME,
             download_mode=datasets.DownloadMode.REUSE_DATASET_IF_EXISTS,
@@ -969,14 +985,16 @@
             return request_list
 
         elif self.OUTPUT_TYPE == "generate_until":
             arguments = (ctx, self.config.generation_kwargs, self.doc_to_visual, doc_id, self.config.task, split)
         return Instance(request_type=self.OUTPUT_TYPE, arguments=arguments, idx=0, **kwargs)
 
     def process_results(self, doc, results):
+        if self.OUTPUT_TYPE == "generate_until":
+            results[0] = results[0].strip()
         if callable(self.config.process_results):
             return self.config.process_results(doc, results)
 
         result_dict = {}
         use_metric = list(self._metric_fn_list.keys())
         if self.OUTPUT_TYPE == "loglikelihood":
             results = results[0]
```

### Comparing `lmms_eval-0.1.1/lmms_eval/evaluator.py` & `lmms_eval-0.1.2/lmms_eval/evaluator.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/filters/__init__.py` & `lmms_eval-0.1.2/lmms_eval/filters/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-from lmms_eval.api.filter import FilterEnsemble
+from lmms_eval.api.filter import FilterEnsemble, Filter
 from . import selection
 from . import extraction
 from . import transformation
 
 
 FILTER_REGISTRY = {
     "take_first": selection.TakeFirstFilter,
     "regex": extraction.RegexFilter,
     "majority_vote": selection.MajorityVoteFilter,
     "take_first_k": selection.TakeKFilter,
     "remove_whitespace": extraction.WhitespaceFilter,
     "lowercase": transformation.LowercaseFilter,
     "uppercase": transformation.UppercaseFilter,
     "map": transformation.MapFilter,
+    "multi_choice_regex": extraction.MultiChoiceRegexFilter,
     # TODO: implement this filter. either it should take in an arbitrary "scoring"/reward function
     # that takes an input and returns a scalar and then should select the max reward,
     # or should implement different filters for different ways of handling a reward model's inference.
     # "arg_max": selection.ArgMaxFilter,
 }
```

### Comparing `lmms_eval-0.1.1/lmms_eval/filters/decontamination.py` & `lmms_eval-0.1.2/lmms_eval/filters/decontamination.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/filters/selection.py` & `lmms_eval-0.1.2/lmms_eval/filters/selection.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/filters/transformation.py` & `lmms_eval-0.1.2/lmms_eval/filters/transformation.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/logging_utils.py` & `lmms_eval-0.1.2/lmms_eval/logging_utils.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/models/fuyu.py` & `lmms_eval-0.1.2/lmms_eval/models/fuyu.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/models/gpt4v.py` & `lmms_eval-0.1.2/lmms_eval/models/gpt4v.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,27 +31,32 @@
     API_KEY = os.getenv("AZURE_API_KEY", "YOUR_API_KEY")
     headers = {
         "api-key": API_KEY,
         "Content-Type": "application/json",
     }
 
 
-@register_model("gpt4V")
+@register_model("gpt4v")
 class GPT4V(lmms):
-    def __init__(self, **kwargs) -> None:
+    def __init__(
+        self,
+        model_version: str = "gpt-4-vision-preview",
+        **kwargs,
+    ) -> None:
         super().__init__()
         # Manually set a image token for GPT4V so that we can search for it
         # and split the text and image
         # Here we just use the same token as llava for convenient
+        self.model_version = model_version
         self.image_token = "<image>"
 
     # Function to encode the image
     def encode_image(self, image: Image):
         output_buffer = BytesIO()
-        image.save(output_buffer, format="JPEG")
+        image.save(output_buffer, format="PNG")
         byte_data = output_buffer.getvalue()
         base64_str = base64.b64encode(byte_data).decode("utf-8")
         return base64_str
 
     def flatten(self, input):
         new_list = []
         for i in input:
@@ -68,15 +73,15 @@
             visuals = [doc_to_visual(self.task_dict[task][split][doc_id])]
             visuals = self.flatten(visuals)
             imgs = []
             for visual in visuals:
                 img = self.encode_image(visual)
                 imgs.append(img)
 
-            payload = {"model": "gpt-4-vision-preview", "messages": []}
+            payload = {"model": self.model_version, "messages": []}
             response_json = {"role": "user", "content": []}
             # When there is no image token in the context, append the image to the text
             if self.image_token not in contexts:
                 payload["messages"].append(deepcopy(response_json))
                 payload["messages"][0]["content"].append({"type": "text", "text": contexts})
                 for img in imgs:
                     payload["messages"][0]["content"].append({"type": "image_url", "image_url": {"url": f"data:image/jpeg;base64,{img}"}})
```

### Comparing `lmms_eval-0.1.1/lmms_eval/models/instructblip.py` & `lmms_eval-0.1.2/lmms_eval/models/instructblip.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/models/llava.py` & `lmms_eval-0.1.2/lmms_eval/models/llava.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,19 @@
 
 from transformers.integrations.deepspeed import (
     is_deepspeed_zero3_enabled,
     set_hf_deepspeed_config,
     unset_hf_deepspeed_config,
 )
 
+if torch.__version__ > "2.1.2":
+    best_fit_attn_implementation = "sdpa"
+else:
+    best_fit_attn_implementation = "eager"
+
 
 @register_model("llava")
 class Llava(lmms):
     """
     Llava Model
     """
 
@@ -48,19 +53,21 @@
         pretrained: str = "liuhaotian/llava-v1.5-7b",
         truncation: Optional[bool] = True,
         device: Optional[str] = "cuda",
         dtype: Optional[Union[str, torch.dtype]] = "auto",
         batch_size: Optional[Union[int, str]] = 1,
         trust_remote_code: Optional[bool] = False,
         revision=None,
+        attn_implementation=best_fit_attn_implementation,
         use_flash_attention_2=True,
-        device_map="",
+        device_map="auto",
         conv_template="vicuna_v1",
         use_cache=True,
         truncate_context=False,  # whether to truncate the context in generation, set it False for LLaVA-1.6
+        customized_config=None,
         **kwargs,
     ) -> None:
         super().__init__()
         # Do not use kwargs for now
         assert kwargs == {}, f"Unexpected kwargs: {kwargs}"
 
         accelerator_kwargs = InitProcessGroupKwargs(timeout=timedelta(weeks=52))
@@ -68,15 +75,20 @@
         if accelerator.num_processes > 1 and device_map == "":
             self._device = torch.device(f"cuda:{accelerator.local_process_index}")
             self.device_map = f"cuda:{accelerator.local_process_index}"
         else:
             self._device = torch.device(device)
             self.device_map = device_map
 
-        self._tokenizer, self._model, self._image_processor, self._max_length = load_pretrained_model(pretrained, None, get_model_name_from_path(pretrained), device_map=self.device_map, use_flash_attention_2=use_flash_attention_2)
+        llava_model_args = {}
+        llava_model_args["attn_implementation"] = attn_implementation
+        if customized_config:
+            llava_model_args["customized_config"] = customized_config
+        llava_model_args["use_flash_attention_2"] = False
+        self._tokenizer, self._model, self._image_processor, self._max_length = load_pretrained_model(pretrained, None, get_model_name_from_path(pretrained), device_map=self.device_map, **llava_model_args)
         self._config = self._model.config
         self.model.eval()
         self.model.tie_weights()
         self.truncation = truncation
         self.batch_size_per_gpu = int(batch_size)
         self.conv_template = conv_template
         self.use_cache = use_cache
@@ -194,26 +206,26 @@
                 if type(image) is list:
                     image = [_image.to(dtype=torch.float16, device=self.device) for _image in image]
                 else:
                     image = image.to(dtype=torch.float16, device=self.device)
             else:
                 image = None
 
-            prompts_input = contexts[0]
+            prompts_input = contexts[0] if isinstance(contexts, list) else contexts
 
             if image is not None and len(image) != 0 and DEFAULT_IMAGE_TOKEN not in prompts_input:
                 """
                 Three senarios:
                 1. No image, and there for, no image token should be added.
                 2. image token is already specified in the context, so we don't need to add it.
                 3. image token is not specified in the context and there is image inputs, so we need to add it. In this case, we add the image token at the beginning of the context and add a new line.
                 """
                 image_tokens = [DEFAULT_IMAGE_TOKEN] * len(visuals)
                 image_tokens = " ".join(image_tokens)
-                prompts_input = image_tokens + "\n" + contexts[0]
+                prompts_input = image_tokens + "\n" + (contexts[0] if isinstance(contexts, list) else contexts)
 
             conv = conv_templates[self.conv_template].copy()
             conv.append_message(conv.roles[0], prompts_input)
             conv.append_message(conv.roles[1], None)
             prompt = conv.get_prompt()
             pad_token_id = self.tokenizer.pad_token_id if self.tokenizer.pad_token_id is not None else self.tokenizer.eos_token_id
             contxt_id = tokenizer_image_token(prompt, self.tokenizer, IMAGE_TOKEN_INDEX, return_tensors="pt").unsqueeze(0).to(self.device)
```

### Comparing `lmms_eval-0.1.1/lmms_eval/models/minicpm_v.py` & `lmms_eval-0.1.2/lmms_eval/models/minicpm_v.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/models/model_utils/qwen/qwen_generate_utils.py` & `lmms_eval-0.1.2/lmms_eval/models/model_utils/qwen/qwen_generate_utils.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/models/qwen_vl.py` & `lmms_eval-0.1.2/lmms_eval/models/qwen_vl.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/__init__.py` & `lmms_eval-0.1.2/lmms_eval/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/__pycache__/__init__.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/__pycache__/__init__.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0008eb65 (Fri Mar  8 12:43:44 2024 UTC)
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
 files sz: 5453
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/_task_utils/__pycache__/file_utils.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/_task_utils/__pycache__/file_utils.cpython-311.pyc`

 * *Files 16% similar despite different names*

#### Python bytecode

```diff
@@ -1,96 +1,98 @@
 magic:    0xa70d0d0a
-moddate:  0x0008eb65 (Fri Mar  8 12:43:44 2024 UTC)
-files sz: 227
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
+files sz: 244
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
-   code 0x9700640064016c005a00640284005a0164015300
+   code 0x9700640064016c005a006404640384015a0164015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (os)
                  8 STORE_NAME               0 (os)
    
-     4          10 LOAD_CONST               2 (<code object generate_submission_file, file "/data/pufanyi/project/lmms-eval/lmms_eval/tasks/_task_utils/file_utils.py", line 4>)
-                12 MAKE_FUNCTION            0
-                14 STORE_NAME               1 (generate_submission_file)
-                16 LOAD_CONST               1 (None)
-                18 RETURN_VALUE
+     4          10 LOAD_CONST               4 (('submissions',))
+                12 LOAD_CONST               3 (<code object generate_submission_file, file "/data/pufanyi/project/lmms-eval/lmms_eval/tasks/_task_utils/file_utils.py", line 4>)
+                14 MAKE_FUNCTION            1 (defaults)
+                16 STORE_NAME               1 (generate_submission_file)
+                18 LOAD_CONST               1 (None)
+                20 RETURN_VALUE
    consts
       0
       None
+      'submissions'
       code
-         argcount  : 2
-         nlocals   : 3
+         argcount  : 3
+         nlocals   : 4
          stacksize : 4
          flags     : 3
          code
             0x97007400000000000000000000006a010000000000000000a002000000
-            00000000000000000000000000000000007c016a03000000000000000064
-            01a6020000ab0200000000000000007d027401000000000000000000006a
-            0400000000000000007c026402ac03a6020000ab02000000000000000001
+            00000000000000000000000000000000007c016a0300000000000000007c
+            02a6020000ab0200000000000000007d037401000000000000000000006a
+            0400000000000000007c036401ac02a6020000ab02000000000000000001
             007400000000000000000000006a010000000000000000a0020000000000
-            0000000000000000000000000000007c027c00a6020000ab020000000000
-            0000007d027400000000000000000000006a010000000000000000a00500
-            000000000000000000000000000000000000007c02a6010000ab01000000
+            0000000000000000000000000000007c037c00a6020000ab020000000000
+            0000007d037400000000000000000000006a010000000000000000a00500
+            000000000000000000000000000000000000007c03a6010000ab01000000
             00000000005300
            4           0 RESUME                   0
          
            5           2 LOAD_GLOBAL              0 (os)
                       14 LOAD_ATTR                1 (path)
                       24 LOAD_METHOD              2 (join)
                       46 LOAD_FAST                1 (args)
                       48 LOAD_ATTR                3 (output_path)
-                      58 LOAD_CONST               1 ('submissions')
+                      58 LOAD_FAST                2 (subpath)
                       60 PRECALL                  2
                       64 CALL                     2
-                      74 STORE_FAST               2 (path)
+                      74 STORE_FAST               3 (path)
          
            6          76 LOAD_GLOBAL              1 (NULL + os)
                       88 LOAD_ATTR                4 (makedirs)
-                      98 LOAD_FAST                2 (path)
-                     100 LOAD_CONST               2 (True)
-                     102 KW_NAMES                 3
+                      98 LOAD_FAST                3 (path)
+                     100 LOAD_CONST               1 (True)
+                     102 KW_NAMES                 2
                      104 PRECALL                  2
                      108 CALL                     2
                      118 POP_TOP
          
            7         120 LOAD_GLOBAL              0 (os)
                      132 LOAD_ATTR                1 (path)
                      142 LOAD_METHOD              2 (join)
-                     164 LOAD_FAST                2 (path)
+                     164 LOAD_FAST                3 (path)
                      166 LOAD_FAST                0 (file_name)
                      168 PRECALL                  2
                      172 CALL                     2
-                     182 STORE_FAST               2 (path)
+                     182 STORE_FAST               3 (path)
          
            8         184 LOAD_GLOBAL              0 (os)
                      196 LOAD_ATTR                1 (path)
                      206 LOAD_METHOD              5 (abspath)
-                     228 LOAD_FAST                2 (path)
+                     228 LOAD_FAST                3 (path)
                      230 PRECALL                  1
                      234 CALL                     1
                      244 RETURN_VALUE
          consts
             None
-            'submissions'
             True
             ('exist_ok',)
          names      ('os', 'path', 'join', 'output_path', 'makedirs', 'abspath')
-         varnames   ('file_name', 'args', 'path')
+         varnames   ('file_name', 'args', 'subpath', 'path')
          freevars   ()
          cellvars   ()
          filename   '/data/pufanyi/project/lmms-eval/lmms_eval/tasks/_task_utils/file_utils.py'
          name       'generate_submission_file'
          firstlineno 4
          lnotab 0x02014a012c014001
+      ('submissions',)
    names      ('os', 'generate_submission_file')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/data/pufanyi/project/lmms-eval/lmms_eval/tasks/_task_utils/file_utils.py'
    name       '<module>'
    firstlineno 1
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/_task_utils/__pycache__/vqa_eval_metric.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/_task_utils/__pycache__/vqa_eval_metric.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0008eb65 (Fri Mar  8 12:43:44 2024 UTC)
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
 files sz: 6056
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/_task_utils/vqa_eval_metric.py` & `lmms_eval-0.1.2/lmms_eval/tasks/_task_utils/vqa_eval_metric.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/ai2d/__pycache__/utils.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/ai2d/__pycache__/utils.cpython-311.pyc`

 * *Files 8% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0008eb65 (Fri Mar  8 12:43:44 2024 UTC)
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
 files sz: 1271
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code 0x97006404640184015a00640284005a01640384005a0264005300
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/ai2d/ai2d.yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/ai2d/ai2d.yaml`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/ai2d/upload_ai2d.py` & `lmms_eval-0.1.2/lmms_eval/tasks/ai2d/upload_ai2d.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/ai2d/utils.py` & `lmms_eval-0.1.2/lmms_eval/tasks/ai2d/utils.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/chartqa/__pycache__/utils.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/chartqa/__pycache__/utils.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0008eb65 (Fri Mar  8 12:43:44 2024 UTC)
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
 files sz: 2378
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/chartqa/chartqa.yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/chartqa/chartqa.yaml`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/chartqa/upload_chartqa.py` & `lmms_eval-0.1.2/lmms_eval/tasks/chartqa/upload_chartqa.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/chartqa/utils.py` & `lmms_eval-0.1.2/lmms_eval/tasks/chartqa/utils.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/cmmmu/__pycache__/utils.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/cmmmu/__pycache__/utils.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x542beb65 (Fri Mar  8 15:14:28 2024 UTC)
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
 files sz: 17232
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/cmmmu/cmmmu_test.yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/cmmmu/cmmmu_test.yaml`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/cmmmu/cmmmu_val.yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/cmmmu/cmmmu_val.yaml`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/cmmmu/utils.py` & `lmms_eval-0.1.2/lmms_eval/tasks/cmmmu/utils.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/coco_cap/__pycache__/utils.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/coco_cap/__pycache__/utils.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0008eb65 (Fri Mar  8 12:43:44 2024 UTC)
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
 files sz: 5273
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/coco_cap/coco2014_cap_test.yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/coco_cap/coco2014_cap_test.yaml`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/coco_cap/coco2014_cap_val.yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/coco_cap/coco2014_cap_val.yaml`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/coco_cap/coco2017_cap_test.yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/coco_cap/coco2017_cap_test.yaml`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/coco_cap/coco2017_cap_val.yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/coco_cap/coco2017_cap_val.yaml`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/coco_cap/utils.py` & `lmms_eval-0.1.2/lmms_eval/tasks/coco_cap/utils.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/docvqa/__pycache__/utils.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/docvqa/__pycache__/utils.cpython-311.pyc`

 * *Files 12% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0008eb65 (Fri Mar  8 12:43:44 2024 UTC)
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
 files sz: 992
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 3
    flags     : 0
    code
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/docvqa/utils.py` & `lmms_eval-0.1.2/lmms_eval/tasks/docvqa/utils.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/ferret/__pycache__/utils.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/ferret/__pycache__/utils.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0008eb65 (Fri Mar  8 12:43:44 2024 UTC)
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
 files sz: 6956
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 11
    flags     : 0
    code
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/ferret/ferret.yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/ferret/ferret.yaml`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/ferret/rule.json` & `lmms_eval-0.1.2/lmms_eval/tasks/ferret/rule.json`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/ferret/utils.py` & `lmms_eval-0.1.2/lmms_eval/tasks/ferret/utils.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/flickr30k/__pycache__/utils.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/flickr30k/__pycache__/utils.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0008eb65 (Fri Mar  8 12:43:44 2024 UTC)
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
 files sz: 4545
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/flickr30k/flickr30k_test.yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/flickr30k/flickr30k_test.yaml`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/flickr30k/utils.py` & `lmms_eval-0.1.2/lmms_eval/tasks/flickr30k/utils.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/gqa/__pycache__/utils.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/gqa/__pycache__/utils.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0008eb65 (Fri Mar  8 12:43:44 2024 UTC)
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
 files sz: 781
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/gqa/gqa.yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/gqa/gqa.yaml`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/gqa/utils.py` & `lmms_eval-0.1.2/lmms_eval/tasks/gqa/utils.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/hallusion_bench/__pycache__/evaluate_hb.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/hallusion_bench/__pycache__/evaluate_hb.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0008eb65 (Fri Mar  8 12:43:44 2024 UTC)
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
 files sz: 4862
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/hallusion_bench/__pycache__/utils.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/hallusion_bench/__pycache__/utils.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0008eb65 (Fri Mar  8 12:43:44 2024 UTC)
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
 files sz: 12366
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/hallusion_bench/evaluate_hb.py` & `lmms_eval-0.1.2/lmms_eval/tasks/hallusion_bench/evaluate_hb.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/hallusion_bench/hallusion_bench_image.yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/hallusion_bench/hallusion_bench_image.yaml`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/hallusion_bench/utils.py` & `lmms_eval-0.1.2/lmms_eval/tasks/hallusion_bench/utils.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/iconqa/__pycache__/utils.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/iconqa/__pycache__/utils.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0008eb65 (Fri Mar  8 12:43:44 2024 UTC)
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
 files sz: 2162
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/iconqa/_default_template_docvqa_yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/iconqa/_default_template_docvqa_yaml`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/iconqa/utils.py` & `lmms_eval-0.1.2/lmms_eval/tasks/iconqa/utils.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/infovqa/__pycache__/utils.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/infovqa/__pycache__/utils.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0008eb65 (Fri Mar  8 12:43:44 2024 UTC)
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
 files sz: 951
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 3
    flags     : 0
    code
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/infovqa/utils.py` & `lmms_eval-0.1.2/lmms_eval/tasks/infovqa/utils.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/llava-bench-coco/__pycache__/utils.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/llava-bench-coco/__pycache__/utils.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0008eb65 (Fri Mar  8 12:43:44 2024 UTC)
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
 files sz: 6883
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 11
    flags     : 0
    code
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/llava-bench-coco/llava-bench-coco.yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/llava-bench-coco/llava-bench-coco.yaml`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/llava-bench-coco/rule.json` & `lmms_eval-0.1.2/lmms_eval/tasks/llava-bench-coco/rule.json`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/llava-bench-coco/utils.py` & `lmms_eval-0.1.2/lmms_eval/tasks/llava-bench-coco/utils.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/llava-in-the-wild/__pycache__/utils.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/llava-in-the-wild/__pycache__/utils.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0008eb65 (Fri Mar  8 12:43:44 2024 UTC)
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
 files sz: 6851
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 11
    flags     : 0
    code
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/llava-in-the-wild/llava-in-the-wild.yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/llava-in-the-wild/llava-in-the-wild.yaml`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/llava-in-the-wild/rule.json` & `lmms_eval-0.1.2/lmms_eval/tasks/llava-in-the-wild/rule.json`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/llava-in-the-wild/utils.py` & `lmms_eval-0.1.2/lmms_eval/tasks/llava-in-the-wild/utils.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/mathvista/__pycache__/mathvista_evals.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/mathvista/__pycache__/mathvista_evals.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0008eb65 (Fri Mar  8 12:43:44 2024 UTC)
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
 files sz: 18971
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/mathvista/__pycache__/utils.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/mathvista/__pycache__/utils.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0008eb65 (Fri Mar  8 12:43:44 2024 UTC)
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
 files sz: 5022
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/mathvista/mathvista_evals.py` & `lmms_eval-0.1.2/lmms_eval/tasks/mathvista/mathvista_evals.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/mathvista/mathvista_test.yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/mathvista/mathvista_test.yaml`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/mathvista/mathvista_testmini.yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/mathvista/mathvista_testmini.yaml`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/mathvista/utils.py` & `lmms_eval-0.1.2/lmms_eval/tasks/mathvista/utils.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/mmbench/__pycache__/cn_utils.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/mmbench/__pycache__/en_utils.cpython-311.pyc`

 * *Files 19% similar despite different names*

#### Python bytecode

```diff
@@ -1,33 +1,41 @@
 magic:    0xa70d0d0a
-moddate:  0x5ac3ef65 (Tue Mar 12 02:52:10 2024 UTC)
-files sz: 3081
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
+files sz: 4550
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
-      026c036d045a040100640064016c055a06640064016c075a07640064036c
-      086d095a090100020065006a0a00000000000000006404a6010000ab0100
-      000000000000005a0b640064056c0c6d0d5a0d01000200650e0200650465
+      026c036d045a040100640064016c055a06640064016c075a07020065006a
+      0800000000000000006403a6010000ab0100000000000000005a09640064
+      046c0a6d0b5a0b0100640064056c0c6d0d5a0d01000200650e0200650465
       0fa6010000ab0100000000000000006a10000000000000000064067a0b00
       006407a6020000ab02000000000000000035005a116511a0120000000000
       000000000000000000000000000000a6000000ab0000000000000000005a
       1367005a14020065156513a6010000ab01000000000000000044005d1e5c
       0200005a165a1764086517760172156514a0180000000000000000000000
       0000000000000000006517a6010000ab01000000000000000001008c1f02
       0065016a1900000000000000006409a01a00000000000000000000000000
       000000000000006514a6010000ab010000000000000000a6010000ab0100
       000000000000005a1b640164016401a6020000ab02000000000000000001
-      006e0b230031007304770278035900770101005900010001000200650d65
-      1b640a19000000000000000000640b19000000000000000000ac0ca60100
-      00ab0100000000000000005a1c640d84005a1d6412640e84015a1e640f84
-      005a1f641084005a20641184005a2164015300
+      006e0b23003100730477027803590077010100590001000100651b640a19
+      000000000000000000640b190000000000000000005a1c020065026a1d00
+      00000000000000640c640da6020000ab0200000000000000005a1e651e64
+      0d6b02000000007223020065026a1d0000000000000000640e640fa60200
+      00ab0200000000000000005a1f020065026a1d0000000000000000641064
+      11a6020000ab0200000000000000005a206e28651e64126b020000000072
+      22020065026a1d000000000000000064136414a6020000ab020000000000
+      0000005a1f020065026a1d000000000000000064156411a6020000ab0200
+      000000000000005a200200650b651b640a19000000000000000000641619
+      0000000000000000006520651f651cac17a6040000ab0400000000000000
+      005a21641884005a22641e641984015a23641a84005a24641b84005a2564
+      1c84005a26641d84005a2764015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (logging)
                  8 STORE_NAME               0 (logging)
    
@@ -54,45 +62,45 @@
                 44 STORE_NAME               6 (pd)
    
      6          46 LOAD_CONST               0 (0)
                 48 LOAD_CONST               1 (None)
                 50 IMPORT_NAME              7 (json)
                 52 STORE_NAME               7 (json)
    
-     7          54 LOAD_CONST               0 (0)
-                56 LOAD_CONST               3 (('generate_submission_file',))
-                58 IMPORT_NAME              8 (lmms_eval.tasks._task_utils.file_utils)
-                60 IMPORT_FROM              9 (generate_submission_file)
-                62 STORE_NAME               9 (generate_submission_file)
-                64 POP_TOP
-   
-     9          66 PUSH_NULL
-                68 LOAD_NAME                0 (logging)
-                70 LOAD_ATTR               10 (getLogger)
-                80 LOAD_CONST               4 ('lmms-eval')
-                82 PRECALL                  1
-                86 CALL                     1
-                96 STORE_NAME              11 (eval_logger)
+     8          54 PUSH_NULL
+                56 LOAD_NAME                0 (logging)
+                58 LOAD_ATTR                8 (getLogger)
+                68 LOAD_CONST               3 ('lmms-eval')
+                70 PRECALL                  1
+                74 CALL                     1
+                84 STORE_NAME               9 (eval_logger)
+   
+     9          86 LOAD_CONST               0 (0)
+                88 LOAD_CONST               4 (('MMBench_Evaluator',))
+                90 IMPORT_NAME             10 (lmms_eval.tasks.mmbench.mmbench_evals)
+                92 IMPORT_FROM             11 (MMBench_Evaluator)
+                94 STORE_NAME              11 (MMBench_Evaluator)
+                96 POP_TOP
    
     10          98 LOAD_CONST               0 (0)
-               100 LOAD_CONST               5 (('MMBench_Evaluator',))
-               102 IMPORT_NAME             12 (lmms_eval.tasks.mmbench.mmbench_evals)
-               104 IMPORT_FROM             13 (MMBench_Evaluator)
-               106 STORE_NAME              13 (MMBench_Evaluator)
+               100 LOAD_CONST               5 (('generate_submission_file',))
+               102 IMPORT_NAME             12 (lmms_eval.tasks._task_utils.file_utils)
+               104 IMPORT_FROM             13 (generate_submission_file)
+               106 STORE_NAME              13 (generate_submission_file)
                108 POP_TOP
    
     12         110 PUSH_NULL
                112 LOAD_NAME               14 (open)
                114 PUSH_NULL
                116 LOAD_NAME                4 (Path)
                118 LOAD_NAME               15 (__file__)
                120 PRECALL                  1
                124 CALL                     1
                134 LOAD_ATTR               16 (parent)
-               144 LOAD_CONST               6 ('mmbench_cn.yaml')
+               144 LOAD_CONST               6 ('mmbench.yaml')
                146 BINARY_OP               11 (/)
                150 LOAD_CONST               7 ('r')
                152 PRECALL                  2
                156 CALL                     2
                166 BEFORE_WITH
                168 STORE_NAME              17 (f)
    
@@ -156,77 +164,158 @@
                402 POP_EXCEPT
                404 RERAISE                  1
            >>  406 POP_TOP
                408 POP_EXCEPT
                410 POP_TOP
                412 POP_TOP
    
-    22     >>  414 PUSH_NULL
-               416 LOAD_NAME               13 (MMBench_Evaluator)
-               418 LOAD_NAME               27 (config)
-               420 LOAD_CONST              10 ('metadata')
-               422 BINARY_SUBSCR
-               432 LOAD_CONST              11 ('sys_prompt')
-               434 BINARY_SUBSCR
-               444 KW_NAMES                12
-               446 PRECALL                  1
-               450 CALL                     1
-               460 STORE_NAME              28 (mmbench_evaluator)
-   
-    25         462 LOAD_CONST              13 (<code object mmbench_doc_to_visual, file "/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/cn_utils.py", line 25>)
-               464 MAKE_FUNCTION            0
-               466 STORE_NAME              29 (mmbench_doc_to_visual)
-   
-    29         468 LOAD_CONST              18 ((None,))
-               470 LOAD_CONST              14 (<code object mmbench_doc_to_text, file "/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/cn_utils.py", line 29>)
-               472 MAKE_FUNCTION            1 (defaults)
-               474 STORE_NAME              30 (mmbench_doc_to_text)
-   
-    55         476 LOAD_CONST              15 (<code object mmbench_process_results, file "/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/cn_utils.py", line 55>)
-               478 MAKE_FUNCTION            0
-               480 STORE_NAME              31 (mmbench_process_results)
-   
-    76         482 LOAD_CONST              16 (<code object mmbench_aggregate_dev_results, file "/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/cn_utils.py", line 76>)
-               484 MAKE_FUNCTION            0
-               486 STORE_NAME              32 (mmbench_aggregate_dev_results)
-   
-    84         488 LOAD_CONST              17 (<code object mmbench_aggregate_test_results, file "/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/cn_utils.py", line 84>)
-               490 MAKE_FUNCTION            0
-               492 STORE_NAME              33 (mmbench_aggregate_test_results)
-               494 LOAD_CONST               1 (None)
-               496 RETURN_VALUE
+    22     >>  414 LOAD_NAME               27 (config)
+               416 LOAD_CONST              10 ('metadata')
+               418 BINARY_SUBSCR
+               428 LOAD_CONST              11 ('gpt_eval_model_name')
+               430 BINARY_SUBSCR
+               440 STORE_NAME              28 (GPT_EVAL_MODEL_NAME)
+   
+    23         442 PUSH_NULL
+               444 LOAD_NAME                2 (os)
+               446 LOAD_ATTR               29 (getenv)
+               456 LOAD_CONST              12 ('API_TYPE')
+               458 LOAD_CONST              13 ('openai')
+               460 PRECALL                  2
+               464 CALL                     2
+               474 STORE_NAME              30 (API_TYPE)
+   
+    25         476 LOAD_NAME               30 (API_TYPE)
+               478 LOAD_CONST              13 ('openai')
+               480 COMPARE_OP               2 (==)
+               486 POP_JUMP_FORWARD_IF_FALSE    35 (to 558)
+   
+    26         488 PUSH_NULL
+               490 LOAD_NAME                2 (os)
+               492 LOAD_ATTR               29 (getenv)
+               502 LOAD_CONST              14 ('OPENAI_API_URL')
+               504 LOAD_CONST              15 ('https://api.openai.com/v1/chat/completions')
+               506 PRECALL                  2
+               510 CALL                     2
+               520 STORE_NAME              31 (API_URL)
+   
+    27         522 PUSH_NULL
+               524 LOAD_NAME                2 (os)
+               526 LOAD_ATTR               29 (getenv)
+               536 LOAD_CONST              16 ('OPENAI_API_KEY')
+               538 LOAD_CONST              17 ('YOUR_API_KEY')
+               540 PRECALL                  2
+               544 CALL                     2
+               554 STORE_NAME              32 (API_KEY)
+               556 JUMP_FORWARD            40 (to 638)
+   
+    28     >>  558 LOAD_NAME               30 (API_TYPE)
+               560 LOAD_CONST              18 ('azure')
+               562 COMPARE_OP               2 (==)
+               568 POP_JUMP_FORWARD_IF_FALSE    34 (to 638)
+   
+    29         570 PUSH_NULL
+               572 LOAD_NAME                2 (os)
+               574 LOAD_ATTR               29 (getenv)
+               584 LOAD_CONST              19 ('AZURE_ENDPOINT')
+               586 LOAD_CONST              20 ('https://api.cognitive.microsoft.com/sts/v1.0/issueToken')
+               588 PRECALL                  2
+               592 CALL                     2
+               602 STORE_NAME              31 (API_URL)
+   
+    30         604 PUSH_NULL
+               606 LOAD_NAME                2 (os)
+               608 LOAD_ATTR               29 (getenv)
+               618 LOAD_CONST              21 ('AZURE_API_KEY')
+               620 LOAD_CONST              17 ('YOUR_API_KEY')
+               622 PRECALL                  2
+               626 CALL                     2
+               636 STORE_NAME              32 (API_KEY)
+   
+    33     >>  638 PUSH_NULL
+               640 LOAD_NAME               11 (MMBench_Evaluator)
+               642 LOAD_NAME               27 (config)
+               644 LOAD_CONST              10 ('metadata')
+               646 BINARY_SUBSCR
+               656 LOAD_CONST              22 ('sys_prompt')
+               658 BINARY_SUBSCR
+               668 LOAD_NAME               32 (API_KEY)
+               670 LOAD_NAME               31 (API_URL)
+               672 LOAD_NAME               28 (GPT_EVAL_MODEL_NAME)
+               674 KW_NAMES                23
+               676 PRECALL                  4
+               680 CALL                     4
+               690 STORE_NAME              33 (mmbench_evaluator)
+   
+    36         692 LOAD_CONST              24 (<code object mmbench_doc_to_visual, file "/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/en_utils.py", line 36>)
+               694 MAKE_FUNCTION            0
+               696 STORE_NAME              34 (mmbench_doc_to_visual)
+   
+    40         698 LOAD_CONST              30 ((None,))
+               700 LOAD_CONST              25 (<code object mmbench_doc_to_text, file "/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/en_utils.py", line 40>)
+               702 MAKE_FUNCTION            1 (defaults)
+               704 STORE_NAME              35 (mmbench_doc_to_text)
+   
+    66         706 LOAD_CONST              26 (<code object mmbench_process_results, file "/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/en_utils.py", line 66>)
+               708 MAKE_FUNCTION            0
+               710 STORE_NAME              36 (mmbench_process_results)
+   
+    99         712 LOAD_CONST              27 (<code object mmbench_aggregate_dev_results_eval, file "/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/en_utils.py", line 99>)
+               714 MAKE_FUNCTION            0
+               716 STORE_NAME              37 (mmbench_aggregate_dev_results_eval)
+   
+   113         718 LOAD_CONST              28 (<code object mmbench_aggregate_dev_results_submission, file "/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/en_utils.py", line 113>)
+               720 MAKE_FUNCTION            0
+               722 STORE_NAME              38 (mmbench_aggregate_dev_results_submission)
+   
+   121         724 LOAD_CONST              29 (<code object mmbench_aggregate_test_results, file "/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/en_utils.py", line 121>)
+               726 MAKE_FUNCTION            0
+               728 STORE_NAME              39 (mmbench_aggregate_test_results)
+               730 LOAD_CONST               1 (None)
+               732 RETURN_VALUE
    ExceptionTable:
      168 to 366 -> 392 [1] lasti
      392 to 398 -> 400 [3] lasti
      406 to 406 -> 400 [3] lasti
    consts
       0
       None
       ('Path',)
-      ('generate_submission_file',)
       'lmms-eval'
       ('MMBench_Evaluator',)
-      'mmbench_cn.yaml'
+      ('generate_submission_file',)
+      'mmbench.yaml'
       'r'
       '!function'
       ''
       'metadata'
+      'gpt_eval_model_name'
+      'API_TYPE'
+      'openai'
+      'OPENAI_API_URL'
+      'https://api.openai.com/v1/chat/completions'
+      'OPENAI_API_KEY'
+      'YOUR_API_KEY'
+      'azure'
+      'AZURE_ENDPOINT'
+      'https://api.cognitive.microsoft.com/sts/v1.0/issueToken'
+      'AZURE_API_KEY'
       'sys_prompt'
-      ('sys_prompt',)
+      ('sys_prompt', 'API_KEY', 'API_URL', 'model_version')
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 3
          flags     : 3
          code
             0x97007c00640119000000000000000000a0000000000000000000000000
             0000000000000000006402a6010000ab01000000000000000067015300
-          25           0 RESUME                   0
+          36           0 RESUME                   0
          
-          26           2 LOAD_FAST                0 (doc)
+          37           2 LOAD_FAST                0 (doc)
                        4 LOAD_CONST               1 ('image')
                        6 BINARY_SUBSCR
                       16 LOAD_METHOD              0 (convert)
                       38 LOAD_CONST               2 ('RGB')
                       40 PRECALL                  1
                       44 CALL                     1
                       54 BUILD_LIST               1
@@ -235,17 +324,17 @@
             None
             'image'
             'RGB'
          names      ('convert',)
          varnames   ('doc',)
          freevars   ()
          cellvars   ()
-         filename   '/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/cn_utils.py'
+         filename   '/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/en_utils.py'
          name       'mmbench_doc_to_visual'
-         firstlineno 25
+         firstlineno 36
          lnotab 0x0201
       code
          argcount  : 2
          nlocals   : 7
          stacksize : 11
          flags     : 3
          code
@@ -254,273 +343,450 @@
             0000005c0200007d037d047c006402190000000000000000007c00a00200
             0000000000000000000000000000000000000064036400a6020000ab0200
             000000000000007c037c006404190000000000000000007c006405190000
             000000000000007c047c006406190000000000000000007c006407190000
             000000000000007c006408190000000000000000007c0064091900000000
             0000000000640a9c0a7d057407000000000000000000006a040000000000
             0000007c05640719000000000000000000a6010000ab0100000000000000
-            00721c7c056407190000000000000000009b00640b7c0564021900000000
-            00000000009b00640b7c05640c190000000000000000009b009d056e127c
-            056402190000000000000000009b00640b7c05640c190000000000000000
-            009b009d037d067c01720d7c069b00640d7c01640e190000000000000000
-            009b009d037d067c065300
-          29           0 RESUME                   0
+            0072287c05640719000000000000000000640b6b0300000000721c7c0564
+            07190000000000000000009b00640c7c056402190000000000000000009b
+            00640c7c05640d190000000000000000009b009d056e127c056402190000
+            000000000000009b00640c7c05640d190000000000000000009b009d037d
+            067c01720d7c069b00640e7c01640f190000000000000000009b009d037d
+            067c065300
+          40           0 RESUME                   0
          
-          30           2 BUILD_LIST               0
+          41           2 BUILD_LIST               0
                        4 LOAD_CONST               1 (('A', 'B', 'C', 'D', 'E'))
                        6 LIST_EXTEND              1
                        8 STORE_FAST               2 (option_candidate)
          
-          31          10 LOAD_GLOBAL              0 (mmbench_evaluator)
+          42          10 LOAD_GLOBAL              0 (mmbench_evaluator)
                       22 LOAD_METHOD              1 (create_options_prompt)
                       44 LOAD_FAST                0 (doc)
                       46 LOAD_FAST                2 (option_candidate)
                       48 PRECALL                  2
                       52 CALL                     2
                       62 UNPACK_SEQUENCE          2
                       66 STORE_FAST               3 (options_prompt)
                       68 STORE_FAST               4 (options_dict)
          
-          35          70 LOAD_FAST                0 (doc)
+          46          70 LOAD_FAST                0 (doc)
                       72 LOAD_CONST               2 ('question')
                       74 BINARY_SUBSCR
          
-          36          84 LOAD_FAST                0 (doc)
+          47          84 LOAD_FAST                0 (doc)
                       86 LOAD_METHOD              2 (get)
                      108 LOAD_CONST               3 ('answer')
                      110 LOAD_CONST               0 (None)
                      112 PRECALL                  2
                      116 CALL                     2
          
-          37         126 LOAD_FAST                3 (options_prompt)
+          48         126 LOAD_FAST                3 (options_prompt)
          
-          38         128 LOAD_FAST                0 (doc)
+          49         128 LOAD_FAST                0 (doc)
                      130 LOAD_CONST               4 ('category')
                      132 BINARY_SUBSCR
          
-          39         142 LOAD_FAST                0 (doc)
+          50         142 LOAD_FAST                0 (doc)
                      144 LOAD_CONST               5 ('L2-category')
                      146 BINARY_SUBSCR
          
-          40         156 LOAD_FAST                4 (options_dict)
+          51         156 LOAD_FAST                4 (options_dict)
          
-          41         158 LOAD_FAST                0 (doc)
+          52         158 LOAD_FAST                0 (doc)
                      160 LOAD_CONST               6 ('index')
                      162 BINARY_SUBSCR
          
-          42         172 LOAD_FAST                0 (doc)
+          53         172 LOAD_FAST                0 (doc)
                      174 LOAD_CONST               7 ('hint')
                      176 BINARY_SUBSCR
          
-          43         186 LOAD_FAST                0 (doc)
+          54         186 LOAD_FAST                0 (doc)
                      188 LOAD_CONST               8 ('source')
                      190 BINARY_SUBSCR
          
-          44         200 LOAD_FAST                0 (doc)
+          55         200 LOAD_FAST                0 (doc)
                      202 LOAD_CONST               9 ('split')
                      204 BINARY_SUBSCR
          
-          33         214 LOAD_CONST              10 (('question', 'answer', 'options', 'category', 'L2-category', 'options_dict', 'index', 'hint', 'source', 'split'))
+          44         214 LOAD_CONST              10 (('question', 'answer', 'options', 'category', 'L2-category', 'options_dict', 'index', 'hint', 'source', 'split'))
                      216 BUILD_CONST_KEY_MAP     10
                      218 STORE_FAST               5 (data)
          
-          47         220 LOAD_GLOBAL              7 (NULL + pd)
+          58         220 LOAD_GLOBAL              7 (NULL + pd)
                      232 LOAD_ATTR                4 (notna)
                      242 LOAD_FAST                5 (data)
                      244 LOAD_CONST               7 ('hint')
                      246 BINARY_SUBSCR
                      256 PRECALL                  1
                      260 CALL                     1
-                     270 POP_JUMP_FORWARD_IF_FALSE    28 (to 328)
+                     270 POP_JUMP_FORWARD_IF_FALSE    40 (to 352)
                      272 LOAD_FAST                5 (data)
                      274 LOAD_CONST               7 ('hint')
                      276 BINARY_SUBSCR
-                     286 FORMAT_VALUE             0
-                     288 LOAD_CONST              11 (' ')
-                     290 LOAD_FAST                5 (data)
-                     292 LOAD_CONST               2 ('question')
-                     294 BINARY_SUBSCR
-                     304 FORMAT_VALUE             0
-                     306 LOAD_CONST              11 (' ')
-                     308 LOAD_FAST                5 (data)
-                     310 LOAD_CONST              12 ('options')
-                     312 BINARY_SUBSCR
-                     322 FORMAT_VALUE             0
-                     324 BUILD_STRING             5
-                     326 JUMP_FORWARD            18 (to 364)
-                 >>  328 LOAD_FAST                5 (data)
-                     330 LOAD_CONST               2 ('question')
-                     332 BINARY_SUBSCR
-                     342 FORMAT_VALUE             0
-                     344 LOAD_CONST              11 (' ')
-                     346 LOAD_FAST                5 (data)
-                     348 LOAD_CONST              12 ('options')
-                     350 BINARY_SUBSCR
-                     360 FORMAT_VALUE             0
-                     362 BUILD_STRING             3
-                 >>  364 STORE_FAST               6 (query_prompt)
-         
-          49         366 LOAD_FAST                1 (model_specific_prompt_kwargs)
-                     368 POP_JUMP_FORWARD_IF_FALSE    13 (to 396)
-         
-          50         370 LOAD_FAST                6 (query_prompt)
-                     372 FORMAT_VALUE             0
-                     374 LOAD_CONST              13 ('\n')
-                     376 LOAD_FAST                1 (model_specific_prompt_kwargs)
-                     378 LOAD_CONST              14 ('post_prompt')
-                     380 BINARY_SUBSCR
-                     390 FORMAT_VALUE             0
-                     392 BUILD_STRING             3
-                     394 STORE_FAST               6 (query_prompt)
+                     286 LOAD_CONST              11 ('nan')
+                     288 COMPARE_OP               3 (!=)
+                     294 POP_JUMP_FORWARD_IF_FALSE    28 (to 352)
+                     296 LOAD_FAST                5 (data)
+                     298 LOAD_CONST               7 ('hint')
+                     300 BINARY_SUBSCR
+                     310 FORMAT_VALUE             0
+                     312 LOAD_CONST              12 (' ')
+                     314 LOAD_FAST                5 (data)
+                     316 LOAD_CONST               2 ('question')
+                     318 BINARY_SUBSCR
+                     328 FORMAT_VALUE             0
+                     330 LOAD_CONST              12 (' ')
+                     332 LOAD_FAST                5 (data)
+                     334 LOAD_CONST              13 ('options')
+                     336 BINARY_SUBSCR
+                     346 FORMAT_VALUE             0
+                     348 BUILD_STRING             5
+                     350 JUMP_FORWARD            18 (to 388)
+                 >>  352 LOAD_FAST                5 (data)
+                     354 LOAD_CONST               2 ('question')
+                     356 BINARY_SUBSCR
+                     366 FORMAT_VALUE             0
+                     368 LOAD_CONST              12 (' ')
+                     370 LOAD_FAST                5 (data)
+                     372 LOAD_CONST              13 ('options')
+                     374 BINARY_SUBSCR
+                     384 FORMAT_VALUE             0
+                     386 BUILD_STRING             3
+                 >>  388 STORE_FAST               6 (query_prompt)
+         
+          60         390 LOAD_FAST                1 (model_specific_prompt_kwargs)
+                     392 POP_JUMP_FORWARD_IF_FALSE    13 (to 420)
+         
+          61         394 LOAD_FAST                6 (query_prompt)
+                     396 FORMAT_VALUE             0
+                     398 LOAD_CONST              14 ('\n')
+                     400 LOAD_FAST                1 (model_specific_prompt_kwargs)
+                     402 LOAD_CONST              15 ('post_prompt')
+                     404 BINARY_SUBSCR
+                     414 FORMAT_VALUE             0
+                     416 BUILD_STRING             3
+                     418 STORE_FAST               6 (query_prompt)
          
-          52     >>  396 LOAD_FAST                6 (query_prompt)
-                     398 RETURN_VALUE
+          63     >>  420 LOAD_FAST                6 (query_prompt)
+                     422 RETURN_VALUE
          consts
             None
             ('A', 'B', 'C', 'D', 'E')
             'question'
             'answer'
             'category'
             'L2-category'
             'index'
             'hint'
             'source'
             'split'
             ('question', 'answer', 'options', 'category', 'L2-category', 'options_dict', 'index', 'hint', 'source', 'split')
+            'nan'
             ' '
             'options'
             '\n'
             'post_prompt'
          names      ('mmbench_evaluator', 'create_options_prompt', 'get', 'pd', 'notna')
          varnames   ('doc', 'model_specific_prompt_kwargs', 'option_candidate', 'options_prompt', 'options_dict', 'data', 'query_prompt')
          freevars   ()
          cellvars   ()
-         filename   '/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/cn_utils.py'
+         filename   '/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/en_utils.py'
          name       'mmbench_doc_to_text'
-         firstlineno 29
+         firstlineno 40
          lnotab
-            0x020108013c040e012a0102010e010e0102010e010e010e010ef5060e92
+            0x020108013c040e012a0102010e010e0102010e010e010e010ef5060eaa
             0204011a02
       code
          argcount  : 2
          nlocals   : 6
          stacksize : 11
          flags     : 3
          code
             0x97007c01640119000000000000000000a0000000000000000000000000
-            000000000000000000a6000000ab0000000000000000007d0264027c0064
-            03190000000000000000007c006404190000000000000000007c00640519
-            0000000000000000007c027c006406190000000000000000007c00640719
-            0000000000000000007c006408190000000000000000007c006409190000
-            000000000000007c00640a19000000000000000000640b9c0969017d0367
-            00640ca2017d047c0444005d217d057c00a0010000000000000000000000
+            000000000000000000a6000000ab0000000000000000007d027c00640219
+            0000000000000000007c006403190000000000000000007c006404190000
+            000000000000007c027c006405190000000000000000007c006406190000
+            000000000000007c006407190000000000000000007c0064081900000000
+            00000000007c00640919000000000000000000640a9c097c006402190000
+            000000000000007c006403190000000000000000007c0064041900000000
+            00000000007c027c006405190000000000000000007c0064061900000000
+            00000000007c006407190000000000000000007c00640819000000000000
+            0000007c00640919000000000000000000640a9c09640b9c027d03670064
+            0ca2017d047c0444005d407d057c00a00100000000000000000000000000
+            000000000000007c05640da6020000ab0200000000000000007c03640e19
+            0000000000000000007c053c0000007c00a0010000000000000000000000
             0000000000000000007c05640da6020000ab0200000000000000007c0364
-            02190000000000000000007c053c0000008c227c035300
-          55           0 RESUME                   0
+            0f190000000000000000007c053c0000008c417c035300
+          66           0 RESUME                   0
          
-          56           2 LOAD_FAST                1 (results)
+          67           2 LOAD_FAST                1 (results)
                        4 LOAD_CONST               1 (0)
                        6 BINARY_SUBSCR
                       16 LOAD_METHOD              0 (strip)
                       38 PRECALL                  0
                       42 CALL                     0
                       52 STORE_FAST               2 (model_response)
          
-          58          54 LOAD_CONST               2 ('submission')
+          70          54 LOAD_FAST                0 (doc)
+                      56 LOAD_CONST               2 ('index')
+                      58 BINARY_SUBSCR
          
-          59          56 LOAD_FAST                0 (doc)
-                      58 LOAD_CONST               3 ('index')
-                      60 BINARY_SUBSCR
+          71          68 LOAD_FAST                0 (doc)
+                      70 LOAD_CONST               3 ('question')
+                      72 BINARY_SUBSCR
          
-          60          70 LOAD_FAST                0 (doc)
-                      72 LOAD_CONST               4 ('question')
-                      74 BINARY_SUBSCR
+          72          82 LOAD_FAST                0 (doc)
+                      84 LOAD_CONST               4 ('answer')
+                      86 BINARY_SUBSCR
          
-          61          84 LOAD_FAST                0 (doc)
-                      86 LOAD_CONST               5 ('answer')
-                      88 BINARY_SUBSCR
-         
-          62          98 LOAD_FAST                2 (model_response)
-         
-          63         100 LOAD_FAST                0 (doc)
-                     102 LOAD_CONST               6 ('hint')
-                     104 BINARY_SUBSCR
-         
-          64         114 LOAD_FAST                0 (doc)
-                     116 LOAD_CONST               7 ('source')
-                     118 BINARY_SUBSCR
+          73          96 LOAD_FAST                2 (model_response)
          
-          65         128 LOAD_FAST                0 (doc)
-                     130 LOAD_CONST               8 ('split')
-                     132 BINARY_SUBSCR
+          74          98 LOAD_FAST                0 (doc)
+                     100 LOAD_CONST               5 ('hint')
+                     102 BINARY_SUBSCR
          
-          66         142 LOAD_FAST                0 (doc)
-                     144 LOAD_CONST               9 ('category')
-                     146 BINARY_SUBSCR
+          75         112 LOAD_FAST                0 (doc)
+                     114 LOAD_CONST               6 ('source')
+                     116 BINARY_SUBSCR
          
-          67         156 LOAD_FAST                0 (doc)
-                     158 LOAD_CONST              10 ('L2-category')
-                     160 BINARY_SUBSCR
-         
-          58         170 LOAD_CONST              11 (('index', 'question', 'answer', 'prediction', 'hint', 'source', 'split', 'category', 'L2-category'))
-                     172 BUILD_CONST_KEY_MAP      9
-         
-          57         174 BUILD_MAP                1
-                     176 STORE_FAST               3 (data)
-         
-          70         178 BUILD_LIST               0
-                     180 LOAD_CONST              12 (('A', 'B', 'C', 'D', 'E'))
-                     182 LIST_EXTEND              1
-                     184 STORE_FAST               4 (option_candidate)
-         
-          71         186 LOAD_FAST                4 (option_candidate)
-                     188 GET_ITER
-                 >>  190 FOR_ITER                33 (to 258)
-                     192 STORE_FAST               5 (c)
-         
-          72         194 LOAD_FAST                0 (doc)
-                     196 LOAD_METHOD              1 (get)
-                     218 LOAD_FAST                5 (c)
-                     220 LOAD_CONST              13 ('nan')
-                     222 PRECALL                  2
-                     226 CALL                     2
-                     236 LOAD_FAST                3 (data)
-                     238 LOAD_CONST               2 ('submission')
-                     240 BINARY_SUBSCR
-                     250 LOAD_FAST                5 (c)
-                     252 STORE_SUBSCR
-                     256 JUMP_BACKWARD           34 (to 190)
+          76         126 LOAD_FAST                0 (doc)
+                     128 LOAD_CONST               7 ('split')
+                     130 BINARY_SUBSCR
+         
+          77         140 LOAD_FAST                0 (doc)
+                     142 LOAD_CONST               8 ('category')
+                     144 BINARY_SUBSCR
+         
+          78         154 LOAD_FAST                0 (doc)
+                     156 LOAD_CONST               9 ('L2-category')
+                     158 BINARY_SUBSCR
+         
+          69         168 LOAD_CONST              10 (('index', 'question', 'answer', 'prediction', 'hint', 'source', 'split', 'category', 'L2-category'))
+                     170 BUILD_CONST_KEY_MAP      9
+         
+          81         172 LOAD_FAST                0 (doc)
+                     174 LOAD_CONST               2 ('index')
+                     176 BINARY_SUBSCR
          
-          73     >>  258 LOAD_FAST                3 (data)
-                     260 RETURN_VALUE
+          82         186 LOAD_FAST                0 (doc)
+                     188 LOAD_CONST               3 ('question')
+                     190 BINARY_SUBSCR
+         
+          83         200 LOAD_FAST                0 (doc)
+                     202 LOAD_CONST               4 ('answer')
+                     204 BINARY_SUBSCR
+         
+          84         214 LOAD_FAST                2 (model_response)
+         
+          85         216 LOAD_FAST                0 (doc)
+                     218 LOAD_CONST               5 ('hint')
+                     220 BINARY_SUBSCR
+         
+          86         230 LOAD_FAST                0 (doc)
+                     232 LOAD_CONST               6 ('source')
+                     234 BINARY_SUBSCR
+         
+          87         244 LOAD_FAST                0 (doc)
+                     246 LOAD_CONST               7 ('split')
+                     248 BINARY_SUBSCR
+         
+          88         258 LOAD_FAST                0 (doc)
+                     260 LOAD_CONST               8 ('category')
+                     262 BINARY_SUBSCR
+         
+          89         272 LOAD_FAST                0 (doc)
+                     274 LOAD_CONST               9 ('L2-category')
+                     276 BINARY_SUBSCR
+         
+          80         286 LOAD_CONST              10 (('index', 'question', 'answer', 'prediction', 'hint', 'source', 'split', 'category', 'L2-category'))
+                     288 BUILD_CONST_KEY_MAP      9
+         
+          68         290 LOAD_CONST              11 (('gpt_eval_score', 'submission'))
+                     292 BUILD_CONST_KEY_MAP      2
+                     294 STORE_FAST               3 (data)
+         
+          92         296 BUILD_LIST               0
+                     298 LOAD_CONST              12 (('A', 'B', 'C', 'D', 'E'))
+                     300 LIST_EXTEND              1
+                     302 STORE_FAST               4 (option_candidate)
+         
+          93         304 LOAD_FAST                4 (option_candidate)
+                     306 GET_ITER
+                 >>  308 FOR_ITER                64 (to 438)
+                     310 STORE_FAST               5 (c)
+         
+          94         312 LOAD_FAST                0 (doc)
+                     314 LOAD_METHOD              1 (get)
+                     336 LOAD_FAST                5 (c)
+                     338 LOAD_CONST              13 ('nan')
+                     340 PRECALL                  2
+                     344 CALL                     2
+                     354 LOAD_FAST                3 (data)
+                     356 LOAD_CONST              14 ('submission')
+                     358 BINARY_SUBSCR
+                     368 LOAD_FAST                5 (c)
+                     370 STORE_SUBSCR
+         
+          95         374 LOAD_FAST                0 (doc)
+                     376 LOAD_METHOD              1 (get)
+                     398 LOAD_FAST                5 (c)
+                     400 LOAD_CONST              13 ('nan')
+                     402 PRECALL                  2
+                     406 CALL                     2
+                     416 LOAD_FAST                3 (data)
+                     418 LOAD_CONST              15 ('gpt_eval_score')
+                     420 BINARY_SUBSCR
+                     430 LOAD_FAST                5 (c)
+                     432 STORE_SUBSCR
+                     436 JUMP_BACKWARD           65 (to 308)
+         
+          96     >>  438 LOAD_FAST                3 (data)
+                     440 RETURN_VALUE
          consts
             None
             0
-            'submission'
             'index'
             'question'
             'answer'
             'hint'
             'source'
             'split'
             'category'
             'L2-category'
             ('index', 'question', 'answer', 'prediction', 'hint', 'source', 'split', 'category', 'L2-category')
+            ('gpt_eval_score', 'submission')
             ('A', 'B', 'C', 'D', 'E')
             'nan'
+            'submission'
+            'gpt_eval_score'
          names      ('strip', 'get')
          varnames   ('doc', 'results', 'model_response', 'data', 'option_candidate', 'c')
          freevars   ()
          cellvars   ()
-         filename   '/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/cn_utils.py'
+         filename   '/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/en_utils.py'
          name       'mmbench_process_results'
-         firstlineno 55
+         firstlineno 66
          lnotab
-            0x0201340202010e010e010e0102010e010e010e010e010ef704ff040d08
-            0108014001
+            0x020134030e010e010e0102010e010e010e010e010ef7040c0e010e010e
+            0102010e010e010e010e010ef704f40618080108013e014001
+      code
+         argcount  : 2
+         nlocals   : 8
+         stacksize : 6
+         flags     : 3
+         code
+            0x97007401000000000000000000006401a6010000ab0100000000000000
+            000100740200000000000000000000a00200000000000000000000000000
+            000000000000007c006402ac03a6020000ab0200000000000000005c0300
+            007d027d037d0474070000000000000000000064047c01a6020000ab0200
+            000000000000007d057c027c037c0464059c037d06740900000000000000
+            0000007c056406a6020000ab02000000000000000035007d07740b000000
+            000000000000006a0600000000000000007c067c07a6020000ab02000000
+            00000000000100640064006400a6020000ab02000000000000000001006e
+            0b230031007304770278035900770101005900010001007c0264077a0500
+            005300
+          99           0 RESUME                   0
+         
+         100           2 LOAD_GLOBAL              1 (NULL + print)
+                      14 LOAD_CONST               1 ('============= MMBench-EN(Dev) Detailed Results =============')
+                      16 PRECALL                  1
+                      20 CALL                     1
+                      30 POP_TOP
+         
+         101          32 LOAD_GLOBAL              2 (mmbench_evaluator)
+                      44 LOAD_METHOD              2 (eval_result)
+                      66 LOAD_FAST                0 (results)
+                      68 LOAD_CONST               2 ('openai')
+                      70 KW_NAMES                 3
+                      72 PRECALL                  2
+                      76 CALL                     2
+                      86 UNPACK_SEQUENCE          3
+                      90 STORE_FAST               2 (overall_acc)
+                      92 STORE_FAST               3 (category_acc)
+                      94 STORE_FAST               4 (l2_category_acc)
+         
+         102          96 LOAD_GLOBAL              7 (NULL + generate_submission_file)
+                     108 LOAD_CONST               4 ('mmbench_en_dev_results.json')
+                     110 LOAD_FAST                1 (args)
+                     112 PRECALL                  2
+                     116 CALL                     2
+                     126 STORE_FAST               5 (file)
+         
+         104         128 LOAD_FAST                2 (overall_acc)
+         
+         105         130 LOAD_FAST                3 (category_acc)
+         
+         106         132 LOAD_FAST                4 (l2_category_acc)
+         
+         103         134 LOAD_CONST               5 (('overall_acc', 'category_acc', 'l2_category_acc'))
+                     136 BUILD_CONST_KEY_MAP      3
+                     138 STORE_FAST               6 (details_info)
+         
+         108         140 LOAD_GLOBAL              9 (NULL + open)
+                     152 LOAD_FAST                5 (file)
+                     154 LOAD_CONST               6 ('w')
+                     156 PRECALL                  2
+                     160 CALL                     2
+                     170 BEFORE_WITH
+                     172 STORE_FAST               7 (f)
+         
+         109         174 LOAD_GLOBAL             11 (NULL + json)
+                     186 LOAD_ATTR                6 (dump)
+                     196 LOAD_FAST                6 (details_info)
+                     198 LOAD_FAST                7 (f)
+                     200 PRECALL                  2
+                     204 CALL                     2
+                     214 POP_TOP
+         
+         108         216 LOAD_CONST               0 (None)
+                     218 LOAD_CONST               0 (None)
+                     220 LOAD_CONST               0 (None)
+                     222 PRECALL                  2
+                     226 CALL                     2
+                     236 POP_TOP
+                     238 JUMP_FORWARD            11 (to 262)
+                 >>  240 PUSH_EXC_INFO
+                     242 WITH_EXCEPT_START
+                     244 POP_JUMP_FORWARD_IF_TRUE     4 (to 254)
+                     246 RERAISE                  2
+                 >>  248 COPY                     3
+                     250 POP_EXCEPT
+                     252 RERAISE                  1
+                 >>  254 POP_TOP
+                     256 POP_EXCEPT
+                     258 POP_TOP
+                     260 POP_TOP
+         
+         110     >>  262 LOAD_FAST                2 (overall_acc)
+                     264 LOAD_CONST               7 (100)
+                     266 BINARY_OP                5 (*)
+                     270 RETURN_VALUE
+         ExceptionTable:
+           172 to 214 -> 240 [1] lasti
+           240 to 246 -> 248 [3] lasti
+           254 to 254 -> 248 [3] lasti
+         consts
+            None
+            '============= MMBench-EN(Dev) Detailed Results ============='
+            'openai'
+            ('eval_method',)
+            'mmbench_en_dev_results.json'
+            ('overall_acc', 'category_acc', 'l2_category_acc')
+            'w'
+            100
+         names      ('print', 'mmbench_evaluator', 'eval_result', 'generate_submission_file', 'open', 'json', 'dump')
+         varnames   ('results', 'args', 'overall_acc', 'category_acc', 'l2_category_acc', 'file', 'details_info', 'f')
+         freevars   ()
+         cellvars   ()
+         filename   '/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/en_utils.py'
+         name       'mmbench_aggregate_dev_results_eval'
+         firstlineno 99
+         lnotab 0x02011e01400120020201020102fd060522012aff2e02
       code
          argcount  : 2
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
             0x97007401000000000000000000006a0100000000000000007c00a60100
@@ -529,48 +795,48 @@
             000000000000007c03a6010000ab01000000000000000035007d047c02a0
             0400000000000000000000000000000000000000007c046402ac03a60200
             00ab0200000000000000000100640064006400a6020000ab020000000000
             00000001006e0b2300310073047702780359007701010059000100010074
             0a00000000000000000000a0060000000000000000000000000000000000
             00000064047c039b009d02a6010000ab0100000000000000000100640053
             00
-          76           0 RESUME                   0
+         113           0 RESUME                   0
          
-          77           2 LOAD_GLOBAL              1 (NULL + pd)
+         114           2 LOAD_GLOBAL              1 (NULL + pd)
                       14 LOAD_ATTR                1 (DataFrame)
                       24 LOAD_FAST                0 (results)
                       26 PRECALL                  1
                       30 CALL                     1
                       40 STORE_FAST               2 (df)
          
-          78          42 LOAD_GLOBAL              5 (NULL + generate_submission_file)
-                      54 LOAD_CONST               1 ('mmbench_cn_dev_results.xlsx')
+         115          42 LOAD_GLOBAL              5 (NULL + generate_submission_file)
+                      54 LOAD_CONST               1 ('mmbench_en_dev_results.xlsx')
                       56 LOAD_FAST                1 (args)
                       58 PRECALL                  2
                       62 CALL                     2
                       72 STORE_FAST               3 (excel_write_path)
          
-          79          74 LOAD_GLOBAL              1 (NULL + pd)
+         116          74 LOAD_GLOBAL              1 (NULL + pd)
                       86 LOAD_ATTR                3 (ExcelWriter)
                       96 LOAD_FAST                3 (excel_write_path)
                       98 PRECALL                  1
                      102 CALL                     1
                      112 BEFORE_WITH
                      114 STORE_FAST               4 (writer)
          
-          80         116 LOAD_FAST                2 (df)
+         117         116 LOAD_FAST                2 (df)
                      118 LOAD_METHOD              4 (to_excel)
                      140 LOAD_FAST                4 (writer)
                      142 LOAD_CONST               2 (False)
                      144 KW_NAMES                 3
                      146 PRECALL                  2
                      150 CALL                     2
                      160 POP_TOP
          
-          79         162 LOAD_CONST               0 (None)
+         116         162 LOAD_CONST               0 (None)
                      164 LOAD_CONST               0 (None)
                      166 LOAD_CONST               0 (None)
                      168 PRECALL                  2
                      172 CALL                     2
                      182 POP_TOP
                      184 JUMP_FORWARD            11 (to 208)
                  >>  186 PUSH_EXC_INFO
@@ -581,15 +847,15 @@
                      196 POP_EXCEPT
                      198 RERAISE                  1
                  >>  200 POP_TOP
                      202 POP_EXCEPT
                      204 POP_TOP
                      206 POP_TOP
          
-          81     >>  208 LOAD_GLOBAL             10 (eval_logger)
+         118     >>  208 LOAD_GLOBAL             10 (eval_logger)
                      220 LOAD_METHOD              6 (info)
                      242 LOAD_CONST               4 ('Saved results to ')
                      244 LOAD_FAST                3 (excel_write_path)
                      246 FORMAT_VALUE             0
                      248 BUILD_STRING             2
                      250 PRECALL                  1
                      254 CALL                     1
@@ -598,155 +864,128 @@
                      268 RETURN_VALUE
          ExceptionTable:
            114 to 160 -> 186 [1] lasti
            186 to 192 -> 194 [3] lasti
            200 to 200 -> 194 [3] lasti
          consts
             None
-            'mmbench_cn_dev_results.xlsx'
+            'mmbench_en_dev_results.xlsx'
             False
             ('index',)
             'Saved results to '
          names      ('pd', 'DataFrame', 'generate_submission_file', 'ExcelWriter', 'to_excel', 'eval_logger', 'info')
          varnames   ('results', 'args', 'df', 'excel_write_path', 'writer')
          freevars   ()
          cellvars   ()
-         filename   '/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/cn_utils.py'
-         name       'mmbench_aggregate_dev_results'
-         firstlineno 76
+         filename   '/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/en_utils.py'
+         name       'mmbench_aggregate_dev_results_submission'
+         firstlineno 113
          lnotab 0x0201280120012a012eff2e02
       code
          argcount  : 2
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
             0x97007401000000000000000000006a0100000000000000007c00a60100
-            00ab0100000000000000007d027405000000000000000000007c016a0300
-            00000000000000a6010000ab010000000000000000a00400000000000000
-            000000000000000000000000006401a6010000ab010000000000000000a0
-            05000000000000000000000000000000000000000064026402ac03a60200
-            00ab02000000000000000001007405000000000000000000007c016a0300
-            00000000000000a6010000ab01000000000000000064017a0b000064047a
-            0b00007d037401000000000000000000006a0600000000000000007c03a6
-            010000ab01000000000000000035007d047c02a007000000000000000000
-            00000000000000000000007c046405ac06a6020000ab0200000000000000
-            000100640064006400a6020000ab02000000000000000001006e0b230031
-            007304770278035900770101005900010001007410000000000000000000
-            00a009000000000000000000000000000000000000000064077c039b009d
-            02a6010000ab010000000000000000010064005300
-          84           0 RESUME                   0
+            00ab0100000000000000007d0274050000000000000000000064017c01a6
+            020000ab0200000000000000007d037401000000000000000000006a0300
+            000000000000007c03a6010000ab01000000000000000035007d047c02a0
+            0400000000000000000000000000000000000000007c046402ac03a60200
+            00ab0200000000000000000100640064006400a6020000ab020000000000
+            00000001006e0b2300310073047702780359007701010059000100010074
+            0a00000000000000000000a0060000000000000000000000000000000000
+            00000064047c039b009d02a6010000ab0100000000000000000100640053
+            00
+         121           0 RESUME                   0
          
-          85           2 LOAD_GLOBAL              1 (NULL + pd)
+         122           2 LOAD_GLOBAL              1 (NULL + pd)
                       14 LOAD_ATTR                1 (DataFrame)
                       24 LOAD_FAST                0 (results)
                       26 PRECALL                  1
                       30 CALL                     1
                       40 STORE_FAST               2 (df)
          
-          86          42 LOAD_GLOBAL              5 (NULL + Path)
-                      54 LOAD_FAST                1 (args)
-                      56 LOAD_ATTR                3 (output_path)
-                      66 PRECALL                  1
-                      70 CALL                     1
-                      80 LOAD_METHOD              4 (joinpath)
-                     102 LOAD_CONST               1 ('submissions')
-                     104 PRECALL                  1
-                     108 CALL                     1
-                     118 LOAD_METHOD              5 (mkdir)
-                     140 LOAD_CONST               2 (True)
-                     142 LOAD_CONST               2 (True)
+         123          42 LOAD_GLOBAL              5 (NULL + generate_submission_file)
+                      54 LOAD_CONST               1 ('mmbench_en_test_results.xlsx')
+                      56 LOAD_FAST                1 (args)
+                      58 PRECALL                  2
+                      62 CALL                     2
+                      72 STORE_FAST               3 (excel_write_path)
+         
+         124          74 LOAD_GLOBAL              1 (NULL + pd)
+                      86 LOAD_ATTR                3 (ExcelWriter)
+                      96 LOAD_FAST                3 (excel_write_path)
+                      98 PRECALL                  1
+                     102 CALL                     1
+                     112 BEFORE_WITH
+                     114 STORE_FAST               4 (writer)
+         
+         125         116 LOAD_FAST                2 (df)
+                     118 LOAD_METHOD              4 (to_excel)
+                     140 LOAD_FAST                4 (writer)
+                     142 LOAD_CONST               2 (False)
                      144 KW_NAMES                 3
                      146 PRECALL                  2
                      150 CALL                     2
                      160 POP_TOP
          
-          87         162 LOAD_GLOBAL              5 (NULL + Path)
-                     174 LOAD_FAST                1 (args)
-                     176 LOAD_ATTR                3 (output_path)
-                     186 PRECALL                  1
-                     190 CALL                     1
-                     200 LOAD_CONST               1 ('submissions')
-                     202 BINARY_OP               11 (/)
-                     206 LOAD_CONST               4 ('mmbench_cn_test_results.xlsx')
-                     208 BINARY_OP               11 (/)
-                     212 STORE_FAST               3 (excel_write_path)
-         
-          88         214 LOAD_GLOBAL              1 (NULL + pd)
-                     226 LOAD_ATTR                6 (ExcelWriter)
-                     236 LOAD_FAST                3 (excel_write_path)
-                     238 PRECALL                  1
-                     242 CALL                     1
-                     252 BEFORE_WITH
-                     254 STORE_FAST               4 (writer)
-         
-          89         256 LOAD_FAST                2 (df)
-                     258 LOAD_METHOD              7 (to_excel)
-                     280 LOAD_FAST                4 (writer)
-                     282 LOAD_CONST               5 (False)
-                     284 KW_NAMES                 6
-                     286 PRECALL                  2
-                     290 CALL                     2
-                     300 POP_TOP
-         
-          88         302 LOAD_CONST               0 (None)
-                     304 LOAD_CONST               0 (None)
-                     306 LOAD_CONST               0 (None)
-                     308 PRECALL                  2
-                     312 CALL                     2
-                     322 POP_TOP
-                     324 JUMP_FORWARD            11 (to 348)
-                 >>  326 PUSH_EXC_INFO
-                     328 WITH_EXCEPT_START
-                     330 POP_JUMP_FORWARD_IF_TRUE     4 (to 340)
-                     332 RERAISE                  2
-                 >>  334 COPY                     3
-                     336 POP_EXCEPT
-                     338 RERAISE                  1
-                 >>  340 POP_TOP
-                     342 POP_EXCEPT
-                     344 POP_TOP
-                     346 POP_TOP
-         
-          90     >>  348 LOAD_GLOBAL             16 (eval_logger)
-                     360 LOAD_METHOD              9 (info)
-                     382 LOAD_CONST               7 ('Saved results to ')
-                     384 LOAD_FAST                3 (excel_write_path)
-                     386 FORMAT_VALUE             0
-                     388 BUILD_STRING             2
-                     390 PRECALL                  1
-                     394 CALL                     1
-                     404 POP_TOP
-                     406 LOAD_CONST               0 (None)
-                     408 RETURN_VALUE
+         124         162 LOAD_CONST               0 (None)
+                     164 LOAD_CONST               0 (None)
+                     166 LOAD_CONST               0 (None)
+                     168 PRECALL                  2
+                     172 CALL                     2
+                     182 POP_TOP
+                     184 JUMP_FORWARD            11 (to 208)
+                 >>  186 PUSH_EXC_INFO
+                     188 WITH_EXCEPT_START
+                     190 POP_JUMP_FORWARD_IF_TRUE     4 (to 200)
+                     192 RERAISE                  2
+                 >>  194 COPY                     3
+                     196 POP_EXCEPT
+                     198 RERAISE                  1
+                 >>  200 POP_TOP
+                     202 POP_EXCEPT
+                     204 POP_TOP
+                     206 POP_TOP
+         
+         126     >>  208 LOAD_GLOBAL             10 (eval_logger)
+                     220 LOAD_METHOD              6 (info)
+                     242 LOAD_CONST               4 ('Saved results to ')
+                     244 LOAD_FAST                3 (excel_write_path)
+                     246 FORMAT_VALUE             0
+                     248 BUILD_STRING             2
+                     250 PRECALL                  1
+                     254 CALL                     1
+                     264 POP_TOP
+                     266 LOAD_CONST               0 (None)
+                     268 RETURN_VALUE
          ExceptionTable:
-           254 to 300 -> 326 [1] lasti
-           326 to 332 -> 334 [3] lasti
-           340 to 340 -> 334 [3] lasti
+           114 to 160 -> 186 [1] lasti
+           186 to 192 -> 194 [3] lasti
+           200 to 200 -> 194 [3] lasti
          consts
             None
-            'submissions'
-            True
-            ('parents', 'exist_ok')
-            'mmbench_cn_test_results.xlsx'
+            'mmbench_en_test_results.xlsx'
             False
             ('index',)
             'Saved results to '
-         names      ('pd', 'DataFrame', 'Path', 'output_path', 'joinpath', 'mkdir', 'ExcelWriter', 'to_excel', 'eval_logger', 'info')
+         names      ('pd', 'DataFrame', 'generate_submission_file', 'ExcelWriter', 'to_excel', 'eval_logger', 'info')
          varnames   ('results', 'args', 'df', 'excel_write_path', 'writer')
          freevars   ()
          cellvars   ()
-         filename   '/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/cn_utils.py'
+         filename   '/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/en_utils.py'
          name       'mmbench_aggregate_test_results'
-         firstlineno 84
-         lnotab 0x02012801780134012a012eff2e02
+         firstlineno 121
+         lnotab 0x0201280120012a012eff2e02
       (None,)
-   names      ('logging', 'yaml', 'os', 'pathlib', 'Path', 'pandas', 'pd', 'json', 'lmms_eval.tasks._task_utils.file_utils', 'generate_submission_file', 'getLogger', 'eval_logger', 'lmms_eval.tasks.mmbench.mmbench_evals', 'MMBench_Evaluator', 'open', '__file__', 'parent', 'f', 'readlines', 'raw_data', 'safe_data', 'enumerate', 'i', 'line', 'append', 'safe_load', 'join', 'config', 'mmbench_evaluator', 'mmbench_doc_to_visual', 'mmbench_doc_to_text', 'mmbench_process_results', 'mmbench_aggregate_dev_results', 'mmbench_aggregate_test_results')
+   names      ('logging', 'yaml', 'os', 'pathlib', 'Path', 'pandas', 'pd', 'json', 'getLogger', 'eval_logger', 'lmms_eval.tasks.mmbench.mmbench_evals', 'MMBench_Evaluator', 'lmms_eval.tasks._task_utils.file_utils', 'generate_submission_file', 'open', '__file__', 'parent', 'f', 'readlines', 'raw_data', 'safe_data', 'enumerate', 'i', 'line', 'append', 'safe_load', 'join', 'config', 'GPT_EVAL_MODEL_NAME', 'getenv', 'API_TYPE', 'API_URL', 'API_KEY', 'mmbench_evaluator', 'mmbench_doc_to_visual', 'mmbench_doc_to_text', 'mmbench_process_results', 'mmbench_aggregate_dev_results_eval', 'mmbench_aggregate_dev_results_submission', 'mmbench_aggregate_test_results')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/cn_utils.py'
+   filename   '/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/en_utils.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010801080108010c01080108010c0220010c023c012801040120
-      0208012c0246f82e0a30030604081a06150608
+      0x00ff02010801080108010c010801080220010c010c023c012801040120
+      0208012c0246f82e0a1c0122020c01220124010c01220122033603060408
+      1a0621060e0608
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/mmbench/__pycache__/en_utils.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/mmbench/__pycache__/cn_utils.cpython-311.pyc`

 * *Files 18% similar despite different names*

#### Python bytecode

```diff
@@ -1,33 +1,41 @@
 magic:    0xa70d0d0a
-moddate:  0x53c3ef65 (Tue Mar 12 02:52:03 2024 UTC)
-files sz: 3081
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
+files sz: 4589
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
-      026c036d045a040100640064016c055a06640064016c075a07020065006a
-      0800000000000000006403a6010000ab0100000000000000005a09640064
-      046c0a6d0b5a0b0100640064056c0c6d0d5a0d01000200650e0200650465
-      0fa6010000ab0100000000000000006a10000000000000000064067a0b00
-      006407a6020000ab02000000000000000035005a116511a0120000000000
-      000000000000000000000000000000a6000000ab0000000000000000005a
-      1367005a14020065156513a6010000ab01000000000000000044005d1e5c
-      0200005a165a1764086517760172156514a0180000000000000000000000
-      0000000000000000006517a6010000ab01000000000000000001008c1f02
-      0065016a1900000000000000006409a01a00000000000000000000000000
-      000000000000006514a6010000ab010000000000000000a6010000ab0100
-      000000000000005a1b640164016401a6020000ab02000000000000000001
-      006e0b230031007304770278035900770101005900010001000200650b65
-      1b640a19000000000000000000640b19000000000000000000ac0ca60100
-      00ab0100000000000000005a1c640d84005a1d6412640e84015a1e640f84
-      005a1f641084005a20641184005a2164015300
+      026c036d045a040100640064016c055a06640064016c075a07640064036c
+      086d095a090100020065006a0a00000000000000006404a6010000ab0100
+      000000000000005a0b640064056c0c6d0d5a0d0100640064036c086d095a
+      0901000200650e02006504650fa6010000ab0100000000000000006a1000
+      0000000000000064067a0b00006407a6020000ab02000000000000000035
+      005a116511a0120000000000000000000000000000000000000000a60000
+      00ab0000000000000000005a1367005a14020065156513a6010000ab0100
+      0000000000000044005d1e5c0200005a165a1764086517760172156514a0
+      1800000000000000000000000000000000000000006517a6010000ab0100
+      0000000000000001008c1f020065016a1900000000000000006409a01a00
+      000000000000000000000000000000000000006514a6010000ab01000000
+      0000000000a6010000ab0100000000000000005a1b640164016401a60200
+      00ab02000000000000000001006e0b230031007304770278035900770101
+      00590001000100651b640a19000000000000000000640b19000000000000
+      0000005a1c020065026a1d0000000000000000640c640da6020000ab0200
+      000000000000005a1e651e640d6b02000000007223020065026a1d000000
+      0000000000640e640fa6020000ab0200000000000000005a1f020065026a
+      1d000000000000000064106411a6020000ab0200000000000000005a206e
+      28651e64126b02000000007222020065026a1d0000000000000000641364
+      14a6020000ab0200000000000000005a1f020065026a1d00000000000000
+      0064156411a6020000ab0200000000000000005a200200650d651b640a19
+      0000000000000000006416190000000000000000006520651f651cac17a6
+      040000ab0400000000000000005a21641884005a22641e641984015a2364
+      1a84005a24641b84005a25641c84005a26641d84005a2764015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (logging)
                  8 STORE_NAME               0 (logging)
    
@@ -54,179 +62,267 @@
                 44 STORE_NAME               6 (pd)
    
      6          46 LOAD_CONST               0 (0)
                 48 LOAD_CONST               1 (None)
                 50 IMPORT_NAME              7 (json)
                 52 STORE_NAME               7 (json)
    
-     8          54 PUSH_NULL
-                56 LOAD_NAME                0 (logging)
-                58 LOAD_ATTR                8 (getLogger)
-                68 LOAD_CONST               3 ('lmms-eval')
-                70 PRECALL                  1
-                74 CALL                     1
-                84 STORE_NAME               9 (eval_logger)
-   
-     9          86 LOAD_CONST               0 (0)
-                88 LOAD_CONST               4 (('MMBench_Evaluator',))
-                90 IMPORT_NAME             10 (lmms_eval.tasks.mmbench.mmbench_evals)
-                92 IMPORT_FROM             11 (MMBench_Evaluator)
-                94 STORE_NAME              11 (MMBench_Evaluator)
-                96 POP_TOP
+     7          54 LOAD_CONST               0 (0)
+                56 LOAD_CONST               3 (('generate_submission_file',))
+                58 IMPORT_NAME              8 (lmms_eval.tasks._task_utils.file_utils)
+                60 IMPORT_FROM              9 (generate_submission_file)
+                62 STORE_NAME               9 (generate_submission_file)
+                64 POP_TOP
+   
+     9          66 PUSH_NULL
+                68 LOAD_NAME                0 (logging)
+                70 LOAD_ATTR               10 (getLogger)
+                80 LOAD_CONST               4 ('lmms-eval')
+                82 PRECALL                  1
+                86 CALL                     1
+                96 STORE_NAME              11 (eval_logger)
    
     10          98 LOAD_CONST               0 (0)
-               100 LOAD_CONST               5 (('generate_submission_file',))
-               102 IMPORT_NAME             12 (lmms_eval.tasks._task_utils.file_utils)
-               104 IMPORT_FROM             13 (generate_submission_file)
-               106 STORE_NAME              13 (generate_submission_file)
+               100 LOAD_CONST               5 (('MMBench_Evaluator',))
+               102 IMPORT_NAME             12 (lmms_eval.tasks.mmbench.mmbench_evals)
+               104 IMPORT_FROM             13 (MMBench_Evaluator)
+               106 STORE_NAME              13 (MMBench_Evaluator)
                108 POP_TOP
    
-    12         110 PUSH_NULL
-               112 LOAD_NAME               14 (open)
-               114 PUSH_NULL
-               116 LOAD_NAME                4 (Path)
-               118 LOAD_NAME               15 (__file__)
-               120 PRECALL                  1
-               124 CALL                     1
-               134 LOAD_ATTR               16 (parent)
-               144 LOAD_CONST               6 ('mmbench_en.yaml')
-               146 BINARY_OP               11 (/)
-               150 LOAD_CONST               7 ('r')
-               152 PRECALL                  2
-               156 CALL                     2
-               166 BEFORE_WITH
-               168 STORE_NAME              17 (f)
-   
-    13         170 LOAD_NAME               17 (f)
-               172 LOAD_METHOD             18 (readlines)
-               194 PRECALL                  0
-               198 CALL                     0
-               208 STORE_NAME              19 (raw_data)
-   
-    14         210 BUILD_LIST               0
-               212 STORE_NAME              20 (safe_data)
-   
-    15         214 PUSH_NULL
-               216 LOAD_NAME               21 (enumerate)
-               218 LOAD_NAME               19 (raw_data)
-               220 PRECALL                  1
-               224 CALL                     1
-               234 GET_ITER
-           >>  236 FOR_ITER                30 (to 298)
-               238 UNPACK_SEQUENCE          2
-               242 STORE_NAME              22 (i)
-               244 STORE_NAME              23 (line)
-   
-    17         246 LOAD_CONST               8 ('!function')
-               248 LOAD_NAME               23 (line)
-               250 CONTAINS_OP              1
-               252 POP_JUMP_FORWARD_IF_FALSE    21 (to 296)
-   
-    18         254 LOAD_NAME               20 (safe_data)
-               256 LOAD_METHOD             24 (append)
-               278 LOAD_NAME               23 (line)
-               280 PRECALL                  1
-               284 CALL                     1
-               294 POP_TOP
-           >>  296 JUMP_BACKWARD           31 (to 236)
-   
-    20     >>  298 PUSH_NULL
-               300 LOAD_NAME                1 (yaml)
-               302 LOAD_ATTR               25 (safe_load)
-               312 LOAD_CONST               9 ('')
-               314 LOAD_METHOD             26 (join)
-               336 LOAD_NAME               20 (safe_data)
-               338 PRECALL                  1
-               342 CALL                     1
-               352 PRECALL                  1
-               356 CALL                     1
-               366 STORE_NAME              27 (config)
-   
-    12         368 LOAD_CONST               1 (None)
-               370 LOAD_CONST               1 (None)
-               372 LOAD_CONST               1 (None)
-               374 PRECALL                  2
-               378 CALL                     2
-               388 POP_TOP
-               390 JUMP_FORWARD            11 (to 414)
-           >>  392 PUSH_EXC_INFO
-               394 WITH_EXCEPT_START
-               396 POP_JUMP_FORWARD_IF_TRUE     4 (to 406)
-               398 RERAISE                  2
-           >>  400 COPY                     3
-               402 POP_EXCEPT
-               404 RERAISE                  1
-           >>  406 POP_TOP
-               408 POP_EXCEPT
-               410 POP_TOP
-               412 POP_TOP
-   
-    22     >>  414 PUSH_NULL
-               416 LOAD_NAME               11 (MMBench_Evaluator)
-               418 LOAD_NAME               27 (config)
-               420 LOAD_CONST              10 ('metadata')
-               422 BINARY_SUBSCR
-               432 LOAD_CONST              11 ('sys_prompt')
-               434 BINARY_SUBSCR
-               444 KW_NAMES                12
-               446 PRECALL                  1
-               450 CALL                     1
-               460 STORE_NAME              28 (mmbench_evaluator)
-   
-    25         462 LOAD_CONST              13 (<code object mmbench_doc_to_visual, file "/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/en_utils.py", line 25>)
-               464 MAKE_FUNCTION            0
-               466 STORE_NAME              29 (mmbench_doc_to_visual)
-   
-    29         468 LOAD_CONST              18 ((None,))
-               470 LOAD_CONST              14 (<code object mmbench_doc_to_text, file "/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/en_utils.py", line 29>)
-               472 MAKE_FUNCTION            1 (defaults)
-               474 STORE_NAME              30 (mmbench_doc_to_text)
-   
-    55         476 LOAD_CONST              15 (<code object mmbench_process_results, file "/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/en_utils.py", line 55>)
-               478 MAKE_FUNCTION            0
-               480 STORE_NAME              31 (mmbench_process_results)
-   
-    76         482 LOAD_CONST              16 (<code object mmbench_aggregate_dev_results, file "/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/en_utils.py", line 76>)
-               484 MAKE_FUNCTION            0
-               486 STORE_NAME              32 (mmbench_aggregate_dev_results)
-   
-    84         488 LOAD_CONST              17 (<code object mmbench_aggregate_test_results, file "/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/en_utils.py", line 84>)
-               490 MAKE_FUNCTION            0
-               492 STORE_NAME              33 (mmbench_aggregate_test_results)
-               494 LOAD_CONST               1 (None)
-               496 RETURN_VALUE
+    11         110 LOAD_CONST               0 (0)
+               112 LOAD_CONST               3 (('generate_submission_file',))
+               114 IMPORT_NAME              8 (lmms_eval.tasks._task_utils.file_utils)
+               116 IMPORT_FROM              9 (generate_submission_file)
+               118 STORE_NAME               9 (generate_submission_file)
+               120 POP_TOP
+   
+    13         122 PUSH_NULL
+               124 LOAD_NAME               14 (open)
+               126 PUSH_NULL
+               128 LOAD_NAME                4 (Path)
+               130 LOAD_NAME               15 (__file__)
+               132 PRECALL                  1
+               136 CALL                     1
+               146 LOAD_ATTR               16 (parent)
+               156 LOAD_CONST               6 ('mmbench.yaml')
+               158 BINARY_OP               11 (/)
+               162 LOAD_CONST               7 ('r')
+               164 PRECALL                  2
+               168 CALL                     2
+               178 BEFORE_WITH
+               180 STORE_NAME              17 (f)
+   
+    14         182 LOAD_NAME               17 (f)
+               184 LOAD_METHOD             18 (readlines)
+               206 PRECALL                  0
+               210 CALL                     0
+               220 STORE_NAME              19 (raw_data)
+   
+    15         222 BUILD_LIST               0
+               224 STORE_NAME              20 (safe_data)
+   
+    16         226 PUSH_NULL
+               228 LOAD_NAME               21 (enumerate)
+               230 LOAD_NAME               19 (raw_data)
+               232 PRECALL                  1
+               236 CALL                     1
+               246 GET_ITER
+           >>  248 FOR_ITER                30 (to 310)
+               250 UNPACK_SEQUENCE          2
+               254 STORE_NAME              22 (i)
+               256 STORE_NAME              23 (line)
+   
+    18         258 LOAD_CONST               8 ('!function')
+               260 LOAD_NAME               23 (line)
+               262 CONTAINS_OP              1
+               264 POP_JUMP_FORWARD_IF_FALSE    21 (to 308)
+   
+    19         266 LOAD_NAME               20 (safe_data)
+               268 LOAD_METHOD             24 (append)
+               290 LOAD_NAME               23 (line)
+               292 PRECALL                  1
+               296 CALL                     1
+               306 POP_TOP
+           >>  308 JUMP_BACKWARD           31 (to 248)
+   
+    21     >>  310 PUSH_NULL
+               312 LOAD_NAME                1 (yaml)
+               314 LOAD_ATTR               25 (safe_load)
+               324 LOAD_CONST               9 ('')
+               326 LOAD_METHOD             26 (join)
+               348 LOAD_NAME               20 (safe_data)
+               350 PRECALL                  1
+               354 CALL                     1
+               364 PRECALL                  1
+               368 CALL                     1
+               378 STORE_NAME              27 (config)
+   
+    13         380 LOAD_CONST               1 (None)
+               382 LOAD_CONST               1 (None)
+               384 LOAD_CONST               1 (None)
+               386 PRECALL                  2
+               390 CALL                     2
+               400 POP_TOP
+               402 JUMP_FORWARD            11 (to 426)
+           >>  404 PUSH_EXC_INFO
+               406 WITH_EXCEPT_START
+               408 POP_JUMP_FORWARD_IF_TRUE     4 (to 418)
+               410 RERAISE                  2
+           >>  412 COPY                     3
+               414 POP_EXCEPT
+               416 RERAISE                  1
+           >>  418 POP_TOP
+               420 POP_EXCEPT
+               422 POP_TOP
+               424 POP_TOP
+   
+    23     >>  426 LOAD_NAME               27 (config)
+               428 LOAD_CONST              10 ('metadata')
+               430 BINARY_SUBSCR
+               440 LOAD_CONST              11 ('gpt_eval_model_name')
+               442 BINARY_SUBSCR
+               452 STORE_NAME              28 (GPT_EVAL_MODEL_NAME)
+   
+    24         454 PUSH_NULL
+               456 LOAD_NAME                2 (os)
+               458 LOAD_ATTR               29 (getenv)
+               468 LOAD_CONST              12 ('API_TYPE')
+               470 LOAD_CONST              13 ('openai')
+               472 PRECALL                  2
+               476 CALL                     2
+               486 STORE_NAME              30 (API_TYPE)
+   
+    26         488 LOAD_NAME               30 (API_TYPE)
+               490 LOAD_CONST              13 ('openai')
+               492 COMPARE_OP               2 (==)
+               498 POP_JUMP_FORWARD_IF_FALSE    35 (to 570)
+   
+    27         500 PUSH_NULL
+               502 LOAD_NAME                2 (os)
+               504 LOAD_ATTR               29 (getenv)
+               514 LOAD_CONST              14 ('OPENAI_API_URL')
+               516 LOAD_CONST              15 ('https://api.openai.com/v1/chat/completions')
+               518 PRECALL                  2
+               522 CALL                     2
+               532 STORE_NAME              31 (API_URL)
+   
+    28         534 PUSH_NULL
+               536 LOAD_NAME                2 (os)
+               538 LOAD_ATTR               29 (getenv)
+               548 LOAD_CONST              16 ('OPENAI_API_KEY')
+               550 LOAD_CONST              17 ('YOUR_API_KEY')
+               552 PRECALL                  2
+               556 CALL                     2
+               566 STORE_NAME              32 (API_KEY)
+               568 JUMP_FORWARD            40 (to 650)
+   
+    29     >>  570 LOAD_NAME               30 (API_TYPE)
+               572 LOAD_CONST              18 ('azure')
+               574 COMPARE_OP               2 (==)
+               580 POP_JUMP_FORWARD_IF_FALSE    34 (to 650)
+   
+    30         582 PUSH_NULL
+               584 LOAD_NAME                2 (os)
+               586 LOAD_ATTR               29 (getenv)
+               596 LOAD_CONST              19 ('AZURE_ENDPOINT')
+               598 LOAD_CONST              20 ('https://api.cognitive.microsoft.com/sts/v1.0/issueToken')
+               600 PRECALL                  2
+               604 CALL                     2
+               614 STORE_NAME              31 (API_URL)
+   
+    31         616 PUSH_NULL
+               618 LOAD_NAME                2 (os)
+               620 LOAD_ATTR               29 (getenv)
+               630 LOAD_CONST              21 ('AZURE_API_KEY')
+               632 LOAD_CONST              17 ('YOUR_API_KEY')
+               634 PRECALL                  2
+               638 CALL                     2
+               648 STORE_NAME              32 (API_KEY)
+   
+    34     >>  650 PUSH_NULL
+               652 LOAD_NAME               13 (MMBench_Evaluator)
+               654 LOAD_NAME               27 (config)
+               656 LOAD_CONST              10 ('metadata')
+               658 BINARY_SUBSCR
+               668 LOAD_CONST              22 ('sys_prompt')
+               670 BINARY_SUBSCR
+               680 LOAD_NAME               32 (API_KEY)
+               682 LOAD_NAME               31 (API_URL)
+               684 LOAD_NAME               28 (GPT_EVAL_MODEL_NAME)
+               686 KW_NAMES                23
+               688 PRECALL                  4
+               692 CALL                     4
+               702 STORE_NAME              33 (mmbench_evaluator)
+   
+    37         704 LOAD_CONST              24 (<code object mmbench_doc_to_visual, file "/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/cn_utils.py", line 37>)
+               706 MAKE_FUNCTION            0
+               708 STORE_NAME              34 (mmbench_doc_to_visual)
+   
+    41         710 LOAD_CONST              30 ((None,))
+               712 LOAD_CONST              25 (<code object mmbench_doc_to_text, file "/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/cn_utils.py", line 41>)
+               714 MAKE_FUNCTION            1 (defaults)
+               716 STORE_NAME              35 (mmbench_doc_to_text)
+   
+    67         718 LOAD_CONST              26 (<code object mmbench_process_results, file "/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/cn_utils.py", line 67>)
+               720 MAKE_FUNCTION            0
+               722 STORE_NAME              36 (mmbench_process_results)
+   
+   100         724 LOAD_CONST              27 (<code object mmbench_aggregate_dev_results_eval, file "/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/cn_utils.py", line 100>)
+               726 MAKE_FUNCTION            0
+               728 STORE_NAME              37 (mmbench_aggregate_dev_results_eval)
+   
+   114         730 LOAD_CONST              28 (<code object mmbench_aggregate_dev_results, file "/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/cn_utils.py", line 114>)
+               732 MAKE_FUNCTION            0
+               734 STORE_NAME              38 (mmbench_aggregate_dev_results)
+   
+   122         736 LOAD_CONST              29 (<code object mmbench_aggregate_test_results, file "/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/cn_utils.py", line 122>)
+               738 MAKE_FUNCTION            0
+               740 STORE_NAME              39 (mmbench_aggregate_test_results)
+               742 LOAD_CONST               1 (None)
+               744 RETURN_VALUE
    ExceptionTable:
-     168 to 366 -> 392 [1] lasti
-     392 to 398 -> 400 [3] lasti
-     406 to 406 -> 400 [3] lasti
+     180 to 378 -> 404 [1] lasti
+     404 to 410 -> 412 [3] lasti
+     418 to 418 -> 412 [3] lasti
    consts
       0
       None
       ('Path',)
+      ('generate_submission_file',)
       'lmms-eval'
       ('MMBench_Evaluator',)
-      ('generate_submission_file',)
-      'mmbench_en.yaml'
+      'mmbench.yaml'
       'r'
       '!function'
       ''
       'metadata'
+      'gpt_eval_model_name'
+      'API_TYPE'
+      'openai'
+      'OPENAI_API_URL'
+      'https://api.openai.com/v1/chat/completions'
+      'OPENAI_API_KEY'
+      'YOUR_API_KEY'
+      'azure'
+      'AZURE_ENDPOINT'
+      'https://api.cognitive.microsoft.com/sts/v1.0/issueToken'
+      'AZURE_API_KEY'
       'sys_prompt'
-      ('sys_prompt',)
+      ('sys_prompt', 'API_KEY', 'API_URL', 'model_version')
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 3
          flags     : 3
          code
             0x97007c00640119000000000000000000a0000000000000000000000000
             0000000000000000006402a6010000ab01000000000000000067015300
-          25           0 RESUME                   0
+          37           0 RESUME                   0
          
-          26           2 LOAD_FAST                0 (doc)
+          38           2 LOAD_FAST                0 (doc)
                        4 LOAD_CONST               1 ('image')
                        6 BINARY_SUBSCR
                       16 LOAD_METHOD              0 (convert)
                       38 LOAD_CONST               2 ('RGB')
                       40 PRECALL                  1
                       44 CALL                     1
                       54 BUILD_LIST               1
@@ -235,17 +331,17 @@
             None
             'image'
             'RGB'
          names      ('convert',)
          varnames   ('doc',)
          freevars   ()
          cellvars   ()
-         filename   '/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/en_utils.py'
+         filename   '/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/cn_utils.py'
          name       'mmbench_doc_to_visual'
-         firstlineno 25
+         firstlineno 37
          lnotab 0x0201
       code
          argcount  : 2
          nlocals   : 7
          stacksize : 11
          flags     : 3
          code
@@ -259,75 +355,75 @@
             0000000000640a9c0a7d057407000000000000000000006a040000000000
             0000007c05640719000000000000000000a6010000ab0100000000000000
             00721c7c056407190000000000000000009b00640b7c0564021900000000
             00000000009b00640b7c05640c190000000000000000009b009d056e127c
             056402190000000000000000009b00640b7c05640c190000000000000000
             009b009d037d067c01720d7c069b00640d7c01640e190000000000000000
             009b009d037d067c065300
-          29           0 RESUME                   0
+          41           0 RESUME                   0
          
-          30           2 BUILD_LIST               0
+          42           2 BUILD_LIST               0
                        4 LOAD_CONST               1 (('A', 'B', 'C', 'D', 'E'))
                        6 LIST_EXTEND              1
                        8 STORE_FAST               2 (option_candidate)
          
-          31          10 LOAD_GLOBAL              0 (mmbench_evaluator)
+          43          10 LOAD_GLOBAL              0 (mmbench_evaluator)
                       22 LOAD_METHOD              1 (create_options_prompt)
                       44 LOAD_FAST                0 (doc)
                       46 LOAD_FAST                2 (option_candidate)
                       48 PRECALL                  2
                       52 CALL                     2
                       62 UNPACK_SEQUENCE          2
                       66 STORE_FAST               3 (options_prompt)
                       68 STORE_FAST               4 (options_dict)
          
-          35          70 LOAD_FAST                0 (doc)
+          47          70 LOAD_FAST                0 (doc)
                       72 LOAD_CONST               2 ('question')
                       74 BINARY_SUBSCR
          
-          36          84 LOAD_FAST                0 (doc)
+          48          84 LOAD_FAST                0 (doc)
                       86 LOAD_METHOD              2 (get)
                      108 LOAD_CONST               3 ('answer')
                      110 LOAD_CONST               0 (None)
                      112 PRECALL                  2
                      116 CALL                     2
          
-          37         126 LOAD_FAST                3 (options_prompt)
+          49         126 LOAD_FAST                3 (options_prompt)
          
-          38         128 LOAD_FAST                0 (doc)
+          50         128 LOAD_FAST                0 (doc)
                      130 LOAD_CONST               4 ('category')
                      132 BINARY_SUBSCR
          
-          39         142 LOAD_FAST                0 (doc)
-                     144 LOAD_CONST               5 ('l2-category')
+          51         142 LOAD_FAST                0 (doc)
+                     144 LOAD_CONST               5 ('L2-category')
                      146 BINARY_SUBSCR
          
-          40         156 LOAD_FAST                4 (options_dict)
+          52         156 LOAD_FAST                4 (options_dict)
          
-          41         158 LOAD_FAST                0 (doc)
+          53         158 LOAD_FAST                0 (doc)
                      160 LOAD_CONST               6 ('index')
                      162 BINARY_SUBSCR
          
-          42         172 LOAD_FAST                0 (doc)
+          54         172 LOAD_FAST                0 (doc)
                      174 LOAD_CONST               7 ('hint')
                      176 BINARY_SUBSCR
          
-          43         186 LOAD_FAST                0 (doc)
+          55         186 LOAD_FAST                0 (doc)
                      188 LOAD_CONST               8 ('source')
                      190 BINARY_SUBSCR
          
-          44         200 LOAD_FAST                0 (doc)
+          56         200 LOAD_FAST                0 (doc)
                      202 LOAD_CONST               9 ('split')
                      204 BINARY_SUBSCR
          
-          33         214 LOAD_CONST              10 (('question', 'answer', 'options', 'category', 'L2-category', 'options_dict', 'index', 'hint', 'source', 'split'))
+          45         214 LOAD_CONST              10 (('question', 'answer', 'options', 'category', 'L2-category', 'options_dict', 'index', 'hint', 'source', 'split'))
                      216 BUILD_CONST_KEY_MAP     10
                      218 STORE_FAST               5 (data)
          
-          47         220 LOAD_GLOBAL              7 (NULL + pd)
+          59         220 LOAD_GLOBAL              7 (NULL + pd)
                      232 LOAD_ATTR                4 (notna)
                      242 LOAD_FAST                5 (data)
                      244 LOAD_CONST               7 ('hint')
                      246 BINARY_SUBSCR
                      256 PRECALL                  1
                      260 CALL                     1
                      270 POP_JUMP_FORWARD_IF_FALSE    28 (to 328)
@@ -355,172 +451,341 @@
                      346 LOAD_FAST                5 (data)
                      348 LOAD_CONST              12 ('options')
                      350 BINARY_SUBSCR
                      360 FORMAT_VALUE             0
                      362 BUILD_STRING             3
                  >>  364 STORE_FAST               6 (query_prompt)
          
-          49         366 LOAD_FAST                1 (model_specific_prompt_kwargs)
+          61         366 LOAD_FAST                1 (model_specific_prompt_kwargs)
                      368 POP_JUMP_FORWARD_IF_FALSE    13 (to 396)
          
-          50         370 LOAD_FAST                6 (query_prompt)
+          62         370 LOAD_FAST                6 (query_prompt)
                      372 FORMAT_VALUE             0
                      374 LOAD_CONST              13 ('\n')
                      376 LOAD_FAST                1 (model_specific_prompt_kwargs)
                      378 LOAD_CONST              14 ('post_prompt')
                      380 BINARY_SUBSCR
                      390 FORMAT_VALUE             0
                      392 BUILD_STRING             3
                      394 STORE_FAST               6 (query_prompt)
          
-          52     >>  396 LOAD_FAST                6 (query_prompt)
+          64     >>  396 LOAD_FAST                6 (query_prompt)
                      398 RETURN_VALUE
          consts
             None
             ('A', 'B', 'C', 'D', 'E')
             'question'
             'answer'
             'category'
-            'l2-category'
+            'L2-category'
             'index'
             'hint'
             'source'
             'split'
             ('question', 'answer', 'options', 'category', 'L2-category', 'options_dict', 'index', 'hint', 'source', 'split')
             ' '
             'options'
             '\n'
             'post_prompt'
          names      ('mmbench_evaluator', 'create_options_prompt', 'get', 'pd', 'notna')
          varnames   ('doc', 'model_specific_prompt_kwargs', 'option_candidate', 'options_prompt', 'options_dict', 'data', 'query_prompt')
          freevars   ()
          cellvars   ()
-         filename   '/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/en_utils.py'
+         filename   '/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/cn_utils.py'
          name       'mmbench_doc_to_text'
-         firstlineno 29
+         firstlineno 41
          lnotab
             0x020108013c040e012a0102010e010e0102010e010e010e010ef5060e92
             0204011a02
       code
          argcount  : 2
          nlocals   : 6
          stacksize : 11
          flags     : 3
          code
             0x97007c01640119000000000000000000a0000000000000000000000000
-            000000000000000000a6000000ab0000000000000000007d0264027c0064
-            03190000000000000000007c006404190000000000000000007c00640519
-            0000000000000000007c027c006406190000000000000000007c00640719
-            0000000000000000007c006408190000000000000000007c006409190000
-            000000000000007c00640a19000000000000000000640b9c0969017d0367
-            00640ca2017d047c0444005d217d057c00a0010000000000000000000000
+            000000000000000000a6000000ab0000000000000000007d027c00640219
+            0000000000000000007c006403190000000000000000007c006404190000
+            000000000000007c027c006405190000000000000000007c006406190000
+            000000000000007c006407190000000000000000007c0064081900000000
+            00000000007c00640919000000000000000000640a9c097c006402190000
+            000000000000007c006403190000000000000000007c0064041900000000
+            00000000007c027c006405190000000000000000007c0064061900000000
+            00000000007c006407190000000000000000007c00640819000000000000
+            0000007c00640919000000000000000000640a9c09640b9c027d03670064
+            0ca2017d047c0444005d407d057c00a00100000000000000000000000000
+            000000000000007c05640da6020000ab0200000000000000007c03640e19
+            0000000000000000007c053c0000007c00a0010000000000000000000000
             0000000000000000007c05640da6020000ab0200000000000000007c0364
-            02190000000000000000007c053c0000008c227c035300
-          55           0 RESUME                   0
+            0f190000000000000000007c053c0000008c417c035300
+          67           0 RESUME                   0
          
-          56           2 LOAD_FAST                1 (results)
+          68           2 LOAD_FAST                1 (results)
                        4 LOAD_CONST               1 (0)
                        6 BINARY_SUBSCR
                       16 LOAD_METHOD              0 (strip)
                       38 PRECALL                  0
                       42 CALL                     0
                       52 STORE_FAST               2 (model_response)
          
-          58          54 LOAD_CONST               2 ('submission')
+          71          54 LOAD_FAST                0 (doc)
+                      56 LOAD_CONST               2 ('index')
+                      58 BINARY_SUBSCR
          
-          59          56 LOAD_FAST                0 (doc)
-                      58 LOAD_CONST               3 ('index')
-                      60 BINARY_SUBSCR
+          72          68 LOAD_FAST                0 (doc)
+                      70 LOAD_CONST               3 ('question')
+                      72 BINARY_SUBSCR
          
-          60          70 LOAD_FAST                0 (doc)
-                      72 LOAD_CONST               4 ('question')
-                      74 BINARY_SUBSCR
+          73          82 LOAD_FAST                0 (doc)
+                      84 LOAD_CONST               4 ('answer')
+                      86 BINARY_SUBSCR
          
-          61          84 LOAD_FAST                0 (doc)
-                      86 LOAD_CONST               5 ('answer')
-                      88 BINARY_SUBSCR
-         
-          62          98 LOAD_FAST                2 (model_response)
-         
-          63         100 LOAD_FAST                0 (doc)
-                     102 LOAD_CONST               6 ('hint')
-                     104 BINARY_SUBSCR
-         
-          64         114 LOAD_FAST                0 (doc)
-                     116 LOAD_CONST               7 ('source')
-                     118 BINARY_SUBSCR
+          74          96 LOAD_FAST                2 (model_response)
          
-          65         128 LOAD_FAST                0 (doc)
-                     130 LOAD_CONST               8 ('split')
-                     132 BINARY_SUBSCR
+          75          98 LOAD_FAST                0 (doc)
+                     100 LOAD_CONST               5 ('hint')
+                     102 BINARY_SUBSCR
          
-          66         142 LOAD_FAST                0 (doc)
-                     144 LOAD_CONST               9 ('category')
-                     146 BINARY_SUBSCR
+          76         112 LOAD_FAST                0 (doc)
+                     114 LOAD_CONST               6 ('source')
+                     116 BINARY_SUBSCR
          
-          67         156 LOAD_FAST                0 (doc)
-                     158 LOAD_CONST              10 ('l2-category')
-                     160 BINARY_SUBSCR
-         
-          58         170 LOAD_CONST              11 (('index', 'question', 'answer', 'prediction', 'hint', 'source', 'split', 'category', 'L2-category'))
-                     172 BUILD_CONST_KEY_MAP      9
-         
-          57         174 BUILD_MAP                1
-                     176 STORE_FAST               3 (data)
-         
-          70         178 BUILD_LIST               0
-                     180 LOAD_CONST              12 (('A', 'B', 'C', 'D', 'E'))
-                     182 LIST_EXTEND              1
-                     184 STORE_FAST               4 (option_candidate)
-         
-          71         186 LOAD_FAST                4 (option_candidate)
-                     188 GET_ITER
-                 >>  190 FOR_ITER                33 (to 258)
-                     192 STORE_FAST               5 (c)
-         
-          72         194 LOAD_FAST                0 (doc)
-                     196 LOAD_METHOD              1 (get)
-                     218 LOAD_FAST                5 (c)
-                     220 LOAD_CONST              13 ('nan')
-                     222 PRECALL                  2
-                     226 CALL                     2
-                     236 LOAD_FAST                3 (data)
-                     238 LOAD_CONST               2 ('submission')
-                     240 BINARY_SUBSCR
-                     250 LOAD_FAST                5 (c)
-                     252 STORE_SUBSCR
-                     256 JUMP_BACKWARD           34 (to 190)
+          77         126 LOAD_FAST                0 (doc)
+                     128 LOAD_CONST               7 ('split')
+                     130 BINARY_SUBSCR
          
-          73     >>  258 LOAD_FAST                3 (data)
-                     260 RETURN_VALUE
+          78         140 LOAD_FAST                0 (doc)
+                     142 LOAD_CONST               8 ('category')
+                     144 BINARY_SUBSCR
+         
+          79         154 LOAD_FAST                0 (doc)
+                     156 LOAD_CONST               9 ('L2-category')
+                     158 BINARY_SUBSCR
+         
+          70         168 LOAD_CONST              10 (('index', 'question', 'answer', 'prediction', 'hint', 'source', 'split', 'category', 'L2-category'))
+                     170 BUILD_CONST_KEY_MAP      9
+         
+          82         172 LOAD_FAST                0 (doc)
+                     174 LOAD_CONST               2 ('index')
+                     176 BINARY_SUBSCR
+         
+          83         186 LOAD_FAST                0 (doc)
+                     188 LOAD_CONST               3 ('question')
+                     190 BINARY_SUBSCR
+         
+          84         200 LOAD_FAST                0 (doc)
+                     202 LOAD_CONST               4 ('answer')
+                     204 BINARY_SUBSCR
+         
+          85         214 LOAD_FAST                2 (model_response)
+         
+          86         216 LOAD_FAST                0 (doc)
+                     218 LOAD_CONST               5 ('hint')
+                     220 BINARY_SUBSCR
+         
+          87         230 LOAD_FAST                0 (doc)
+                     232 LOAD_CONST               6 ('source')
+                     234 BINARY_SUBSCR
+         
+          88         244 LOAD_FAST                0 (doc)
+                     246 LOAD_CONST               7 ('split')
+                     248 BINARY_SUBSCR
+         
+          89         258 LOAD_FAST                0 (doc)
+                     260 LOAD_CONST               8 ('category')
+                     262 BINARY_SUBSCR
+         
+          90         272 LOAD_FAST                0 (doc)
+                     274 LOAD_CONST               9 ('L2-category')
+                     276 BINARY_SUBSCR
+         
+          81         286 LOAD_CONST              10 (('index', 'question', 'answer', 'prediction', 'hint', 'source', 'split', 'category', 'L2-category'))
+                     288 BUILD_CONST_KEY_MAP      9
+         
+          69         290 LOAD_CONST              11 (('gpt_eval_score', 'submission'))
+                     292 BUILD_CONST_KEY_MAP      2
+                     294 STORE_FAST               3 (data)
+         
+          93         296 BUILD_LIST               0
+                     298 LOAD_CONST              12 (('A', 'B', 'C', 'D', 'E'))
+                     300 LIST_EXTEND              1
+                     302 STORE_FAST               4 (option_candidate)
+         
+          94         304 LOAD_FAST                4 (option_candidate)
+                     306 GET_ITER
+                 >>  308 FOR_ITER                64 (to 438)
+                     310 STORE_FAST               5 (c)
+         
+          95         312 LOAD_FAST                0 (doc)
+                     314 LOAD_METHOD              1 (get)
+                     336 LOAD_FAST                5 (c)
+                     338 LOAD_CONST              13 ('nan')
+                     340 PRECALL                  2
+                     344 CALL                     2
+                     354 LOAD_FAST                3 (data)
+                     356 LOAD_CONST              14 ('submission')
+                     358 BINARY_SUBSCR
+                     368 LOAD_FAST                5 (c)
+                     370 STORE_SUBSCR
+         
+          96         374 LOAD_FAST                0 (doc)
+                     376 LOAD_METHOD              1 (get)
+                     398 LOAD_FAST                5 (c)
+                     400 LOAD_CONST              13 ('nan')
+                     402 PRECALL                  2
+                     406 CALL                     2
+                     416 LOAD_FAST                3 (data)
+                     418 LOAD_CONST              15 ('gpt_eval_score')
+                     420 BINARY_SUBSCR
+                     430 LOAD_FAST                5 (c)
+                     432 STORE_SUBSCR
+                     436 JUMP_BACKWARD           65 (to 308)
+         
+          97     >>  438 LOAD_FAST                3 (data)
+                     440 RETURN_VALUE
          consts
             None
             0
-            'submission'
             'index'
             'question'
             'answer'
             'hint'
             'source'
             'split'
             'category'
-            'l2-category'
+            'L2-category'
             ('index', 'question', 'answer', 'prediction', 'hint', 'source', 'split', 'category', 'L2-category')
+            ('gpt_eval_score', 'submission')
             ('A', 'B', 'C', 'D', 'E')
             'nan'
+            'submission'
+            'gpt_eval_score'
          names      ('strip', 'get')
          varnames   ('doc', 'results', 'model_response', 'data', 'option_candidate', 'c')
          freevars   ()
          cellvars   ()
-         filename   '/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/en_utils.py'
+         filename   '/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/cn_utils.py'
          name       'mmbench_process_results'
-         firstlineno 55
+         firstlineno 67
          lnotab
-            0x0201340202010e010e010e0102010e010e010e010e010ef704ff040d08
-            0108014001
+            0x020134030e010e010e0102010e010e010e010e010ef7040c0e010e010e
+            0102010e010e010e010e010ef704f40618080108013e014001
+      code
+         argcount  : 2
+         nlocals   : 8
+         stacksize : 6
+         flags     : 3
+         code
+            0x97007401000000000000000000006401a6010000ab0100000000000000
+            000100740200000000000000000000a00200000000000000000000000000
+            000000000000007c006402ac03a6020000ab0200000000000000005c0300
+            007d027d037d0474070000000000000000000064047c01a6020000ab0200
+            000000000000007d057c027c037c0464059c037d06740900000000000000
+            0000007c056406a6020000ab02000000000000000035007d07740b000000
+            000000000000006a0600000000000000007c067c07a6020000ab02000000
+            00000000000100640064006400a6020000ab02000000000000000001006e
+            0b230031007304770278035900770101005900010001007c0264077a0500
+            005300
+         100           0 RESUME                   0
+         
+         101           2 LOAD_GLOBAL              1 (NULL + print)
+                      14 LOAD_CONST               1 ('============= MMBench-CN(Dev) Detailed Results =============')
+                      16 PRECALL                  1
+                      20 CALL                     1
+                      30 POP_TOP
+         
+         102          32 LOAD_GLOBAL              2 (mmbench_evaluator)
+                      44 LOAD_METHOD              2 (eval_result)
+                      66 LOAD_FAST                0 (results)
+                      68 LOAD_CONST               2 ('openai')
+                      70 KW_NAMES                 3
+                      72 PRECALL                  2
+                      76 CALL                     2
+                      86 UNPACK_SEQUENCE          3
+                      90 STORE_FAST               2 (overall_acc)
+                      92 STORE_FAST               3 (category_acc)
+                      94 STORE_FAST               4 (l2_category_acc)
+         
+         103          96 LOAD_GLOBAL              7 (NULL + generate_submission_file)
+                     108 LOAD_CONST               4 ('mmbench_cn_dev_results.json')
+                     110 LOAD_FAST                1 (args)
+                     112 PRECALL                  2
+                     116 CALL                     2
+                     126 STORE_FAST               5 (file)
+         
+         105         128 LOAD_FAST                2 (overall_acc)
+         
+         106         130 LOAD_FAST                3 (category_acc)
+         
+         107         132 LOAD_FAST                4 (l2_category_acc)
+         
+         104         134 LOAD_CONST               5 (('overall_acc', 'category_acc', 'l2_category_acc'))
+                     136 BUILD_CONST_KEY_MAP      3
+                     138 STORE_FAST               6 (details_info)
+         
+         109         140 LOAD_GLOBAL              9 (NULL + open)
+                     152 LOAD_FAST                5 (file)
+                     154 LOAD_CONST               6 ('w')
+                     156 PRECALL                  2
+                     160 CALL                     2
+                     170 BEFORE_WITH
+                     172 STORE_FAST               7 (f)
+         
+         110         174 LOAD_GLOBAL             11 (NULL + json)
+                     186 LOAD_ATTR                6 (dump)
+                     196 LOAD_FAST                6 (details_info)
+                     198 LOAD_FAST                7 (f)
+                     200 PRECALL                  2
+                     204 CALL                     2
+                     214 POP_TOP
+         
+         109         216 LOAD_CONST               0 (None)
+                     218 LOAD_CONST               0 (None)
+                     220 LOAD_CONST               0 (None)
+                     222 PRECALL                  2
+                     226 CALL                     2
+                     236 POP_TOP
+                     238 JUMP_FORWARD            11 (to 262)
+                 >>  240 PUSH_EXC_INFO
+                     242 WITH_EXCEPT_START
+                     244 POP_JUMP_FORWARD_IF_TRUE     4 (to 254)
+                     246 RERAISE                  2
+                 >>  248 COPY                     3
+                     250 POP_EXCEPT
+                     252 RERAISE                  1
+                 >>  254 POP_TOP
+                     256 POP_EXCEPT
+                     258 POP_TOP
+                     260 POP_TOP
+         
+         111     >>  262 LOAD_FAST                2 (overall_acc)
+                     264 LOAD_CONST               7 (100)
+                     266 BINARY_OP                5 (*)
+                     270 RETURN_VALUE
+         ExceptionTable:
+           172 to 214 -> 240 [1] lasti
+           240 to 246 -> 248 [3] lasti
+           254 to 254 -> 248 [3] lasti
+         consts
+            None
+            '============= MMBench-CN(Dev) Detailed Results ============='
+            'openai'
+            ('eval_method',)
+            'mmbench_cn_dev_results.json'
+            ('overall_acc', 'category_acc', 'l2_category_acc')
+            'w'
+            100
+         names      ('print', 'mmbench_evaluator', 'eval_result', 'generate_submission_file', 'open', 'json', 'dump')
+         varnames   ('results', 'args', 'overall_acc', 'category_acc', 'l2_category_acc', 'file', 'details_info', 'f')
+         freevars   ()
+         cellvars   ()
+         filename   '/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/cn_utils.py'
+         name       'mmbench_aggregate_dev_results_eval'
+         firstlineno 100
+         lnotab 0x02011e01400120020201020102fd060522012aff2e02
       code
          argcount  : 2
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
             0x97007401000000000000000000006a0100000000000000007c00a60100
@@ -529,48 +794,48 @@
             000000000000007c03a6010000ab01000000000000000035007d047c02a0
             0400000000000000000000000000000000000000007c046402ac03a60200
             00ab0200000000000000000100640064006400a6020000ab020000000000
             00000001006e0b2300310073047702780359007701010059000100010074
             0a00000000000000000000a0060000000000000000000000000000000000
             00000064047c039b009d02a6010000ab0100000000000000000100640053
             00
-          76           0 RESUME                   0
+         114           0 RESUME                   0
          
-          77           2 LOAD_GLOBAL              1 (NULL + pd)
+         115           2 LOAD_GLOBAL              1 (NULL + pd)
                       14 LOAD_ATTR                1 (DataFrame)
                       24 LOAD_FAST                0 (results)
                       26 PRECALL                  1
                       30 CALL                     1
                       40 STORE_FAST               2 (df)
          
-          78          42 LOAD_GLOBAL              5 (NULL + generate_submission_file)
-                      54 LOAD_CONST               1 ('mmbench_en_dev_results.xlsx')
+         116          42 LOAD_GLOBAL              5 (NULL + generate_submission_file)
+                      54 LOAD_CONST               1 ('mmbench_cn_dev_results.xlsx')
                       56 LOAD_FAST                1 (args)
                       58 PRECALL                  2
                       62 CALL                     2
                       72 STORE_FAST               3 (excel_write_path)
          
-          79          74 LOAD_GLOBAL              1 (NULL + pd)
+         117          74 LOAD_GLOBAL              1 (NULL + pd)
                       86 LOAD_ATTR                3 (ExcelWriter)
                       96 LOAD_FAST                3 (excel_write_path)
                       98 PRECALL                  1
                      102 CALL                     1
                      112 BEFORE_WITH
                      114 STORE_FAST               4 (writer)
          
-          80         116 LOAD_FAST                2 (df)
+         118         116 LOAD_FAST                2 (df)
                      118 LOAD_METHOD              4 (to_excel)
                      140 LOAD_FAST                4 (writer)
                      142 LOAD_CONST               2 (False)
                      144 KW_NAMES                 3
                      146 PRECALL                  2
                      150 CALL                     2
                      160 POP_TOP
          
-          79         162 LOAD_CONST               0 (None)
+         117         162 LOAD_CONST               0 (None)
                      164 LOAD_CONST               0 (None)
                      166 LOAD_CONST               0 (None)
                      168 PRECALL                  2
                      172 CALL                     2
                      182 POP_TOP
                      184 JUMP_FORWARD            11 (to 208)
                  >>  186 PUSH_EXC_INFO
@@ -581,15 +846,15 @@
                      196 POP_EXCEPT
                      198 RERAISE                  1
                  >>  200 POP_TOP
                      202 POP_EXCEPT
                      204 POP_TOP
                      206 POP_TOP
          
-          81     >>  208 LOAD_GLOBAL             10 (eval_logger)
+         119     >>  208 LOAD_GLOBAL             10 (eval_logger)
                      220 LOAD_METHOD              6 (info)
                      242 LOAD_CONST               4 ('Saved results to ')
                      244 LOAD_FAST                3 (excel_write_path)
                      246 FORMAT_VALUE             0
                      248 BUILD_STRING             2
                      250 PRECALL                  1
                      254 CALL                     1
@@ -598,155 +863,128 @@
                      268 RETURN_VALUE
          ExceptionTable:
            114 to 160 -> 186 [1] lasti
            186 to 192 -> 194 [3] lasti
            200 to 200 -> 194 [3] lasti
          consts
             None
-            'mmbench_en_dev_results.xlsx'
+            'mmbench_cn_dev_results.xlsx'
             False
             ('index',)
             'Saved results to '
          names      ('pd', 'DataFrame', 'generate_submission_file', 'ExcelWriter', 'to_excel', 'eval_logger', 'info')
          varnames   ('results', 'args', 'df', 'excel_write_path', 'writer')
          freevars   ()
          cellvars   ()
-         filename   '/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/en_utils.py'
+         filename   '/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/cn_utils.py'
          name       'mmbench_aggregate_dev_results'
-         firstlineno 76
+         firstlineno 114
          lnotab 0x0201280120012a012eff2e02
       code
          argcount  : 2
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
             0x97007401000000000000000000006a0100000000000000007c00a60100
-            00ab0100000000000000007d027405000000000000000000007c016a0300
-            00000000000000a6010000ab010000000000000000a00400000000000000
-            000000000000000000000000006401a6010000ab010000000000000000a0
-            05000000000000000000000000000000000000000064026402ac03a60200
-            00ab02000000000000000001007405000000000000000000007c016a0300
-            00000000000000a6010000ab01000000000000000064017a0b000064047a
-            0b00007d037401000000000000000000006a0600000000000000007c03a6
-            010000ab01000000000000000035007d047c02a007000000000000000000
-            00000000000000000000007c046405ac06a6020000ab0200000000000000
-            000100640064006400a6020000ab02000000000000000001006e0b230031
-            007304770278035900770101005900010001007410000000000000000000
-            00a009000000000000000000000000000000000000000064077c039b009d
-            02a6010000ab010000000000000000010064005300
-          84           0 RESUME                   0
+            00ab0100000000000000007d0274050000000000000000000064017c01a6
+            020000ab0200000000000000007d037401000000000000000000006a0300
+            000000000000007c03a6010000ab01000000000000000035007d047c02a0
+            0400000000000000000000000000000000000000007c046402ac03a60200
+            00ab0200000000000000000100640064006400a6020000ab020000000000
+            00000001006e0b2300310073047702780359007701010059000100010074
+            0a00000000000000000000a0060000000000000000000000000000000000
+            00000064047c039b009d02a6010000ab0100000000000000000100640053
+            00
+         122           0 RESUME                   0
          
-          85           2 LOAD_GLOBAL              1 (NULL + pd)
+         123           2 LOAD_GLOBAL              1 (NULL + pd)
                       14 LOAD_ATTR                1 (DataFrame)
                       24 LOAD_FAST                0 (results)
                       26 PRECALL                  1
                       30 CALL                     1
                       40 STORE_FAST               2 (df)
          
-          86          42 LOAD_GLOBAL              5 (NULL + Path)
-                      54 LOAD_FAST                1 (args)
-                      56 LOAD_ATTR                3 (output_path)
-                      66 PRECALL                  1
-                      70 CALL                     1
-                      80 LOAD_METHOD              4 (joinpath)
-                     102 LOAD_CONST               1 ('submissions')
-                     104 PRECALL                  1
-                     108 CALL                     1
-                     118 LOAD_METHOD              5 (mkdir)
-                     140 LOAD_CONST               2 (True)
-                     142 LOAD_CONST               2 (True)
+         124          42 LOAD_GLOBAL              5 (NULL + generate_submission_file)
+                      54 LOAD_CONST               1 ('mmbench_cn_test_results.xlsx')
+                      56 LOAD_FAST                1 (args)
+                      58 PRECALL                  2
+                      62 CALL                     2
+                      72 STORE_FAST               3 (excel_write_path)
+         
+         125          74 LOAD_GLOBAL              1 (NULL + pd)
+                      86 LOAD_ATTR                3 (ExcelWriter)
+                      96 LOAD_FAST                3 (excel_write_path)
+                      98 PRECALL                  1
+                     102 CALL                     1
+                     112 BEFORE_WITH
+                     114 STORE_FAST               4 (writer)
+         
+         126         116 LOAD_FAST                2 (df)
+                     118 LOAD_METHOD              4 (to_excel)
+                     140 LOAD_FAST                4 (writer)
+                     142 LOAD_CONST               2 (False)
                      144 KW_NAMES                 3
                      146 PRECALL                  2
                      150 CALL                     2
                      160 POP_TOP
          
-          87         162 LOAD_GLOBAL              5 (NULL + Path)
-                     174 LOAD_FAST                1 (args)
-                     176 LOAD_ATTR                3 (output_path)
-                     186 PRECALL                  1
-                     190 CALL                     1
-                     200 LOAD_CONST               1 ('submissions')
-                     202 BINARY_OP               11 (/)
-                     206 LOAD_CONST               4 ('mmbench_en_test_results.xlsx')
-                     208 BINARY_OP               11 (/)
-                     212 STORE_FAST               3 (excel_write_path)
-         
-          88         214 LOAD_GLOBAL              1 (NULL + pd)
-                     226 LOAD_ATTR                6 (ExcelWriter)
-                     236 LOAD_FAST                3 (excel_write_path)
-                     238 PRECALL                  1
-                     242 CALL                     1
-                     252 BEFORE_WITH
-                     254 STORE_FAST               4 (writer)
-         
-          89         256 LOAD_FAST                2 (df)
-                     258 LOAD_METHOD              7 (to_excel)
-                     280 LOAD_FAST                4 (writer)
-                     282 LOAD_CONST               5 (False)
-                     284 KW_NAMES                 6
-                     286 PRECALL                  2
-                     290 CALL                     2
-                     300 POP_TOP
-         
-          88         302 LOAD_CONST               0 (None)
-                     304 LOAD_CONST               0 (None)
-                     306 LOAD_CONST               0 (None)
-                     308 PRECALL                  2
-                     312 CALL                     2
-                     322 POP_TOP
-                     324 JUMP_FORWARD            11 (to 348)
-                 >>  326 PUSH_EXC_INFO
-                     328 WITH_EXCEPT_START
-                     330 POP_JUMP_FORWARD_IF_TRUE     4 (to 340)
-                     332 RERAISE                  2
-                 >>  334 COPY                     3
-                     336 POP_EXCEPT
-                     338 RERAISE                  1
-                 >>  340 POP_TOP
-                     342 POP_EXCEPT
-                     344 POP_TOP
-                     346 POP_TOP
-         
-          90     >>  348 LOAD_GLOBAL             16 (eval_logger)
-                     360 LOAD_METHOD              9 (info)
-                     382 LOAD_CONST               7 ('Saved results to ')
-                     384 LOAD_FAST                3 (excel_write_path)
-                     386 FORMAT_VALUE             0
-                     388 BUILD_STRING             2
-                     390 PRECALL                  1
-                     394 CALL                     1
-                     404 POP_TOP
-                     406 LOAD_CONST               0 (None)
-                     408 RETURN_VALUE
+         125         162 LOAD_CONST               0 (None)
+                     164 LOAD_CONST               0 (None)
+                     166 LOAD_CONST               0 (None)
+                     168 PRECALL                  2
+                     172 CALL                     2
+                     182 POP_TOP
+                     184 JUMP_FORWARD            11 (to 208)
+                 >>  186 PUSH_EXC_INFO
+                     188 WITH_EXCEPT_START
+                     190 POP_JUMP_FORWARD_IF_TRUE     4 (to 200)
+                     192 RERAISE                  2
+                 >>  194 COPY                     3
+                     196 POP_EXCEPT
+                     198 RERAISE                  1
+                 >>  200 POP_TOP
+                     202 POP_EXCEPT
+                     204 POP_TOP
+                     206 POP_TOP
+         
+         127     >>  208 LOAD_GLOBAL             10 (eval_logger)
+                     220 LOAD_METHOD              6 (info)
+                     242 LOAD_CONST               4 ('Saved results to ')
+                     244 LOAD_FAST                3 (excel_write_path)
+                     246 FORMAT_VALUE             0
+                     248 BUILD_STRING             2
+                     250 PRECALL                  1
+                     254 CALL                     1
+                     264 POP_TOP
+                     266 LOAD_CONST               0 (None)
+                     268 RETURN_VALUE
          ExceptionTable:
-           254 to 300 -> 326 [1] lasti
-           326 to 332 -> 334 [3] lasti
-           340 to 340 -> 334 [3] lasti
+           114 to 160 -> 186 [1] lasti
+           186 to 192 -> 194 [3] lasti
+           200 to 200 -> 194 [3] lasti
          consts
             None
-            'submissions'
-            True
-            ('parents', 'exist_ok')
-            'mmbench_en_test_results.xlsx'
+            'mmbench_cn_test_results.xlsx'
             False
             ('index',)
             'Saved results to '
-         names      ('pd', 'DataFrame', 'Path', 'output_path', 'joinpath', 'mkdir', 'ExcelWriter', 'to_excel', 'eval_logger', 'info')
+         names      ('pd', 'DataFrame', 'generate_submission_file', 'ExcelWriter', 'to_excel', 'eval_logger', 'info')
          varnames   ('results', 'args', 'df', 'excel_write_path', 'writer')
          freevars   ()
          cellvars   ()
-         filename   '/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/en_utils.py'
+         filename   '/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/cn_utils.py'
          name       'mmbench_aggregate_test_results'
-         firstlineno 84
-         lnotab 0x02012801780134012a012eff2e02
+         firstlineno 122
+         lnotab 0x0201280120012a012eff2e02
       (None,)
-   names      ('logging', 'yaml', 'os', 'pathlib', 'Path', 'pandas', 'pd', 'json', 'getLogger', 'eval_logger', 'lmms_eval.tasks.mmbench.mmbench_evals', 'MMBench_Evaluator', 'lmms_eval.tasks._task_utils.file_utils', 'generate_submission_file', 'open', '__file__', 'parent', 'f', 'readlines', 'raw_data', 'safe_data', 'enumerate', 'i', 'line', 'append', 'safe_load', 'join', 'config', 'mmbench_evaluator', 'mmbench_doc_to_visual', 'mmbench_doc_to_text', 'mmbench_process_results', 'mmbench_aggregate_dev_results', 'mmbench_aggregate_test_results')
+   names      ('logging', 'yaml', 'os', 'pathlib', 'Path', 'pandas', 'pd', 'json', 'lmms_eval.tasks._task_utils.file_utils', 'generate_submission_file', 'getLogger', 'eval_logger', 'lmms_eval.tasks.mmbench.mmbench_evals', 'MMBench_Evaluator', 'open', '__file__', 'parent', 'f', 'readlines', 'raw_data', 'safe_data', 'enumerate', 'i', 'line', 'append', 'safe_load', 'join', 'config', 'GPT_EVAL_MODEL_NAME', 'getenv', 'API_TYPE', 'API_URL', 'API_KEY', 'mmbench_evaluator', 'mmbench_doc_to_visual', 'mmbench_doc_to_text', 'mmbench_process_results', 'mmbench_aggregate_dev_results_eval', 'mmbench_aggregate_dev_results', 'mmbench_aggregate_test_results')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/en_utils.py'
+   filename   '/data/pufanyi/project/lmms-eval/lmms_eval/tasks/mmbench/cn_utils.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010801080108010c010801080220010c010c023c012801040120
-      0208012c0246f82e0a30030604081a06150608
+      0x00ff02010801080108010c01080108010c0220010c010c023c01280104
+      01200208012c0246f82e0a1c0122020c01220124010c0122012203360306
+      04081a0621060e0608
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/mmbench/cn_utils.py` & `lmms_eval-0.1.2/lmms_eval/tasks/mmbench/en_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 import logging
 import yaml
 import os
 from pathlib import Path
 import pandas as pd
 import json
-from lmms_eval.tasks._task_utils.file_utils import generate_submission_file
 
 eval_logger = logging.getLogger("lmms-eval")
 from lmms_eval.tasks.mmbench.mmbench_evals import MMBench_Evaluator
+from lmms_eval.tasks._task_utils.file_utils import generate_submission_file
 
-with open(Path(__file__).parent / "mmbench_cn.yaml", "r") as f:
+with open(Path(__file__).parent / "mmbench.yaml", "r") as f:
     raw_data = f.readlines()
     safe_data = []
     for i, line in enumerate(raw_data):
         # remove function definition since yaml load cannot handle it
         if "!function" not in line:
             safe_data.append(line)
 
     config = yaml.safe_load("".join(safe_data))
 
-mmbench_evaluator = MMBench_Evaluator(sys_prompt=config["metadata"]["sys_prompt"])
+GPT_EVAL_MODEL_NAME = config["metadata"]["gpt_eval_model_name"]
+API_TYPE = os.getenv("API_TYPE", "openai")
+
+if API_TYPE == "openai":
+    API_URL = os.getenv("OPENAI_API_URL", "https://api.openai.com/v1/chat/completions")
+    API_KEY = os.getenv("OPENAI_API_KEY", "YOUR_API_KEY")
+elif API_TYPE == "azure":
+    API_URL = os.getenv("AZURE_ENDPOINT", "https://api.cognitive.microsoft.com/sts/v1.0/issueToken")
+    API_KEY = os.getenv("AZURE_API_KEY", "YOUR_API_KEY")
+
+
+mmbench_evaluator = MMBench_Evaluator(sys_prompt=config["metadata"]["sys_prompt"], API_KEY=API_KEY, API_URL=API_URL, model_version=GPT_EVAL_MODEL_NAME)
 
 
 def mmbench_doc_to_visual(doc):
     return [doc["image"].convert("RGB")]
 
 
 def mmbench_doc_to_text(doc, model_specific_prompt_kwargs=None):
@@ -40,51 +51,76 @@
         "options_dict": options_dict,
         "index": doc["index"],
         "hint": doc["hint"],
         "source": doc["source"],
         "split": doc["split"],
     }
 
-    query_prompt = f"{data['hint']} {data['question']} {data['options']}" if pd.notna(data["hint"]) else f"{data['question']} {data['options']}"
+    query_prompt = f"{data['hint']} {data['question']} {data['options']}" if pd.notna(data["hint"]) and data["hint"] != "nan" else f"{data['question']} {data['options']}"
 
     if model_specific_prompt_kwargs:
         query_prompt = f"{query_prompt}\n{model_specific_prompt_kwargs['post_prompt']}"
 
     return query_prompt
 
 
 def mmbench_process_results(doc, results):
     model_response = results[0].strip()
     data = {
+        "gpt_eval_score": {
+            "index": doc["index"],
+            "question": doc["question"],
+            "answer": doc["answer"],
+            "prediction": model_response,
+            "hint": doc["hint"],
+            "source": doc["source"],
+            "split": doc["split"],
+            "category": doc["category"],
+            "L2-category": doc["L2-category"],
+        },
         "submission": {
             "index": doc["index"],
             "question": doc["question"],
             "answer": doc["answer"],
             "prediction": model_response,
             "hint": doc["hint"],
             "source": doc["source"],
             "split": doc["split"],
             "category": doc["category"],
             "L2-category": doc["L2-category"],
-        }
+        },
     }
     option_candidate = ["A", "B", "C", "D", "E"]
     for c in option_candidate:
         data["submission"][c] = doc.get(c, "nan")
+        data["gpt_eval_score"][c] = doc.get(c, "nan")
     return data
 
 
-def mmbench_aggregate_dev_results(results, args):
+def mmbench_aggregate_dev_results_eval(results, args):
+    print(f"============= MMBench-EN(Dev) Detailed Results =============")
+    overall_acc, category_acc, l2_category_acc = mmbench_evaluator.eval_result(results, eval_method="openai")
+    file = generate_submission_file("mmbench_en_dev_results.json", args)
+    details_info = {
+        "overall_acc": overall_acc,
+        "category_acc": category_acc,
+        "l2_category_acc": l2_category_acc,
+    }
+    with open(file, "w") as f:
+        json.dump(details_info, f)
+    return overall_acc * 100
+
+
+def mmbench_aggregate_dev_results_submission(results, args):
     df = pd.DataFrame(results)
-    excel_write_path = generate_submission_file("mmbench_cn_dev_results.xlsx", args)
+    excel_write_path = generate_submission_file("mmbench_en_dev_results.xlsx", args)
     with pd.ExcelWriter(excel_write_path) as writer:
         df.to_excel(writer, index=False)
     eval_logger.info(f"Saved results to {excel_write_path}")
 
 
 def mmbench_aggregate_test_results(results, args):
     df = pd.DataFrame(results)
-    Path(args.output_path).joinpath("submissions").mkdir(parents=True, exist_ok=True)
-    excel_write_path = Path(args.output_path) / "submissions" / f"mmbench_cn_test_results.xlsx"
+    excel_write_path = generate_submission_file("mmbench_en_test_results.xlsx", args)
     with pd.ExcelWriter(excel_write_path) as writer:
         df.to_excel(writer, index=False)
     eval_logger.info(f"Saved results to {excel_write_path}")
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/mmbench/mmbench_cc.yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/mmbench/mmbench_cc.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-dataset_path: lmms-lab/MMBench_CN
+dataset_path: lmms-lab/MMBench
+dataset_name: cc
 dataset_kwargs:
   token: True
-group: mmbench_cn
 task: "mmbench_cn_cc"
-dataset_name: "chinese_culture"
 test_split: test
 output_type: generate_until
 doc_to_visual: !function cc_utils.mmbench_doc_to_visual
 doc_to_text: !function cc_utils.mmbench_cn_cc_doc_to_text
 doc_to_target: "answer"
 generation_kwargs:
   max_new_tokens: 256
   temperature: 0
   top_p: 0
   num_beams: 1
   do_sample: false
 process_results: !function cc_utils.mmbench_cn_cc_process_results
 metric_list:
+  - metric: gpt_eval_score
+    aggregation: !function cc_utils.mmbench_cn_cc_aggregate_dev_results_eval
+    higher_is_better: true
   - metric: submission
     aggregation: !function cc_utils.mmbench_cn_cc_aggregate_results
 metadata:
   version: 0.0
-  gpt_eval_model_name: "gpt-3.5-turbo"
-  quick_extract: true
+  gpt_eval_model_name: "gpt-3.5-turbo-0613"
 
 model_specific_prompt_kwargs:
   default:
     pre_prompt: ""
     post_prompt: "\n请直接使用所提供的选项字母作为答案回答。"
 model_specific_generation_kwargs:
   llava:
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/mmbench/mmbench_cn_dev.yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/pope/pope.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-dataset_path: lmms-lab/MMBench_CN
+dataset_path: lmms-lab/POPE
 dataset_kwargs:
   token: True
-group: mmbench_cn
-task: "mmbench_cn_dev"
-dataset_name: "default"
-test_split: "dev"
+task: "pope"
+test_split: test
 output_type: generate_until
-doc_to_visual: !function cn_utils.mmbench_doc_to_visual
-doc_to_text: !function cn_utils.mmbench_doc_to_text
+doc_to_visual: !function utils.pope_doc_to_visual
+doc_to_text: !function utils.pope_doc_to_text
 doc_to_target: "answer"
 generation_kwargs:
-  max_new_tokens: 256
+  max_new_tokens: 128
   temperature: 0
   top_p: 0
   num_beams: 1
   do_sample: false
-process_results: !function cn_utils.mmbench_process_results
+process_results: !function utils.pope_process_results
 metric_list:
-  - metric: submission
-    aggregation: !function cn_utils.mmbench_aggregate_dev_results
+  - metric: pope_accuracy
+    aggregation: !function utils.pope_aggregate_accuracy
+    higher_is_better: true
+  - metric: pope_precision
+    aggregation: !function utils.pope_aggregate_precision
+    higher_is_better: true
+  - metric: pope_recall
+    aggregation: !function utils.pope_aggregate_recall
+    higher_is_better: true
+  - metric: pope_f1_score
+    aggregation: !function utils.pope_aggregate_f1_score
+    higher_is_better: true
+  - metric: pope_yes_ratio
+    aggregation: !function utils.pope_aggregate_yes_ratio
+    higher_is_better: true
 metadata:
-  version: 0.0
-  gpt_eval_model_name: "gpt-3.5-turbo"
-  quick_extract: true
-
-model_specific_prompt_kwargs:
-  default:
-    pre_prompt: ""
-    post_prompt: "\n请直接使用所提供的选项字母作为答案回答。"
-model_specific_generation_kwargs:
-  llava:
-    image_aspect_ratio: original
+  - version: 0.0
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/mmbench/mmbench_cn_test.yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/mmvet/mmvet.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,29 @@
-dataset_path: lmms-lab/MMBench_CN
+dataset_path: lmms-lab/MMVet
 dataset_kwargs:
   token: True
-task: "mmbench_cn_test"
-dataset_name: "default"
+task: "mmvet"
 test_split: test
 output_type: generate_until
-doc_to_visual: !function cn_utils.mmbench_doc_to_visual
-doc_to_text: !function cn_utils.mmbench_doc_to_text
-doc_to_target: "answer"
+doc_to_visual: !function utils.mmvet_doc_to_visual
+doc_to_text: !function utils.doc_to_text # Such that {{question}} will be replaced by doc["question"]
+doc_to_target: "{{answer}}"
 generation_kwargs:
-  max_new_tokens: 256
+  until:
+    - "ASSISTANT:"
+  max_new_tokens: 1024
   temperature: 0
   top_p: 0
   num_beams: 1
   do_sample: false
-process_results: !function cn_utils.mmbench_process_results
+process_results: !function utils.mmvet_process_results # apply gpt eval here
 metric_list:
-  - metric: submission
-    aggregation: !function cn_utils.mmbench_aggregate_test_results
+  - metric: gpt_eval_score
+    aggregation: !function utils.mmvet_aggregate_results
     higher_is_better: true
 metadata:
   version: 0.0
-  gpt_eval_model_name: "gpt-3.5-turbo"
-  quick_extract: true
-
+  gpt_eval_model_name: "gpt-4"
 model_specific_prompt_kwargs:
   default:
     pre_prompt: ""
-    post_prompt: "\n请直接使用所提供的选项字母作为答案回答。"
-model_specific_generation_kwargs:
-  llava:
-    image_aspect_ratio: original
+    post_prompt: ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/mmbench/mmbench_en_dev.yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/mmbench/_default_template_mmbench_cn_yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-dataset_path: lmms-lab/MMBench_EN
+dataset_path: lmms-lab/MMBench
 dataset_kwargs:
   token: True
-task: "mmbench_en_dev"
-test_split: dev
-output_type: generate_until
-doc_to_visual: !function en_utils.mmbench_doc_to_visual
-doc_to_text: !function en_utils.mmbench_doc_to_text
 doc_to_target: "answer"
+dataset_name: "cn"
+output_type: generate_until
+doc_to_visual: !function cn_utils.mmbench_doc_to_visual
+doc_to_text: !function cn_utils.mmbench_doc_to_text
 generation_kwargs:
-  until:
-    - "ASSISTANT:"
-  max_new_tokens: 1024
+  max_new_tokens: 256
   temperature: 0
   top_p: 0
   num_beams: 1
   do_sample: false
-process_results: !function en_utils.mmbench_process_results
-metric_list:
-  - metric: submission
-    aggregation: !function en_utils.mmbench_aggregate_dev_results
-metadata:
-  version: 0.0
+process_results: !function cn_utils.mmbench_process_results
+model_specific_prompt_kwargs:
+  default:
+    pre_prompt: ""
+    post_prompt: "\n请直接使用所提供的选项字母作为答案回答。"
+model_specific_generation_kwargs:
+  llava:
+    image_aspect_ratio: original
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/mmbench/mmbench_en_test.yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/mmmu/mmmu_test.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,19 @@
-dataset_path: lmms-lab/MMBench_EN
-dataset_kwargs:
-  token: True
-task: "mmbench_en_test"
+dataset_path: lmms-lab/MMMU
+task: "mmmu_test"
 test_split: test
 output_type: generate_until
-doc_to_visual: !function en_utils.mmbench_doc_to_visual
-doc_to_text: !function en_utils.mmbench_doc_to_text
+doc_to_visual: !function utils.mmmu_doc_to_visual
+doc_to_text: !function utils.mmmu_doc_to_text
 doc_to_target: "answer"
+# The return value of process_results will be used by metrics
+process_results: !function utils.mmmu_process_results
+# Note that the metric name can be either a registed metric function (such as the case for GQA) or a key name returned by process_results
 generation_kwargs:
-  max_new_tokens: 256
-  temperature: 0
-  top_p: 0
-  num_beams: 1
-  do_sample: false
-process_results: !function en_utils.mmbench_process_results
+  max_new_tokens: 16
+  image_aspect_ratio: original
 metric_list:
   - metric: submission
-    aggregation: !function en_utils.mmbench_aggregate_test_results
+    aggregation: !function utils.mmmu_test_aggregate_results_for_submission
     higher_is_better: true
 metadata:
-  version: 0.0
+  - version: 0.0
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/mme/__pycache__/utils.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/mme/__pycache__/utils.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0008eb65 (Fri Mar  8 12:43:44 2024 UTC)
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
 files sz: 3925
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/mme/mme.yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/mme/mme.yaml`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/mme/utils.py` & `lmms_eval-0.1.2/lmms_eval/tasks/mme/utils.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/mmmu/__pycache__/utils.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/mmmu/__pycache__/utils.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0008eb65 (Fri Mar  8 12:43:44 2024 UTC)
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
 files sz: 16383
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/mmmu/mmmu_test.yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/nocaps/nocaps_test.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,25 @@
-dataset_path: lmms-lab/MMMU
-task: "mmmu_test"
+dataset_path: lmms-lab/NoCaps
+dataset_kwargs:
+  token: True
+task : "nocaps_test"
+group : "nocaps_caption"
 test_split: test
 output_type: generate_until
-doc_to_visual: !function utils.mmmu_doc_to_visual
-doc_to_text: !function utils.mmmu_doc_to_text
-doc_to_target: "answer"
-# The return value of process_results will be used by metrics
-process_results: !function utils.mmmu_process_results
-# Note that the metric name can be either a registed metric function (such as the case for GQA) or a key name returned by process_results
+doc_to_visual: !function utils.nocaps_doc_to_visual
+doc_to_text: !function utils.nocaps_doc_to_text
+doc_to_target: "annotations_captions"
 generation_kwargs:
-  max_new_tokens: 16
-  image_aspect_ratio: original
+  max_new_tokens: 64
+  temperature: 0
+  top_p: 0
+  num_beams: 1
+  do_sample: false
+process_results: !function utils.nocaps_test_process_result
+# Note that the metric name can be either a registed metric function (such as the case for GQA) or a key name returned by process_results
 metric_list:
-  - metric: submission
-    aggregation: !function utils.mmmu_test_aggregate_results_for_submission
-    higher_is_better: true
+  - metric: nocaps_passthrough 
+    aggregation : !function utils.nocaps_test_aggregation_result
+    higher_is_better : true
 metadata:
-  - version: 0.0
+  - version: 0.0
+include: _default_template_nocaps_yaml
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/mmmu/mmmu_val.yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/mmmu/mmmu_val.yaml`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/mmmu/utils.py` & `lmms_eval-0.1.2/lmms_eval/tasks/mmmu/utils.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/mmvet/__pycache__/utils.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/mmvet/__pycache__/utils.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0008eb65 (Fri Mar  8 12:43:44 2024 UTC)
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
 files sz: 9027
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/mmvet/utils.py` & `lmms_eval-0.1.2/lmms_eval/tasks/mmvet/utils.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/multidocvqa/__pycache__/utils.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/multidocvqa/__pycache__/utils.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0008eb65 (Fri Mar  8 12:43:44 2024 UTC)
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
 files sz: 3903
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/multidocvqa/multidocvqa_test.yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/multidocvqa/multidocvqa_test.yaml`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/multidocvqa/multidocvqa_val.yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/multidocvqa/multidocvqa_val.yaml`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/multidocvqa/utils.py` & `lmms_eval-0.1.2/lmms_eval/tasks/multidocvqa/utils.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/nocaps/__pycache__/utils.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/nocaps/__pycache__/utils.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0008eb65 (Fri Mar  8 12:43:44 2024 UTC)
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
 files sz: 5255
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/nocaps/nocaps_val.yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/nocaps/nocaps_val.yaml`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/nocaps/utils.py` & `lmms_eval-0.1.2/lmms_eval/tasks/nocaps/utils.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/ok_vqa/__pycache__/utils.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/ok_vqa/__pycache__/utils.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0008eb65 (Fri Mar  8 12:43:44 2024 UTC)
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
 files sz: 2233
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 3
    flags     : 0
    code
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/ok_vqa/_default_template_vqa_yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/ok_vqa/_default_template_vqa_yaml`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/ok_vqa/_generate_config.py` & `lmms_eval-0.1.2/lmms_eval/tasks/ok_vqa/_generate_config.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/ok_vqa/utils.py` & `lmms_eval-0.1.2/lmms_eval/tasks/ok_vqa/utils.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/pope/__pycache__/utils.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/pope/__pycache__/utils.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0008eb65 (Fri Mar  8 12:43:44 2024 UTC)
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
 files sz: 2991
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 1
    flags     : 0
    code
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/pope/pope.yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/refcocog/_default_template_seg_yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-dataset_path: lmms-lab/POPE
-dataset_kwargs:
-  token: True
-task: "pope"
-test_split: test
+dataset_path: lmms-lab/RefCOCOg
 output_type: generate_until
-doc_to_visual: !function utils.pope_doc_to_visual
-doc_to_text: !function utils.pope_doc_to_text
+doc_to_visual: !function utils.refcoco_seg_doc_to_visual
+doc_to_text: !function utils.refcoco_doc_to_text
 doc_to_target: "answer"
 generation_kwargs:
-  max_new_tokens: 128
-  temperature: 0
-  top_p: 0
-  num_beams: 1
-  do_sample: false
-process_results: !function utils.pope_process_results
+  until:
+    - "ASSISTANT:"
+process_results: !function utils.refcoco_process_result
 metric_list:
-  - metric: pope_accuracy
-    aggregation: !function utils.pope_aggregate_accuracy
-    higher_is_better: true
-  - metric: pope_precision
-    aggregation: !function utils.pope_aggregate_precision
-    higher_is_better: true
-  - metric: pope_recall
-    aggregation: !function utils.pope_aggregate_recall
-    higher_is_better: true
-  - metric: pope_f1_score
-    aggregation: !function utils.pope_aggregate_f1_score
-    higher_is_better: true
-  - metric: pope_yes_ratio
-    aggregation: !function utils.pope_aggregate_yes_ratio
-    higher_is_better: true
+  - metric: refcoco_Bleu_4 
+    aggregation : !function utils.refcoco_bleu4
+    higher_is_better : true
+  - metric: refcoco_Bleu_3
+    aggregation : !function utils.refcoco_bleu3
+    higher_is_better : true
+  - metric: refcoco_Bleu_2
+    aggregation : !function utils.refcoco_bleu2
+    higher_is_better : true
+  - metric: refcoco_Bleu_1
+    aggregation : !function utils.refcoco_bleu1
+    higher_is_better : true
+  - metric: refcoco_METEOR
+    aggregation : !function utils.refcoco_meteor
+    higher_is_better : true
+  - metric: refcoco_ROUGE_L
+    aggregation : !function utils.refcoco_rougel
+    higher_is_better : true
+  - metric: refcoco_CIDEr
+    aggregation : !function utils.refcoco_cider
+    higher_is_better : true
+  #- metric: refcoco_SPICE
+  #  aggregation : !function utils.refcoco_spice
+  #  higher_is_better : true
 metadata:
-  - version: 0.0
+  version: '0.0'
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/pope/utils.py` & `lmms_eval-0.1.2/lmms_eval/tasks/pope/utils.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/refcoco/__pycache__/utils.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/refcoco/__pycache__/utils.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0008eb65 (Fri Mar  8 12:43:44 2024 UTC)
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
 files sz: 4122
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 3
    flags     : 0
    code
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/refcoco/_default_template_bbox_yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/refcoco/_default_template_bbox_yaml`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/refcoco/_default_template_seg_yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/refcoco/_default_template_seg_yaml`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/refcoco/_generate_config.py` & `lmms_eval-0.1.2/lmms_eval/tasks/refcoco/_generate_config.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/refcoco/utils.py` & `lmms_eval-0.1.2/lmms_eval/tasks/refcoco/utils.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/refcoco+/__pycache__/utils.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/refcoco+/__pycache__/utils.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0008eb65 (Fri Mar  8 12:43:44 2024 UTC)
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
 files sz: 4122
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 3
    flags     : 0
    code
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/refcoco+/_default_template_bbox_yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/refcoco+/_default_template_bbox_yaml`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/refcoco+/_default_template_seg_yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/refcoco+/_default_template_seg_yaml`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/refcoco+/_generate_config.py` & `lmms_eval-0.1.2/lmms_eval/tasks/refcoco+/_generate_config.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/refcoco+/utils.py` & `lmms_eval-0.1.2/lmms_eval/tasks/refcoco+/utils.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/refcocog/__pycache__/utils.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/refcocog/__pycache__/utils.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0008eb65 (Fri Mar  8 12:43:44 2024 UTC)
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
 files sz: 4122
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 3
    flags     : 0
    code
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/refcocog/_default_template_bbox_yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/refcocog/_default_template_bbox_yaml`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/refcocog/_default_template_seg_yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/textcaps/textcaps_train.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,48 @@
-dataset_path: lmms-lab/RefCOCOg
+dataset_path: lmms-lab/TextCaps
+dataset_kwargs:
+  token: True
+task : "textcaps_train"
+group : "textcaps_caption"
+test_split: train
 output_type: generate_until
-doc_to_visual: !function utils.refcoco_seg_doc_to_visual
-doc_to_text: !function utils.refcoco_doc_to_text
+doc_to_visual: !function utils.textcaps_doc_to_visual
+doc_to_text: !function utils.textcaps_doc_to_text
 doc_to_target: "answer"
 generation_kwargs:
   until:
     - "ASSISTANT:"
-process_results: !function utils.refcoco_process_result
+  max_new_tokens: 1024
+  temperature: 0
+  top_p: 0
+  num_beams: 1
+  do_sample: false
+process_results: !function utils.textcaps_process_result
+# Note that the metric name can be either a registed metric function (such as the case for GQA) or a key name returned by process_results
 metric_list:
-  - metric: refcoco_Bleu_4 
-    aggregation : !function utils.refcoco_bleu4
+  - metric: textcaps_Bleu_4 
+    aggregation : !function utils.textcaps_bleu4
     higher_is_better : true
-  - metric: refcoco_Bleu_3
-    aggregation : !function utils.refcoco_bleu3
+  - metric: textcaps_Bleu_3
+    aggregation : !function utils.textcaps_bleu3
     higher_is_better : true
-  - metric: refcoco_Bleu_2
-    aggregation : !function utils.refcoco_bleu2
+  - metric: textcaps_Bleu_2
+    aggregation : !function utils.textcaps_bleu2
     higher_is_better : true
-  - metric: refcoco_Bleu_1
-    aggregation : !function utils.refcoco_bleu1
+  - metric: textcaps_Bleu_1
+    aggregation : !function utils.textcaps_bleu1
     higher_is_better : true
-  - metric: refcoco_METEOR
-    aggregation : !function utils.refcoco_meteor
+  - metric: textcaps_METEOR
+    aggregation : !function utils.textcaps_meteor
     higher_is_better : true
-  - metric: refcoco_ROUGE_L
-    aggregation : !function utils.refcoco_rougel
+  - metric: textcaps_ROUGE_L
+    aggregation : !function utils.textcaps_rougel
     higher_is_better : true
-  - metric: refcoco_CIDEr
-    aggregation : !function utils.refcoco_cider
+  - metric: textcaps_CIDEr
+    aggregation : !function utils.textcaps_cider
     higher_is_better : true
-  #- metric: refcoco_SPICE
-  #  aggregation : !function utils.refcoco_spice
+  #- metric: textcaps_SPICE
+  #  aggregation : !function utils.textcaps_spice
   #  higher_is_better : true
 metadata:
-  version: '0.0'
+  - version: 0.0
+include: _default_template_textcaps_yaml
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/refcocog/_generate_config.py` & `lmms_eval-0.1.2/lmms_eval/tasks/refcocog/_generate_config.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/refcocog/utils.py` & `lmms_eval-0.1.2/lmms_eval/tasks/refcocog/utils.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/scienceqa/__pycache__/utils.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/scienceqa/__pycache__/utils.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0008eb65 (Fri Mar  8 12:43:44 2024 UTC)
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
 files sz: 1729
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/scienceqa/scienceqa.yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/scienceqa/scienceqa.yaml`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/scienceqa/scienceqa_img.yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/scienceqa/scienceqa_img.yaml`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/scienceqa/utils.py` & `lmms_eval-0.1.2/lmms_eval/tasks/scienceqa/utils.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/seedbench/__pycache__/utils.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/seedbench/__pycache__/utils.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0008eb65 (Fri Mar  8 12:43:44 2024 UTC)
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
 files sz: 1820
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/seedbench/seedbench.yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/seedbench/seedbench.yaml`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/seedbench/seedbench_ppl.yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/seedbench/seedbench_ppl.yaml`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/seedbench/utils.py` & `lmms_eval-0.1.2/lmms_eval/tasks/seedbench/utils.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/seedbench_2/__pycache__/utils.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/seedbench_2/__pycache__/utils.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0008eb65 (Fri Mar  8 12:43:44 2024 UTC)
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
 files sz: 2188
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/seedbench_2/seedbench_2.yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/seedbench_2/seedbench_2.yaml`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/seedbench_2/utils.py` & `lmms_eval-0.1.2/lmms_eval/tasks/seedbench_2/utils.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/stvqa/__pycache__/utils.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/stvqa/__pycache__/utils.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0008eb65 (Fri Mar  8 12:43:44 2024 UTC)
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
 files sz: 858
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/stvqa/stvqa.yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/stvqa/stvqa.yaml`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/stvqa/utils.py` & `lmms_eval-0.1.2/lmms_eval/tasks/stvqa/utils.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/textcaps/__pycache__/utils.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/textcaps/__pycache__/utils.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0008eb65 (Fri Mar  8 12:43:44 2024 UTC)
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
 files sz: 5050
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/textcaps/textcaps_test.yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/textcaps/textcaps_test.yaml`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/textcaps/textcaps_train.yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/textcaps/textcaps_val.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 dataset_path: lmms-lab/TextCaps
 dataset_kwargs:
   token: True
-task : "textcaps_train"
+task: "textcaps_val"
 group : "textcaps_caption"
-test_split: train
+test_split: val
 output_type: generate_until
 doc_to_visual: !function utils.textcaps_doc_to_visual
 doc_to_text: !function utils.textcaps_doc_to_text
 doc_to_target: "answer"
 generation_kwargs:
-  until:
-    - "ASSISTANT:"
-  max_new_tokens: 1024
+  max_new_tokens: 64
   temperature: 0
   top_p: 0
   num_beams: 1
   do_sample: false
 process_results: !function utils.textcaps_process_result
 # Note that the metric name can be either a registed metric function (such as the case for GQA) or a key name returned by process_results
 metric_list:
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/textcaps/utils.py` & `lmms_eval-0.1.2/lmms_eval/tasks/textcaps/utils.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/textvqa/__pycache__/utils.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/textvqa/__pycache__/utils.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0008eb65 (Fri Mar  8 12:43:44 2024 UTC)
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
 files sz: 2362
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 3
    flags     : 0
    code
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/textvqa/utils.py` & `lmms_eval-0.1.2/lmms_eval/tasks/textvqa/utils.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/vizwiz_vqa/__pycache__/utils.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/vizwiz_vqa/__pycache__/utils.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0008eb65 (Fri Mar  8 12:43:44 2024 UTC)
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
 files sz: 2290
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 3
    flags     : 0
    code
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/vizwiz_vqa/_default_template_vqa_yaml` & `lmms_eval-0.1.2/lmms_eval/tasks/vizwiz_vqa/_default_template_vqa_yaml`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/vizwiz_vqa/_generate_config.py` & `lmms_eval-0.1.2/lmms_eval/tasks/vizwiz_vqa/_generate_config.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/vizwiz_vqa/utils.py` & `lmms_eval-0.1.2/lmms_eval/tasks/vizwiz_vqa/utils.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/vqav2/__pycache__/utils.cpython-311.pyc` & `lmms_eval-0.1.2/lmms_eval/tasks/vqav2/__pycache__/utils.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0008eb65 (Fri Mar  8 12:43:44 2024 UTC)
+moddate:  0x24691d66 (Mon Apr 15 17:51:32 2024 UTC)
 files sz: 3031
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 3
    flags     : 0
    code
```

### Comparing `lmms_eval-0.1.1/lmms_eval/tasks/vqav2/utils.py` & `lmms_eval-0.1.2/lmms_eval/tasks/vqav2/utils.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/lmms_eval/utils.py` & `lmms_eval-0.1.2/lmms_eval/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -407,14 +407,16 @@
         for (mf), v in dic.items():
             m, _, f = mf.partition(",")
             if m.endswith("_stderr"):
                 continue
 
             points = "N/A"
             if v is not None:
+                if 0 <= v <= 1:
+                    v *= 100
                 points = "%.4f" % v
 
             if m + "_stderr" + "," + f in dic:
                 if v is None:
                     se = "N/A"
                 else:
                     se = dic[m + "_stderr" + "," + f]
```

### Comparing `lmms_eval-0.1.1/lmms_eval.egg-info/PKG-INFO` & `lmms_eval-0.1.2/lmms_eval.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6c6d 6d73  : 2.1.Name: lmms
 00000020: 5f65 7661 6c0a 5665 7273 696f 6e3a 2030  _eval.Version: 0
-00000030: 2e31 2e31 0a53 756d 6d61 7279 3a20 4120  .1.1.Summary: A 
+00000030: 2e31 2e32 0a53 756d 6d61 7279 3a20 4120  .1.2.Summary: A 
 00000040: 6672 616d 6577 6f72 6b20 666f 7220 6576  framework for ev
 00000050: 616c 7561 7469 6e67 206c 6172 6765 206d  aluating large m
 00000060: 756c 7469 2d6d 6f64 616c 6974 7920 6c61  ulti-modality la
 00000070: 6e67 7561 6765 206d 6f64 656c 730a 4175  nguage models.Au
 00000080: 7468 6f72 2d65 6d61 696c 3a20 4c4d 4d4d  thor-email: LMMM
 00000090: 732d 4c61 6220 4576 616c 7561 7469 6f6e  s-Lab Evaluation
 000000a0: 2054 6561 6d20 3c6c 6d6d 735f 6576 616c   Team <lmms_eval
@@ -61,999 +61,1032 @@
 000003c0: 312e 380a 5265 7175 6972 6573 2d44 6973  1.8.Requires-Dis
 000003d0: 743a 206f 7065 6e61 693e 3d31 2e30 2e30  t: openai>=1.0.0
 000003e0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
 000003f0: 7079 636f 636f 6576 616c 6361 700a 5265  pycocoevalcap.Re
 00000400: 7175 6972 6573 2d44 6973 743a 2074 7164  quires-Dist: tqd
 00000410: 6d2d 6d75 6c74 6970 726f 6365 7373 0a52  m-multiprocess.R
 00000420: 6571 7569 7265 732d 4469 7374 3a20 7472  equires-Dist: tr
-00000430: 616e 7366 6f72 6d65 7273 3d3d 342e 3337  ansformers==4.37
-00000440: 2e32 0a52 6571 7569 7265 732d 4469 7374  .2.Requires-Dist
-00000450: 3a20 7a73 7461 6e64 6172 640a 5265 7175  : zstandard.Requ
-00000460: 6972 6573 2d44 6973 743a 2070 696c 6c6f  ires-Dist: pillo
-00000470: 770a 5265 7175 6972 6573 2d44 6973 743a  w.Requires-Dist:
-00000480: 2070 7979 616d 6c0a 5265 7175 6972 6573   pyyaml.Requires
-00000490: 2d44 6973 743a 2073 796d 7079 0a52 6571  -Dist: sympy.Req
-000004a0: 7569 7265 732d 4469 7374 3a20 6d70 6d61  uires-Dist: mpma
-000004b0: 7468 0a52 6571 7569 7265 732d 4469 7374  th.Requires-Dist
-000004c0: 3a20 4a69 6e6a 6132 0a52 6571 7569 7265  : Jinja2.Require
-000004d0: 732d 4469 7374 3a20 6f70 656e 7079 786c  s-Dist: openpyxl
-000004e0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000004f0: 4c65 7665 6e73 6874 6569 6e0a 5265 7175  Levenshtein.Requ
-00000500: 6972 6573 2d44 6973 743a 2068 665f 7472  ires-Dist: hf_tr
-00000510: 616e 7366 6572 0a52 6571 7569 7265 732d  ansfer.Requires-
-00000520: 4469 7374 3a20 7465 6e61 6369 7479 0a52  Dist: tenacity.R
-00000530: 6571 7569 7265 732d 4469 7374 3a20 7761  equires-Dist: wa
-00000540: 6e64 623e 3d30 2e31 362e 300a 5265 7175  ndb>=0.16.0.Requ
-00000550: 6972 6573 2d44 6973 743a 2074 7261 6e73  ires-Dist: trans
-00000560: 666f 726d 6572 732d 7374 7265 616d 2d67  formers-stream-g
-00000570: 656e 6572 6174 6f72 0a52 6571 7569 7265  enerator.Require
-00000580: 732d 4469 7374 3a20 7469 6b74 6f6b 656e  s-Dist: tiktoken
-00000590: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000005a0: 7072 652d 636f 6d6d 6974 0a52 6571 7569  pre-commit.Requi
-000005b0: 7265 732d 4469 7374 3a20 7079 6461 6e74  res-Dist: pydant
-000005c0: 6963 0a0a 3c70 2061 6c69 676e 3d22 6365  ic..<p align="ce
-000005d0: 6e74 6572 2220 7769 6474 683d 2231 3030  nter" width="100
-000005e0: 2522 3e0a 3c69 6d67 2073 7263 3d22 6874  %">.<img src="ht
-000005f0: 7470 733a 2f2f 692e 706f 7374 696d 672e  tps://i.postimg.
-00000600: 6363 2f67 3051 5267 4d56 762f 5758 3230  cc/g0QRgMVv/WX20
-00000610: 3234 3032 3238 2d31 3133 3333 372d 3278  240228-113337-2x
-00000620: 2e70 6e67 2220 2077 6964 7468 3d22 3130  .png"  width="10
-00000630: 3025 2220 6865 6967 6874 3d22 3730 2522  0%" height="70%"
-00000640: 3e0a 3c2f 703e 0a0a 2320 5468 6520 4576  >.</p>..# The Ev
-00000650: 616c 7561 7469 6f6e 2053 7569 7465 206f  aluation Suite o
-00000660: 6620 4c61 7267 6520 4d75 6c74 696d 6f64  f Large Multimod
-00000670: 616c 204d 6f64 656c 7320 0a0a 3e20 4163  al Models ..> Ac
-00000680: 6365 6c65 7261 7469 6e67 2074 6865 2064  celerating the d
-00000690: 6576 656c 6f70 6d65 6e74 206f 6620 6c61  evelopment of la
-000006a0: 7267 6520 6d75 6c74 696d 6f64 616c 206d  rge multimodal m
-000006b0: 6f64 656c 7320 284c 4d4d 7329 2077 6974  odels (LMMs) wit
-000006c0: 6820 606c 6d6d 732d 6576 616c 600a 0af0  h `lmms-eval`...
-000006d0: 9f8f a020 5b48 6f6d 6570 6167 655d 2868  ... [Homepage](h
-000006e0: 7474 7073 3a2f 2f6c 6d6d 732d 6c61 622e  ttps://lmms-lab.
-000006f0: 6769 7468 7562 2e69 6f2f 2920 7c20 20f0  github.io/) |  .
-00000700: 9f8e 8920 5b42 6c6f 675d 2868 7474 7073  ... [Blog](https
-00000710: 3a2f 2f6c 6d6d 732d 6c61 622e 6769 7468  ://lmms-lab.gith
-00000720: 7562 2e69 6f2f 6c6d 6d73 2d65 7661 6c2d  ub.io/lmms-eval-
-00000730: 626c 6f67 2f6c 6d6d 732d 6576 616c 2d30  blog/lmms-eval-0
-00000740: 2e31 2f29 207c 20f0 9f93 9a20 5b44 6f63  .1/) | .... [Doc
-00000750: 756d 656e 7461 7469 6f6e 5d28 646f 6373  umentation](docs
-00000760: 2f52 4541 444d 452e 6d64 2920 7c20 f09f  /README.md) | ..
-00000770: a497 205b 4875 6767 696e 6766 6163 6520  .. [Huggingface 
-00000780: 4461 7461 7365 7473 5d28 6874 7470 733a  Datasets](https:
-00000790: 2f2f 6875 6767 696e 6766 6163 652e 636f  //huggingface.co
-000007a0: 2f6c 6d6d 732d 6c61 6229 0a0a 496e 2061  /lmms-lab)..In a
-000007b0: 6e20 6572 6120 7768 6572 6520 7065 6f70  n era where peop
-000007c0: 6c65 2070 7572 7375 6520 4147 4920 2841  le pursue AGI (A
-000007d0: 7274 6966 6963 6961 6c20 4765 6e65 7261  rtificial Genera
-000007e0: 6c20 496e 7465 6c6c 6967 656e 6365 2920  l Intelligence) 
-000007f0: 7769 7468 2074 6865 207a 6561 6c20 616b  with the zeal ak
-00000800: 696e 2074 6f20 3139 3630 7320 6d6f 6f6e  in to 1960s moon
-00000810: 206c 616e 6469 6e67 206d 6973 7369 6f6e   landing mission
-00000820: 2e20 0a45 7661 6c75 6174 696e 6720 7468  . .Evaluating th
-00000830: 6520 636f 7265 206f 6620 4147 492c 2074  e core of AGI, t
-00000840: 6865 206c 6172 6765 206c 616e 6775 6167  he large languag
-00000850: 6520 6d6f 6465 6c73 2028 4c4c 4d73 2920  e models (LLMs) 
-00000860: 616e 6420 6c61 7267 6520 6d75 6c74 696d  and large multim
-00000870: 6f64 616c 206d 6f64 656c 7320 284c 4d4d  odal models (LMM
-00000880: 7329 2077 6974 6820 756e 7072 6563 6564  s) with unpreced
-00000890: 656e 7465 6420 6361 7061 6269 6c69 7469  ented capabiliti
-000008a0: 6573 2074 6861 7420 6361 6e20 756e 6465  es that can unde
-000008b0: 7273 7461 6e64 2c20 6c65 6172 6e2c 2061  rstand, learn, a
-000008c0: 6e64 2069 6e74 6572 6163 7420 6163 726f  nd interact acro
-000008d0: 7373 2061 2062 726f 6164 2072 616e 6765  ss a broad range
-000008e0: 206f 6620 6875 6d61 6e20 7461 736b 732c   of human tasks,
-000008f0: 2068 6173 2062 6563 6f6d 6520 6120 7069   has become a pi
-00000900: 766f 7461 6c20 6368 616c 6c65 6e67 652e  votal challenge.
-00000910: 0a0a 546f 2073 7572 6d6f 756e 7420 7468  ..To surmount th
-00000920: 6973 2c20 6120 6272 6f61 6420 7370 6563  is, a broad spec
-00000930: 7472 756d 206f 6620 6576 616c 7561 7469  trum of evaluati
-00000940: 6f6e 2064 6174 6173 6574 7320 6973 2070  on datasets is p
-00000950: 726f 706f 7365 6420 616e 6420 7573 6564  roposed and used
-00000960: 2074 6f20 6173 7365 7373 206d 6f64 656c   to assess model
-00000970: 2063 6170 6162 696c 6974 6965 7320 6163   capabilities ac
-00000980: 726f 7373 2076 6172 696f 7573 2064 696d  ross various dim
-00000990: 656e 7369 6f6e 732c 2063 7265 6174 696e  ensions, creatin
-000009a0: 6720 6120 636f 6d70 7265 6865 6e73 6976  g a comprehensiv
-000009b0: 6520 6361 7061 6269 6c69 7479 2063 6861  e capability cha
-000009c0: 7274 2074 6861 7420 7265 7665 616c 7320  rt that reveals 
-000009d0: 7468 6520 7472 7565 2070 6572 666f 726d  the true perform
-000009e0: 616e 6365 206f 6620 6d6f 6465 6c73 2e20  ance of models. 
-000009f0: 486f 7765 7665 722c 2065 7661 6c75 6174  However, evaluat
-00000a00: 696f 6e20 6f66 206d 6f64 656c 7320 6861  ion of models ha
-00000a10: 7320 6265 636f 6d65 2071 7569 7465 2068  s become quite h
-00000a20: 6172 6420 7369 6e63 6520 7468 6572 6520  ard since there 
-00000a30: 6172 6520 636f 756e 746c 6573 7320 6576  are countless ev
-00000a40: 616c 7561 7469 6f6e 2062 656e 6368 6d61  aluation benchma
-00000a50: 726b 7320 616e 6420 6461 7461 7365 7473  rks and datasets
-00000a60: 206f 7267 616e 697a 6564 2069 6e20 7661   organized in va
-00000a70: 7269 6f75 7320 7761 7973 2c20 7363 6174  rious ways, scat
-00000a80: 7465 7265 6420 6163 726f 7373 2074 6865  tered across the
-00000a90: 2069 6e74 6572 6e65 742c 2073 6c65 6570   internet, sleep
-00000aa0: 696e 6720 696e 2073 6f6d 6562 6f64 7927  ing in somebody'
-00000ab0: 7320 476f 6f67 6c65 2044 7269 7665 2c20  s Google Drive, 
-00000ac0: 4472 6f70 626f 782c 2061 6e64 206f 7468  Dropbox, and oth
-00000ad0: 6572 2077 6562 7369 7465 7320 686f 7374  er websites host
-00000ae0: 6564 2062 7920 7363 686f 6f6c 7320 6f72  ed by schools or
-00000af0: 2072 6573 6561 7263 6820 6c61 6273 2e0a   research labs..
-00000b00: 0a49 6e20 7468 6520 6669 656c 6420 6f66  .In the field of
-00000b10: 206c 616e 6775 6167 6520 6d6f 6465 6c73   language models
-00000b20: 2c20 7468 6572 6520 6861 7320 6265 656e  , there has been
-00000b30: 2061 2076 616c 7561 626c 6520 7072 6563   a valuable prec
-00000b40: 6564 656e 7420 7365 7420 6279 2074 6865  edent set by the
-00000b50: 2077 6f72 6b20 6f66 205b 6c6d 2d65 7661   work of [lm-eva
-00000b60: 6c75 6174 696f 6e2d 6861 726e 6573 735d  luation-harness]
-00000b70: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000b80: 636f 6d2f 456c 6575 7468 6572 4149 2f6c  com/EleutherAI/l
-00000b90: 6d2d 6576 616c 7561 7469 6f6e 2d68 6172  m-evaluation-har
-00000ba0: 6e65 7373 292e 2054 6865 7920 6f66 6665  ness). They offe
-00000bb0: 7220 696e 7465 6772 6174 6564 2064 6174  r integrated dat
-00000bc0: 6120 616e 6420 6d6f 6465 6c20 696e 7465  a and model inte
-00000bd0: 7266 6163 6573 2c20 656e 6162 6c69 6e67  rfaces, enabling
-00000be0: 2072 6170 6964 2065 7661 6c75 6174 696f   rapid evaluatio
-00000bf0: 6e20 6f66 206c 616e 6775 6167 6520 6d6f  n of language mo
-00000c00: 6465 6c73 2061 6e64 2073 6572 7669 6e67  dels and serving
-00000c10: 2061 7320 7468 6520 6261 636b 656e 6420   as the backend 
-00000c20: 7375 7070 6f72 7420 6672 616d 6577 6f72  support framewor
-00000c30: 6b20 666f 7220 7468 6520 5b6f 7065 6e2d  k for the [open-
-00000c40: 6c6c 6d2d 6c65 6164 6572 626f 6172 645d  llm-leaderboard]
-00000c50: 2868 7474 7073 3a2f 2f68 7567 6769 6e67  (https://hugging
-00000c60: 6661 6365 2e63 6f2f 7370 6163 6573 2f48  face.co/spaces/H
-00000c70: 7567 6769 6e67 4661 6365 4834 2f6f 7065  uggingFaceH4/ope
-00000c80: 6e5f 6c6c 6d5f 6c65 6164 6572 626f 6172  n_llm_leaderboar
-00000c90: 6429 2c20 616e 6420 6861 7320 6772 6164  d), and has grad
-00000ca0: 7561 6c6c 7920 6265 636f 6d65 2074 6865  ually become the
-00000cb0: 2075 6e64 6572 6c79 696e 6720 6563 6f73   underlying ecos
-00000cc0: 7973 7465 6d20 6f66 2074 6865 2065 7261  ystem of the era
-00000cd0: 206f 6620 666f 756e 6461 7469 6f6e 206d   of foundation m
-00000ce0: 6f64 656c 732e 0a0a 486f 7765 7665 722c  odels...However,
-00000cf0: 2074 686f 7567 6820 7468 6572 6520 6172   though there ar
-00000d00: 6520 6d61 6e79 206e 6577 2065 7661 6c75  e many new evalu
-00000d10: 6174 696f 6e20 6461 7461 7365 7473 2061  ation datasets a
-00000d20: 7265 2072 6563 656e 746c 7920 7072 6f70  re recently prop
-00000d30: 6f73 6564 2c20 7468 6520 6566 6669 6369  osed, the effici
-00000d40: 656e 7420 6576 616c 7561 7469 6f6e 2070  ent evaluation p
-00000d50: 6970 656c 696e 6520 6f66 204c 4d4d 2069  ipeline of LMM i
-00000d60: 7320 7374 696c 6c20 696e 2069 7473 2069  s still in its i
-00000d70: 6e66 616e 6379 2c20 616e 6420 7468 6572  nfancy, and ther
-00000d80: 6520 6973 206e 6f20 756e 6966 6965 6420  e is no unified 
-00000d90: 6576 616c 7561 7469 6f6e 2066 7261 6d65  evaluation frame
-00000da0: 776f 726b 2074 6861 7420 6361 6e20 6265  work that can be
-00000db0: 2075 7365 6420 746f 2065 7661 6c75 6174   used to evaluat
-00000dc0: 6520 4c4d 4d20 6163 726f 7373 2061 2077  e LMM across a w
-00000dd0: 6964 6520 7261 6e67 6520 6f66 2064 6174  ide range of dat
-00000de0: 6173 6574 732e 2054 6f20 6164 6472 6573  asets. To addres
-00000df0: 7320 7468 6973 2063 6861 6c6c 656e 6765  s this challenge
-00000e00: 2c20 7765 2069 6e74 726f 6475 6365 202a  , we introduce *
-00000e10: 2a6c 6d6d 732d 6576 616c 2a2a 2c20 616e  *lmms-eval**, an
-00000e20: 2065 7661 6c75 6174 696f 6e20 6672 616d   evaluation fram
-00000e30: 6577 6f72 6b20 6d65 7469 6375 6c6f 7573  ework meticulous
-00000e40: 6c79 2063 7261 6674 6564 2066 6f72 2063  ly crafted for c
-00000e50: 6f6e 7369 7374 656e 7420 616e 6420 6566  onsistent and ef
-00000e60: 6669 6369 656e 7420 6576 616c 7561 7469  ficient evaluati
-00000e70: 6f6e 206f 6620 4c4d 4d2e 0a0a 5765 2068  on of LMM...We h
-00000e80: 756d 626c 7920 6f62 736f 7262 6564 2074  umbly obsorbed t
-00000e90: 6865 2065 7871 7569 7369 7465 2061 6e64  he exquisite and
-00000ea0: 2065 6666 6963 6965 6e74 2064 6573 6967   efficient desig
-00000eb0: 6e20 6f66 205b 6c6d 2d65 7661 6c75 6174  n of [lm-evaluat
-00000ec0: 696f 6e2d 6861 726e 6573 735d 2868 7474  ion-harness](htt
-00000ed0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000ee0: 456c 6575 7468 6572 4149 2f6c 6d2d 6576  EleutherAI/lm-ev
-00000ef0: 616c 7561 7469 6f6e 2d68 6172 6e65 7373  aluation-harness
-00000f00: 292e 2042 7569 6c64 696e 6720 7570 6f6e  ). Building upon
-00000f10: 2069 7473 2066 6f75 6e64 6174 696f 6e2c   its foundation,
-00000f20: 2077 6520 696d 706c 656d 656e 7465 6420   we implemented 
-00000f30: 6f75 7220 606c 6d6d 732d 6576 616c 6020  our `lmms-eval` 
-00000f40: 6672 616d 6577 6f72 6b20 7769 7468 2070  framework with p
-00000f50: 6572 666f 726d 616e 6365 206f 7074 696d  erformance optim
-00000f60: 697a 6174 696f 6e73 2073 7065 6369 6669  izations specifi
-00000f70: 6361 6c6c 7920 666f 7220 4c4d 4d73 2e0a  cally for LMMs..
-00000f80: 0a23 2320 4e65 6365 7373 6974 7920 6f66  .## Necessity of
-00000f90: 206c 6d6d 732d 6576 616c 0a0a 5765 2062   lmms-eval..We b
-00000fa0: 656c 6965 7665 206f 7572 2065 6666 6f72  elieve our effor
-00000fb0: 7420 636f 756c 6420 7072 6f76 6964 6520  t could provide 
-00000fc0: 616e 2065 6666 6963 6965 6e74 2069 6e74  an efficient int
-00000fd0: 6572 6661 6365 2066 6f72 2074 6865 2064  erface for the d
-00000fe0: 6574 6169 6c65 6420 636f 6d70 6172 6973  etailed comparis
-00000ff0: 6f6e 206f 6620 7075 626c 6963 6c79 2061  on of publicly a
-00001000: 7661 696c 6162 6c65 206d 6f64 656c 7320  vailable models 
-00001010: 746f 2064 6973 6365 726e 2074 6865 6972  to discern their
-00001020: 2073 7472 656e 6774 6873 2061 6e64 2077   strengths and w
-00001030: 6561 6b6e 6573 7365 732e 2049 7427 7320  eaknesses. It's 
-00001040: 616c 736f 2075 7365 6675 6c20 666f 7220  also useful for 
-00001050: 7265 7365 6172 6368 2069 6e73 7469 7475  research institu
-00001060: 7469 6f6e 7320 616e 6420 7072 6f64 7563  tions and produc
-00001070: 7469 6f6e 2d6f 7269 656e 7465 6420 636f  tion-oriented co
-00001080: 6d70 616e 6965 7320 746f 2061 6363 656c  mpanies to accel
-00001090: 6572 6174 6520 7468 6520 6465 7665 6c6f  erate the develo
-000010a0: 706d 656e 7420 6f66 206c 6172 6765 206d  pment of large m
-000010b0: 756c 7469 6d6f 6461 6c20 6d6f 6465 6c73  ultimodal models
-000010c0: 2e20 5769 7468 2074 6865 2060 6c6d 6d73  . With the `lmms
-000010d0: 2d65 7661 6c60 2c20 7765 2068 6176 6520  -eval`, we have 
-000010e0: 7369 676e 6966 6963 616e 746c 7920 6163  significantly ac
-000010f0: 6365 6c65 7261 7465 6420 7468 6520 6c69  celerated the li
-00001100: 6665 6379 636c 6520 6f66 206d 6f64 656c  fecycle of model
-00001110: 2069 7465 7261 7469 6f6e 2e20 496e 7369   iteration. Insi
-00001120: 6465 2074 6865 204c 4c61 5641 2074 6561  de the LLaVA tea
-00001130: 6d2c 2074 6865 2075 7469 6c69 7a61 7469  m, the utilizati
-00001140: 6f6e 206f 6620 606c 6d6d 732d 6576 616c  on of `lmms-eval
-00001150: 6020 6c61 7267 656c 7920 696d 7072 6f76  ` largely improv
-00001160: 6573 2074 6865 2065 6666 6963 6965 6e63  es the efficienc
-00001170: 7920 6f66 2074 6865 206d 6f64 656c 2064  y of the model d
-00001180: 6576 656c 6f70 6d65 6e74 2063 7963 6c65  evelopment cycle
-00001190: 2c20 6173 2077 6520 6172 6520 6162 6c65  , as we are able
-000011a0: 2074 6f20 6576 616c 7561 7465 2077 6565   to evaluate wee
-000011b0: 6b6c 7920 7472 6169 6e65 6420 6875 6e64  kly trained hund
-000011c0: 7265 6473 206f 6620 6368 6563 6b70 6f69  reds of checkpoi
-000011d0: 6e74 7320 6f6e 2032 302d 3330 2064 6174  nts on 20-30 dat
-000011e0: 6173 6574 732c 2069 6465 6e74 6966 7969  asets, identifyi
-000011f0: 6e67 2074 6865 2073 7472 656e 6774 6873  ng the strengths
-00001200: 2061 6e64 2077 6561 6b6e 6573 7365 732c   and weaknesses,
-00001210: 2061 6e64 2074 6865 6e20 6d61 6b65 2074   and then make t
-00001220: 6172 6765 7465 6420 696d 7072 6f76 656d  argeted improvem
-00001230: 656e 7473 2e0a 0a23 2041 6e6e 6f75 6365  ents...# Annouce
-00001240: 6d65 6e74 0a0a 2323 2076 302e 312e 3020  ment..## v0.1.0 
-00001250: 5265 6c65 6173 6564 0a0a 5468 6520 6669  Released..The fi
-00001260: 7273 7420 7665 7273 696f 6e20 6f66 2074  rst version of t
-00001270: 6865 2060 6c6d 6d73 2d65 7661 6c60 2069  he `lmms-eval` i
-00001280: 7320 7265 6c65 6173 6564 2e20 5765 2061  s released. We a
-00001290: 7265 2077 6f72 6b69 6e67 206f 6e20 7072  re working on pr
-000012a0: 6f76 6964 696e 6720 616e 206f 6e65 2d63  oviding an one-c
-000012b0: 6f6d 6d61 6e64 2065 7661 6c75 6174 696f  ommand evaluatio
-000012c0: 6e20 7375 6974 6520 666f 7220 6163 6365  n suite for acce
-000012d0: 6c65 7261 7469 6e67 2074 6865 2064 6576  lerating the dev
-000012e0: 656c 6f70 6d65 6e74 206f 6620 4c4d 4d73  elopment of LMMs
-000012f0: 2e20 0a0a 3e20 496e 205b 4c4c 6156 4120  . ..> In [LLaVA 
-00001300: 4e65 7874 5d28 6874 7470 733a 2f2f 6c6c  Next](https://ll
-00001310: 6176 612d 766c 2e67 6974 6875 622e 696f  ava-vl.github.io
-00001320: 2f62 6c6f 672f 3230 3234 2d30 312d 3330  /blog/2024-01-30
-00001330: 2d6c 6c61 7661 2d6e 6578 742f 2920 6465  -llava-next/) de
-00001340: 7665 6c6f 706d 656e 742c 2077 6520 696e  velopment, we in
-00001350: 7465 726e 616c 6c79 2075 7469 6c69 7a65  ternally utilize
-00001360: 2074 6869 7320 7375 6974 6520 746f 2065   this suite to e
-00001370: 7661 6c75 6174 6520 7468 6520 6d75 6c74  valuate the mult
-00001380: 6970 6c65 2064 6966 6665 7265 6e74 206d  iple different m
-00001390: 6f64 656c 2076 6572 7369 6f6e 7320 6f6e  odel versions on
-000013a0: 2076 6172 696f 7573 2064 6174 6173 6574   various dataset
-000013b0: 732e 2049 7420 7369 676e 6966 6963 616e  s. It significan
-000013c0: 746c 7920 6163 6365 6c65 7261 7465 7320  tly accelerates 
-000013d0: 7468 6520 6d6f 6465 6c20 6465 7665 6c6f  the model develo
-000013e0: 706d 656e 7420 6379 636c 6520 666f 7220  pment cycle for 
-000013f0: 6974 2773 2065 6173 7920 696e 7465 6772  it's easy integr
-00001400: 6174 696f 6e20 616e 6420 6661 7374 2065  ation and fast e
-00001410: 7661 6c75 6174 696f 6e20 7370 6565 642e  valuation speed.
-00001420: 0a0a 5468 6520 6d61 696e 2066 6561 7475  ..The main featu
-00001430: 7265 2069 6e63 6c75 6465 733a 0a0a 3c70  re includes:..<p
-00001440: 2061 6c69 676e 3d22 6365 6e74 6572 2220   align="center" 
-00001450: 7769 6474 683d 2231 3030 2522 3e0a 3c69  width="100%">.<i
-00001460: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00001470: 692e 706f 7374 696d 672e 6363 2f73 677a  i.postimg.cc/sgz
-00001480: 4e6d 4a78 372f 7465 6173 6572 2e70 6e67  NmJx7/teaser.png
-00001490: 2220 2077 6964 7468 3d22 3130 3025 2220  "  width="100%" 
-000014a0: 6865 6967 6874 3d22 3830 2522 3e0a 3c2f  height="80%">.</
-000014b0: 703e 0a0a 2323 2320 4f6e 652d 636f 6d6d  p>..### One-comm
-000014c0: 616e 6420 6576 616c 7561 7469 6f6e 2c20  and evaluation, 
-000014d0: 7769 7468 2064 6574 6169 6c65 6420 6c6f  with detailed lo
-000014e0: 6773 2061 6e64 2073 616d 706c 6573 2e0a  gs and samples..
-000014f0: 596f 7520 6361 6e20 6576 616c 7561 7465  You can evaluate
-00001500: 2074 6865 206d 6f64 656c 7320 6f6e 206d   the models on m
-00001510: 756c 7469 706c 6520 6461 7461 7365 7473  ultiple datasets
-00001520: 2077 6974 6820 6120 7369 6e67 6c65 2063   with a single c
-00001530: 6f6d 6d61 6e64 2e20 4e6f 206d 6f64 656c  ommand. No model
-00001540: 2f64 6174 6120 7072 6570 6172 6174 696f  /data preparatio
-00001550: 6e20 6973 206e 6565 6465 642c 206a 7573  n is needed, jus
-00001560: 7420 6f6e 6520 636f 6d6d 616e 6420 6c69  t one command li
-00001570: 6e65 2c20 6665 7720 6d69 6e75 7465 732c  ne, few minutes,
-00001580: 2061 6e64 2067 6574 2074 6865 2072 6573   and get the res
-00001590: 756c 7473 2e20 4e6f 7420 6a75 7374 2061  ults. Not just a
-000015a0: 2072 6573 756c 7420 6e75 6d62 6572 2c20   result number, 
-000015b0: 6275 7420 616c 736f 2074 6865 2064 6574  but also the det
-000015c0: 6169 6c65 6420 6c6f 6773 2061 6e64 2073  ailed logs and s
-000015d0: 616d 706c 6573 2c20 696e 636c 7564 696e  amples, includin
-000015e0: 6720 7468 6520 6d6f 6465 6c20 6172 6773  g the model args
-000015f0: 2c20 696e 7075 7420 7175 6573 7469 6f6e  , input question
-00001600: 2c20 6d6f 6465 6c20 7265 7370 6f6e 7365  , model response
-00001610: 2c20 616e 6420 6772 6f75 6e64 2074 7275  , and ground tru
-00001620: 7468 2061 6e73 7765 722e 0a0a 6060 6070  th answer...```p
-00001630: 7974 686f 6e0a 2320 4576 616c 7561 7469  ython.# Evaluati
-00001640: 6e67 204c 4c61 5641 206f 6e20 6d75 6c74  ng LLaVA on mult
-00001650: 6970 6c65 2064 6174 6173 6574 730a 6163  iple datasets.ac
-00001660: 6365 6c65 7261 7465 206c 6175 6e63 6820  celerate launch 
-00001670: 2d2d 6e75 6d5f 7072 6f63 6573 7365 733d  --num_processes=
-00001680: 3820 2d6d 206c 6d6d 735f 6576 616c 202d  8 -m lmms_eval -
-00001690: 2d6d 6f64 656c 206c 6c61 7661 2020 202d  -model llava   -
-000016a0: 2d6d 6f64 656c 5f61 7267 7320 7072 6574  -model_args pret
-000016b0: 7261 696e 6564 3d22 6c69 7568 616f 7469  rained="liuhaoti
-000016c0: 616e 2f6c 6c61 7661 2d76 312e 352d 3762  an/llava-v1.5-7b
-000016d0: 2220 2020 2d2d 7461 736b 7320 6d6d 652c  "   --tasks mme,
-000016e0: 6d6d 6265 6e63 685f 656e 202d 2d62 6174  mmbench_en --bat
-000016f0: 6368 5f73 697a 6520 3120 2d2d 6c6f 675f  ch_size 1 --log_
-00001700: 7361 6d70 6c65 7320 2d2d 6c6f 675f 7361  samples --log_sa
-00001710: 6d70 6c65 735f 7375 6666 6978 206c 6c61  mples_suffix lla
-00001720: 7661 5f76 312e 355f 6d6d 655f 6d6d 6265  va_v1.5_mme_mmbe
-00001730: 6e63 6865 6e20 2d2d 6f75 7470 7574 5f70  nchen --output_p
-00001740: 6174 6820 2e2f 6c6f 6773 2f20 230a 6060  ath ./logs/ #.``
-00001750: 600a 0a23 2323 2041 6363 656c 6572 6174  `..### Accelerat
-00001760: 6f72 2073 7570 706f 7274 2061 6e64 2054  or support and T
-00001770: 6173 6b73 2067 726f 7570 696e 672e 0a57  asks grouping..W
-00001780: 6520 7375 7070 6f72 7420 7468 6520 7573  e support the us
-00001790: 6167 6520 6f66 2060 6163 6365 6c65 7261  age of `accelera
-000017a0: 7465 6020 746f 2077 7261 7020 7468 6520  te` to wrap the 
-000017b0: 6d6f 6465 6c20 666f 7220 6469 7374 7269  model for distri
-000017c0: 6275 7465 6420 6576 616c 7561 7469 6f6e  buted evaluation
-000017d0: 2c20 7375 7070 6f72 7469 6e67 206d 756c  , supporting mul
-000017e0: 7469 2d67 7075 2061 6e64 2074 656e 736f  ti-gpu and tenso
-000017f0: 7220 7061 7261 6c6c 656c 6973 6d2e 2057  r parallelism. W
-00001800: 6974 6820 2a2a 5461 736b 2047 726f 7570  ith **Task Group
-00001810: 696e 672a 2a2c 2061 6c6c 2069 6e73 7461  ing**, all insta
-00001820: 6e63 6573 2066 726f 6d20 616c 6c20 7461  nces from all ta
-00001830: 736b 7320 6172 6520 6772 6f75 7065 6420  sks are grouped 
-00001840: 616e 6420 6576 616c 7561 7465 6420 696e  and evaluated in
-00001850: 2070 6172 616c 6c65 6c2c 2077 6869 6368   parallel, which
-00001860: 2073 6967 6e69 6669 6361 6e74 6c79 2069   significantly i
-00001870: 6d70 726f 7665 7320 7468 6520 7468 726f  mproves the thro
-00001880: 7567 6870 7574 206f 6620 7468 6520 6576  ughput of the ev
-00001890: 616c 7561 7469 6f6e 2e20 4166 7465 7220  aluation. After 
-000018a0: 6576 616c 7561 7469 6f6e 2c20 616c 6c20  evaluation, all 
-000018b0: 696e 7374 616e 6365 7320 6172 6520 7365  instances are se
-000018c0: 6e74 2074 6f20 706f 7374 7072 6f63 6573  nt to postproces
-000018d0: 7369 6e67 206d 6f64 756c 6520 666f 7220  sing module for 
-000018e0: 6d65 7472 6963 2063 616c 6375 6174 696f  metric calcuatio
-000018f0: 6e73 2061 6e64 2070 6f74 656e 7469 616c  ns and potential
-00001900: 2047 5054 342d 6576 616c 2071 7565 7269   GPT4-eval queri
-00001910: 6573 2e0a 0a42 656c 6f77 2061 7265 2074  es...Below are t
-00001920: 6865 2074 6f74 616c 2072 756e 7469 6d65  he total runtime
-00001930: 206f 6e20 6469 6666 6572 656e 7420 6461   on different da
-00001940: 7461 7365 7473 2075 7369 6e67 2034 2078  tasets using 4 x
-00001950: 2041 3130 3020 3430 472e 0a0a 7c20 4461   A100 40G...| Da
-00001960: 7461 7365 7420 2823 6e75 6d29 2020 2020  taset (#num)    
-00001970: 2020 2020 2020 7c20 4c4c 6156 412d 7631        | LLaVA-v1
-00001980: 2e35 2d37 6220 2020 2020 207c 204c 4c61  .5-7b      | LLa
-00001990: 5641 2d76 312e 352d 3133 6220 2020 2020  VA-v1.5-13b     
-000019a0: 7c0a 7c20 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d  |.| :-----------
-000019b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c20 3a2d  ----------- | :-
-000019c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000019d0: 207c 203a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   | :------------
-000019e0: 2d2d 2d2d 2d20 7c0a 7c20 6d6d 6520 2832  ----- |.| mme (2
-000019f0: 3337 3429 2020 2020 2020 2020 2020 2020  374)            
-00001a00: 2020 7c20 3220 6d69 6e73 2034 3320 7365    | 2 mins 43 se
-00001a10: 636f 6e64 7320 207c 2033 206d 696e 7320  conds  | 3 mins 
-00001a20: 3237 2073 6563 6f6e 6473 2020 7c0a 7c20  27 seconds  |.| 
-00001a30: 6771 6120 2831 3235 3738 2920 2020 2020  gqa (12578)     
-00001a40: 2020 2020 2020 2020 7c20 3130 206d 696e          | 10 min
-00001a50: 7320 3433 2073 6563 6f6e 6473 207c 2031  s 43 seconds | 1
-00001a60: 3420 6d69 6e73 2032 3320 7365 636f 6e64  4 mins 23 second
-00001a70: 7320 7c0a 7c20 7363 6965 6e63 6571 615f  s |.| scienceqa_
-00001a80: 696d 6720 2832 3031 3729 2020 2020 7c20  img (2017)    | 
-00001a90: 3120 6d69 6e73 2035 3820 7365 636f 6e64  1 mins 58 second
-00001aa0: 7320 207c 2032 206d 696e 7320 3532 2073  s  | 2 mins 52 s
-00001ab0: 6563 6f6e 6473 2020 7c0a 7c20 6169 3264  econds  |.| ai2d
-00001ac0: 2028 3330 3838 2920 2020 2020 2020 2020   (3088)         
-00001ad0: 2020 2020 7c20 3320 6d69 6e73 2031 3720      | 3 mins 17 
-00001ae0: 7365 636f 6e64 7320 207c 2034 206d 696e  seconds  | 4 min
-00001af0: 7320 3132 2073 6563 6f6e 6473 2020 7c0a  s 12 seconds  |.
-00001b00: 7c20 636f 636f 3230 3137 5f63 6170 5f76  | coco2017_cap_v
-00001b10: 616c 2028 3530 3030 2920 7c20 3134 206d  al (5000) | 14 m
-00001b20: 696e 7320 3133 2073 6563 6f6e 6473 207c  ins 13 seconds |
-00001b30: 2031 3920 6d69 6e73 2035 3820 7365 636f   19 mins 58 seco
-00001b40: 6e64 7320 7c0a 0a23 2323 2041 6c6c 2d49  nds |..### All-I
-00001b50: 6e2d 4f6e 6520 4846 2064 6174 6173 6574  n-One HF dataset
-00001b60: 2068 7562 732e 0a0a 5765 2061 7265 2068   hubs...We are h
-00001b70: 6f73 7469 6e67 206d 6f72 6520 7468 616e  osting more than
-00001b80: 2034 3020 2861 6e64 2069 6e63 7265 6173   40 (and increas
-00001b90: 696e 6729 2064 6174 6173 6574 7320 6f6e  ing) datasets on
-00001ba0: 205b 6875 6767 696e 6766 6163 652f 6c6d   [huggingface/lm
-00001bb0: 6d73 2d6c 6162 5d28 6874 7470 733a 2f2f  ms-lab](https://
-00001bc0: 6875 6767 696e 6766 6163 652e 636f 2f6c  huggingface.co/l
-00001bd0: 6d6d 732d 6c61 6229 2c20 7765 2063 6172  mms-lab), we car
-00001be0: 6566 756c 6c79 2063 6f6e 7665 7274 6564  efully converted
-00001bf0: 2074 6865 7365 2064 6174 6173 6574 7320   these datasets 
-00001c00: 6672 6f6d 206f 7269 6769 6e61 6c20 736f  from original so
-00001c10: 7572 6365 7320 616e 6420 696e 636c 7564  urces and includ
-00001c20: 6564 2061 6c6c 2076 6172 6961 6e74 732c  ed all variants,
-00001c30: 2076 6572 7369 6f6e 7320 616e 6420 7370   versions and sp
-00001c40: 6c69 7473 2e20 4e6f 7720 7468 6579 2063  lits. Now they c
-00001c50: 616e 2062 6520 6469 7265 6374 6c79 2061  an be directly a
-00001c60: 6363 6573 7365 6420 7769 7468 6f75 7420  ccessed without 
-00001c70: 616e 7920 6275 7264 656e 206f 6620 6461  any burden of da
-00001c80: 7461 2070 7265 7072 6f63 6573 7369 6e67  ta preprocessing
-00001c90: 2e20 5468 6579 2061 6c73 6f20 7365 7276  . They also serv
-00001ca0: 6520 666f 7220 7468 6520 7075 7270 6f73  e for the purpos
-00001cb0: 6520 6f66 2076 6973 7561 6c69 7a69 6e67  e of visualizing
-00001cc0: 2074 6865 2064 6174 6120 616e 6420 6772   the data and gr
-00001cd0: 6173 7069 6e67 2074 6865 2073 656e 7365  asping the sense
-00001ce0: 206f 6620 6576 616c 7561 7469 6f6e 2074   of evaluation t
-00001cf0: 6173 6b73 2064 6973 7472 6962 7574 696f  asks distributio
-00001d00: 6e2e 0a0a 3c70 2061 6c69 676e 3d22 6365  n...<p align="ce
-00001d10: 6e74 6572 2220 7769 6474 683d 2231 3030  nter" width="100
-00001d20: 2522 3e0a 3c69 6d67 2073 7263 3d22 6874  %">.<img src="ht
-00001d30: 7470 733a 2f2f 692e 706f 7374 696d 672e  tps://i.postimg.
-00001d40: 6363 2f38 5058 4657 3973 6b2f 5758 3230  cc/8PXFW9sk/WX20
-00001d50: 3234 3032 3238 2d31 3233 3131 305f 3278  240228-123110_2x
-00001d60: 2e70 6e67 2220 2077 6964 7468 3d22 3130  .png"  width="10
-00001d70: 3025 2220 6865 6967 6874 3d22 3830 2522  0%" height="80%"
-00001d80: 3e0a 3c2f 703e 0a0a 2323 2320 4465 7461  >.</p>..### Deta
-00001d90: 696c 6564 204c 6f67 6769 6e67 2055 7469  iled Logging Uti
-00001da0: 6c69 7465 730a 0a57 6520 7072 6f76 6964  lites..We provid
-00001db0: 6520 6465 7461 696c 6564 206c 6f67 6769  e detailed loggi
-00001dc0: 6e67 2075 7469 6c69 7469 6573 2074 6f20  ng utilities to 
-00001dd0: 6865 6c70 2079 6f75 2075 6e64 6572 7374  help you underst
-00001de0: 616e 6420 7468 6520 6576 616c 7561 7469  and the evaluati
-00001df0: 6f6e 2070 726f 6365 7373 2061 6e64 2072  on process and r
-00001e00: 6573 756c 7473 2e20 5468 6520 6c6f 6773  esults. The logs
-00001e10: 2069 6e63 6c75 6465 2074 6865 206d 6f64   include the mod
-00001e20: 656c 2061 7267 732c 2067 656e 6572 6174  el args, generat
-00001e30: 696f 6e20 7061 7261 6d65 7465 7273 2c20  ion parameters, 
-00001e40: 696e 7075 7420 7175 6573 7469 6f6e 2c20  input question, 
-00001e50: 6d6f 6465 6c20 7265 7370 6f6e 7365 2c20  model response, 
-00001e60: 616e 6420 6772 6f75 6e64 2074 7275 7468  and ground truth
-00001e70: 2061 6e73 7765 722e 2059 6f75 2063 616e   answer. You can
-00001e80: 2061 6c73 6f20 7265 636f 7264 2065 7665   also record eve
-00001e90: 7279 2064 6574 6169 6c73 2061 6e64 2076  ry details and v
-00001ea0: 6973 7561 6c69 7a65 2074 6865 6d20 696e  isualize them in
-00001eb0: 7369 6465 2072 756e 7320 6f6e 2057 6569  side runs on Wei
-00001ec0: 6768 7473 2026 2042 6961 7365 732e 0a0a  ghts & Biases...
-00001ed0: 7b25 2069 6e63 6c75 6465 2066 6967 7572  {% include figur
-00001ee0: 652e 6c69 7175 6964 206c 6f61 6469 6e67  e.liquid loading
-00001ef0: 3d22 6561 6765 7222 2070 6174 683d 2261  ="eager" path="a
-00001f00: 7373 6574 732f 696d 672f 7761 6e64 625f  ssets/img/wandb_
-00001f10: 7461 626c 652e 706e 6722 2063 6c61 7373  table.png" class
-00001f20: 3d22 696d 672d 666c 7569 6420 726f 756e  ="img-fluid roun
-00001f30: 6465 6420 7a2d 6465 7074 682d 3122 207a  ded z-depth-1" z
-00001f40: 6f6f 6d61 626c 653d 7472 7565 2025 7d0a  oomable=true %}.
-00001f50: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
-00001f60: 7222 2077 6964 7468 3d22 3130 3025 223e  r" width="100%">
-00001f70: 0a3c 696d 6720 7372 633d 2268 7474 7073  .<img src="https
-00001f80: 3a2f 2f69 2e70 6f73 7469 6d67 2e63 632f  ://i.postimg.cc/
-00001f90: 5731 6331 7642 444a 2f57 6563 6861 742d  W1c1vBDJ/Wechat-
-00001fa0: 494d 4731 3939 332e 706e 6722 2020 7769  IMG1993.png"  wi
-00001fb0: 6474 683d 2231 3030 2522 2068 6569 6768  dth="100%" heigh
-00001fc0: 743d 2238 3025 223e 0a3c 2f70 3e0a 0a23  t="80%">.</p>..#
-00001fd0: 2049 6e73 7461 6c6c 6174 696f 6e0a 0a46   Installation..F
-00001fe0: 6f72 2066 6f72 6d61 6c20 7573 6167 652c  or formal usage,
-00001ff0: 2079 6f75 2063 616e 2069 6e73 7461 6c6c   you can install
-00002000: 2074 6865 2070 6163 6b61 6765 2066 726f   the package fro
-00002010: 6d20 5079 5049 2062 7920 7275 6e6e 696e  m PyPI by runnin
-00002020: 6720 7468 6520 666f 6c6c 6f77 696e 6720  g the following 
-00002030: 636f 6d6d 616e 643a 0a60 6060 6261 7368  command:.```bash
-00002040: 0a70 6970 2069 6e73 7461 6c6c 206c 6d6d  .pip install lmm
-00002050: 732d 6576 616c 0a60 6060 0a0a 466f 7220  s-eval.```..For 
-00002060: 6465 7665 6c6f 706d 656e 742c 2079 6f75  development, you
-00002070: 2063 616e 2069 6e73 7461 6c6c 2074 6865   can install the
-00002080: 2070 6163 6b61 6765 2062 7920 636c 6f6e   package by clon
-00002090: 696e 6720 7468 6520 7265 706f 7369 746f  ing the reposito
-000020a0: 7279 2061 6e64 2072 756e 6e69 6e67 2074  ry and running t
-000020b0: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6d  he following com
-000020c0: 6d61 6e64 3a0a 6060 6062 6173 680a 6769  mand:.```bash.gi
-000020d0: 7420 636c 6f6e 6520 6874 7470 733a 2f2f  t clone https://
-000020e0: 6769 7468 7562 2e63 6f6d 2f45 766f 6c76  github.com/Evolv
-000020f0: 696e 674c 4d4d 732d 4c61 622f 6c6d 6d73  ingLMMs-Lab/lmms
-00002100: 2d65 7661 6c0a 6364 206c 6d6d 732d 6576  -eval.cd lmms-ev
-00002110: 616c 0a70 6970 2069 6e73 7461 6c6c 202d  al.pip install -
-00002120: 6520 2e0a 6060 600a 0a49 6620 796f 7520  e ..```..If you 
-00002130: 7761 6e74 6564 2074 6f20 7465 7374 206c  wanted to test l
-00002140: 6c61 7661 2c20 796f 7520 7769 6c6c 2068  lava, you will h
-00002150: 6176 6520 746f 2063 6c6f 6e65 2074 6865  ave to clone the
-00002160: 6972 2072 6570 6f20 6672 6f6d 205b 4c4c  ir repo from [LL
-00002170: 6156 415d 2868 7474 7073 3a2f 2f67 6974  aVA](https://git
-00002180: 6875 622e 636f 6d2f 6861 6f74 6961 6e2d  hub.com/haotian-
-00002190: 6c69 752f 4c4c 6156 4129 2061 6e64 0a60  liu/LLaVA) and.`
-000021a0: 6060 0a67 6974 2063 6c6f 6e65 2068 7474  ``.git clone htt
-000021b0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000021c0: 6861 6f74 6961 6e2d 6c69 752f 4c4c 6156  haotian-liu/LLaV
-000021d0: 410a 6364 204c 4c61 5641 0a70 6970 2069  A.cd LLaVA.pip i
-000021e0: 6e73 7461 6c6c 202d 6520 2e0a 6060 600a  nstall -e ..```.
-000021f0: 0a59 6f75 2063 616e 2063 6865 636b 2074  .You can check t
-00002200: 6865 205b 656e 7669 726f 6e6d 656e 7420  he [environment 
-00002210: 696e 7374 616c 6c20 7363 7269 7074 5d28  install script](
-00002220: 6d69 7363 732f 7265 7072 5f73 6372 6970  miscs/repr_scrip
-00002230: 7473 2e73 6829 2061 6e64 205b 746f 7263  ts.sh) and [torc
-00002240: 6820 656e 7669 726f 6e6d 656e 7420 696e  h environment in
-00002250: 666f 5d28 6d69 7363 732f 7265 7072 5f74  fo](miscs/repr_t
-00002260: 6f72 6368 5f65 6e76 732e 7478 7429 2074  orch_envs.txt) t
-00002270: 6f20 2a2a 7265 7072 6f64 7563 6520 4c4c  o **reproduce LL
-00002280: 6156 412d 312e 3527 7320 7061 7065 7220  aVA-1.5's paper 
-00002290: 7265 7375 6c74 732a 2a2e 2057 6520 666f  results**. We fo
-000022a0: 756e 6420 746f 7263 682f 6375 6461 2076  und torch/cuda v
-000022b0: 6572 7369 6f6e 7320 6469 6666 6572 656e  ersions differen
-000022c0: 6365 2077 6f75 6c64 2063 6175 7365 2073  ce would cause s
-000022d0: 6d61 6c6c 2076 6172 6961 7469 6f6e 7320  mall variations 
-000022e0: 696e 2074 6865 2072 6573 756c 7473 2c20  in the results, 
-000022f0: 7765 2070 726f 7669 6465 2074 6865 205b  we provide the [
-00002300: 7265 7375 6c74 7320 6368 6563 6b5d 286d  results check](m
-00002310: 6973 6373 2f6c 6c61 7661 5f72 6573 756c  iscs/llava_resul
-00002320: 745f 6368 6563 6b2e 6d64 2920 7769 7468  t_check.md) with
-00002330: 2064 6966 6665 7265 6e74 2065 6e76 6972   different envir
-00002340: 6f6e 6d65 6e74 732e 0a0a 4966 2079 6f75  onments...If you
-00002350: 2077 616e 7420 746f 2074 6573 7420 6f6e   want to test on
-00002360: 2063 6170 7469 6f6e 2064 6174 6173 6574   caption dataset
-00002370: 2073 7563 6820 6173 2060 636f 636f 602c   such as `coco`,
-00002380: 2060 7265 6663 6f63 6f60 2c20 616e 6420   `refcoco`, and 
-00002390: 606e 6f63 6170 7360 2c20 796f 7520 7769  `nocaps`, you wi
-000023a0: 6c6c 206e 6565 6420 746f 2068 6176 6520  ll need to have 
-000023b0: 606a 6176 613d 3d31 2e38 2e30 2060 2074  `java==1.8.0 ` t
-000023c0: 6f20 6c65 7420 7079 636f 636f 6576 616c  o let pycocoeval
-000023d0: 2061 7069 2074 6f20 776f 726b 2e20 4966   api to work. If
-000023e0: 2079 6f75 2064 6f6e 2774 2068 6176 6520   you don't have 
-000023f0: 6974 2c20 796f 7520 6361 6e20 696e 7374  it, you can inst
-00002400: 616c 6c20 6279 2075 7369 6e67 2063 6f6e  all by using con
-00002410: 6461 0a60 6060 0a63 6f6e 6461 2069 6e73  da.```.conda ins
-00002420: 7461 6c6c 206f 7065 6e6a 646b 3d38 0a60  tall openjdk=8.`
-00002430: 6060 0a79 6f75 2063 616e 2074 6865 6e20  ``.you can then 
-00002440: 6368 6563 6b20 796f 7572 206a 6176 6120  check your java 
-00002450: 7665 7273 696f 6e20 6279 2060 6a61 7661  version by `java
-00002460: 202d 7665 7273 696f 6e60 200a 0a23 2055   -version` ..# U
-00002470: 7361 6765 0a60 6060 6261 7368 0a23 2045  sage.```bash.# E
-00002480: 7661 6c75 6174 696e 6720 4c4c 6156 4120  valuating LLaVA 
-00002490: 6f6e 204d 4d45 0a61 6363 656c 6572 6174  on MME.accelerat
-000024a0: 6520 6c61 756e 6368 202d 2d6e 756d 5f70  e launch --num_p
-000024b0: 726f 6365 7373 6573 3d38 202d 6d20 6c6d  rocesses=8 -m lm
-000024c0: 6d73 5f65 7661 6c20 2d2d 6d6f 6465 6c20  ms_eval --model 
-000024d0: 6c6c 6176 6120 2020 2d2d 6d6f 6465 6c5f  llava   --model_
-000024e0: 6172 6773 2070 7265 7472 6169 6e65 643d  args pretrained=
-000024f0: 226c 6975 6861 6f74 6961 6e2f 6c6c 6176  "liuhaotian/llav
-00002500: 612d 7631 2e35 2d37 6222 2020 202d 2d74  a-v1.5-7b"   --t
-00002510: 6173 6b73 206d 6d65 2020 2d2d 6261 7463  asks mme  --batc
-00002520: 685f 7369 7a65 2031 202d 2d6c 6f67 5f73  h_size 1 --log_s
-00002530: 616d 706c 6573 202d 2d6c 6f67 5f73 616d  amples --log_sam
-00002540: 706c 6573 5f73 7566 6669 7820 6c6c 6176  ples_suffix llav
-00002550: 615f 7631 2e35 5f6d 6d65 202d 2d6f 7574  a_v1.5_mme --out
-00002560: 7075 745f 7061 7468 202e 2f6c 6f67 732f  put_path ./logs/
-00002570: 200a 0a23 2045 7661 6c75 6174 696e 6720   ..# Evaluating 
-00002580: 4c4c 6156 4120 6f6e 206d 756c 7469 706c  LLaVA on multipl
-00002590: 6520 6461 7461 7365 7473 0a61 6363 656c  e datasets.accel
-000025a0: 6572 6174 6520 6c61 756e 6368 202d 2d6e  erate launch --n
-000025b0: 756d 5f70 726f 6365 7373 6573 3d38 202d  um_processes=8 -
-000025c0: 6d20 6c6d 6d73 5f65 7661 6c20 2d2d 6d6f  m lmms_eval --mo
-000025d0: 6465 6c20 6c6c 6176 6120 2020 2d2d 6d6f  del llava   --mo
-000025e0: 6465 6c5f 6172 6773 2070 7265 7472 6169  del_args pretrai
-000025f0: 6e65 643d 226c 6975 6861 6f74 6961 6e2f  ned="liuhaotian/
-00002600: 6c6c 6176 612d 7631 2e35 2d37 6222 2020  llava-v1.5-7b"  
-00002610: 202d 2d74 6173 6b73 206d 6d65 2c6d 6d62   --tasks mme,mmb
-00002620: 656e 6368 5f65 6e20 2d2d 6261 7463 685f  ench_en --batch_
-00002630: 7369 7a65 2031 202d 2d6c 6f67 5f73 616d  size 1 --log_sam
-00002640: 706c 6573 202d 2d6c 6f67 5f73 616d 706c  ples --log_sampl
-00002650: 6573 5f73 7566 6669 7820 6c6c 6176 615f  es_suffix llava_
-00002660: 7631 2e35 5f6d 6d65 5f6d 6d62 656e 6368  v1.5_mme_mmbench
-00002670: 656e 202d 2d6f 7574 7075 745f 7061 7468  en --output_path
-00002680: 202e 2f6c 6f67 732f 2023 0a0a 2320 466f   ./logs/ #..# Fo
-00002690: 7220 6f74 6865 7220 7661 7269 616e 7473  r other variants
-000026a0: 206c 6c61 7661 2e20 4e6f 7465 2074 6861   llava. Note tha
-000026b0: 7420 6063 6f6e 765f 7465 6d70 6c61 7465  t `conv_template
-000026c0: 6020 6973 2061 6e20 6172 6720 6f66 2074  ` is an arg of t
-000026d0: 6865 2069 6e69 7420 6675 6e63 7469 6f6e  he init function
-000026e0: 206f 6620 6c6c 6176 6120 696e 2060 6c6d   of llava in `lm
-000026f0: 6d73 5f65 7661 6c2f 6d6f 6465 6c73 2f6c  ms_eval/models/l
-00002700: 6c61 7661 2e70 7960 0a61 6363 656c 6572  lava.py`.acceler
-00002710: 6174 6520 6c61 756e 6368 202d 2d6e 756d  ate launch --num
-00002720: 5f70 726f 6365 7373 6573 3d38 202d 6d20  _processes=8 -m 
-00002730: 6c6d 6d73 5f65 7661 6c20 2d2d 6d6f 6465  lmms_eval --mode
-00002740: 6c20 6c6c 6176 6120 2020 2d2d 6d6f 6465  l llava   --mode
-00002750: 6c5f 6172 6773 2070 7265 7472 6169 6e65  l_args pretraine
-00002760: 643d 226c 6975 6861 6f74 6961 6e2f 6c6c  d="liuhaotian/ll
-00002770: 6176 612d 7631 2e36 2d6d 6973 7472 616c  ava-v1.6-mistral
-00002780: 2d37 622c 636f 6e76 5f74 656d 706c 6174  -7b,conv_templat
-00002790: 653d 6d69 7374 7261 6c5f 696e 7374 7275  e=mistral_instru
-000027a0: 6374 2220 2020 2d2d 7461 736b 7320 6d6d  ct"   --tasks mm
-000027b0: 652c 6d6d 6265 6e63 685f 656e 202d 2d62  e,mmbench_en --b
-000027c0: 6174 6368 5f73 697a 6520 3120 2d2d 6c6f  atch_size 1 --lo
-000027d0: 675f 7361 6d70 6c65 7320 2d2d 6c6f 675f  g_samples --log_
-000027e0: 7361 6d70 6c65 735f 7375 6666 6978 206c  samples_suffix l
-000027f0: 6c61 7661 5f76 312e 355f 6d6d 655f 6d6d  lava_v1.5_mme_mm
-00002800: 6265 6e63 6865 6e20 2d2d 6f75 7470 7574  benchen --output
-00002810: 5f70 6174 6820 2e2f 6c6f 6773 2f20 230a  _path ./logs/ #.
-00002820: 6163 6365 6c65 7261 7465 206c 6175 6e63  accelerate launc
-00002830: 6820 2d2d 6e75 6d5f 7072 6f63 6573 7365  h --num_processe
-00002840: 733d 3820 2d6d 206c 6d6d 735f 6576 616c  s=8 -m lmms_eval
-00002850: 202d 2d6d 6f64 656c 206c 6c61 7661 2020   --model llava  
-00002860: 202d 2d6d 6f64 656c 5f61 7267 7320 7072   --model_args pr
-00002870: 6574 7261 696e 6564 3d22 6c69 7568 616f  etrained="liuhao
-00002880: 7469 616e 2f6c 6c61 7661 2d76 312e 362d  tian/llava-v1.6-
-00002890: 3334 622c 636f 6e76 5f74 656d 706c 6174  34b,conv_templat
-000028a0: 653d 6d69 7374 7261 6c5f 6469 7265 6374  e=mistral_direct
-000028b0: 2220 2020 2d2d 7461 736b 7320 6d6d 652c  "   --tasks mme,
-000028c0: 6d6d 6265 6e63 685f 656e 202d 2d62 6174  mmbench_en --bat
-000028d0: 6368 5f73 697a 6520 3120 2d2d 6c6f 675f  ch_size 1 --log_
-000028e0: 7361 6d70 6c65 7320 2d2d 6c6f 675f 7361  samples --log_sa
-000028f0: 6d70 6c65 735f 7375 6666 6978 206c 6c61  mples_suffix lla
-00002900: 7661 5f76 312e 355f 6d6d 655f 6d6d 6265  va_v1.5_mme_mmbe
-00002910: 6e63 6865 6e20 2d2d 6f75 7470 7574 5f70  nchen --output_p
-00002920: 6174 6820 2e2f 6c6f 6773 2f20 230a 0a23  ath ./logs/ #..#
-00002930: 2046 726f 6d20 6120 7072 6564 6566 696e   From a predefin
-00002940: 6564 2063 6f6e 6669 6775 7261 7469 6f6e  ed configuration
-00002950: 2c20 7375 7070 6f72 7469 6e67 2065 7661  , supporting eva
-00002960: 6c75 6174 696f 6e20 6f66 206d 756c 7469  luation of multi
-00002970: 706c 6520 6d6f 6465 6c73 2061 6e64 2064  ple models and d
-00002980: 6174 6173 6574 730a 6163 6365 6c65 7261  atasets.accelera
-00002990: 7465 206c 6175 6e63 6820 2d2d 6e75 6d5f  te launch --num_
-000029a0: 7072 6f63 6573 7365 733d 3820 2d6d 206c  processes=8 -m l
-000029b0: 6d6d 735f 6576 616c 202d 2d63 6f6e 6669  mms_eval --confi
-000029c0: 6720 6578 616d 706c 655f 6576 616c 2e79  g example_eval.y
-000029d0: 616d 6c20 0a60 6060 0a0a 2320 4d6f 6465  aml .```..# Mode
-000029e0: 6c20 5265 7375 6c74 730a 0a41 7320 6465  l Results..As de
-000029f0: 6d6f 6e73 7472 6174 6564 2062 7920 7468  monstrated by th
-00002a00: 6520 6578 7465 6e73 6976 6520 7461 626c  e extensive tabl
-00002a10: 6520 6265 6c6f 772c 2077 6520 6169 6d20  e below, we aim 
-00002a20: 746f 2070 726f 7669 6465 2064 6574 6169  to provide detai
-00002a30: 6c65 6420 696e 666f 726d 6174 696f 6e20  led information 
-00002a40: 666f 7220 7265 6164 6572 7320 746f 2075  for readers to u
-00002a50: 6e64 6572 7374 616e 6420 7468 6520 6461  nderstand the da
-00002a60: 7461 7365 7473 2069 6e63 6c75 6465 6420  tasets included 
-00002a70: 696e 206c 6d6d 732d 6576 616c 2061 6e64  in lmms-eval and
-00002a80: 2073 6f6d 6520 7370 6563 6966 6963 2064   some specific d
-00002a90: 6574 6169 6c73 2061 626f 7574 2074 6865  etails about the
-00002aa0: 7365 2064 6174 6173 6574 7320 2877 6520  se datasets (we 
-00002ab0: 7265 6d61 696e 2067 7261 7465 6675 6c20  remain grateful 
-00002ac0: 666f 7220 616e 7920 636f 7272 6563 7469  for any correcti
-00002ad0: 6f6e 7320 7265 6164 6572 7320 6d61 7920  ons readers may 
-00002ae0: 6861 7665 2064 7572 696e 6720 6f75 7220  have during our 
-00002af0: 6576 616c 7561 7469 6f6e 2070 726f 6365  evaluation proce
-00002b00: 7373 292e 0a0a 5765 2070 726f 7669 6465  ss)...We provide
-00002b10: 2061 2047 6f6f 676c 6520 5368 6565 7420   a Google Sheet 
-00002b20: 666f 7220 7468 6520 6465 7461 696c 6564  for the detailed
-00002b30: 2072 6573 756c 7473 206f 6620 7468 6520   results of the 
-00002b40: 4c4c 6156 4120 7365 7269 6573 206d 6f64  LLaVA series mod
-00002b50: 656c 7320 6f6e 2064 6966 6665 7265 6e74  els on different
-00002b60: 2064 6174 6173 6574 732e 2059 6f75 2063   datasets. You c
-00002b70: 616e 2061 6363 6573 7320 7468 6520 7368  an access the sh
-00002b80: 6565 7420 5b68 6572 655d 2868 7474 7073  eet [here](https
-00002b90: 3a2f 2f64 6f63 732e 676f 6f67 6c65 2e63  ://docs.google.c
-00002ba0: 6f6d 2f73 7072 6561 6473 6865 6574 732f  om/spreadsheets/
-00002bb0: 642f 3161 3549 6d66 644b 4154 4449 3854  d/1a5ImfdKATDI8T
-00002bc0: 3743 7768 3665 482d 6245 736e 5146 7a61  7Cwh6eH-bEsnQFza
-00002bd0: 6e46 7261 4655 6763 5339 4b48 5763 2f65  nFraFUgcS9KHWc/e
-00002be0: 6469 743f 7573 703d 7368 6172 696e 6729  dit?usp=sharing)
-00002bf0: 2e20 4974 2773 2061 206c 6976 6520 7368  . It's a live sh
-00002c00: 6565 742c 2061 6e64 2077 6520 6172 6520  eet, and we are 
-00002c10: 7570 6461 7469 6e67 2069 7420 7769 7468  updating it with
-00002c20: 206e 6577 2072 6573 756c 7473 2e0a 0a3c   new results...<
-00002c30: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
-00002c40: 2077 6964 7468 3d22 3130 3025 223e 0a3c   width="100%">.<
-00002c50: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00002c60: 2f69 2e70 6f73 7469 6d67 2e63 632f 6a64  /i.postimg.cc/jd
-00002c70: 7734 3937 4e53 2f57 5832 3032 3430 3330  w497NS/WX2024030
-00002c80: 372d 3136 3235 3236 2d32 782e 706e 6722  7-162526-2x.png"
-00002c90: 2020 7769 6474 683d 2231 3030 2522 2068    width="100%" h
-00002ca0: 6569 6768 743d 2238 3025 223e 0a3c 2f70  eight="80%">.</p
-00002cb0: 3e0a 0a57 6520 616c 736f 2070 726f 7669  >..We also provi
-00002cc0: 6465 2074 6865 2072 6177 2064 6174 6120  de the raw data 
-00002cd0: 6578 706f 7274 6564 2066 726f 6d20 5765  exported from We
-00002ce0: 6967 6874 7320 2620 4269 6173 6573 2066  ights & Biases f
-00002cf0: 6f72 2074 6865 2064 6574 6169 6c65 6420  or the detailed 
-00002d00: 7265 7375 6c74 7320 6f66 2074 6865 204c  results of the L
-00002d10: 4c61 5641 2073 6572 6965 7320 6d6f 6465  LaVA series mode
-00002d20: 6c73 206f 6e20 6469 6666 6572 656e 7420  ls on different 
-00002d30: 6461 7461 7365 7473 2e20 596f 7520 6361  datasets. You ca
-00002d40: 6e20 6163 6365 7373 2074 6865 2072 6177  n access the raw
-00002d50: 2064 6174 6120 5b68 6572 655d 2868 7474   data [here](htt
-00002d60: 7073 3a2f 2f64 6f63 732e 676f 6f67 6c65  ps://docs.google
-00002d70: 2e63 6f6d 2f73 7072 6561 6473 6865 6574  .com/spreadsheet
-00002d80: 732f 642f 3141 7661 456d 7547 3463 7353  s/d/1AvaEmuG4csS
-00002d90: 6d58 6148 6a67 7534 6569 314b 424d 6d4e  mXaHjgu4ei1KBMmN
-00002da0: 4e57 3877 666c 4f44 5f6b 6b54 4464 7638  NW8wflOD_kkTDdv8
-00002db0: 2f65 6469 743f 7573 703d 7368 6172 696e  /edit?usp=sharin
-00002dc0: 6729 2e0a 0a3e 2044 6576 656c 6f70 6d65  g)...> Developme
-00002dd0: 6e74 2077 696c 6c20 6265 2063 6f6e 7469  nt will be conti
-00002de0: 6e75 696e 6720 6f6e 2074 6865 206d 6169  nuing on the mai
-00002df0: 6e20 6272 616e 6368 2c20 616e 6420 7765  n branch, and we
-00002e00: 2065 6e63 6f75 7261 6765 2079 6f75 2074   encourage you t
-00002e10: 6f20 6769 7665 2075 7320 6665 6564 6261  o give us feedba
-00002e20: 636b 206f 6e20 7768 6174 2066 6561 7475  ck on what featu
-00002e30: 7265 7320 6172 6520 6465 7369 7265 6420  res are desired 
-00002e40: 616e 6420 686f 7720 746f 2069 6d70 726f  and how to impro
-00002e50: 7665 2074 6865 206c 6962 7261 7279 2066  ve the library f
-00002e60: 7572 7468 6572 2c20 6f72 2061 736b 2071  urther, or ask q
-00002e70: 7565 7374 696f 6e73 2c20 6569 7468 6572  uestions, either
-00002e80: 2069 6e20 6973 7375 6573 206f 7220 5052   in issues or PR
-00002e90: 7320 6f6e 2047 6974 4875 622e 0a0a 0a23  s on GitHub....#
-00002ea0: 2320 5375 7070 6f72 7465 6420 6d6f 6465  # Supported mode
-00002eb0: 6c73 0a0a 2d20 4750 5434 5620 2841 5049  ls..- GPT4V (API
-00002ec0: 2c20 6f6e 6c79 2067 656e 6572 6174 696f  , only generatio
-00002ed0: 6e2d 6261 7365 6420 6576 616c 7561 7469  n-based evaluati
-00002ee0: 6f6e 290a 2d20 4c4c 6156 412d 7631 2e35  on).- LLaVA-v1.5
-00002ef0: 2f76 312e 362d 3742 2f31 3342 2f33 3442  /v1.6-7B/13B/34B
-00002f00: 2028 7070 6c2d 6261 7365 642c 2067 656e   (ppl-based, gen
-00002f10: 6572 6174 696f 6e2d 6261 7365 6429 0a2d  eration-based).-
-00002f20: 2051 7765 6e2d 564c 2073 6572 6965 7320   Qwen-VL series 
-00002f30: 2870 706c 2d62 6173 6564 2c20 6765 6e65  (ppl-based, gene
-00002f40: 7261 7469 6f6e 2d62 6173 6564 290a 2d20  ration-based).- 
-00002f50: 4675 7975 2073 6572 6965 7320 2870 706c  Fuyu series (ppl
-00002f60: 2d62 6173 6564 2c20 6765 6e65 7261 7469  -based, generati
-00002f70: 6f6e 2d62 6173 6564 290a 2d20 496e 7374  on-based).- Inst
-00002f80: 7275 6374 424c 4950 2073 6572 6965 7320  ructBLIP series 
-00002f90: 2867 656e 6572 6174 696f 6e2d 6261 7365  (generation-base
-00002fa0: 6429 0a0a 2323 2053 7570 706f 7274 6564  d)..## Supported
-00002fb0: 2064 6174 6173 6574 730a 3e20 2829 2069   datasets.> () i
-00002fc0: 6e64 6963 6174 6573 2074 6865 2074 6173  ndicates the tas
-00002fd0: 6b20 6e61 6d65 2069 6e20 7468 6520 6c6d  k name in the lm
-00002fe0: 6d73 5f65 7661 6c2e 2054 6865 2074 6173  ms_eval. The tas
-00002ff0: 6b20 6e61 6d65 2069 7320 616c 736f 2075  k name is also u
-00003000: 7365 6420 746f 2073 7065 6369 6679 2074  sed to specify t
-00003010: 6865 2064 6174 6173 6574 2069 6e20 7468  he dataset in th
-00003020: 6520 636f 6e66 6967 7572 6174 696f 6e20  e configuration 
-00003030: 6669 6c65 2e0a 0a2d 2041 4932 4420 2861  file...- AI2D (a
-00003040: 6932 6429 0a2d 2043 6861 7274 5141 2028  i2d).- ChartQA (
-00003050: 6368 6172 7471 6129 0a2d 2043 4d4d 4d55  chartqa).- CMMMU
-00003060: 2028 636d 6d6d 7529 0a20 202d 2043 4d4d   (cmmmu).  - CMM
-00003070: 4d55 2056 616c 6964 6174 696f 6e20 2863  MU Validation (c
-00003080: 6d6d 6d75 5f76 616c 290a 2020 2d20 434d  mmmu_val).  - CM
-00003090: 4d4d 5520 5465 7374 2028 636d 6d6d 755f  MMU Test (cmmmu_
-000030a0: 7465 7374 290a 2d20 434f 434f 2043 6170  test).- COCO Cap
-000030b0: 7469 6f6e 2028 636f 636f 5f63 6170 290a  tion (coco_cap).
-000030c0: 2020 2d20 434f 434f 2032 3031 3420 4361    - COCO 2014 Ca
-000030d0: 7074 696f 6e20 2863 6f63 6f32 3031 345f  ption (coco2014_
-000030e0: 6361 7029 0a20 2020 202d 2043 4f43 4f20  cap).    - COCO 
-000030f0: 3230 3134 2043 6170 7469 6f6e 2056 616c  2014 Caption Val
-00003100: 6964 6174 696f 6e20 2863 6f63 6f32 3031  idation (coco201
-00003110: 345f 6361 705f 7661 6c29 0a20 2020 202d  4_cap_val).    -
-00003120: 2043 4f43 4f20 3230 3134 2043 6170 7469   COCO 2014 Capti
-00003130: 6f6e 2054 6573 7420 2863 6f63 6f32 3031  on Test (coco201
-00003140: 345f 6361 705f 7465 7374 290a 2020 2d20  4_cap_test).  - 
-00003150: 434f 434f 2032 3031 3720 4361 7074 696f  COCO 2017 Captio
-00003160: 6e20 2863 6f63 6f32 3031 375f 6361 7029  n (coco2017_cap)
-00003170: 0a20 2020 202d 2043 4f43 4f20 3230 3137  .    - COCO 2017
-00003180: 2043 6170 7469 6f6e 204d 696e 6956 616c   Caption MiniVal
-00003190: 2028 636f 636f 3230 3137 5f63 6170 5f76   (coco2017_cap_v
-000031a0: 616c 290a 2020 2020 2d20 434f 434f 2032  al).    - COCO 2
-000031b0: 3031 3720 4361 7074 696f 6e20 4d69 6e69  017 Caption Mini
-000031c0: 5465 7374 2028 636f 636f 3230 3137 5f63  Test (coco2017_c
-000031d0: 6170 5f74 6573 7429 0a2d 2044 4f43 5651  ap_test).- DOCVQ
-000031e0: 4120 2864 6f63 7671 6129 0a20 202d 2044  A (docvqa).  - D
-000031f0: 4f43 5651 4120 5661 6c69 6461 7469 6f6e  OCVQA Validation
-00003200: 2028 646f 6376 7161 5f76 616c 290a 2020   (docvqa_val).  
-00003210: 2d20 444f 4356 5141 2054 6573 7420 2864  - DOCVQA Test (d
-00003220: 6f63 7671 615f 7465 7374 290a 2d20 4665  ocvqa_test).- Fe
-00003230: 7272 6574 2028 6665 7272 6574 290a 2d20  rret (ferret).- 
-00003240: 466c 6963 6b72 3330 4b20 2866 6c69 636b  Flickr30K (flick
-00003250: 7233 306b 290a 2020 2d20 4665 7272 6574  r30k).  - Ferret
-00003260: 2054 6573 7420 2866 6572 7265 745f 7465   Test (ferret_te
-00003270: 7374 290a 2d20 4751 4120 2867 7161 290a  st).- GQA (gqa).
-00003280: 2d20 4861 6c6c 7573 696f 6e42 656e 6368  - HallusionBench
-00003290: 6d61 726b 2028 6861 6c6c 7573 696f 6e5f  mark (hallusion_
-000032a0: 6265 6e63 685f 696d 6167 6529 0a2d 2049  bench_image).- I
-000032b0: 6e66 6f67 7261 7068 6963 2056 5141 2028  nfographic VQA (
-000032c0: 696e 666f 5f76 7161 290a 2020 2d20 496e  info_vqa).  - In
-000032d0: 666f 6772 6170 6869 6320 5651 4120 5661  fographic VQA Va
-000032e0: 6c69 6461 7469 6f6e 2028 696e 666f 5f76  lidation (info_v
-000032f0: 7161 5f76 616c 290a 2020 2d20 496e 666f  qa_val).  - Info
-00003300: 6772 6170 6869 6320 5651 4120 5465 7374  graphic VQA Test
-00003310: 2028 696e 666f 5f76 7161 5f74 6573 7429   (info_vqa_test)
-00003320: 0a2d 204c 4c61 5641 2d42 656e 6368 2028  .- LLaVA-Bench (
-00003330: 6c6c 6176 615f 696e 5f74 6865 5f77 696c  llava_in_the_wil
-00003340: 6429 0a2d 204c 4c61 5641 2d42 656e 6368  d).- LLaVA-Bench
-00003350: 2d43 4f43 4f20 286c 6c61 7661 5f62 656e  -COCO (llava_ben
-00003360: 6368 5f63 6f63 6f29 0a2d 204d 6174 6856  ch_coco).- MathV
-00003370: 6973 7461 2028 6d61 7468 7669 7374 6129  ista (mathvista)
-00003380: 0a20 202d 204d 6174 6856 6973 7461 2056  .  - MathVista V
-00003390: 616c 6964 6174 696f 6e20 286d 6174 6876  alidation (mathv
-000033a0: 6973 7461 5f74 6573 746d 696e 6929 0a20  ista_testmini). 
-000033b0: 202d 204d 6174 6856 6973 7461 2054 6573   - MathVista Tes
-000033c0: 7420 286d 6174 6876 6973 7461 5f74 6573  t (mathvista_tes
-000033d0: 7429 0a2d 204d 4d42 656e 6368 2028 6d6d  t).- MMBench (mm
-000033e0: 6265 6e63 6829 0a20 202d 204d 4d42 656e  bench).  - MMBen
-000033f0: 6368 2045 6e67 6c69 7368 2028 6d6d 6265  ch English (mmbe
-00003400: 6e63 685f 656e 290a 2020 2020 2d20 4d4d  nch_en).    - MM
-00003410: 4265 6e63 6820 456e 676c 6973 6820 4465  Bench English De
-00003420: 7620 286d 6d62 656e 6368 5f65 6e5f 6465  v (mmbench_en_de
-00003430: 7629 0a20 2020 202d 204d 4d42 656e 6368  v).    - MMBench
-00003440: 2045 6e67 6c69 7368 2054 6573 7420 286d   English Test (m
-00003450: 6d62 656e 6368 5f65 6e5f 7465 7374 290a  mbench_en_test).
-00003460: 2020 2d20 4d4d 4265 6e63 6820 4368 696e    - MMBench Chin
-00003470: 6573 6520 286d 6d62 656e 6368 5f63 6e29  ese (mmbench_cn)
-00003480: 0a20 2020 202d 204d 4d42 656e 6368 2043  .    - MMBench C
-00003490: 6869 6e65 7365 2044 6576 2028 6d6d 6265  hinese Dev (mmbe
-000034a0: 6e63 685f 636e 5f64 6576 290a 2020 2020  nch_cn_dev).    
-000034b0: 2d20 4d4d 4265 6e63 6820 4368 696e 6573  - MMBench Chines
-000034c0: 6520 5465 7374 2028 6d6d 6265 6e63 685f  e Test (mmbench_
-000034d0: 636e 5f74 6573 7429 0a2d 204d 4d45 2028  cn_test).- MME (
-000034e0: 6d6d 6529 0a2d 204d 4d4d 5520 286d 6d6d  mme).- MMMU (mmm
-000034f0: 7529 0a20 202d 204d 4d4d 5520 5661 6c69  u).  - MMMU Vali
-00003500: 6461 7469 6f6e 2028 6d6d 6d75 5f76 616c  dation (mmmu_val
-00003510: 290a 2020 2d20 4d4d 4d55 2054 6573 7420  ).  - MMMU Test 
-00003520: 286d 6d6d 755f 7465 7374 290a 2d20 4d4d  (mmmu_test).- MM
-00003530: 5665 7420 286d 6d76 6574 290a 2d20 4d75  Vet (mmvet).- Mu
-00003540: 6c74 692d 446f 6356 5141 2028 6d75 6c74  lti-DocVQA (mult
-00003550: 6964 6f63 7671 6129 0a20 202d 204d 756c  idocvqa).  - Mul
-00003560: 7469 2d44 6f63 5651 4120 5661 6c69 6461  ti-DocVQA Valida
-00003570: 7469 6f6e 2028 6d75 6c74 6964 6f63 7671  tion (multidocvq
-00003580: 615f 7661 6c29 0a20 202d 204d 756c 7469  a_val).  - Multi
-00003590: 2d44 6f63 5651 4120 5465 7374 2028 6d75  -DocVQA Test (mu
-000035a0: 6c74 6964 6f63 7671 615f 7465 7374 290a  ltidocvqa_test).
-000035b0: 2d20 4e6f 4361 7073 2028 6e6f 6361 7073  - NoCaps (nocaps
-000035c0: 290a 2020 2d20 4e6f 4361 7073 2056 616c  ).  - NoCaps Val
-000035d0: 6964 6174 696f 6e20 286e 6f63 6170 735f  idation (nocaps_
-000035e0: 7661 6c29 0a20 202d 204e 6f43 6170 7320  val).  - NoCaps 
-000035f0: 5465 7374 2028 6e6f 6361 7073 5f74 6573  Test (nocaps_tes
-00003600: 7429 0a2d 204f 4b56 5141 2028 6f6b 5f76  t).- OKVQA (ok_v
-00003610: 7161 290a 2020 2d20 4f4b 5651 4120 5661  qa).  - OKVQA Va
-00003620: 6c69 6461 7469 6f6e 2032 3031 3420 286f  lidation 2014 (o
-00003630: 6b5f 7671 615f 7661 6c32 3031 3429 0a2d  k_vqa_val2014).-
-00003640: 2050 4f50 4520 2870 6f70 6529 0a2d 2052   POPE (pope).- R
-00003650: 6566 434f 434f 2028 7265 6663 6f63 6f29  efCOCO (refcoco)
-00003660: 0a20 2020 202d 2072 6566 636f 636f 5f73  .    - refcoco_s
-00003670: 6567 5f74 6573 740a 2020 2020 2d20 7265  eg_test.    - re
-00003680: 6663 6f63 6f5f 7365 675f 7661 6c0a 2020  fcoco_seg_val.  
-00003690: 2020 2d20 7265 6663 6f63 6f5f 7365 675f    - refcoco_seg_
-000036a0: 7465 7374 410a 2020 2020 2d20 7265 6663  testA.    - refc
-000036b0: 6f63 6f5f 7365 675f 7465 7374 420a 2020  oco_seg_testB.  
-000036c0: 2020 2d20 7265 6663 6f63 6f5f 6262 6f78    - refcoco_bbox
-000036d0: 5f74 6573 740a 2020 2020 2d20 7265 6663  _test.    - refc
-000036e0: 6f63 6f5f 6262 6f78 5f76 616c 0a20 2020  oco_bbox_val.   
-000036f0: 202d 2072 6566 636f 636f 5f62 626f 785f   - refcoco_bbox_
-00003700: 7465 7374 410a 2020 2020 2d20 7265 6663  testA.    - refc
-00003710: 6f63 6f5f 6262 6f78 5f74 6573 7442 0a2d  oco_bbox_testB.-
-00003720: 2052 6566 434f 434f 2b20 2872 6566 636f   RefCOCO+ (refco
-00003730: 636f 2b29 0a20 2020 202d 2072 6566 636f  co+).    - refco
-00003740: 636f 2b5f 7365 670a 2020 2020 2020 2020  co+_seg.        
-00003750: 2d20 7265 6663 6f63 6f2b 5f73 6567 5f76  - refcoco+_seg_v
-00003760: 616c 0a20 2020 2020 2020 202d 2072 6566  al.        - ref
-00003770: 636f 636f 2b5f 7365 675f 7465 7374 410a  coco+_seg_testA.
-00003780: 2020 2020 2020 2020 2d20 7265 6663 6f63          - refcoc
-00003790: 6f2b 5f73 6567 5f74 6573 7442 0a20 2020  o+_seg_testB.   
-000037a0: 202d 2072 6566 636f 636f 2b5f 6262 6f78   - refcoco+_bbox
-000037b0: 0a20 2020 2020 2020 202d 2072 6566 636f  .        - refco
-000037c0: 636f 2b5f 6262 6f78 5f76 616c 0a20 2020  co+_bbox_val.   
-000037d0: 2020 2020 202d 2072 6566 636f 636f 2b5f       - refcoco+_
-000037e0: 6262 6f78 5f74 6573 7441 0a20 2020 2020  bbox_testA.     
-000037f0: 2020 202d 2072 6566 636f 636f 2b5f 6262     - refcoco+_bb
-00003800: 6f78 5f74 6573 7442 0a2d 2052 6566 434f  ox_testB.- RefCO
-00003810: 434f 6720 2872 6566 636f 636f 6729 0a20  COg (refcocog). 
-00003820: 2020 202d 2072 6566 636f 636f 675f 7365     - refcocog_se
-00003830: 675f 7465 7374 0a20 2020 202d 2072 6566  g_test.    - ref
-00003840: 636f 636f 675f 7365 675f 7661 6c0a 2020  cocog_seg_val.  
-00003850: 2020 2d20 7265 6663 6f63 6f67 5f62 626f    - refcocog_bbo
-00003860: 785f 7465 7374 0a20 2020 202d 2072 6566  x_test.    - ref
-00003870: 636f 636f 675f 6262 6f78 5f76 616c 0a2d  cocog_bbox_val.-
-00003880: 2053 6369 656e 6365 5141 2028 7363 6965   ScienceQA (scie
-00003890: 6e63 6571 615f 6675 6c6c 290a 2020 2d20  nceqa_full).  - 
-000038a0: 5363 6965 6e63 6551 4120 4675 6c6c 2028  ScienceQA Full (
-000038b0: 7363 6965 6e63 6571 6129 0a20 202d 2053  scienceqa).  - S
-000038c0: 6369 656e 6365 5141 2049 4d47 2028 7363  cienceQA IMG (sc
-000038d0: 6965 6e63 6571 615f 696d 6729 0a2d 2053  ienceqa_img).- S
-000038e0: 6565 6442 656e 6368 2028 7365 6564 6265  eedBench (seedbe
-000038f0: 6e63 6829 0a2d 2053 6565 6442 656e 6368  nch).- SeedBench
-00003900: 2032 2028 7365 6564 6265 6e63 685f 3229   2 (seedbench_2)
-00003910: 0a2d 2053 542d 5651 4120 2873 7476 7161  .- ST-VQA (stvqa
-00003920: 290a 2d20 5465 7874 4361 7073 2028 7465  ).- TextCaps (te
-00003930: 7874 6361 7073 290a 2020 2d20 5465 7874  xtcaps).  - Text
-00003940: 4361 7073 2056 616c 6964 6174 696f 6e20  Caps Validation 
-00003950: 2874 6578 7463 6170 735f 7661 6c29 0a20  (textcaps_val). 
-00003960: 202d 2054 6578 7443 6170 7320 5465 7374   - TextCaps Test
-00003970: 2028 7465 7874 6361 7073 5f74 6573 7429   (textcaps_test)
-00003980: 0a2d 2054 6578 7456 5141 2028 7465 7874  .- TextVQA (text
-00003990: 7671 6129 0a20 202d 2054 6578 7456 5141  vqa).  - TextVQA
-000039a0: 2056 616c 6964 6174 696f 6e20 2874 6578   Validation (tex
-000039b0: 7476 7161 5f76 616c 290a 2020 2d20 5465  tvqa_val).  - Te
-000039c0: 7874 5651 4120 5465 7374 2028 7465 7874  xtVQA Test (text
-000039d0: 7671 615f 7465 7374 290a 2d20 5669 7a57  vqa_test).- VizW
-000039e0: 697a 5651 4120 2876 697a 7769 7a5f 7671  izVQA (vizwiz_vq
-000039f0: 6129 0a20 202d 2056 697a 5769 7a56 5141  a).  - VizWizVQA
-00003a00: 2056 616c 6964 6174 696f 6e20 2876 697a   Validation (viz
-00003a10: 7769 7a5f 7671 615f 7661 6c29 0a20 202d  wiz_vqa_val).  -
-00003a20: 2056 697a 5769 7a56 5141 2054 6573 7420   VizWizVQA Test 
-00003a30: 2876 697a 7769 7a5f 7671 615f 7465 7374  (vizwiz_vqa_test
-00003a40: 290a 2d20 5651 4176 3220 2876 7161 7632  ).- VQAv2 (vqav2
-00003a50: 290a 2020 2d20 5651 4176 3220 5661 6c69  ).  - VQAv2 Vali
-00003a60: 6461 7469 6f6e 2028 7671 6176 325f 7661  dation (vqav2_va
-00003a70: 6c29 0a20 202d 2056 5141 7632 2054 6573  l).  - VQAv2 Tes
-00003a80: 7420 2876 7161 7632 5f74 6573 7429 0a0a  t (vqav2_test)..
-00003a90: 2323 2044 6174 6173 6574 7320 746f 2062  ## Datasets to b
-00003aa0: 6520 6164 6465 6420 616e 6420 7465 7374  e added and test
-00003ab0: 6564 0a2d 2054 616c 6c79 5141 2028 7461  ed.- TallyQA (ta
-00003ac0: 6c6c 7971 6129 0a2d 2056 5352 2028 7673  llyqa).- VSR (vs
-00003ad0: 7229 0a2d 2057 696e 6f67 726f 756e 6420  r).- Winoground 
-00003ae0: 2877 696e 6f67 726f 756e 6429 0a2d 204e  (winoground).- N
-00003af0: 4c56 5232 2028 6e6c 7672 3229 0a2d 2052  LVR2 (nlvr2).- R
-00003b00: 6176 656e 4951 2d54 6573 7420 2872 6176  avenIQ-Test (rav
-00003b10: 656e 6971 290a 2d20 4963 6f6e 5141 2028  eniq).- IconQA (
-00003b20: 6963 6f6e 7161 290a 2d20 5669 7374 4265  iconqa).- VistBe
-00003b30: 6e63 6820 2876 6973 7462 656e 6368 290a  nch (vistbench).
-00003b40: 0a23 2041 6464 2043 7573 746f 6d69 7a65  .# Add Customize
-00003b50: 6420 4d6f 6465 6c20 616e 6420 4461 7461  d Model and Data
-00003b60: 7365 740a 0a50 6c65 6173 6520 7265 6665  set..Please refe
-00003b70: 7220 746f 206f 7572 205b 646f 6375 6d65  r to our [docume
-00003b80: 6e74 6174 696f 6e5d 2864 6f63 732f 5245  ntation](docs/RE
-00003b90: 4144 4d45 2e6d 6429 2e0a 0a23 2041 636b  ADME.md)...# Ack
-00003ba0: 6e6f 776c 6564 6765 6d65 6e74 0a0a 6c6d  nowledgement..lm
-00003bb0: 6d73 5f65 7661 6c20 6973 2061 2066 6f72  ms_eval is a for
-00003bc0: 6b20 6f66 205b 6c6d 2d65 7661 6c2d 6861  k of [lm-eval-ha
-00003bd0: 726e 6573 735d 2868 7474 7073 3a2f 2f67  rness](https://g
-00003be0: 6974 6875 622e 636f 6d2f 456c 6575 7468  ithub.com/Eleuth
-00003bf0: 6572 4149 2f6c 6d2d 6576 616c 7561 7469  erAI/lm-evaluati
-00003c00: 6f6e 2d68 6172 6e65 7373 292e 2057 6520  on-harness). We 
-00003c10: 7265 636f 6d6d 656e 6420 796f 7520 746f  recommend you to
-00003c20: 2072 6561 6420 7468 726f 7567 6820 7468   read through th
-00003c30: 6520 5b64 6f63 7320 6f66 206c 6d2d 6576  e [docs of lm-ev
-00003c40: 616c 2d68 6172 6e65 7373 5d28 6874 7470  al-harness](http
-00003c50: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f45  s://github.com/E
-00003c60: 6c65 7574 6865 7241 492f 6c6d 2d65 7661  leutherAI/lm-eva
-00003c70: 6c75 6174 696f 6e2d 6861 726e 6573 732f  luation-harness/
-00003c80: 7472 6565 2f6d 6169 6e2f 646f 6373 2920  tree/main/docs) 
-00003c90: 666f 7220 7265 6c65 7661 6e74 2069 6e66  for relevant inf
-00003ca0: 6f72 6d61 7469 6f6e 2e20 0a0a 4265 6c6f  ormation. ..Belo
-00003cb0: 7720 6172 6520 7468 6520 6368 616e 6765  w are the change
-00003cc0: 7320 7765 206d 6164 6520 746f 2074 6865  s we made to the
-00003cd0: 206f 7269 6769 6e61 6c20 4150 493a 0a2d   original API:.-
-00003ce0: 2042 7569 6c64 2063 6f6e 7465 7874 206e   Build context n
-00003cf0: 6f77 206f 6e6c 7920 7061 7373 2069 6e20  ow only pass in 
-00003d00: 6964 7820 616e 6420 7072 6f63 6573 7320  idx and process 
-00003d10: 696d 6167 6520 616e 6420 646f 6320 6475  image and doc du
-00003d20: 7269 6e67 2074 6865 206d 6f64 656c 2072  ring the model r
-00003d30: 6573 706f 6e64 696e 6720 7068 6173 652e  esponding phase.
-00003d40: 2054 6869 7320 6973 2064 7565 2074 6f20   This is due to 
-00003d50: 7468 6520 6661 6374 2074 6861 7420 6461  the fact that da
-00003d60: 7461 7365 7420 6e6f 7720 636f 6e74 6169  taset now contai
-00003d70: 6e73 206c 6f74 7320 6f66 2069 6d61 6765  ns lots of image
-00003d80: 7320 616e 6420 7765 2063 616e 2774 2073  s and we can't s
-00003d90: 746f 7265 2074 6865 6d20 696e 2074 6865  tore them in the
-00003da0: 2064 6f63 206c 696b 6520 7468 6520 6f72   doc like the or
-00003db0: 6967 696e 616c 206c 6d2d 6576 616c 2d68  iginal lm-eval-h
-00003dc0: 6172 6e65 7373 206f 7468 6572 2077 6973  arness other wis
-00003dd0: 6520 7468 6520 6370 7520 6d65 6d6f 7279  e the cpu memory
-00003de0: 2077 6f75 6c64 2065 7870 6c6f 6465 2e0a   would explode..
-00003df0: 2d20 496e 7374 616e 6365 2e61 7267 7320  - Instance.args 
-00003e00: 286c 6d6d 735f 6576 616c 2f61 7069 2f69  (lmms_eval/api/i
-00003e10: 6e73 7461 6e63 652e 7079 2920 6e6f 7720  nstance.py) now 
-00003e20: 636f 6e74 6169 6e73 2061 206c 6973 7420  contains a list 
-00003e30: 6f66 2069 6d61 6765 7320 746f 2062 6520  of images to be 
-00003e40: 696e 7075 7474 6564 2074 6f20 6c6d 6d73  inputted to lmms
-00003e50: 2e0a 2d20 6c6d 2d65 7661 6c2d 6861 726e  ..- lm-eval-harn
-00003e60: 6573 7320 7375 7070 6f72 7473 2061 6c6c  ess supports all
-00003e70: 2048 4620 6c61 6e67 7561 6765 206d 6f64   HF language mod
-00003e80: 656c 7320 6173 2073 696e 676c 6520 6d6f  els as single mo
-00003e90: 6465 6c20 636c 6173 732e 2043 7572 7265  del class. Curre
-00003ea0: 6e74 6c79 2074 6869 7320 6973 206e 6f74  ntly this is not
-00003eb0: 2070 6f73 7369 626c 6520 6f66 206c 6d6d   possible of lmm
-00003ec0: 7320 6265 6361 7573 6520 7468 6520 696e  s because the in
-00003ed0: 7075 742f 6f75 7470 7574 2066 6f72 6d61  put/output forma
-00003ee0: 7420 6f66 206c 6d6d 7320 696e 2048 4620  t of lmms in HF 
-00003ef0: 6172 6520 6e6f 7420 7965 7420 756e 6966  are not yet unif
-00003f00: 6965 642e 2054 6865 7265 7266 6f72 652c  ied. Thererfore,
-00003f10: 2077 6520 6861 7665 2074 6f20 6372 6561   we have to crea
-00003f20: 7465 2061 206e 6577 2063 6c61 7373 2066  te a new class f
-00003f30: 6f72 2065 6163 6820 6c6d 6d73 206d 6f64  or each lmms mod
-00003f40: 656c 2e20 5468 6973 2069 7320 6e6f 7420  el. This is not 
-00003f50: 6964 6561 6c20 616e 6420 7765 2077 696c  ideal and we wil
-00003f60: 6c20 7472 7920 746f 2075 6e69 6679 2074  l try to unify t
-00003f70: 6865 6d20 696e 2074 6865 2066 7574 7572  hem in the futur
-00003f80: 652e 0a0a 5765 2061 6c73 6f20 7468 616e  e...We also than
-00003f90: 6b3a 0a2d 205b 5869 616e 6720 5975 655d  k:.- [Xiang Yue]
-00003fa0: 2868 7474 7073 3a2f 2f78 6961 6e67 7975  (https://xiangyu
-00003fb0: 6539 3630 372e 6769 7468 7562 2e69 6f2f  e9607.github.io/
-00003fc0: 292c 205b 4a69 6e67 6b61 6e67 2059 616e  ), [Jingkang Yan
-00003fd0: 675d 2868 7474 7073 3a2f 2f6a 696e 676b  g](https://jingk
-00003fe0: 616e 6735 302e 6769 7468 7562 2e69 6f2f  ang50.github.io/
-00003ff0: 292c 205b 446f 6e67 2047 756f 5d28 6874  ), [Dong Guo](ht
-00004000: 7470 733a 2f2f 7777 772e 6c69 6e6b 6564  tps://www.linked
-00004010: 696e 2e63 6f6d 2f69 6e2f 646f 6e67 6775  in.com/in/donggu
-00004020: 6f73 6574 2f29 2061 6e64 205b 5368 656e  oset/) and [Shen
-00004030: 6720 5368 656e 5d28 6874 7470 733a 2f2f  g Shen](https://
-00004040: 7369 6e63 6572 6173 732e 6769 7468 7562  sincerass.github
-00004050: 2e69 6f2f 2920 666f 7220 6561 726c 7920  .io/) for early 
-00004060: 6469 7363 7573 7369 6f6e 2061 6e64 2074  discussion and t
-00004070: 6573 7469 6e67 2e0a 0a23 2320 4369 7461  esting...## Cita
-00004080: 7469 6f6e 730a 0a60 6060 7368 656c 6c0a  tions..```shell.
-00004090: 406d 6973 637b 6c6d 6d73 5f65 7661 6c32  @misc{lmms_eval2
-000040a0: 3032 342c 0a20 2020 2074 6974 6c65 3d7b  024,.    title={
-000040b0: 4c4d 4d73 2d45 7661 6c3a 2041 6363 656c  LMMs-Eval: Accel
-000040c0: 6572 6174 696e 6720 7468 6520 4465 7665  erating the Deve
-000040d0: 6c6f 706d 656e 7420 6f66 204c 6172 6765  lopment of Large
-000040e0: 204d 756c 7469 6d6f 616c 204d 6f64 656c   Multimoal Model
-000040f0: 737d 2c0a 2020 2020 7572 6c3d 7b68 7474  s},.    url={htt
-00004100: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00004110: 4576 6f6c 7669 6e67 4c4d 4d73 2d4c 6162  EvolvingLMMs-Lab
-00004120: 2f6c 6d6d 732d 6576 616c 7d2c 0a20 2020  /lmms-eval},.   
-00004130: 2061 7574 686f 723d 7b42 6f20 4c69 2a2c   author={Bo Li*,
-00004140: 2050 6569 7975 616e 205a 6861 6e67 2a2c   Peiyuan Zhang*,
-00004150: 204b 6169 6368 656e 205a 6861 6e67 2a2c   Kaichen Zhang*,
-00004160: 2046 616e 7969 2050 752a 2c20 5869 6e72   Fanyi Pu*, Xinr
-00004170: 756e 2044 752c 2059 7568 616f 2044 6f6e  un Du, Yuhao Don
-00004180: 672c 2048 616f 7469 616e 204c 6975 2c20  g, Haotian Liu, 
-00004190: 5975 616e 6861 6e20 5a68 616e 672c 2047  Yuanhan Zhang, G
-000041a0: 6520 5a68 616e 672c 2043 6875 6e79 7561  e Zhang, Chunyua
-000041b0: 6e20 4c69 2061 6e64 205a 6977 6569 204c  n Li and Ziwei L
-000041c0: 6975 7d2c 0a20 2020 2070 7562 6c69 7368  iu},.    publish
-000041d0: 6572 2020 2020 3d20 7b5a 656e 6f64 6f7d  er    = {Zenodo}
-000041e0: 2c0a 2020 2020 7665 7273 696f 6e20 2020  ,.    version   
-000041f0: 2020 203d 207b 7630 2e31 2e30 7d2c 0a20     = {v0.1.0},. 
-00004200: 2020 206d 6f6e 7468 3d7b 4d61 7263 687d     month={March}
-00004210: 2c0a 2020 2020 7965 6172 3d7b 3230 3234  ,.    year={2024
-00004220: 7d0a 7d0a 6060 600a                      }.}.```.
+00000430: 616e 7366 6f72 6d65 7273 0a52 6571 7569  ansformers.Requi
+00000440: 7265 732d 4469 7374 3a20 7a73 7461 6e64  res-Dist: zstand
+00000450: 6172 640a 5265 7175 6972 6573 2d44 6973  ard.Requires-Dis
+00000460: 743a 2070 696c 6c6f 770a 5265 7175 6972  t: pillow.Requir
+00000470: 6573 2d44 6973 743a 2070 7979 616d 6c0a  es-Dist: pyyaml.
+00000480: 5265 7175 6972 6573 2d44 6973 743a 2073  Requires-Dist: s
+00000490: 796d 7079 0a52 6571 7569 7265 732d 4469  ympy.Requires-Di
+000004a0: 7374 3a20 6d70 6d61 7468 0a52 6571 7569  st: mpmath.Requi
+000004b0: 7265 732d 4469 7374 3a20 4a69 6e6a 6132  res-Dist: Jinja2
+000004c0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+000004d0: 6f70 656e 7079 786c 0a52 6571 7569 7265  openpyxl.Require
+000004e0: 732d 4469 7374 3a20 4c65 7665 6e73 6874  s-Dist: Levensht
+000004f0: 6569 6e0a 5265 7175 6972 6573 2d44 6973  ein.Requires-Dis
+00000500: 743a 2068 665f 7472 616e 7366 6572 0a52  t: hf_transfer.R
+00000510: 6571 7569 7265 732d 4469 7374 3a20 7465  equires-Dist: te
+00000520: 6e61 6369 7479 0a52 6571 7569 7265 732d  nacity.Requires-
+00000530: 4469 7374 3a20 7761 6e64 623e 3d30 2e31  Dist: wandb>=0.1
+00000540: 362e 300a 5265 7175 6972 6573 2d44 6973  6.0.Requires-Dis
+00000550: 743a 2074 7261 6e73 666f 726d 6572 732d  t: transformers-
+00000560: 7374 7265 616d 2d67 656e 6572 6174 6f72  stream-generator
+00000570: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000580: 7469 6b74 6f6b 656e 0a52 6571 7569 7265  tiktoken.Require
+00000590: 732d 4469 7374 3a20 7072 652d 636f 6d6d  s-Dist: pre-comm
+000005a0: 6974 0a52 6571 7569 7265 732d 4469 7374  it.Requires-Dist
+000005b0: 3a20 7079 6461 6e74 6963 0a0a 3c70 2061  : pydantic..<p a
+000005c0: 6c69 676e 3d22 6365 6e74 6572 2220 7769  lign="center" wi
+000005d0: 6474 683d 2231 3030 2522 3e0a 3c69 6d67  dth="100%">.<img
+000005e0: 2073 7263 3d22 6874 7470 733a 2f2f 692e   src="https://i.
+000005f0: 706f 7374 696d 672e 6363 2f67 3051 5267  postimg.cc/g0QRg
+00000600: 4d56 762f 5758 3230 3234 3032 3238 2d31  MVv/WX20240228-1
+00000610: 3133 3333 372d 3278 2e70 6e67 2220 2077  13337-2x.png"  w
+00000620: 6964 7468 3d22 3130 3025 2220 6865 6967  idth="100%" heig
+00000630: 6874 3d22 3730 2522 3e0a 3c2f 703e 0a0a  ht="70%">.</p>..
+00000640: 2320 5468 6520 4576 616c 7561 7469 6f6e  # The Evaluation
+00000650: 2053 7569 7465 206f 6620 4c61 7267 6520   Suite of Large 
+00000660: 4d75 6c74 696d 6f64 616c 204d 6f64 656c  Multimodal Model
+00000670: 7320 0a0a 3e20 4163 6365 6c65 7261 7469  s ..> Accelerati
+00000680: 6e67 2074 6865 2064 6576 656c 6f70 6d65  ng the developme
+00000690: 6e74 206f 6620 6c61 7267 6520 6d75 6c74  nt of large mult
+000006a0: 696d 6f64 616c 206d 6f64 656c 7320 284c  imodal models (L
+000006b0: 4d4d 7329 2077 6974 6820 606c 6d6d 732d  MMs) with `lmms-
+000006c0: 6576 616c 600a 0af0 9f8f a020 5b48 6f6d  eval`...... [Hom
+000006d0: 6570 6167 655d 2868 7474 7073 3a2f 2f6c  epage](https://l
+000006e0: 6d6d 732d 6c61 622e 6769 7468 7562 2e69  mms-lab.github.i
+000006f0: 6f2f 2920 7c20 20f0 9f8e 8920 5b42 6c6f  o/) |  .... [Blo
+00000700: 675d 2868 7474 7073 3a2f 2f6c 6d6d 732d  g](https://lmms-
+00000710: 6c61 622e 6769 7468 7562 2e69 6f2f 6c6d  lab.github.io/lm
+00000720: 6d73 2d65 7661 6c2d 626c 6f67 2f6c 6d6d  ms-eval-blog/lmm
+00000730: 732d 6576 616c 2d30 2e31 2f29 207c 20f0  s-eval-0.1/) | .
+00000740: 9f93 9a20 5b44 6f63 756d 656e 7461 7469  ... [Documentati
+00000750: 6f6e 5d28 646f 6373 2f52 4541 444d 452e  on](docs/README.
+00000760: 6d64 2920 7c20 f09f a497 205b 4875 6767  md) | .... [Hugg
+00000770: 696e 6766 6163 6520 4461 7461 7365 7473  ingface Datasets
+00000780: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
+00000790: 6766 6163 652e 636f 2f6c 6d6d 732d 6c61  gface.co/lmms-la
+000007a0: 6229 207c 203c 6120 6872 6566 3d22 6874  b) | <a href="ht
+000007b0: 7470 733a 2f2f 656d 6f6a 692e 6767 2f65  tps://emoji.gg/e
+000007c0: 6d6f 6a69 2f31 3638 342d 6469 7363 6f72  moji/1684-discor
+000007d0: 642d 7468 7265 6164 223e 3c69 6d67 2073  d-thread"><img s
+000007e0: 7263 3d22 6874 7470 733a 2f2f 6364 6e33  rc="https://cdn3
+000007f0: 2e65 6d6f 6a69 2e67 672f 656d 6f6a 6973  .emoji.gg/emojis
+00000800: 2f31 3638 342d 6469 7363 6f72 642d 7468  /1684-discord-th
+00000810: 7265 6164 2e70 6e67 2220 7769 6474 683d  read.png" width=
+00000820: 2231 3470 7822 2068 6569 6768 743d 2231  "14px" height="1
+00000830: 3470 7822 2061 6c74 3d22 4469 7363 6f72  4px" alt="Discor
+00000840: 645f 5468 7265 6164 223e 3c2f 613e 205b  d_Thread"></a> [
+00000850: 6469 7363 6f72 642f 6c6d 6d73 2d65 7661  discord/lmms-eva
+00000860: 6c5d 2868 7474 7073 3a2f 2f64 6973 636f  l](https://disco
+00000870: 7264 2e67 672f 7a64 6b77 4b55 7172 5079  rd.gg/zdkwKUqrPy
+00000880: 290a 0a0a 496e 2074 6f64 6179 2773 2077  )...In today's w
+00000890: 6f72 6c64 2c20 7765 2772 6520 6f6e 2061  orld, we're on a
+000008a0: 6e20 6578 6369 7469 6e67 206a 6f75 726e  n exciting journ
+000008b0: 6579 2074 6f77 6172 6420 6372 6561 7469  ey toward creati
+000008c0: 6e67 2041 7274 6966 6963 6961 6c20 4765  ng Artificial Ge
+000008d0: 6e65 7261 6c20 496e 7465 6c6c 6967 656e  neral Intelligen
+000008e0: 6365 2028 4147 4929 2c20 6d75 6368 206c  ce (AGI), much l
+000008f0: 696b 6520 7468 6520 656e 7468 7573 6961  ike the enthusia
+00000900: 736d 206f 6620 7468 6520 3139 3630 7320  sm of the 1960s 
+00000910: 6d6f 6f6e 206c 616e 6469 6e67 2e20 5468  moon landing. Th
+00000920: 6973 206a 6f75 726e 6579 2069 7320 706f  is journey is po
+00000930: 7765 7265 6420 6279 2061 6476 616e 6365  wered by advance
+00000940: 6420 6c61 7267 6520 6c61 6e67 7561 6765  d large language
+00000950: 206d 6f64 656c 7320 284c 4c4d 7329 2061   models (LLMs) a
+00000960: 6e64 206c 6172 6765 206d 756c 7469 6d6f  nd large multimo
+00000970: 6461 6c20 6d6f 6465 6c73 2028 4c4d 4d73  dal models (LMMs
+00000980: 292c 2077 6869 6368 2061 7265 2063 6f6d  ), which are com
+00000990: 706c 6578 2073 7973 7465 6d73 2063 6170  plex systems cap
+000009a0: 6162 6c65 206f 6620 756e 6465 7273 7461  able of understa
+000009b0: 6e64 696e 672c 206c 6561 726e 696e 672c  nding, learning,
+000009c0: 2061 6e64 2070 6572 666f 726d 696e 6720   and performing 
+000009d0: 6120 7769 6465 2076 6172 6965 7479 206f  a wide variety o
+000009e0: 6620 6875 6d61 6e20 7461 736b 732e 2054  f human tasks. T
+000009f0: 6865 7365 2061 6476 616e 6365 6d65 6e74  hese advancement
+00000a00: 7320 6272 696e 6720 7573 2063 6c6f 7365  s bring us close
+00000a10: 7220 746f 2061 6368 6965 7669 6e67 2041  r to achieving A
+00000a20: 4749 2e0a 0a54 6f20 6761 7567 6520 686f  GI...To gauge ho
+00000a30: 7720 6164 7661 6e63 6564 2074 6865 7365  w advanced these
+00000a40: 206d 6f64 656c 7320 6172 652c 2077 6520   models are, we 
+00000a50: 7573 6520 6120 7661 7269 6574 7920 6f66  use a variety of
+00000a60: 2065 7661 6c75 6174 696f 6e20 6265 6e63   evaluation benc
+00000a70: 686d 6172 6b73 2e20 5468 6573 6520 6265  hmarks. These be
+00000a80: 6e63 686d 6172 6b73 2061 7265 2074 6f6f  nchmarks are too
+00000a90: 6c73 2074 6861 7420 6865 6c70 2075 7320  ls that help us 
+00000aa0: 756e 6465 7273 7461 6e64 2074 6865 2063  understand the c
+00000ab0: 6170 6162 696c 6974 6965 7320 6f66 2074  apabilities of t
+00000ac0: 6865 7365 206d 6f64 656c 732c 2073 686f  hese models, sho
+00000ad0: 7769 6e67 2075 7320 686f 7720 636c 6f73  wing us how clos
+00000ae0: 6520 7765 2061 7265 2074 6f20 6163 6869  e we are to achi
+00000af0: 6576 696e 6720 4147 492e 2048 6f77 6576  eving AGI. Howev
+00000b00: 6572 2c20 6669 6e64 696e 6720 616e 6420  er, finding and 
+00000b10: 7573 696e 6720 7468 6573 6520 6265 6e63  using these benc
+00000b20: 686d 6172 6b73 2069 7320 6120 6269 6720  hmarks is a big 
+00000b30: 6368 616c 6c65 6e67 652e 2054 6865 206e  challenge. The n
+00000b40: 6563 6573 7361 7279 2062 656e 6368 6d61  ecessary benchma
+00000b50: 726b 7320 616e 6420 6461 7461 7365 7473  rks and datasets
+00000b60: 2061 7265 2073 7072 6561 6420 6f75 7420   are spread out 
+00000b70: 616e 6420 6869 6464 656e 2069 6e20 7661  and hidden in va
+00000b80: 7269 6f75 7320 706c 6163 6573 206c 696b  rious places lik
+00000b90: 6520 476f 6f67 6c65 2044 7269 7665 2c20  e Google Drive, 
+00000ba0: 4472 6f70 626f 782c 2061 6e64 2064 6966  Dropbox, and dif
+00000bb0: 6665 7265 6e74 2073 6368 6f6f 6c20 616e  ferent school an
+00000bc0: 6420 7265 7365 6172 6368 206c 6162 2077  d research lab w
+00000bd0: 6562 7369 7465 732e 2049 7420 6665 656c  ebsites. It feel
+00000be0: 7320 6c69 6b65 2077 6527 7265 206f 6e20  s like we're on 
+00000bf0: 6120 7472 6561 7375 7265 2068 756e 742c  a treasure hunt,
+00000c00: 2062 7574 2074 6865 206d 6170 7320 6172   but the maps ar
+00000c10: 6520 7363 6174 7465 7265 6420 6576 6572  e scattered ever
+00000c20: 7977 6865 7265 2e0a 0a49 6e20 7468 6520  ywhere...In the 
+00000c30: 6669 656c 6420 6f66 206c 616e 6775 6167  field of languag
+00000c40: 6520 6d6f 6465 6c73 2c20 7468 6572 6520  e models, there 
+00000c50: 6861 7320 6265 656e 2061 2076 616c 7561  has been a valua
+00000c60: 626c 6520 7072 6563 6564 656e 7420 7365  ble precedent se
+00000c70: 7420 6279 2074 6865 2077 6f72 6b20 6f66  t by the work of
+00000c80: 205b 6c6d 2d65 7661 6c75 6174 696f 6e2d   [lm-evaluation-
+00000c90: 6861 726e 6573 735d 2868 7474 7073 3a2f  harness](https:/
+00000ca0: 2f67 6974 6875 622e 636f 6d2f 456c 6575  /github.com/Eleu
+00000cb0: 7468 6572 4149 2f6c 6d2d 6576 616c 7561  therAI/lm-evalua
+00000cc0: 7469 6f6e 2d68 6172 6e65 7373 292e 2054  tion-harness). T
+00000cd0: 6865 7920 6f66 6665 7220 696e 7465 6772  hey offer integr
+00000ce0: 6174 6564 2064 6174 6120 616e 6420 6d6f  ated data and mo
+00000cf0: 6465 6c20 696e 7465 7266 6163 6573 2c20  del interfaces, 
+00000d00: 656e 6162 6c69 6e67 2072 6170 6964 2065  enabling rapid e
+00000d10: 7661 6c75 6174 696f 6e20 6f66 206c 616e  valuation of lan
+00000d20: 6775 6167 6520 6d6f 6465 6c73 2061 6e64  guage models and
+00000d30: 2073 6572 7669 6e67 2061 7320 7468 6520   serving as the 
+00000d40: 6261 636b 656e 6420 7375 7070 6f72 7420  backend support 
+00000d50: 6672 616d 6577 6f72 6b20 666f 7220 7468  framework for th
+00000d60: 6520 5b6f 7065 6e2d 6c6c 6d2d 6c65 6164  e [open-llm-lead
+00000d70: 6572 626f 6172 645d 2868 7474 7073 3a2f  erboard](https:/
+00000d80: 2f68 7567 6769 6e67 6661 6365 2e63 6f2f  /huggingface.co/
+00000d90: 7370 6163 6573 2f48 7567 6769 6e67 4661  spaces/HuggingFa
+00000da0: 6365 4834 2f6f 7065 6e5f 6c6c 6d5f 6c65  ceH4/open_llm_le
+00000db0: 6164 6572 626f 6172 6429 2c20 616e 6420  aderboard), and 
+00000dc0: 6861 7320 6772 6164 7561 6c6c 7920 6265  has gradually be
+00000dd0: 636f 6d65 2074 6865 2075 6e64 6572 6c79  come the underly
+00000de0: 696e 6720 6563 6f73 7973 7465 6d20 6f66  ing ecosystem of
+00000df0: 2074 6865 2065 7261 206f 6620 666f 756e   the era of foun
+00000e00: 6461 7469 6f6e 206d 6f64 656c 732e 0a0a  dation models...
+00000e10: 486f 7765 7665 722c 2074 686f 7567 6820  However, though 
+00000e20: 7468 6572 6520 6172 6520 6d61 6e79 206e  there are many n
+00000e30: 6577 2065 7661 6c75 6174 696f 6e20 6461  ew evaluation da
+00000e40: 7461 7365 7473 2061 7265 2072 6563 656e  tasets are recen
+00000e50: 746c 7920 7072 6f70 6f73 6564 2c20 7468  tly proposed, th
+00000e60: 6520 6566 6669 6369 656e 7420 6576 616c  e efficient eval
+00000e70: 7561 7469 6f6e 2070 6970 656c 696e 6520  uation pipeline 
+00000e80: 6f66 204c 4d4d 2069 7320 7374 696c 6c20  of LMM is still 
+00000e90: 696e 2069 7473 2069 6e66 616e 6379 2c20  in its infancy, 
+00000ea0: 616e 6420 7468 6572 6520 6973 206e 6f20  and there is no 
+00000eb0: 756e 6966 6965 6420 6576 616c 7561 7469  unified evaluati
+00000ec0: 6f6e 2066 7261 6d65 776f 726b 2074 6861  on framework tha
+00000ed0: 7420 6361 6e20 6265 2075 7365 6420 746f  t can be used to
+00000ee0: 2065 7661 6c75 6174 6520 4c4d 4d20 6163   evaluate LMM ac
+00000ef0: 726f 7373 2061 2077 6964 6520 7261 6e67  ross a wide rang
+00000f00: 6520 6f66 2064 6174 6173 6574 732e 2054  e of datasets. T
+00000f10: 6f20 6164 6472 6573 7320 7468 6973 2063  o address this c
+00000f20: 6861 6c6c 656e 6765 2c20 7765 2069 6e74  hallenge, we int
+00000f30: 726f 6475 6365 202a 2a6c 6d6d 732d 6576  roduce **lmms-ev
+00000f40: 616c 2a2a 2c20 616e 2065 7661 6c75 6174  al**, an evaluat
+00000f50: 696f 6e20 6672 616d 6577 6f72 6b20 6d65  ion framework me
+00000f60: 7469 6375 6c6f 7573 6c79 2063 7261 6674  ticulously craft
+00000f70: 6564 2066 6f72 2063 6f6e 7369 7374 656e  ed for consisten
+00000f80: 7420 616e 6420 6566 6669 6369 656e 7420  t and efficient 
+00000f90: 6576 616c 7561 7469 6f6e 206f 6620 4c4d  evaluation of LM
+00000fa0: 4d2e 0a0a 5765 2068 756d 626c 7920 6f62  M...We humbly ob
+00000fb0: 736f 7262 6564 2074 6865 2065 7871 7569  sorbed the exqui
+00000fc0: 7369 7465 2061 6e64 2065 6666 6963 6965  site and efficie
+00000fd0: 6e74 2064 6573 6967 6e20 6f66 205b 6c6d  nt design of [lm
+00000fe0: 2d65 7661 6c75 6174 696f 6e2d 6861 726e  -evaluation-harn
+00000ff0: 6573 735d 2868 7474 7073 3a2f 2f67 6974  ess](https://git
+00001000: 6875 622e 636f 6d2f 456c 6575 7468 6572  hub.com/Eleuther
+00001010: 4149 2f6c 6d2d 6576 616c 7561 7469 6f6e  AI/lm-evaluation
+00001020: 2d68 6172 6e65 7373 292e 2042 7569 6c64  -harness). Build
+00001030: 696e 6720 7570 6f6e 2069 7473 2066 6f75  ing upon its fou
+00001040: 6e64 6174 696f 6e2c 2077 6520 696d 706c  ndation, we impl
+00001050: 656d 656e 7465 6420 6f75 7220 606c 6d6d  emented our `lmm
+00001060: 732d 6576 616c 6020 6672 616d 6577 6f72  s-eval` framewor
+00001070: 6b20 7769 7468 2070 6572 666f 726d 616e  k with performan
+00001080: 6365 206f 7074 696d 697a 6174 696f 6e73  ce optimizations
+00001090: 2073 7065 6369 6669 6361 6c6c 7920 666f   specifically fo
+000010a0: 7220 4c4d 4d73 2e0a 0a23 2320 4e65 6365  r LMMs...## Nece
+000010b0: 7373 6974 7920 6f66 206c 6d6d 732d 6576  ssity of lmms-ev
+000010c0: 616c 0a0a 5765 2062 656c 6965 7665 206f  al..We believe o
+000010d0: 7572 2065 6666 6f72 7420 636f 756c 6420  ur effort could 
+000010e0: 7072 6f76 6964 6520 616e 2065 6666 6963  provide an effic
+000010f0: 6965 6e74 2069 6e74 6572 6661 6365 2066  ient interface f
+00001100: 6f72 2074 6865 2064 6574 6169 6c65 6420  or the detailed 
+00001110: 636f 6d70 6172 6973 6f6e 206f 6620 7075  comparison of pu
+00001120: 626c 6963 6c79 2061 7661 696c 6162 6c65  blicly available
+00001130: 206d 6f64 656c 7320 746f 2064 6973 6365   models to disce
+00001140: 726e 2074 6865 6972 2073 7472 656e 6774  rn their strengt
+00001150: 6873 2061 6e64 2077 6561 6b6e 6573 7365  hs and weaknesse
+00001160: 732e 2049 7427 7320 616c 736f 2075 7365  s. It's also use
+00001170: 6675 6c20 666f 7220 7265 7365 6172 6368  ful for research
+00001180: 2069 6e73 7469 7475 7469 6f6e 7320 616e   institutions an
+00001190: 6420 7072 6f64 7563 7469 6f6e 2d6f 7269  d production-ori
+000011a0: 656e 7465 6420 636f 6d70 616e 6965 7320  ented companies 
+000011b0: 746f 2061 6363 656c 6572 6174 6520 7468  to accelerate th
+000011c0: 6520 6465 7665 6c6f 706d 656e 7420 6f66  e development of
+000011d0: 206c 6172 6765 206d 756c 7469 6d6f 6461   large multimoda
+000011e0: 6c20 6d6f 6465 6c73 2e20 5769 7468 2074  l models. With t
+000011f0: 6865 2060 6c6d 6d73 2d65 7661 6c60 2c20  he `lmms-eval`, 
+00001200: 7765 2068 6176 6520 7369 676e 6966 6963  we have signific
+00001210: 616e 746c 7920 6163 6365 6c65 7261 7465  antly accelerate
+00001220: 6420 7468 6520 6c69 6665 6379 636c 6520  d the lifecycle 
+00001230: 6f66 206d 6f64 656c 2069 7465 7261 7469  of model iterati
+00001240: 6f6e 2e20 496e 7369 6465 2074 6865 204c  on. Inside the L
+00001250: 4c61 5641 2074 6561 6d2c 2074 6865 2075  LaVA team, the u
+00001260: 7469 6c69 7a61 7469 6f6e 206f 6620 606c  tilization of `l
+00001270: 6d6d 732d 6576 616c 6020 6c61 7267 656c  mms-eval` largel
+00001280: 7920 696d 7072 6f76 6573 2074 6865 2065  y improves the e
+00001290: 6666 6963 6965 6e63 7920 6f66 2074 6865  fficiency of the
+000012a0: 206d 6f64 656c 2064 6576 656c 6f70 6d65   model developme
+000012b0: 6e74 2063 7963 6c65 2c20 6173 2077 6520  nt cycle, as we 
+000012c0: 6172 6520 6162 6c65 2074 6f20 6576 616c  are able to eval
+000012d0: 7561 7465 2077 6565 6b6c 7920 7472 6169  uate weekly trai
+000012e0: 6e65 6420 6875 6e64 7265 6473 206f 6620  ned hundreds of 
+000012f0: 6368 6563 6b70 6f69 6e74 7320 6f6e 2032  checkpoints on 2
+00001300: 302d 3330 2064 6174 6173 6574 732c 2069  0-30 datasets, i
+00001310: 6465 6e74 6966 7969 6e67 2074 6865 2073  dentifying the s
+00001320: 7472 656e 6774 6873 2061 6e64 2077 6561  trengths and wea
+00001330: 6b6e 6573 7365 732c 2061 6e64 2074 6865  knesses, and the
+00001340: 6e20 6d61 6b65 2074 6172 6765 7465 6420  n make targeted 
+00001350: 696d 7072 6f76 656d 656e 7473 2e0a 0a23  improvements...#
+00001360: 2041 6e6e 6f75 6365 6d65 6e74 0a0a 2323   Annoucement..##
+00001370: 2043 6f6e 7472 6962 7574 696f 6e20 4775   Contribution Gu
+00001380: 6964 616e 6365 0a0a 5765 2776 6520 6164  idance..We've ad
+00001390: 6465 6420 6775 6964 616e 6365 206f 6e20  ded guidance on 
+000013a0: 636f 6e74 7269 6275 7469 6e67 206e 6577  contributing new
+000013b0: 2064 6174 6173 6574 7320 616e 6420 6d6f   datasets and mo
+000013c0: 6465 6c73 2e20 506c 6561 7365 2072 6566  dels. Please ref
+000013d0: 6572 2074 6f20 6f75 7220 5b64 6f63 756d  er to our [docum
+000013e0: 656e 7461 7469 6f6e 5d28 646f 6373 2f52  entation](docs/R
+000013f0: 4541 444d 452e 6d64 292e 2049 6620 796f  EADME.md). If yo
+00001400: 7520 6e65 6564 2061 7373 6973 7461 6e63  u need assistanc
+00001410: 652c 2079 6f75 2063 616e 2063 6f6e 7461  e, you can conta
+00001420: 6374 2075 7320 7669 6120 5b64 6973 636f  ct us via [disco
+00001430: 7264 2f6c 6d6d 732d 6576 616c 5d28 6874  rd/lmms-eval](ht
+00001440: 7470 733a 2f2f 6469 7363 6f72 642e 6767  tps://discord.gg
+00001450: 2f65 6241 4d47 5373 5329 2e0a 0a23 2320  /ebAMGSsS)...## 
+00001460: 7630 2e31 2e30 2052 656c 6561 7365 640a  v0.1.0 Released.
+00001470: 0a54 6865 2066 6972 7374 2076 6572 7369  .The first versi
+00001480: 6f6e 206f 6620 7468 6520 606c 6d6d 732d  on of the `lmms-
+00001490: 6576 616c 6020 6973 2072 656c 6561 7365  eval` is release
+000014a0: 642e 2057 6520 6172 6520 776f 726b 696e  d. We are workin
+000014b0: 6720 6f6e 2070 726f 7669 6469 6e67 2061  g on providing a
+000014c0: 6e20 6f6e 652d 636f 6d6d 616e 6420 6576  n one-command ev
+000014d0: 616c 7561 7469 6f6e 2073 7569 7465 2066  aluation suite f
+000014e0: 6f72 2061 6363 656c 6572 6174 696e 6720  or accelerating 
+000014f0: 7468 6520 6465 7665 6c6f 706d 656e 7420  the development 
+00001500: 6f66 204c 4d4d 732e 200a 0a3e 2049 6e20  of LMMs. ..> In 
+00001510: 5b4c 4c61 5641 204e 6578 745d 2868 7474  [LLaVA Next](htt
+00001520: 7073 3a2f 2f6c 6c61 7661 2d76 6c2e 6769  ps://llava-vl.gi
+00001530: 7468 7562 2e69 6f2f 626c 6f67 2f32 3032  thub.io/blog/202
+00001540: 342d 3031 2d33 302d 6c6c 6176 612d 6e65  4-01-30-llava-ne
+00001550: 7874 2f29 2064 6576 656c 6f70 6d65 6e74  xt/) development
+00001560: 2c20 7765 2069 6e74 6572 6e61 6c6c 7920  , we internally 
+00001570: 7574 696c 697a 6520 7468 6973 2073 7569  utilize this sui
+00001580: 7465 2074 6f20 6576 616c 7561 7465 2074  te to evaluate t
+00001590: 6865 206d 756c 7469 706c 6520 6469 6666  he multiple diff
+000015a0: 6572 656e 7420 6d6f 6465 6c20 7665 7273  erent model vers
+000015b0: 696f 6e73 206f 6e20 7661 7269 6f75 7320  ions on various 
+000015c0: 6461 7461 7365 7473 2e20 4974 2073 6967  datasets. It sig
+000015d0: 6e69 6669 6361 6e74 6c79 2061 6363 656c  nificantly accel
+000015e0: 6572 6174 6573 2074 6865 206d 6f64 656c  erates the model
+000015f0: 2064 6576 656c 6f70 6d65 6e74 2063 7963   development cyc
+00001600: 6c65 2066 6f72 2069 7427 7320 6561 7379  le for it's easy
+00001610: 2069 6e74 6567 7261 7469 6f6e 2061 6e64   integration and
+00001620: 2066 6173 7420 6576 616c 7561 7469 6f6e   fast evaluation
+00001630: 2073 7065 6564 2e0a 0a54 6865 206d 6169   speed...The mai
+00001640: 6e20 6665 6174 7572 6520 696e 636c 7564  n feature includ
+00001650: 6573 3a0a 0a3c 7020 616c 6967 6e3d 2263  es:..<p align="c
+00001660: 656e 7465 7222 2077 6964 7468 3d22 3130  enter" width="10
+00001670: 3025 223e 0a3c 696d 6720 7372 633d 2268  0%">.<img src="h
+00001680: 7474 7073 3a2f 2f69 2e70 6f73 7469 6d67  ttps://i.postimg
+00001690: 2e63 632f 7367 7a4e 6d4a 7837 2f74 6561  .cc/sgzNmJx7/tea
+000016a0: 7365 722e 706e 6722 2020 7769 6474 683d  ser.png"  width=
+000016b0: 2231 3030 2522 2068 6569 6768 743d 2238  "100%" height="8
+000016c0: 3025 223e 0a3c 2f70 3e0a 0a23 2323 204f  0%">.</p>..### O
+000016d0: 6e65 2d63 6f6d 6d61 6e64 2065 7661 6c75  ne-command evalu
+000016e0: 6174 696f 6e2c 2077 6974 6820 6465 7461  ation, with deta
+000016f0: 696c 6564 206c 6f67 7320 616e 6420 7361  iled logs and sa
+00001700: 6d70 6c65 732e 0a59 6f75 2063 616e 2065  mples..You can e
+00001710: 7661 6c75 6174 6520 7468 6520 6d6f 6465  valuate the mode
+00001720: 6c73 206f 6e20 6d75 6c74 6970 6c65 2064  ls on multiple d
+00001730: 6174 6173 6574 7320 7769 7468 2061 2073  atasets with a s
+00001740: 696e 676c 6520 636f 6d6d 616e 642e 204e  ingle command. N
+00001750: 6f20 6d6f 6465 6c2f 6461 7461 2070 7265  o model/data pre
+00001760: 7061 7261 7469 6f6e 2069 7320 6e65 6564  paration is need
+00001770: 6564 2c20 6a75 7374 206f 6e65 2063 6f6d  ed, just one com
+00001780: 6d61 6e64 206c 696e 652c 2066 6577 206d  mand line, few m
+00001790: 696e 7574 6573 2c20 616e 6420 6765 7420  inutes, and get 
+000017a0: 7468 6520 7265 7375 6c74 732e 204e 6f74  the results. Not
+000017b0: 206a 7573 7420 6120 7265 7375 6c74 206e   just a result n
+000017c0: 756d 6265 722c 2062 7574 2061 6c73 6f20  umber, but also 
+000017d0: 7468 6520 6465 7461 696c 6564 206c 6f67  the detailed log
+000017e0: 7320 616e 6420 7361 6d70 6c65 732c 2069  s and samples, i
+000017f0: 6e63 6c75 6469 6e67 2074 6865 206d 6f64  ncluding the mod
+00001800: 656c 2061 7267 732c 2069 6e70 7574 2071  el args, input q
+00001810: 7565 7374 696f 6e2c 206d 6f64 656c 2072  uestion, model r
+00001820: 6573 706f 6e73 652c 2061 6e64 2067 726f  esponse, and gro
+00001830: 756e 6420 7472 7574 6820 616e 7377 6572  und truth answer
+00001840: 2e0a 0a60 6060 7079 7468 6f6e 0a23 2045  ...```python.# E
+00001850: 7661 6c75 6174 696e 6720 4c4c 6156 4120  valuating LLaVA 
+00001860: 6f6e 206d 756c 7469 706c 6520 6461 7461  on multiple data
+00001870: 7365 7473 0a61 6363 656c 6572 6174 6520  sets.accelerate 
+00001880: 6c61 756e 6368 202d 2d6e 756d 5f70 726f  launch --num_pro
+00001890: 6365 7373 6573 3d38 202d 6d20 6c6d 6d73  cesses=8 -m lmms
+000018a0: 5f65 7661 6c20 2d2d 6d6f 6465 6c20 6c6c  _eval --model ll
+000018b0: 6176 6120 2020 2d2d 6d6f 6465 6c5f 6172  ava   --model_ar
+000018c0: 6773 2070 7265 7472 6169 6e65 643d 226c  gs pretrained="l
+000018d0: 6975 6861 6f74 6961 6e2f 6c6c 6176 612d  iuhaotian/llava-
+000018e0: 7631 2e35 2d37 6222 2020 202d 2d74 6173  v1.5-7b"   --tas
+000018f0: 6b73 206d 6d65 2c6d 6d62 656e 6368 5f65  ks mme,mmbench_e
+00001900: 6e20 2d2d 6261 7463 685f 7369 7a65 2031  n --batch_size 1
+00001910: 202d 2d6c 6f67 5f73 616d 706c 6573 202d   --log_samples -
+00001920: 2d6c 6f67 5f73 616d 706c 6573 5f73 7566  -log_samples_suf
+00001930: 6669 7820 6c6c 6176 615f 7631 2e35 5f6d  fix llava_v1.5_m
+00001940: 6d65 5f6d 6d62 656e 6368 656e 202d 2d6f  me_mmbenchen --o
+00001950: 7574 7075 745f 7061 7468 202e 2f6c 6f67  utput_path ./log
+00001960: 732f 2023 0a60 6060 0a0a 2323 2320 4163  s/ #.```..### Ac
+00001970: 6365 6c65 7261 746f 7220 7375 7070 6f72  celerator suppor
+00001980: 7420 616e 6420 5461 736b 7320 6772 6f75  t and Tasks grou
+00001990: 7069 6e67 2e0a 5765 2073 7570 706f 7274  ping..We support
+000019a0: 2074 6865 2075 7361 6765 206f 6620 6061   the usage of `a
+000019b0: 6363 656c 6572 6174 6560 2074 6f20 7772  ccelerate` to wr
+000019c0: 6170 2074 6865 206d 6f64 656c 2066 6f72  ap the model for
+000019d0: 2064 6973 7472 6962 7574 6564 2065 7661   distributed eva
+000019e0: 6c75 6174 696f 6e2c 2073 7570 706f 7274  luation, support
+000019f0: 696e 6720 6d75 6c74 692d 6770 7520 616e  ing multi-gpu an
+00001a00: 6420 7465 6e73 6f72 2070 6172 616c 6c65  d tensor paralle
+00001a10: 6c69 736d 2e20 5769 7468 202a 2a54 6173  lism. With **Tas
+00001a20: 6b20 4772 6f75 7069 6e67 2a2a 2c20 616c  k Grouping**, al
+00001a30: 6c20 696e 7374 616e 6365 7320 6672 6f6d  l instances from
+00001a40: 2061 6c6c 2074 6173 6b73 2061 7265 2067   all tasks are g
+00001a50: 726f 7570 6564 2061 6e64 2065 7661 6c75  rouped and evalu
+00001a60: 6174 6564 2069 6e20 7061 7261 6c6c 656c  ated in parallel
+00001a70: 2c20 7768 6963 6820 7369 676e 6966 6963  , which signific
+00001a80: 616e 746c 7920 696d 7072 6f76 6573 2074  antly improves t
+00001a90: 6865 2074 6872 6f75 6768 7075 7420 6f66  he throughput of
+00001aa0: 2074 6865 2065 7661 6c75 6174 696f 6e2e   the evaluation.
+00001ab0: 2041 6674 6572 2065 7661 6c75 6174 696f   After evaluatio
+00001ac0: 6e2c 2061 6c6c 2069 6e73 7461 6e63 6573  n, all instances
+00001ad0: 2061 7265 2073 656e 7420 746f 2070 6f73   are sent to pos
+00001ae0: 7470 726f 6365 7373 696e 6720 6d6f 6475  tprocessing modu
+00001af0: 6c65 2066 6f72 206d 6574 7269 6320 6361  le for metric ca
+00001b00: 6c63 7561 7469 6f6e 7320 616e 6420 706f  lcuations and po
+00001b10: 7465 6e74 6961 6c20 4750 5434 2d65 7661  tential GPT4-eva
+00001b20: 6c20 7175 6572 6965 732e 0a0a 4265 6c6f  l queries...Belo
+00001b30: 7720 6172 6520 7468 6520 746f 7461 6c20  w are the total 
+00001b40: 7275 6e74 696d 6520 6f6e 2064 6966 6665  runtime on diffe
+00001b50: 7265 6e74 2064 6174 6173 6574 7320 7573  rent datasets us
+00001b60: 696e 6720 3420 7820 4131 3030 2034 3047  ing 4 x A100 40G
+00001b70: 2e0a 0a7c 2044 6174 6173 6574 2028 236e  ...| Dataset (#n
+00001b80: 756d 2920 2020 2020 2020 2020 207c 204c  um)          | L
+00001b90: 4c61 5641 2d76 312e 352d 3762 2020 2020  LaVA-v1.5-7b    
+00001ba0: 2020 7c20 4c4c 6156 412d 7631 2e35 2d31    | LLaVA-v1.5-1
+00001bb0: 3362 2020 2020 207c 0a7c 203a 2d2d 2d2d  3b     |.| :----
+00001bc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001bd0: 2d2d 207c 203a 2d2d 2d2d 2d2d 2d2d 2d2d  -- | :----------
+00001be0: 2d2d 2d2d 2d2d 2d20 7c20 3a2d 2d2d 2d2d  ------- | :-----
+00001bf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c 0a7c  ------------ |.|
+00001c00: 206d 6d65 2028 3233 3734 2920 2020 2020   mme (2374)     
+00001c10: 2020 2020 2020 2020 207c 2032 206d 696e           | 2 min
+00001c20: 7320 3433 2073 6563 6f6e 6473 2020 7c20  s 43 seconds  | 
+00001c30: 3320 6d69 6e73 2032 3720 7365 636f 6e64  3 mins 27 second
+00001c40: 7320 207c 0a7c 2067 7161 2028 3132 3537  s  |.| gqa (1257
+00001c50: 3829 2020 2020 2020 2020 2020 2020 207c  8)             |
+00001c60: 2031 3020 6d69 6e73 2034 3320 7365 636f   10 mins 43 seco
+00001c70: 6e64 7320 7c20 3134 206d 696e 7320 3233  nds | 14 mins 23
+00001c80: 2073 6563 6f6e 6473 207c 0a7c 2073 6369   seconds |.| sci
+00001c90: 656e 6365 7161 5f69 6d67 2028 3230 3137  enceqa_img (2017
+00001ca0: 2920 2020 207c 2031 206d 696e 7320 3538  )    | 1 mins 58
+00001cb0: 2073 6563 6f6e 6473 2020 7c20 3220 6d69   seconds  | 2 mi
+00001cc0: 6e73 2035 3220 7365 636f 6e64 7320 207c  ns 52 seconds  |
+00001cd0: 0a7c 2061 6932 6420 2833 3038 3829 2020  .| ai2d (3088)  
+00001ce0: 2020 2020 2020 2020 2020 207c 2033 206d             | 3 m
+00001cf0: 696e 7320 3137 2073 6563 6f6e 6473 2020  ins 17 seconds  
+00001d00: 7c20 3420 6d69 6e73 2031 3220 7365 636f  | 4 mins 12 seco
+00001d10: 6e64 7320 207c 0a7c 2063 6f63 6f32 3031  nds  |.| coco201
+00001d20: 375f 6361 705f 7661 6c20 2835 3030 3029  7_cap_val (5000)
+00001d30: 207c 2031 3420 6d69 6e73 2031 3320 7365   | 14 mins 13 se
+00001d40: 636f 6e64 7320 7c20 3139 206d 696e 7320  conds | 19 mins 
+00001d50: 3538 2073 6563 6f6e 6473 207c 0a0a 2323  58 seconds |..##
+00001d60: 2320 416c 6c2d 496e 2d4f 6e65 2048 4620  # All-In-One HF 
+00001d70: 6461 7461 7365 7420 6875 6273 2e0a 0a57  dataset hubs...W
+00001d80: 6520 6172 6520 686f 7374 696e 6720 6d6f  e are hosting mo
+00001d90: 7265 2074 6861 6e20 3430 2028 616e 6420  re than 40 (and 
+00001da0: 696e 6372 6561 7369 6e67 2920 6461 7461  increasing) data
+00001db0: 7365 7473 206f 6e20 5b68 7567 6769 6e67  sets on [hugging
+00001dc0: 6661 6365 2f6c 6d6d 732d 6c61 625d 2868  face/lmms-lab](h
+00001dd0: 7474 7073 3a2f 2f68 7567 6769 6e67 6661  ttps://huggingfa
+00001de0: 6365 2e63 6f2f 6c6d 6d73 2d6c 6162 292c  ce.co/lmms-lab),
+00001df0: 2077 6520 6361 7265 6675 6c6c 7920 636f   we carefully co
+00001e00: 6e76 6572 7465 6420 7468 6573 6520 6461  nverted these da
+00001e10: 7461 7365 7473 2066 726f 6d20 6f72 6967  tasets from orig
+00001e20: 696e 616c 2073 6f75 7263 6573 2061 6e64  inal sources and
+00001e30: 2069 6e63 6c75 6465 6420 616c 6c20 7661   included all va
+00001e40: 7269 616e 7473 2c20 7665 7273 696f 6e73  riants, versions
+00001e50: 2061 6e64 2073 706c 6974 732e 204e 6f77   and splits. Now
+00001e60: 2074 6865 7920 6361 6e20 6265 2064 6972   they can be dir
+00001e70: 6563 746c 7920 6163 6365 7373 6564 2077  ectly accessed w
+00001e80: 6974 686f 7574 2061 6e79 2062 7572 6465  ithout any burde
+00001e90: 6e20 6f66 2064 6174 6120 7072 6570 726f  n of data prepro
+00001ea0: 6365 7373 696e 672e 2054 6865 7920 616c  cessing. They al
+00001eb0: 736f 2073 6572 7665 2066 6f72 2074 6865  so serve for the
+00001ec0: 2070 7572 706f 7365 206f 6620 7669 7375   purpose of visu
+00001ed0: 616c 697a 696e 6720 7468 6520 6461 7461  alizing the data
+00001ee0: 2061 6e64 2067 7261 7370 696e 6720 7468   and grasping th
+00001ef0: 6520 7365 6e73 6520 6f66 2065 7661 6c75  e sense of evalu
+00001f00: 6174 696f 6e20 7461 736b 7320 6469 7374  ation tasks dist
+00001f10: 7269 6275 7469 6f6e 2e0a 0a3c 7020 616c  ribution...<p al
+00001f20: 6967 6e3d 2263 656e 7465 7222 2077 6964  ign="center" wid
+00001f30: 7468 3d22 3130 3025 223e 0a3c 696d 6720  th="100%">.<img 
+00001f40: 7372 633d 2268 7474 7073 3a2f 2f69 2e70  src="https://i.p
+00001f50: 6f73 7469 6d67 2e63 632f 3850 5846 5739  ostimg.cc/8PXFW9
+00001f60: 736b 2f57 5832 3032 3430 3232 382d 3132  sk/WX20240228-12
+00001f70: 3331 3130 5f32 782e 706e 6722 2020 7769  3110_2x.png"  wi
+00001f80: 6474 683d 2231 3030 2522 2068 6569 6768  dth="100%" heigh
+00001f90: 743d 2238 3025 223e 0a3c 2f70 3e0a 0a23  t="80%">.</p>..#
+00001fa0: 2323 2044 6574 6169 6c65 6420 4c6f 6767  ## Detailed Logg
+00001fb0: 696e 6720 5574 696c 6974 6573 0a0a 5765  ing Utilites..We
+00001fc0: 2070 726f 7669 6465 2064 6574 6169 6c65   provide detaile
+00001fd0: 6420 6c6f 6767 696e 6720 7574 696c 6974  d logging utilit
+00001fe0: 6965 7320 746f 2068 656c 7020 796f 7520  ies to help you 
+00001ff0: 756e 6465 7273 7461 6e64 2074 6865 2065  understand the e
+00002000: 7661 6c75 6174 696f 6e20 7072 6f63 6573  valuation proces
+00002010: 7320 616e 6420 7265 7375 6c74 732e 2054  s and results. T
+00002020: 6865 206c 6f67 7320 696e 636c 7564 6520  he logs include 
+00002030: 7468 6520 6d6f 6465 6c20 6172 6773 2c20  the model args, 
+00002040: 6765 6e65 7261 7469 6f6e 2070 6172 616d  generation param
+00002050: 6574 6572 732c 2069 6e70 7574 2071 7565  eters, input que
+00002060: 7374 696f 6e2c 206d 6f64 656c 2072 6573  stion, model res
+00002070: 706f 6e73 652c 2061 6e64 2067 726f 756e  ponse, and groun
+00002080: 6420 7472 7574 6820 616e 7377 6572 2e20  d truth answer. 
+00002090: 596f 7520 6361 6e20 616c 736f 2072 6563  You can also rec
+000020a0: 6f72 6420 6576 6572 7920 6465 7461 696c  ord every detail
+000020b0: 7320 616e 6420 7669 7375 616c 697a 6520  s and visualize 
+000020c0: 7468 656d 2069 6e73 6964 6520 7275 6e73  them inside runs
+000020d0: 206f 6e20 5765 6967 6874 7320 2620 4269   on Weights & Bi
+000020e0: 6173 6573 2e0a 0a7b 2520 696e 636c 7564  ases...{% includ
+000020f0: 6520 6669 6775 7265 2e6c 6971 7569 6420  e figure.liquid 
+00002100: 6c6f 6164 696e 673d 2265 6167 6572 2220  loading="eager" 
+00002110: 7061 7468 3d22 6173 7365 7473 2f69 6d67  path="assets/img
+00002120: 2f77 616e 6462 5f74 6162 6c65 2e70 6e67  /wandb_table.png
+00002130: 2220 636c 6173 733d 2269 6d67 2d66 6c75  " class="img-flu
+00002140: 6964 2072 6f75 6e64 6564 207a 2d64 6570  id rounded z-dep
+00002150: 7468 2d31 2220 7a6f 6f6d 6162 6c65 3d74  th-1" zoomable=t
+00002160: 7275 6520 257d 0a0a 3c70 2061 6c69 676e  rue %}..<p align
+00002170: 3d22 6365 6e74 6572 2220 7769 6474 683d  ="center" width=
+00002180: 2231 3030 2522 3e0a 3c69 6d67 2073 7263  "100%">.<img src
+00002190: 3d22 6874 7470 733a 2f2f 692e 706f 7374  ="https://i.post
+000021a0: 696d 672e 6363 2f57 3163 3176 4244 4a2f  img.cc/W1c1vBDJ/
+000021b0: 5765 6368 6174 2d49 4d47 3139 3933 2e70  Wechat-IMG1993.p
+000021c0: 6e67 2220 2077 6964 7468 3d22 3130 3025  ng"  width="100%
+000021d0: 2220 6865 6967 6874 3d22 3830 2522 3e0a  " height="80%">.
+000021e0: 3c2f 703e 0a0a 2320 496e 7374 616c 6c61  </p>..# Installa
+000021f0: 7469 6f6e 0a0a 466f 7220 666f 726d 616c  tion..For formal
+00002200: 2075 7361 6765 2c20 796f 7520 6361 6e20   usage, you can 
+00002210: 696e 7374 616c 6c20 7468 6520 7061 636b  install the pack
+00002220: 6167 6520 6672 6f6d 2050 7950 4920 6279  age from PyPI by
+00002230: 2072 756e 6e69 6e67 2074 6865 2066 6f6c   running the fol
+00002240: 6c6f 7769 6e67 2063 6f6d 6d61 6e64 3a0a  lowing command:.
+00002250: 6060 6062 6173 680a 7069 7020 696e 7374  ```bash.pip inst
+00002260: 616c 6c20 6c6d 6d73 2d65 7661 6c0a 6060  all lmms-eval.``
+00002270: 600a 0a46 6f72 2064 6576 656c 6f70 6d65  `..For developme
+00002280: 6e74 2c20 796f 7520 6361 6e20 696e 7374  nt, you can inst
+00002290: 616c 6c20 7468 6520 7061 636b 6167 6520  all the package 
+000022a0: 6279 2063 6c6f 6e69 6e67 2074 6865 2072  by cloning the r
+000022b0: 6570 6f73 6974 6f72 7920 616e 6420 7275  epository and ru
+000022c0: 6e6e 696e 6720 7468 6520 666f 6c6c 6f77  nning the follow
+000022d0: 696e 6720 636f 6d6d 616e 643a 0a60 6060  ing command:.```
+000022e0: 6261 7368 0a67 6974 2063 6c6f 6e65 2068  bash.git clone h
+000022f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00002300: 6d2f 4576 6f6c 7669 6e67 4c4d 4d73 2d4c  m/EvolvingLMMs-L
+00002310: 6162 2f6c 6d6d 732d 6576 616c 0a63 6420  ab/lmms-eval.cd 
+00002320: 6c6d 6d73 2d65 7661 6c0a 7069 7020 696e  lmms-eval.pip in
+00002330: 7374 616c 6c20 2d65 202e 0a60 6060 0a0a  stall -e ..```..
+00002340: 4966 2079 6f75 2077 616e 7465 6420 746f  If you wanted to
+00002350: 2074 6573 7420 6c6c 6176 612c 2079 6f75   test llava, you
+00002360: 2077 696c 6c20 6861 7665 2074 6f20 636c   will have to cl
+00002370: 6f6e 6520 7468 6569 7220 7265 706f 2066  one their repo f
+00002380: 726f 6d20 5b4c 4c61 5641 5d28 6874 7470  rom [LLaVA](http
+00002390: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f68  s://github.com/h
+000023a0: 616f 7469 616e 2d6c 6975 2f4c 4c61 5641  aotian-liu/LLaVA
+000023b0: 2920 616e 640a 6060 600a 6769 7420 636c  ) and.```.git cl
+000023c0: 6f6e 6520 6874 7470 733a 2f2f 6769 7468  one https://gith
+000023d0: 7562 2e63 6f6d 2f68 616f 7469 616e 2d6c  ub.com/haotian-l
+000023e0: 6975 2f4c 4c61 5641 0a63 6420 4c4c 6156  iu/LLaVA.cd LLaV
+000023f0: 410a 7069 7020 696e 7374 616c 6c20 2d65  A.pip install -e
+00002400: 202e 0a60 6060 0a0a 596f 7520 6361 6e20   ..```..You can 
+00002410: 6368 6563 6b20 7468 6520 5b65 6e76 6972  check the [envir
+00002420: 6f6e 6d65 6e74 2069 6e73 7461 6c6c 2073  onment install s
+00002430: 6372 6970 745d 286d 6973 6373 2f72 6570  cript](miscs/rep
+00002440: 725f 7363 7269 7074 732e 7368 2920 616e  r_scripts.sh) an
+00002450: 6420 5b74 6f72 6368 2065 6e76 6972 6f6e  d [torch environ
+00002460: 6d65 6e74 2069 6e66 6f5d 286d 6973 6373  ment info](miscs
+00002470: 2f72 6570 725f 746f 7263 685f 656e 7673  /repr_torch_envs
+00002480: 2e74 7874 2920 746f 202a 2a72 6570 726f  .txt) to **repro
+00002490: 6475 6365 204c 4c61 5641 2d31 2e35 2773  duce LLaVA-1.5's
+000024a0: 2070 6170 6572 2072 6573 756c 7473 2a2a   paper results**
+000024b0: 2e20 5765 2066 6f75 6e64 2074 6f72 6368  . We found torch
+000024c0: 2f63 7564 6120 7665 7273 696f 6e73 2064  /cuda versions d
+000024d0: 6966 6665 7265 6e63 6520 776f 756c 6420  ifference would 
+000024e0: 6361 7573 6520 736d 616c 6c20 7661 7269  cause small vari
+000024f0: 6174 696f 6e73 2069 6e20 7468 6520 7265  ations in the re
+00002500: 7375 6c74 732c 2077 6520 7072 6f76 6964  sults, we provid
+00002510: 6520 7468 6520 5b72 6573 756c 7473 2063  e the [results c
+00002520: 6865 636b 5d28 6d69 7363 732f 6c6c 6176  heck](miscs/llav
+00002530: 615f 7265 7375 6c74 5f63 6865 636b 2e6d  a_result_check.m
+00002540: 6429 2077 6974 6820 6469 6666 6572 656e  d) with differen
+00002550: 7420 656e 7669 726f 6e6d 656e 7473 2e0a  t environments..
+00002560: 0a49 6620 796f 7520 7761 6e74 2074 6f20  .If you want to 
+00002570: 7465 7374 206f 6e20 6361 7074 696f 6e20  test on caption 
+00002580: 6461 7461 7365 7420 7375 6368 2061 7320  dataset such as 
+00002590: 6063 6f63 6f60 2c20 6072 6566 636f 636f  `coco`, `refcoco
+000025a0: 602c 2061 6e64 2060 6e6f 6361 7073 602c  `, and `nocaps`,
+000025b0: 2079 6f75 2077 696c 6c20 6e65 6564 2074   you will need t
+000025c0: 6f20 6861 7665 2060 6a61 7661 3d3d 312e  o have `java==1.
+000025d0: 382e 3020 6020 746f 206c 6574 2070 7963  8.0 ` to let pyc
+000025e0: 6f63 6f65 7661 6c20 6170 6920 746f 2077  ocoeval api to w
+000025f0: 6f72 6b2e 2049 6620 796f 7520 646f 6e27  ork. If you don'
+00002600: 7420 6861 7665 2069 742c 2079 6f75 2063  t have it, you c
+00002610: 616e 2069 6e73 7461 6c6c 2062 7920 7573  an install by us
+00002620: 696e 6720 636f 6e64 610a 6060 600a 636f  ing conda.```.co
+00002630: 6e64 6120 696e 7374 616c 6c20 6f70 656e  nda install open
+00002640: 6a64 6b3d 380a 6060 600a 796f 7520 6361  jdk=8.```.you ca
+00002650: 6e20 7468 656e 2063 6865 636b 2079 6f75  n then check you
+00002660: 7220 6a61 7661 2076 6572 7369 6f6e 2062  r java version b
+00002670: 7920 606a 6176 6120 2d76 6572 7369 6f6e  y `java -version
+00002680: 6020 0a0a 2320 5573 6167 650a 6060 6062  ` ..# Usage.```b
+00002690: 6173 680a 2320 4576 616c 7561 7469 6e67  ash.# Evaluating
+000026a0: 204c 4c61 5641 206f 6e20 4d4d 450a 6163   LLaVA on MME.ac
+000026b0: 6365 6c65 7261 7465 206c 6175 6e63 6820  celerate launch 
+000026c0: 2d2d 6e75 6d5f 7072 6f63 6573 7365 733d  --num_processes=
+000026d0: 3820 2d6d 206c 6d6d 735f 6576 616c 202d  8 -m lmms_eval -
+000026e0: 2d6d 6f64 656c 206c 6c61 7661 2020 202d  -model llava   -
+000026f0: 2d6d 6f64 656c 5f61 7267 7320 7072 6574  -model_args pret
+00002700: 7261 696e 6564 3d22 6c69 7568 616f 7469  rained="liuhaoti
+00002710: 616e 2f6c 6c61 7661 2d76 312e 352d 3762  an/llava-v1.5-7b
+00002720: 2220 2020 2d2d 7461 736b 7320 6d6d 6520  "   --tasks mme 
+00002730: 202d 2d62 6174 6368 5f73 697a 6520 3120   --batch_size 1 
+00002740: 2d2d 6c6f 675f 7361 6d70 6c65 7320 2d2d  --log_samples --
+00002750: 6c6f 675f 7361 6d70 6c65 735f 7375 6666  log_samples_suff
+00002760: 6978 206c 6c61 7661 5f76 312e 355f 6d6d  ix llava_v1.5_mm
+00002770: 6520 2d2d 6f75 7470 7574 5f70 6174 6820  e --output_path 
+00002780: 2e2f 6c6f 6773 2f20 0a0a 2320 4576 616c  ./logs/ ..# Eval
+00002790: 7561 7469 6e67 204c 4c61 5641 206f 6e20  uating LLaVA on 
+000027a0: 6d75 6c74 6970 6c65 2064 6174 6173 6574  multiple dataset
+000027b0: 730a 6163 6365 6c65 7261 7465 206c 6175  s.accelerate lau
+000027c0: 6e63 6820 2d2d 6e75 6d5f 7072 6f63 6573  nch --num_proces
+000027d0: 7365 733d 3820 2d6d 206c 6d6d 735f 6576  ses=8 -m lmms_ev
+000027e0: 616c 202d 2d6d 6f64 656c 206c 6c61 7661  al --model llava
+000027f0: 2020 202d 2d6d 6f64 656c 5f61 7267 7320     --model_args 
+00002800: 7072 6574 7261 696e 6564 3d22 6c69 7568  pretrained="liuh
+00002810: 616f 7469 616e 2f6c 6c61 7661 2d76 312e  aotian/llava-v1.
+00002820: 352d 3762 2220 2020 2d2d 7461 736b 7320  5-7b"   --tasks 
+00002830: 6d6d 652c 6d6d 6265 6e63 685f 656e 202d  mme,mmbench_en -
+00002840: 2d62 6174 6368 5f73 697a 6520 3120 2d2d  -batch_size 1 --
+00002850: 6c6f 675f 7361 6d70 6c65 7320 2d2d 6c6f  log_samples --lo
+00002860: 675f 7361 6d70 6c65 735f 7375 6666 6978  g_samples_suffix
+00002870: 206c 6c61 7661 5f76 312e 355f 6d6d 655f   llava_v1.5_mme_
+00002880: 6d6d 6265 6e63 6865 6e20 2d2d 6f75 7470  mmbenchen --outp
+00002890: 7574 5f70 6174 6820 2e2f 6c6f 6773 2f20  ut_path ./logs/ 
+000028a0: 230a 0a23 2046 6f72 206f 7468 6572 2076  #..# For other v
+000028b0: 6172 6961 6e74 7320 6c6c 6176 612e 204e  ariants llava. N
+000028c0: 6f74 6520 7468 6174 2060 636f 6e76 5f74  ote that `conv_t
+000028d0: 656d 706c 6174 6560 2069 7320 616e 2061  emplate` is an a
+000028e0: 7267 206f 6620 7468 6520 696e 6974 2066  rg of the init f
+000028f0: 756e 6374 696f 6e20 6f66 206c 6c61 7661  unction of llava
+00002900: 2069 6e20 606c 6d6d 735f 6576 616c 2f6d   in `lmms_eval/m
+00002910: 6f64 656c 732f 6c6c 6176 612e 7079 600a  odels/llava.py`.
+00002920: 6163 6365 6c65 7261 7465 206c 6175 6e63  accelerate launc
+00002930: 6820 2d2d 6e75 6d5f 7072 6f63 6573 7365  h --num_processe
+00002940: 733d 3820 2d6d 206c 6d6d 735f 6576 616c  s=8 -m lmms_eval
+00002950: 202d 2d6d 6f64 656c 206c 6c61 7661 2020   --model llava  
+00002960: 202d 2d6d 6f64 656c 5f61 7267 7320 7072   --model_args pr
+00002970: 6574 7261 696e 6564 3d22 6c69 7568 616f  etrained="liuhao
+00002980: 7469 616e 2f6c 6c61 7661 2d76 312e 362d  tian/llava-v1.6-
+00002990: 6d69 7374 7261 6c2d 3762 2c63 6f6e 765f  mistral-7b,conv_
+000029a0: 7465 6d70 6c61 7465 3d6d 6973 7472 616c  template=mistral
+000029b0: 5f69 6e73 7472 7563 7422 2020 202d 2d74  _instruct"   --t
+000029c0: 6173 6b73 206d 6d65 2c6d 6d62 656e 6368  asks mme,mmbench
+000029d0: 5f65 6e20 2d2d 6261 7463 685f 7369 7a65  _en --batch_size
+000029e0: 2031 202d 2d6c 6f67 5f73 616d 706c 6573   1 --log_samples
+000029f0: 202d 2d6c 6f67 5f73 616d 706c 6573 5f73   --log_samples_s
+00002a00: 7566 6669 7820 6c6c 6176 615f 7631 2e35  uffix llava_v1.5
+00002a10: 5f6d 6d65 5f6d 6d62 656e 6368 656e 202d  _mme_mmbenchen -
+00002a20: 2d6f 7574 7075 745f 7061 7468 202e 2f6c  -output_path ./l
+00002a30: 6f67 732f 2023 0a61 6363 656c 6572 6174  ogs/ #.accelerat
+00002a40: 6520 6c61 756e 6368 202d 2d6e 756d 5f70  e launch --num_p
+00002a50: 726f 6365 7373 6573 3d38 202d 6d20 6c6d  rocesses=8 -m lm
+00002a60: 6d73 5f65 7661 6c20 2d2d 6d6f 6465 6c20  ms_eval --model 
+00002a70: 6c6c 6176 6120 2020 2d2d 6d6f 6465 6c5f  llava   --model_
+00002a80: 6172 6773 2070 7265 7472 6169 6e65 643d  args pretrained=
+00002a90: 226c 6975 6861 6f74 6961 6e2f 6c6c 6176  "liuhaotian/llav
+00002aa0: 612d 7631 2e36 2d33 3462 2c63 6f6e 765f  a-v1.6-34b,conv_
+00002ab0: 7465 6d70 6c61 7465 3d6d 6973 7472 616c  template=mistral
+00002ac0: 5f64 6972 6563 7422 2020 202d 2d74 6173  _direct"   --tas
+00002ad0: 6b73 206d 6d65 2c6d 6d62 656e 6368 5f65  ks mme,mmbench_e
+00002ae0: 6e20 2d2d 6261 7463 685f 7369 7a65 2031  n --batch_size 1
+00002af0: 202d 2d6c 6f67 5f73 616d 706c 6573 202d   --log_samples -
+00002b00: 2d6c 6f67 5f73 616d 706c 6573 5f73 7566  -log_samples_suf
+00002b10: 6669 7820 6c6c 6176 615f 7631 2e35 5f6d  fix llava_v1.5_m
+00002b20: 6d65 5f6d 6d62 656e 6368 656e 202d 2d6f  me_mmbenchen --o
+00002b30: 7574 7075 745f 7061 7468 202e 2f6c 6f67  utput_path ./log
+00002b40: 732f 2023 0a0a 2320 4672 6f6d 2061 2070  s/ #..# From a p
+00002b50: 7265 6465 6669 6e65 6420 636f 6e66 6967  redefined config
+00002b60: 7572 6174 696f 6e2c 2073 7570 706f 7274  uration, support
+00002b70: 696e 6720 6576 616c 7561 7469 6f6e 206f  ing evaluation o
+00002b80: 6620 6d75 6c74 6970 6c65 206d 6f64 656c  f multiple model
+00002b90: 7320 616e 6420 6461 7461 7365 7473 0a61  s and datasets.a
+00002ba0: 6363 656c 6572 6174 6520 6c61 756e 6368  ccelerate launch
+00002bb0: 202d 2d6e 756d 5f70 726f 6365 7373 6573   --num_processes
+00002bc0: 3d38 202d 6d20 6c6d 6d73 5f65 7661 6c20  =8 -m lmms_eval 
+00002bd0: 2d2d 636f 6e66 6967 2065 7861 6d70 6c65  --config example
+00002be0: 5f65 7661 6c2e 7961 6d6c 200a 6060 600a  _eval.yaml .```.
+00002bf0: 0a23 204d 6f64 656c 2052 6573 756c 7473  .# Model Results
+00002c00: 0a0a 4173 2064 656d 6f6e 7374 7261 7465  ..As demonstrate
+00002c10: 6420 6279 2074 6865 2065 7874 656e 7369  d by the extensi
+00002c20: 7665 2074 6162 6c65 2062 656c 6f77 2c20  ve table below, 
+00002c30: 7765 2061 696d 2074 6f20 7072 6f76 6964  we aim to provid
+00002c40: 6520 6465 7461 696c 6564 2069 6e66 6f72  e detailed infor
+00002c50: 6d61 7469 6f6e 2066 6f72 2072 6561 6465  mation for reade
+00002c60: 7273 2074 6f20 756e 6465 7273 7461 6e64  rs to understand
+00002c70: 2074 6865 2064 6174 6173 6574 7320 696e   the datasets in
+00002c80: 636c 7564 6564 2069 6e20 6c6d 6d73 2d65  cluded in lmms-e
+00002c90: 7661 6c20 616e 6420 736f 6d65 2073 7065  val and some spe
+00002ca0: 6369 6669 6320 6465 7461 696c 7320 6162  cific details ab
+00002cb0: 6f75 7420 7468 6573 6520 6461 7461 7365  out these datase
+00002cc0: 7473 2028 7765 2072 656d 6169 6e20 6772  ts (we remain gr
+00002cd0: 6174 6566 756c 2066 6f72 2061 6e79 2063  ateful for any c
+00002ce0: 6f72 7265 6374 696f 6e73 2072 6561 6465  orrections reade
+00002cf0: 7273 206d 6179 2068 6176 6520 6475 7269  rs may have duri
+00002d00: 6e67 206f 7572 2065 7661 6c75 6174 696f  ng our evaluatio
+00002d10: 6e20 7072 6f63 6573 7329 2e0a 0a57 6520  n process)...We 
+00002d20: 7072 6f76 6964 6520 6120 476f 6f67 6c65  provide a Google
+00002d30: 2053 6865 6574 2066 6f72 2074 6865 2064   Sheet for the d
+00002d40: 6574 6169 6c65 6420 7265 7375 6c74 7320  etailed results 
+00002d50: 6f66 2074 6865 204c 4c61 5641 2073 6572  of the LLaVA ser
+00002d60: 6965 7320 6d6f 6465 6c73 206f 6e20 6469  ies models on di
+00002d70: 6666 6572 656e 7420 6461 7461 7365 7473  fferent datasets
+00002d80: 2e20 596f 7520 6361 6e20 6163 6365 7373  . You can access
+00002d90: 2074 6865 2073 6865 6574 205b 6865 7265   the sheet [here
+00002da0: 5d28 6874 7470 733a 2f2f 646f 6373 2e67  ](https://docs.g
+00002db0: 6f6f 676c 652e 636f 6d2f 7370 7265 6164  oogle.com/spread
+00002dc0: 7368 6565 7473 2f64 2f31 6135 496d 6664  sheets/d/1a5Imfd
+00002dd0: 4b41 5444 4938 5437 4377 6836 6548 2d62  KATDI8T7Cwh6eH-b
+00002de0: 4573 6e51 467a 616e 4672 6146 5567 6353  EsnQFzanFraFUgcS
+00002df0: 394b 4857 632f 6564 6974 3f75 7370 3d73  9KHWc/edit?usp=s
+00002e00: 6861 7269 6e67 292e 2049 7427 7320 6120  haring). It's a 
+00002e10: 6c69 7665 2073 6865 6574 2c20 616e 6420  live sheet, and 
+00002e20: 7765 2061 7265 2075 7064 6174 696e 6720  we are updating 
+00002e30: 6974 2077 6974 6820 6e65 7720 7265 7375  it with new resu
+00002e40: 6c74 732e 0a0a 3c70 2061 6c69 676e 3d22  lts...<p align="
+00002e50: 6365 6e74 6572 2220 7769 6474 683d 2231  center" width="1
+00002e60: 3030 2522 3e0a 3c69 6d67 2073 7263 3d22  00%">.<img src="
+00002e70: 6874 7470 733a 2f2f 692e 706f 7374 696d  https://i.postim
+00002e80: 672e 6363 2f6a 6477 3439 374e 532f 5758  g.cc/jdw497NS/WX
+00002e90: 3230 3234 3033 3037 2d31 3632 3532 362d  20240307-162526-
+00002ea0: 3278 2e70 6e67 2220 2077 6964 7468 3d22  2x.png"  width="
+00002eb0: 3130 3025 2220 6865 6967 6874 3d22 3830  100%" height="80
+00002ec0: 2522 3e0a 3c2f 703e 0a0a 5765 2061 6c73  %">.</p>..We als
+00002ed0: 6f20 7072 6f76 6964 6520 7468 6520 7261  o provide the ra
+00002ee0: 7720 6461 7461 2065 7870 6f72 7465 6420  w data exported 
+00002ef0: 6672 6f6d 2057 6569 6768 7473 2026 2042  from Weights & B
+00002f00: 6961 7365 7320 666f 7220 7468 6520 6465  iases for the de
+00002f10: 7461 696c 6564 2072 6573 756c 7473 206f  tailed results o
+00002f20: 6620 7468 6520 4c4c 6156 4120 7365 7269  f the LLaVA seri
+00002f30: 6573 206d 6f64 656c 7320 6f6e 2064 6966  es models on dif
+00002f40: 6665 7265 6e74 2064 6174 6173 6574 732e  ferent datasets.
+00002f50: 2059 6f75 2063 616e 2061 6363 6573 7320   You can access 
+00002f60: 7468 6520 7261 7720 6461 7461 205b 6865  the raw data [he
+00002f70: 7265 5d28 6874 7470 733a 2f2f 646f 6373  re](https://docs
+00002f80: 2e67 6f6f 676c 652e 636f 6d2f 7370 7265  .google.com/spre
+00002f90: 6164 7368 6565 7473 2f64 2f31 4176 6145  adsheets/d/1AvaE
+00002fa0: 6d75 4734 6373 536d 5861 486a 6775 3465  muG4csSmXaHjgu4e
+00002fb0: 6931 4b42 4d6d 4e4e 5738 7766 6c4f 445f  i1KBMmNNW8wflOD_
+00002fc0: 6b6b 5444 6476 382f 6564 6974 3f75 7370  kkTDdv8/edit?usp
+00002fd0: 3d73 6861 7269 6e67 292e 0a0a 3e20 4465  =sharing)...> De
+00002fe0: 7665 6c6f 706d 656e 7420 7769 6c6c 2062  velopment will b
+00002ff0: 6520 636f 6e74 696e 7569 6e67 206f 6e20  e continuing on 
+00003000: 7468 6520 6d61 696e 2062 7261 6e63 682c  the main branch,
+00003010: 2061 6e64 2077 6520 656e 636f 7572 6167   and we encourag
+00003020: 6520 796f 7520 746f 2067 6976 6520 7573  e you to give us
+00003030: 2066 6565 6462 6163 6b20 6f6e 2077 6861   feedback on wha
+00003040: 7420 6665 6174 7572 6573 2061 7265 2064  t features are d
+00003050: 6573 6972 6564 2061 6e64 2068 6f77 2074  esired and how t
+00003060: 6f20 696d 7072 6f76 6520 7468 6520 6c69  o improve the li
+00003070: 6272 6172 7920 6675 7274 6865 722c 206f  brary further, o
+00003080: 7220 6173 6b20 7175 6573 7469 6f6e 732c  r ask questions,
+00003090: 2065 6974 6865 7220 696e 2069 7373 7565   either in issue
+000030a0: 7320 6f72 2050 5273 206f 6e20 4769 7448  s or PRs on GitH
+000030b0: 7562 2e0a 0a0a 2323 2053 7570 706f 7274  ub....## Support
+000030c0: 6564 206d 6f64 656c 730a 0a2d 2047 5054  ed models..- GPT
+000030d0: 3456 2028 4150 492c 206f 6e6c 7920 6765  4V (API, only ge
+000030e0: 6e65 7261 7469 6f6e 2d62 6173 6564 2065  neration-based e
+000030f0: 7661 6c75 6174 696f 6e29 0a2d 204c 4c61  valuation).- LLa
+00003100: 5641 2d76 312e 352f 7631 2e36 2d37 422f  VA-v1.5/v1.6-7B/
+00003110: 3133 422f 3334 4220 2870 706c 2d62 6173  13B/34B (ppl-bas
+00003120: 6564 2c20 6765 6e65 7261 7469 6f6e 2d62  ed, generation-b
+00003130: 6173 6564 290a 2d20 5177 656e 2d56 4c20  ased).- Qwen-VL 
+00003140: 7365 7269 6573 2028 7070 6c2d 6261 7365  series (ppl-base
+00003150: 642c 2067 656e 6572 6174 696f 6e2d 6261  d, generation-ba
+00003160: 7365 6429 0a2d 2046 7579 7520 7365 7269  sed).- Fuyu seri
+00003170: 6573 2028 7070 6c2d 6261 7365 642c 2067  es (ppl-based, g
+00003180: 656e 6572 6174 696f 6e2d 6261 7365 6429  eneration-based)
+00003190: 0a2d 2049 6e73 7472 7563 7442 4c49 5020  .- InstructBLIP 
+000031a0: 7365 7269 6573 2028 6765 6e65 7261 7469  series (generati
+000031b0: 6f6e 2d62 6173 6564 290a 0a23 2320 5375  on-based)..## Su
+000031c0: 7070 6f72 7465 6420 6461 7461 7365 7473  pported datasets
+000031d0: 0a3e 2028 2920 696e 6469 6361 7465 7320  .> () indicates 
+000031e0: 7468 6520 7461 736b 206e 616d 6520 696e  the task name in
+000031f0: 2074 6865 206c 6d6d 735f 6576 616c 2e20   the lmms_eval. 
+00003200: 5468 6520 7461 736b 206e 616d 6520 6973  The task name is
+00003210: 2061 6c73 6f20 7573 6564 2074 6f20 7370   also used to sp
+00003220: 6563 6966 7920 7468 6520 6461 7461 7365  ecify the datase
+00003230: 7420 696e 2074 6865 2063 6f6e 6669 6775  t in the configu
+00003240: 7261 7469 6f6e 2066 696c 652e 0a0a 2d20  ration file...- 
+00003250: 4149 3244 2028 6169 3264 290a 2d20 4368  AI2D (ai2d).- Ch
+00003260: 6172 7451 4120 2863 6861 7274 7161 290a  artQA (chartqa).
+00003270: 2d20 434d 4d4d 5520 2863 6d6d 6d75 290a  - CMMMU (cmmmu).
+00003280: 2020 2d20 434d 4d4d 5520 5661 6c69 6461    - CMMMU Valida
+00003290: 7469 6f6e 2028 636d 6d6d 755f 7661 6c29  tion (cmmmu_val)
+000032a0: 0a20 202d 2043 4d4d 4d55 2054 6573 7420  .  - CMMMU Test 
+000032b0: 2863 6d6d 6d75 5f74 6573 7429 0a2d 2043  (cmmmu_test).- C
+000032c0: 4f43 4f20 4361 7074 696f 6e20 2863 6f63  OCO Caption (coc
+000032d0: 6f5f 6361 7029 0a20 202d 2043 4f43 4f20  o_cap).  - COCO 
+000032e0: 3230 3134 2043 6170 7469 6f6e 2028 636f  2014 Caption (co
+000032f0: 636f 3230 3134 5f63 6170 290a 2020 2020  co2014_cap).    
+00003300: 2d20 434f 434f 2032 3031 3420 4361 7074  - COCO 2014 Capt
+00003310: 696f 6e20 5661 6c69 6461 7469 6f6e 2028  ion Validation (
+00003320: 636f 636f 3230 3134 5f63 6170 5f76 616c  coco2014_cap_val
+00003330: 290a 2020 2020 2d20 434f 434f 2032 3031  ).    - COCO 201
+00003340: 3420 4361 7074 696f 6e20 5465 7374 2028  4 Caption Test (
+00003350: 636f 636f 3230 3134 5f63 6170 5f74 6573  coco2014_cap_tes
+00003360: 7429 0a20 202d 2043 4f43 4f20 3230 3137  t).  - COCO 2017
+00003370: 2043 6170 7469 6f6e 2028 636f 636f 3230   Caption (coco20
+00003380: 3137 5f63 6170 290a 2020 2020 2d20 434f  17_cap).    - CO
+00003390: 434f 2032 3031 3720 4361 7074 696f 6e20  CO 2017 Caption 
+000033a0: 4d69 6e69 5661 6c20 2863 6f63 6f32 3031  MiniVal (coco201
+000033b0: 375f 6361 705f 7661 6c29 0a20 2020 202d  7_cap_val).    -
+000033c0: 2043 4f43 4f20 3230 3137 2043 6170 7469   COCO 2017 Capti
+000033d0: 6f6e 204d 696e 6954 6573 7420 2863 6f63  on MiniTest (coc
+000033e0: 6f32 3031 375f 6361 705f 7465 7374 290a  o2017_cap_test).
+000033f0: 2d20 444f 4356 5141 2028 646f 6376 7161  - DOCVQA (docvqa
+00003400: 290a 2020 2d20 444f 4356 5141 2056 616c  ).  - DOCVQA Val
+00003410: 6964 6174 696f 6e20 2864 6f63 7671 615f  idation (docvqa_
+00003420: 7661 6c29 0a20 202d 2044 4f43 5651 4120  val).  - DOCVQA 
+00003430: 5465 7374 2028 646f 6376 7161 5f74 6573  Test (docvqa_tes
+00003440: 7429 0a2d 2046 6572 7265 7420 2866 6572  t).- Ferret (fer
+00003450: 7265 7429 0a2d 2046 6c69 636b 7233 304b  ret).- Flickr30K
+00003460: 2028 666c 6963 6b72 3330 6b29 0a20 202d   (flickr30k).  -
+00003470: 2046 6572 7265 7420 5465 7374 2028 6665   Ferret Test (fe
+00003480: 7272 6574 5f74 6573 7429 0a2d 2047 5141  rret_test).- GQA
+00003490: 2028 6771 6129 0a2d 2048 616c 6c75 7369   (gqa).- Hallusi
+000034a0: 6f6e 4265 6e63 686d 6172 6b20 2868 616c  onBenchmark (hal
+000034b0: 6c75 7369 6f6e 5f62 656e 6368 5f69 6d61  lusion_bench_ima
+000034c0: 6765 290a 2d20 496e 666f 6772 6170 6869  ge).- Infographi
+000034d0: 6320 5651 4120 2869 6e66 6f5f 7671 6129  c VQA (info_vqa)
+000034e0: 0a20 202d 2049 6e66 6f67 7261 7068 6963  .  - Infographic
+000034f0: 2056 5141 2056 616c 6964 6174 696f 6e20   VQA Validation 
+00003500: 2869 6e66 6f5f 7671 615f 7661 6c29 0a20  (info_vqa_val). 
+00003510: 202d 2049 6e66 6f67 7261 7068 6963 2056   - Infographic V
+00003520: 5141 2054 6573 7420 2869 6e66 6f5f 7671  QA Test (info_vq
+00003530: 615f 7465 7374 290a 2d20 4c4c 6156 412d  a_test).- LLaVA-
+00003540: 4265 6e63 6820 286c 6c61 7661 5f69 6e5f  Bench (llava_in_
+00003550: 7468 655f 7769 6c64 290a 2d20 4c4c 6156  the_wild).- LLaV
+00003560: 412d 4265 6e63 682d 434f 434f 2028 6c6c  A-Bench-COCO (ll
+00003570: 6176 615f 6265 6e63 685f 636f 636f 290a  ava_bench_coco).
+00003580: 2d20 4d61 7468 5669 7374 6120 286d 6174  - MathVista (mat
+00003590: 6876 6973 7461 290a 2020 2d20 4d61 7468  hvista).  - Math
+000035a0: 5669 7374 6120 5661 6c69 6461 7469 6f6e  Vista Validation
+000035b0: 2028 6d61 7468 7669 7374 615f 7465 7374   (mathvista_test
+000035c0: 6d69 6e69 290a 2020 2d20 4d61 7468 5669  mini).  - MathVi
+000035d0: 7374 6120 5465 7374 2028 6d61 7468 7669  sta Test (mathvi
+000035e0: 7374 615f 7465 7374 290a 2d20 4d4d 4265  sta_test).- MMBe
+000035f0: 6e63 6820 286d 6d62 656e 6368 290a 2020  nch (mmbench).  
+00003600: 2d20 4d4d 4265 6e63 6820 456e 676c 6973  - MMBench Englis
+00003610: 6820 286d 6d62 656e 6368 5f65 6e29 0a20  h (mmbench_en). 
+00003620: 2020 202d 204d 4d42 656e 6368 2045 6e67     - MMBench Eng
+00003630: 6c69 7368 2044 6576 2028 6d6d 6265 6e63  lish Dev (mmbenc
+00003640: 685f 656e 5f64 6576 290a 2020 2020 2d20  h_en_dev).    - 
+00003650: 4d4d 4265 6e63 6820 456e 676c 6973 6820  MMBench English 
+00003660: 5465 7374 2028 6d6d 6265 6e63 685f 656e  Test (mmbench_en
+00003670: 5f74 6573 7429 0a20 202d 204d 4d42 656e  _test).  - MMBen
+00003680: 6368 2043 6869 6e65 7365 2028 6d6d 6265  ch Chinese (mmbe
+00003690: 6e63 685f 636e 290a 2020 2020 2d20 4d4d  nch_cn).    - MM
+000036a0: 4265 6e63 6820 4368 696e 6573 6520 4465  Bench Chinese De
+000036b0: 7620 286d 6d62 656e 6368 5f63 6e5f 6465  v (mmbench_cn_de
+000036c0: 7629 0a20 2020 202d 204d 4d42 656e 6368  v).    - MMBench
+000036d0: 2043 6869 6e65 7365 2054 6573 7420 286d   Chinese Test (m
+000036e0: 6d62 656e 6368 5f63 6e5f 7465 7374 290a  mbench_cn_test).
+000036f0: 2d20 4d4d 4520 286d 6d65 290a 2d20 4d4d  - MME (mme).- MM
+00003700: 4d55 2028 6d6d 6d75 290a 2020 2d20 4d4d  MU (mmmu).  - MM
+00003710: 4d55 2056 616c 6964 6174 696f 6e20 286d  MU Validation (m
+00003720: 6d6d 755f 7661 6c29 0a20 202d 204d 4d4d  mmu_val).  - MMM
+00003730: 5520 5465 7374 2028 6d6d 6d75 5f74 6573  U Test (mmmu_tes
+00003740: 7429 0a2d 204d 4d56 6574 2028 6d6d 7665  t).- MMVet (mmve
+00003750: 7429 0a2d 204d 756c 7469 2d44 6f63 5651  t).- Multi-DocVQ
+00003760: 4120 286d 756c 7469 646f 6376 7161 290a  A (multidocvqa).
+00003770: 2020 2d20 4d75 6c74 692d 446f 6356 5141    - Multi-DocVQA
+00003780: 2056 616c 6964 6174 696f 6e20 286d 756c   Validation (mul
+00003790: 7469 646f 6376 7161 5f76 616c 290a 2020  tidocvqa_val).  
+000037a0: 2d20 4d75 6c74 692d 446f 6356 5141 2054  - Multi-DocVQA T
+000037b0: 6573 7420 286d 756c 7469 646f 6376 7161  est (multidocvqa
+000037c0: 5f74 6573 7429 0a2d 204e 6f43 6170 7320  _test).- NoCaps 
+000037d0: 286e 6f63 6170 7329 0a20 202d 204e 6f43  (nocaps).  - NoC
+000037e0: 6170 7320 5661 6c69 6461 7469 6f6e 2028  aps Validation (
+000037f0: 6e6f 6361 7073 5f76 616c 290a 2020 2d20  nocaps_val).  - 
+00003800: 4e6f 4361 7073 2054 6573 7420 286e 6f63  NoCaps Test (noc
+00003810: 6170 735f 7465 7374 290a 2d20 4f4b 5651  aps_test).- OKVQ
+00003820: 4120 286f 6b5f 7671 6129 0a20 202d 204f  A (ok_vqa).  - O
+00003830: 4b56 5141 2056 616c 6964 6174 696f 6e20  KVQA Validation 
+00003840: 3230 3134 2028 6f6b 5f76 7161 5f76 616c  2014 (ok_vqa_val
+00003850: 3230 3134 290a 2d20 504f 5045 2028 706f  2014).- POPE (po
+00003860: 7065 290a 2d20 5265 6643 4f43 4f20 2872  pe).- RefCOCO (r
+00003870: 6566 636f 636f 290a 2020 2020 2d20 7265  efcoco).    - re
+00003880: 6663 6f63 6f5f 7365 675f 7465 7374 0a20  fcoco_seg_test. 
+00003890: 2020 202d 2072 6566 636f 636f 5f73 6567     - refcoco_seg
+000038a0: 5f76 616c 0a20 2020 202d 2072 6566 636f  _val.    - refco
+000038b0: 636f 5f73 6567 5f74 6573 7441 0a20 2020  co_seg_testA.   
+000038c0: 202d 2072 6566 636f 636f 5f73 6567 5f74   - refcoco_seg_t
+000038d0: 6573 7442 0a20 2020 202d 2072 6566 636f  estB.    - refco
+000038e0: 636f 5f62 626f 785f 7465 7374 0a20 2020  co_bbox_test.   
+000038f0: 202d 2072 6566 636f 636f 5f62 626f 785f   - refcoco_bbox_
+00003900: 7661 6c0a 2020 2020 2d20 7265 6663 6f63  val.    - refcoc
+00003910: 6f5f 6262 6f78 5f74 6573 7441 0a20 2020  o_bbox_testA.   
+00003920: 202d 2072 6566 636f 636f 5f62 626f 785f   - refcoco_bbox_
+00003930: 7465 7374 420a 2d20 5265 6643 4f43 4f2b  testB.- RefCOCO+
+00003940: 2028 7265 6663 6f63 6f2b 290a 2020 2020   (refcoco+).    
+00003950: 2d20 7265 6663 6f63 6f2b 5f73 6567 0a20  - refcoco+_seg. 
+00003960: 2020 2020 2020 202d 2072 6566 636f 636f         - refcoco
+00003970: 2b5f 7365 675f 7661 6c0a 2020 2020 2020  +_seg_val.      
+00003980: 2020 2d20 7265 6663 6f63 6f2b 5f73 6567    - refcoco+_seg
+00003990: 5f74 6573 7441 0a20 2020 2020 2020 202d  _testA.        -
+000039a0: 2072 6566 636f 636f 2b5f 7365 675f 7465   refcoco+_seg_te
+000039b0: 7374 420a 2020 2020 2d20 7265 6663 6f63  stB.    - refcoc
+000039c0: 6f2b 5f62 626f 780a 2020 2020 2020 2020  o+_bbox.        
+000039d0: 2d20 7265 6663 6f63 6f2b 5f62 626f 785f  - refcoco+_bbox_
+000039e0: 7661 6c0a 2020 2020 2020 2020 2d20 7265  val.        - re
+000039f0: 6663 6f63 6f2b 5f62 626f 785f 7465 7374  fcoco+_bbox_test
+00003a00: 410a 2020 2020 2020 2020 2d20 7265 6663  A.        - refc
+00003a10: 6f63 6f2b 5f62 626f 785f 7465 7374 420a  oco+_bbox_testB.
+00003a20: 2d20 5265 6643 4f43 4f67 2028 7265 6663  - RefCOCOg (refc
+00003a30: 6f63 6f67 290a 2020 2020 2d20 7265 6663  ocog).    - refc
+00003a40: 6f63 6f67 5f73 6567 5f74 6573 740a 2020  ocog_seg_test.  
+00003a50: 2020 2d20 7265 6663 6f63 6f67 5f73 6567    - refcocog_seg
+00003a60: 5f76 616c 0a20 2020 202d 2072 6566 636f  _val.    - refco
+00003a70: 636f 675f 6262 6f78 5f74 6573 740a 2020  cog_bbox_test.  
+00003a80: 2020 2d20 7265 6663 6f63 6f67 5f62 626f    - refcocog_bbo
+00003a90: 785f 7661 6c0a 2d20 5363 6965 6e63 6551  x_val.- ScienceQ
+00003aa0: 4120 2873 6369 656e 6365 7161 5f66 756c  A (scienceqa_ful
+00003ab0: 6c29 0a20 202d 2053 6369 656e 6365 5141  l).  - ScienceQA
+00003ac0: 2046 756c 6c20 2873 6369 656e 6365 7161   Full (scienceqa
+00003ad0: 290a 2020 2d20 5363 6965 6e63 6551 4120  ).  - ScienceQA 
+00003ae0: 494d 4720 2873 6369 656e 6365 7161 5f69  IMG (scienceqa_i
+00003af0: 6d67 290a 2d20 5365 6564 4265 6e63 6820  mg).- SeedBench 
+00003b00: 2873 6565 6462 656e 6368 290a 2d20 5365  (seedbench).- Se
+00003b10: 6564 4265 6e63 6820 3220 2873 6565 6462  edBench 2 (seedb
+00003b20: 656e 6368 5f32 290a 2d20 5354 2d56 5141  ench_2).- ST-VQA
+00003b30: 2028 7374 7671 6129 0a2d 2054 6578 7443   (stvqa).- TextC
+00003b40: 6170 7320 2874 6578 7463 6170 7329 0a20  aps (textcaps). 
+00003b50: 202d 2054 6578 7443 6170 7320 5661 6c69   - TextCaps Vali
+00003b60: 6461 7469 6f6e 2028 7465 7874 6361 7073  dation (textcaps
+00003b70: 5f76 616c 290a 2020 2d20 5465 7874 4361  _val).  - TextCa
+00003b80: 7073 2054 6573 7420 2874 6578 7463 6170  ps Test (textcap
+00003b90: 735f 7465 7374 290a 2d20 5465 7874 5651  s_test).- TextVQ
+00003ba0: 4120 2874 6578 7476 7161 290a 2020 2d20  A (textvqa).  - 
+00003bb0: 5465 7874 5651 4120 5661 6c69 6461 7469  TextVQA Validati
+00003bc0: 6f6e 2028 7465 7874 7671 615f 7661 6c29  on (textvqa_val)
+00003bd0: 0a20 202d 2054 6578 7456 5141 2054 6573  .  - TextVQA Tes
+00003be0: 7420 2874 6578 7476 7161 5f74 6573 7429  t (textvqa_test)
+00003bf0: 0a2d 2056 697a 5769 7a56 5141 2028 7669  .- VizWizVQA (vi
+00003c00: 7a77 697a 5f76 7161 290a 2020 2d20 5669  zwiz_vqa).  - Vi
+00003c10: 7a57 697a 5651 4120 5661 6c69 6461 7469  zWizVQA Validati
+00003c20: 6f6e 2028 7669 7a77 697a 5f76 7161 5f76  on (vizwiz_vqa_v
+00003c30: 616c 290a 2020 2d20 5669 7a57 697a 5651  al).  - VizWizVQ
+00003c40: 4120 5465 7374 2028 7669 7a77 697a 5f76  A Test (vizwiz_v
+00003c50: 7161 5f74 6573 7429 0a2d 2056 5141 7632  qa_test).- VQAv2
+00003c60: 2028 7671 6176 3229 0a20 202d 2056 5141   (vqav2).  - VQA
+00003c70: 7632 2056 616c 6964 6174 696f 6e20 2876  v2 Validation (v
+00003c80: 7161 7632 5f76 616c 290a 2020 2d20 5651  qav2_val).  - VQ
+00003c90: 4176 3220 5465 7374 2028 7671 6176 325f  Av2 Test (vqav2_
+00003ca0: 7465 7374 290a 0a23 2320 4461 7461 7365  test)..## Datase
+00003cb0: 7473 2074 6f20 6265 2061 6464 6564 2061  ts to be added a
+00003cc0: 6e64 2074 6573 7465 640a 2d20 5461 6c6c  nd tested.- Tall
+00003cd0: 7951 4120 2874 616c 6c79 7161 290a 2d20  yQA (tallyqa).- 
+00003ce0: 5653 5220 2876 7372 290a 2d20 5769 6e6f  VSR (vsr).- Wino
+00003cf0: 6772 6f75 6e64 2028 7769 6e6f 6772 6f75  ground (winogrou
+00003d00: 6e64 290a 2d20 4e4c 5652 3220 286e 6c76  nd).- NLVR2 (nlv
+00003d10: 7232 290a 2d20 5261 7665 6e49 512d 5465  r2).- RavenIQ-Te
+00003d20: 7374 2028 7261 7665 6e69 7129 0a2d 2049  st (raveniq).- I
+00003d30: 636f 6e51 4120 2869 636f 6e71 6129 0a2d  conQA (iconqa).-
+00003d40: 2056 6973 7442 656e 6368 2028 7669 7374   VistBench (vist
+00003d50: 6265 6e63 6829 0a0a 2320 4164 6420 4375  bench)..# Add Cu
+00003d60: 7374 6f6d 697a 6564 204d 6f64 656c 2061  stomized Model a
+00003d70: 6e64 2044 6174 6173 6574 0a0a 506c 6561  nd Dataset..Plea
+00003d80: 7365 2072 6566 6572 2074 6f20 6f75 7220  se refer to our 
+00003d90: 5b64 6f63 756d 656e 7461 7469 6f6e 5d28  [documentation](
+00003da0: 646f 6373 2f52 4541 444d 452e 6d64 292e  docs/README.md).
+00003db0: 0a0a 2320 4163 6b6e 6f77 6c65 6467 656d  ..# Acknowledgem
+00003dc0: 656e 740a 0a6c 6d6d 735f 6576 616c 2069  ent..lmms_eval i
+00003dd0: 7320 6120 666f 726b 206f 6620 5b6c 6d2d  s a fork of [lm-
+00003de0: 6576 616c 2d68 6172 6e65 7373 5d28 6874  eval-harness](ht
+00003df0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00003e00: 2f45 6c65 7574 6865 7241 492f 6c6d 2d65  /EleutherAI/lm-e
+00003e10: 7661 6c75 6174 696f 6e2d 6861 726e 6573  valuation-harnes
+00003e20: 7329 2e20 5765 2072 6563 6f6d 6d65 6e64  s). We recommend
+00003e30: 2079 6f75 2074 6f20 7265 6164 2074 6872   you to read thr
+00003e40: 6f75 6768 2074 6865 205b 646f 6373 206f  ough the [docs o
+00003e50: 6620 6c6d 2d65 7661 6c2d 6861 726e 6573  f lm-eval-harnes
+00003e60: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
+00003e70: 622e 636f 6d2f 456c 6575 7468 6572 4149  b.com/EleutherAI
+00003e80: 2f6c 6d2d 6576 616c 7561 7469 6f6e 2d68  /lm-evaluation-h
+00003e90: 6172 6e65 7373 2f74 7265 652f 6d61 696e  arness/tree/main
+00003ea0: 2f64 6f63 7329 2066 6f72 2072 656c 6576  /docs) for relev
+00003eb0: 616e 7420 696e 666f 726d 6174 696f 6e2e  ant information.
+00003ec0: 200a 0a42 656c 6f77 2061 7265 2074 6865   ..Below are the
+00003ed0: 2063 6861 6e67 6573 2077 6520 6d61 6465   changes we made
+00003ee0: 2074 6f20 7468 6520 6f72 6967 696e 616c   to the original
+00003ef0: 2041 5049 3a0a 2d20 4275 696c 6420 636f   API:.- Build co
+00003f00: 6e74 6578 7420 6e6f 7720 6f6e 6c79 2070  ntext now only p
+00003f10: 6173 7320 696e 2069 6478 2061 6e64 2070  ass in idx and p
+00003f20: 726f 6365 7373 2069 6d61 6765 2061 6e64  rocess image and
+00003f30: 2064 6f63 2064 7572 696e 6720 7468 6520   doc during the 
+00003f40: 6d6f 6465 6c20 7265 7370 6f6e 6469 6e67  model responding
+00003f50: 2070 6861 7365 2e20 5468 6973 2069 7320   phase. This is 
+00003f60: 6475 6520 746f 2074 6865 2066 6163 7420  due to the fact 
+00003f70: 7468 6174 2064 6174 6173 6574 206e 6f77  that dataset now
+00003f80: 2063 6f6e 7461 696e 7320 6c6f 7473 206f   contains lots o
+00003f90: 6620 696d 6167 6573 2061 6e64 2077 6520  f images and we 
+00003fa0: 6361 6e27 7420 7374 6f72 6520 7468 656d  can't store them
+00003fb0: 2069 6e20 7468 6520 646f 6320 6c69 6b65   in the doc like
+00003fc0: 2074 6865 206f 7269 6769 6e61 6c20 6c6d   the original lm
+00003fd0: 2d65 7661 6c2d 6861 726e 6573 7320 6f74  -eval-harness ot
+00003fe0: 6865 7220 7769 7365 2074 6865 2063 7075  her wise the cpu
+00003ff0: 206d 656d 6f72 7920 776f 756c 6420 6578   memory would ex
+00004000: 706c 6f64 652e 0a2d 2049 6e73 7461 6e63  plode..- Instanc
+00004010: 652e 6172 6773 2028 6c6d 6d73 5f65 7661  e.args (lmms_eva
+00004020: 6c2f 6170 692f 696e 7374 616e 6365 2e70  l/api/instance.p
+00004030: 7929 206e 6f77 2063 6f6e 7461 696e 7320  y) now contains 
+00004040: 6120 6c69 7374 206f 6620 696d 6167 6573  a list of images
+00004050: 2074 6f20 6265 2069 6e70 7574 7465 6420   to be inputted 
+00004060: 746f 206c 6d6d 732e 0a2d 206c 6d2d 6576  to lmms..- lm-ev
+00004070: 616c 2d68 6172 6e65 7373 2073 7570 706f  al-harness suppo
+00004080: 7274 7320 616c 6c20 4846 206c 616e 6775  rts all HF langu
+00004090: 6167 6520 6d6f 6465 6c73 2061 7320 7369  age models as si
+000040a0: 6e67 6c65 206d 6f64 656c 2063 6c61 7373  ngle model class
+000040b0: 2e20 4375 7272 656e 746c 7920 7468 6973  . Currently this
+000040c0: 2069 7320 6e6f 7420 706f 7373 6962 6c65   is not possible
+000040d0: 206f 6620 6c6d 6d73 2062 6563 6175 7365   of lmms because
+000040e0: 2074 6865 2069 6e70 7574 2f6f 7574 7075   the input/outpu
+000040f0: 7420 666f 726d 6174 206f 6620 6c6d 6d73  t format of lmms
+00004100: 2069 6e20 4846 2061 7265 206e 6f74 2079   in HF are not y
+00004110: 6574 2075 6e69 6669 6564 2e20 5468 6572  et unified. Ther
+00004120: 6572 666f 7265 2c20 7765 2068 6176 6520  erfore, we have 
+00004130: 746f 2063 7265 6174 6520 6120 6e65 7720  to create a new 
+00004140: 636c 6173 7320 666f 7220 6561 6368 206c  class for each l
+00004150: 6d6d 7320 6d6f 6465 6c2e 2054 6869 7320  mms model. This 
+00004160: 6973 206e 6f74 2069 6465 616c 2061 6e64  is not ideal and
+00004170: 2077 6520 7769 6c6c 2074 7279 2074 6f20   we will try to 
+00004180: 756e 6966 7920 7468 656d 2069 6e20 7468  unify them in th
+00004190: 6520 6675 7475 7265 2e0a 0a57 6520 616c  e future...We al
+000041a0: 736f 2074 6861 6e6b 3a0a 2d20 5b58 6961  so thank:.- [Xia
+000041b0: 6e67 2059 7565 5d28 6874 7470 733a 2f2f  ng Yue](https://
+000041c0: 7869 616e 6779 7565 3936 3037 2e67 6974  xiangyue9607.git
+000041d0: 6875 622e 696f 2f29 2c20 5b4a 696e 676b  hub.io/), [Jingk
+000041e0: 616e 6720 5961 6e67 5d28 6874 7470 733a  ang Yang](https:
+000041f0: 2f2f 6a69 6e67 6b61 6e67 3530 2e67 6974  //jingkang50.git
+00004200: 6875 622e 696f 2f29 2c20 5b44 6f6e 6720  hub.io/), [Dong 
+00004210: 4775 6f5d 2868 7474 7073 3a2f 2f77 7777  Guo](https://www
+00004220: 2e6c 696e 6b65 6469 6e2e 636f 6d2f 696e  .linkedin.com/in
+00004230: 2f64 6f6e 6767 756f 7365 742f 2920 616e  /dongguoset/) an
+00004240: 6420 5b53 6865 6e67 2053 6865 6e5d 2868  d [Sheng Shen](h
+00004250: 7474 7073 3a2f 2f73 696e 6365 7261 7373  ttps://sincerass
+00004260: 2e67 6974 6875 622e 696f 2f29 2066 6f72  .github.io/) for
+00004270: 2065 6172 6c79 2064 6973 6375 7373 696f   early discussio
+00004280: 6e20 616e 6420 7465 7374 696e 672e 0a0a  n and testing...
+00004290: 2323 2043 6974 6174 696f 6e73 0a0a 6060  ## Citations..``
+000042a0: 6073 6865 6c6c 0a40 6d69 7363 7b6c 6d6d  `shell.@misc{lmm
+000042b0: 735f 6576 616c 3230 3234 2c0a 2020 2020  s_eval2024,.    
+000042c0: 7469 746c 653d 7b4c 4d4d 732d 4576 616c  title={LMMs-Eval
+000042d0: 3a20 4163 6365 6c65 7261 7469 6e67 2074  : Accelerating t
+000042e0: 6865 2044 6576 656c 6f70 6d65 6e74 206f  he Development o
+000042f0: 6620 4c61 7267 6520 4d75 6c74 696d 6f61  f Large Multimoa
+00004300: 6c20 4d6f 6465 6c73 7d2c 0a20 2020 2075  l Models},.    u
+00004310: 726c 3d7b 6874 7470 733a 2f2f 6769 7468  rl={https://gith
+00004320: 7562 2e63 6f6d 2f45 766f 6c76 696e 674c  ub.com/EvolvingL
+00004330: 4d4d 732d 4c61 622f 6c6d 6d73 2d65 7661  MMs-Lab/lmms-eva
+00004340: 6c7d 2c0a 2020 2020 6175 7468 6f72 3d7b  l},.    author={
+00004350: 426f 204c 692a 2c20 5065 6979 7561 6e20  Bo Li*, Peiyuan 
+00004360: 5a68 616e 672a 2c20 4b61 6963 6865 6e20  Zhang*, Kaichen 
+00004370: 5a68 616e 672a 2c20 4661 6e79 6920 5075  Zhang*, Fanyi Pu
+00004380: 2a2c 2058 696e 7275 6e20 4475 2c20 5975  *, Xinrun Du, Yu
+00004390: 6861 6f20 446f 6e67 2c20 4861 6f74 6961  hao Dong, Haotia
+000043a0: 6e20 4c69 752c 2059 7561 6e68 616e 205a  n Liu, Yuanhan Z
+000043b0: 6861 6e67 2c20 4765 205a 6861 6e67 2c20  hang, Ge Zhang, 
+000043c0: 4368 756e 7975 616e 204c 6920 616e 6420  Chunyuan Li and 
+000043d0: 5a69 7765 6920 4c69 757d 2c0a 2020 2020  Ziwei Liu},.    
+000043e0: 7075 626c 6973 6865 7220 2020 203d 207b  publisher    = {
+000043f0: 5a65 6e6f 646f 7d2c 0a20 2020 2076 6572  Zenodo},.    ver
+00004400: 7369 6f6e 2020 2020 2020 3d20 7b76 302e  sion      = {v0.
+00004410: 312e 307d 2c0a 2020 2020 6d6f 6e74 683d  1.0},.    month=
+00004420: 7b4d 6172 6368 7d2c 0a20 2020 2079 6561  {March},.    yea
+00004430: 723d 7b32 3032 347d 0a7d 0a60 6060 0a    r={2024}.}.```.
```

### Comparing `lmms_eval-0.1.1/lmms_eval.egg-info/SOURCES.txt` & `lmms_eval-0.1.2/lmms_eval.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 lmms_eval/filters/selection.py
 lmms_eval/filters/transformation.py
 lmms_eval/models/__init__.py
 lmms_eval/models/fuyu.py
 lmms_eval/models/gpt4v.py
 lmms_eval/models/instructblip.py
 lmms_eval/models/llava.py
+lmms_eval/models/llava_hf.py
 lmms_eval/models/minicpm_v.py
 lmms_eval/models/qwen_vl.py
 lmms_eval/models/model_utils/__init__.py
 lmms_eval/models/model_utils/qwen/qwen_generate_utils.py
 lmms_eval/tasks/__init__.py
 lmms_eval/tasks/__pycache__/__init__.cpython-311.pyc
 lmms_eval/tasks/_task_utils/file_utils.py
@@ -120,14 +121,16 @@
 lmms_eval/tasks/mathvista/mathvista.yaml
 lmms_eval/tasks/mathvista/mathvista_evals.py
 lmms_eval/tasks/mathvista/mathvista_test.yaml
 lmms_eval/tasks/mathvista/mathvista_testmini.yaml
 lmms_eval/tasks/mathvista/utils.py
 lmms_eval/tasks/mathvista/__pycache__/mathvista_evals.cpython-311.pyc
 lmms_eval/tasks/mathvista/__pycache__/utils.cpython-311.pyc
+lmms_eval/tasks/mmbench/_default_template_mmbench_cn_yaml
+lmms_eval/tasks/mmbench/_default_template_mmbench_en_yaml
 lmms_eval/tasks/mmbench/cc_utils.py
 lmms_eval/tasks/mmbench/cn_utils.py
 lmms_eval/tasks/mmbench/en_utils.py
 lmms_eval/tasks/mmbench/mmbench.yaml
 lmms_eval/tasks/mmbench/mmbench_cc.yaml
 lmms_eval/tasks/mmbench/mmbench_cn.yaml
 lmms_eval/tasks/mmbench/mmbench_cn_dev.yaml
@@ -158,23 +161,40 @@
 lmms_eval/tasks/multidocvqa/__pycache__/utils.cpython-311.pyc
 lmms_eval/tasks/nocaps/_default_template_nocaps_yaml
 lmms_eval/tasks/nocaps/nocaps.yaml
 lmms_eval/tasks/nocaps/nocaps_test.yaml
 lmms_eval/tasks/nocaps/nocaps_val.yaml
 lmms_eval/tasks/nocaps/utils.py
 lmms_eval/tasks/nocaps/__pycache__/utils.cpython-311.pyc
+lmms_eval/tasks/ocrbench/ocrbench.yaml
+lmms_eval/tasks/ocrbench/upload_ocrbench.py
+lmms_eval/tasks/ocrbench/utils.py
+lmms_eval/tasks/ocrbench/__pycache__/utils.cpython-311.pyc
 lmms_eval/tasks/ok_vqa/_default_template_vqa_yaml
 lmms_eval/tasks/ok_vqa/_generate_config.py
 lmms_eval/tasks/ok_vqa/_ok_vqa.yaml
 lmms_eval/tasks/ok_vqa/ok_vqa_val2014.yaml
 lmms_eval/tasks/ok_vqa/utils.py
 lmms_eval/tasks/ok_vqa/__pycache__/utils.cpython-311.pyc
+lmms_eval/tasks/olympiadbench/cn_utils.py
+lmms_eval/tasks/olympiadbench/en_utils.py
+lmms_eval/tasks/olympiadbench/olympiadbench.yaml
+lmms_eval/tasks/olympiadbench/olympiadbench_evals.py
+lmms_eval/tasks/olympiadbench/olympiadbench_test_cn.yaml
+lmms_eval/tasks/olympiadbench/olympiadbench_test_en.yaml
+lmms_eval/tasks/olympiadbench/__pycache__/cn_utils.cpython-311.pyc
+lmms_eval/tasks/olympiadbench/__pycache__/en_utils.cpython-311.pyc
+lmms_eval/tasks/olympiadbench/__pycache__/olympiadbench_evals.cpython-311.pyc
+lmms_eval/tasks/olympiadbench/__pycache__/utils.cpython-311.pyc
 lmms_eval/tasks/pope/pope.yaml
 lmms_eval/tasks/pope/utils.py
 lmms_eval/tasks/pope/__pycache__/utils.cpython-311.pyc
+lmms_eval/tasks/realworldqa/realworldqa.yaml
+lmms_eval/tasks/realworldqa/utils.py
+lmms_eval/tasks/realworldqa/__pycache__/utils.cpython-311.pyc
 lmms_eval/tasks/refcoco/_default_template_bbox_yaml
 lmms_eval/tasks/refcoco/_default_template_seg_yaml
 lmms_eval/tasks/refcoco/_generate_config.py
 lmms_eval/tasks/refcoco/_refcoco.yaml
 lmms_eval/tasks/refcoco/refcoco_bbox_test.yaml
 lmms_eval/tasks/refcoco/refcoco_bbox_testA.yaml
 lmms_eval/tasks/refcoco/refcoco_bbox_testB.yaml
```

### Comparing `lmms_eval-0.1.1/miscs/repr_torch_envs.txt` & `lmms_eval-0.1.2/miscs/repr_torch_envs.txt`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/miscs/scienceqa_id.txt` & `lmms_eval-0.1.2/miscs/scienceqa_id.txt`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/miscs/script.sh` & `lmms_eval-0.1.2/miscs/script.sh`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/miscs/test_llava.py` & `lmms_eval-0.1.2/miscs/test_llava.py`

 * *Files identical despite different names*

### Comparing `lmms_eval-0.1.1/pyproject.toml` & `lmms_eval-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [build-system]
 requires = ["setuptools>=42", "wheel", "setuptools_scm[tomli]>=6.3"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lmms_eval"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     { name = "LMMMs-Lab Evaluation Team", email = "lmms_eval@outlook.com" },
 ]
 description = "A framework for evaluating large multi-modality language models"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -34,15 +34,15 @@
     "sacrebleu>=1.5.0",
     "scikit-learn>=0.24.1",
     "sqlitedict",
     "torch>=1.8",
     "openai>=1.0.0",
     "pycocoevalcap",
     "tqdm-multiprocess",
-    "transformers==4.37.2",
+    "transformers",
     "zstandard",
     "pillow",
     "pyyaml",
     "sympy",
     "mpmath",
     "Jinja2",
     "openpyxl",
```

### Comparing `lmms_eval-0.1.1/tools/make_hf_dataset.ipynb` & `lmms_eval-0.1.2/tools/make_hf_dataset.ipynb`

 * *Files identical despite different names*

