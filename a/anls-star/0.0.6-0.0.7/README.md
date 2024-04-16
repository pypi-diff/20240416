# Comparing `tmp/anls_star-0.0.6.tar.gz` & `tmp/anls_star-0.0.7.tar.gz`

## Comparing `anls_star-0.0.6.tar` & `anls_star-0.0.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 anls_star-0.0.6/src/__init__.py
--rw-r--r--   0        0        0    11414 2020-02-02 00:00:00.000000 anls_star-0.0.6/src/anls_star.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anls_star-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0    13536 2020-02-02 00:00:00.000000 anls_star-0.0.6/tests/test_anls_star.py
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 anls_star-0.0.6/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 anls_star-0.0.6/LICENSE
--rw-r--r--   0        0        0     7497 2020-02-02 00:00:00.000000 anls_star-0.0.6/README.md
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 anls_star-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     8194 2020-02-02 00:00:00.000000 anls_star-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 anls_star-0.0.7/src/__init__.py
+-rw-r--r--   0        0        0    11795 2020-02-02 00:00:00.000000 anls_star-0.0.7/src/anls_star.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anls_star-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0    13806 2020-02-02 00:00:00.000000 anls_star-0.0.7/tests/test_anls_star.py
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 anls_star-0.0.7/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 anls_star-0.0.7/LICENSE
+-rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 anls_star-0.0.7/README.md
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 anls_star-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     8812 2020-02-02 00:00:00.000000 anls_star-0.0.7/PKG-INFO
```

### Comparing `anls_star-0.0.6/src/anls_star.py` & `anls_star-0.0.7/src/anls_star.py`

 * *Files 4% similar despite different names*

```diff
@@ -191,14 +191,23 @@
         if not isinstance(other, ANLSDict):
             return [0.0]
 
         nlss = []
         for k in self.tree.keys() | other.tree.keys():
             self_value = self.tree.get(k, ANLSNone())
             other_value = other.tree.get(k, ANLSNone())
+
+            is_hallucinated_none_key = (
+                k not in self.tree 
+                and k in other.tree 
+                and ANLSNone.check_if_none(other_value.obj)
+            )
+            if is_hallucinated_none_key:
+                continue
+
             nls_list = self_value.nls_list(other_value)
             nlss.extend(nls_list)
         return nlss
 
 
 class ANLSNone(ANLSTree):
     def __init__(self):
@@ -207,15 +216,19 @@
     def __len__(self):
         return 1
 
     def pairwise_len(self, other):
         return max(len(self), len(other))
 
     def nls_list(self, other):
-        return [1.0 if other.obj in (None, {}, [], "") else 0.0]
+        return [1.0 if self.check_if_none(other.obj) else 0.0]
+
+    @classmethod
+    def check_if_none(cls, value):
+        return isinstance(value, ANLSNone) or value in (None, {}, [], "")
 
 
 class ANLSLeaf(ANLSTree):
     def __init__(self, obj):
         if not isinstance(obj, (str, float, int, bool)):
             raise ValueError(f"Leaf must be a primitive type, got {type(obj)}")
         self.obj = obj
```

### Comparing `anls_star-0.0.6/tests/test_anls_star.py` & `anls_star-0.0.7/tests/test_anls_star.py`

 * *Files 1% similar despite different names*

```diff
@@ -555,8 +555,22 @@
 
 
 def test_paper_unanswerable_no_answer():
     gt = "Yesterday"
     answer = None
     anls = anls_score(gt, answer)
 
+    assert anls == approx(0.0)
+
+
+def test_answer_dict_with_additional_nones_is_ignored():
+    gt = { }
+    answer = {
+        "string": "", 
+        "dict": {}, 
+        "list": [], 
+        "none": None, 
+        "bool": False,
+    }
+
+    anls = anls_score(gt, answer)
     assert anls == approx(0.0)
```

### Comparing `anls_star-0.0.6/.gitignore` & `anls_star-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `anls_star-0.0.6/LICENSE` & `anls_star-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `anls_star-0.0.6/README.md` & `anls_star-0.0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -41,37 +41,37 @@
 
 ## Benchmarks
 
 The following table shows the ANLS* score for the different models and prompt methods on different datasets. Note that we evaluate the models and prompt methods on 100 samples for single page datasets and 20 samples for multi page datasets in order to reduce the execution time and costs. Note that the provided validation set is used for the report.
 
 
 <!-- Use the following page to convert to latex for the paper https://tableconvert.com/markdown-to-latex -->
-| Dataset           | Method          | gpt-3.5-turbo-16k | gpt-4-turbo | gpt-4-vision | gemini-pro | mistral-large  | claude-3  |
-| ----------------- | --------------- | ----------------- | ----------- | ------------ | ---------- | -------------- | --------- |
-| DocVQA            | Simple          | 0.586             | 0.607       | 0.759        | 0.586      | 0.445          | 0.768     |
-|                   | Latin Prompting | 0.659             | 0.699       | -            | 0.676      | 0.447          | 0.762     |
-|                   | SFT (Ours)      | 0.809             | 0.790       | -            | 0.741      | 0.648          | **0.831** |
-| MPDocVQA          | Simple          | 0.517             | 0.635       | 0.708        | 0.603      | 0.364          | 0.636     |
-|                   | Latin Prompting | 0.499             | 0.739       | -            | 0.502      | 0.335          | 0.438     |
-|                   | SFT (Ours)      | 0.734             | **0.781**   | -            | 0.616      | 0.476          | 0.575     |
-| Kleister Charity  | Simple          | 0.490             | 0.743       | 0.751        | 0.583      | 0.652          | **0.800** |
-|                   | Latin Prompting | 0.442             | 0.735       | -            | 0.478      | 0.576          | 0.787     |
-|                   | SFT (Ours)      | 0.476             | 0.763       | -            | 0.633      | 0.657          | 0.786     |
-| Kleister NDA      | Simple          | 0.343             | 0.695       | 0.664        | 0.623      | 0.637          | 0.673     |
-|                   | Latin Prompting | 0.434             | **0.705**   | -            | 0.599      | 0.624          | 0.67      |
-|                   | SFT (Ours)      | 0.355             | 0.703       | -            | 0.552      | 0.641          | 0.677     |
-| SROIE             | Simple          | 0.874             | 0.835       | 0.834        | 0.263      | 0.855          | 0.933     |
-|                   | Latin Prompting | 0.849             | 0.851       | -            | 0.371      | 0.863          | 0.926     |
-|                   | SFT (Ours)      | 0.893             | 0.873       | -            | 0.288      | 0.905          | **0.949** |
-| VRDU AD Buy       | Simple          | 0.402             | 0.553       | 0.640        | 0.510      | 0.386          | 0.577     |
-|                   | Latin Prompting | 0.389             | 0.586       | -            | 0.556      | 0.435          | 0.608     |
-|                   | SFT (Ours)      | 0.661             | **0.770**   | -            | 0.685      | 0.594          | 0.633     |
-| VRDU Registration | Simple          | 0.659             | 0.676       | 0.665        | 0.699      | 0.579          | 0.685     |
-|                   | Latin Prompting | 0.693             | 0.673       | -            | 0.740      | 0.587          | 0.715     |
-|                   | SFT (Ours)      | **0.723**         | 0.711       | -            | 0.720      | 0.639          | 0.705     |
+| Dataset           | Method          | gpt-3.5-turbo-16k | gpt-4-turbo | gpt-4-vision | gemini-v1.0-pro | gemini-v1.5-pro | mistral-large  | claude-3  |
+| ----------------- | --------------- | ----------------- | ----------- | ------------ | --------------- | --------------- | -------------- | --------- |
+| DocVQA            | Simple          | 0.576             | 0.607       | 0.759        | 0.586           | 0.647           | 0.445          | 0.768     |
+|                   | Latin Prompting | 0.62              | 0.699       | -            | 0.676           | 0.668           | 0.447          | 0.762     |
+|                   | SFT (Ours)      | 0.768             | 0.790       | -            | 0.741           | 0.737           | 0.648          | **0.831** |
+| MPDocVQA          | Simple          | 0.507             | 0.635       | 0.708        | 0.603           | 0.627           | 0.364          | 0.636     |
+|                   | Latin Prompting | 0.489             | 0.739       | -            | 0.502           | 0.726           | 0.335          | 0.438     |
+|                   | SFT (Ours)      | 0.724             | 0.781       | -            | 0.616           | **0.794**       | 0.476          | 0.575     |
+| Kleister Charity  | Simple          | 0.527             | 0.743       | 0.751        | 0.583           | 0.764           | 0.652          | **0.800** |
+|                   | Latin Prompting | 0.477             | 0.735       | -            | 0.478           | 0.763           | 0.576          | 0.787     |
+|                   | SFT (Ours)      | 0.534             | 0.763       | -            | 0.633           | 0.779           | 0.657          | 0.786     |
+| Kleister NDA      | Simple          | 0.361             | 0.695       | 0.664        | 0.623           | 0.722           | 0.637          | 0.673     |
+|                   | Latin Prompting | 0.412             | 0.705       | -            | 0.599           | 0.707           | 0.624          | 0.67      |
+|                   | SFT (Ours)      | 0.315             | 0.703       | -            | 0.552           | **0.715**       | 0.641          | 0.677     |
+| SROIE             | Simple          | 0.509             | 0.835       | 0.834        | 0.263           | 0.594           | 0.855          | 0.933     |
+|                   | Latin Prompting | 0.723             | 0.851       | -            | 0.371           | 0.623           | 0.863          | 0.926     |
+|                   | SFT (Ours)      | 0.792             | 0.873       | -            | 0.288           | 0.623           | 0.905          | **0.949** |
+| VRDU AD Buy       | Simple          | 0.414             | 0.553       | 0.640        | 0.510           | 0.645           | 0.386          | 0.577     |
+|                   | Latin Prompting | 0.424             | 0.586       | -            | 0.556           | 0.686           | 0.435          | 0.608     |
+|                   | SFT (Ours)      | 0.676             | **0.770**   | -            | 0.685           | 0.765           | 0.594          | 0.633     |
+| VRDU Registration | Simple          | 0.586             | 0.676       | 0.665        | 0.699           | 0.730           | 0.579          | 0.685     |
+|                   | Latin Prompting | 0.606             | 0.673       | -            | 0.740           | 0.749           | 0.587          | 0.715     |
+|                   | SFT (Ours)      | 0.637             | 0.711       | -            | 0.720           | **0.780**       | 0.639          | 0.705     |
 
 
 ### How To Execute
 1. Install all dependencies via `pip install -r requirements_dev.txt`
 2. Setup the keys
  - OpenAI: Ensure that your OpenAI API key is set as environment variable `OPENAI_API_KEY`. 
  - Gemini: Ensure that your VertexAI setup is correct in case you wanna benchmark gemini-pro too.
@@ -80,21 +80,22 @@
 3. Download all datasets - the download link is provided when executing the benchmark script for the first time. Please note that the `datasets` folder should be on the same level as the repository folder.
 4. Execute the corresponding benchmark script. For example:
 
 ```bash
     python3 src/benchmark_doc_vqa.py "gpt-3.5-turbo-16k" "simple"
 ```
 
-The following models are benchmarked:
+The following model versions are benchmarked:
 - `gpt-3.5-turbo-16k`       (Version `gpt-3.5-turbo-16k-0613` )
 - `gpt-4-turbo`             (Version `gpt-4-1106-preview`)
-- `gemini-pro`              (Version 1.0)
+- `gemini-v1.0-pro`         (Version `gemini-1.0-pro`)
 - `mistral-large`           (Version 03/2024)
 - `claude-3`                (Version `claude-3-opus-20240229`)
-- `gpt-4-vision-preview`    (Version `gpt-4-1106-vision-preview	`)
+- `gpt-4-vision`            (Version `gpt-4-1106-vision-preview	`)
+- `gemini-v1.5-pro`         (Version `gemini-1.5-pro-preview-0409`)
 
 The following prompt methods are supported:
 - `simple` - Simple text concatenation after OCR with GooleOCR
 - `latin` - Method as introduced by [Wang et al.](https://arxiv.org/abs/2306.00526)
 - `sft` - DeepOpinion internal only
 - `vision` - If images should directly be used. Requires a model with vision capabilities e.g. gpt-4-vision
```

#### html2text {}

```diff
@@ -29,50 +29,53 @@
 extracting the date and total value from an invoice. Missing keys as well as
 hallucinated keys are penalized. ## Benchmarks The following table shows the
 ANLS* score for the different models and prompt methods on different datasets.
 Note that we evaluate the models and prompt methods on 100 samples for single
 page datasets and 20 samples for multi page datasets in order to reduce the
 execution time and costs. Note that the provided validation set is used for the
 report. | Dataset | Method | gpt-3.5-turbo-16k | gpt-4-turbo | gpt-4-vision |
-gemini-pro | mistral-large | claude-3 | | ----------------- | --------------- |
------------------ | ----------- | ------------ | ---------- | -------------- |
---------- | | DocVQA | Simple | 0.586 | 0.607 | 0.759 | 0.586 | 0.445 | 0.768 |
-| | Latin Prompting | 0.659 | 0.699 | - | 0.676 | 0.447 | 0.762 | | | SFT
-(Ours) | 0.809 | 0.790 | - | 0.741 | 0.648 | **0.831** | | MPDocVQA | Simple |
-0.517 | 0.635 | 0.708 | 0.603 | 0.364 | 0.636 | | | Latin Prompting | 0.499 |
-0.739 | - | 0.502 | 0.335 | 0.438 | | | SFT (Ours) | 0.734 | **0.781** | - |
-0.616 | 0.476 | 0.575 | | Kleister Charity | Simple | 0.490 | 0.743 | 0.751 |
-0.583 | 0.652 | **0.800** | | | Latin Prompting | 0.442 | 0.735 | - | 0.478 |
-0.576 | 0.787 | | | SFT (Ours) | 0.476 | 0.763 | - | 0.633 | 0.657 | 0.786 | |
-Kleister NDA | Simple | 0.343 | 0.695 | 0.664 | 0.623 | 0.637 | 0.673 | | |
-Latin Prompting | 0.434 | **0.705** | - | 0.599 | 0.624 | 0.67 | | | SFT (Ours)
-| 0.355 | 0.703 | - | 0.552 | 0.641 | 0.677 | | SROIE | Simple | 0.874 | 0.835
-| 0.834 | 0.263 | 0.855 | 0.933 | | | Latin Prompting | 0.849 | 0.851 | - |
-0.371 | 0.863 | 0.926 | | | SFT (Ours) | 0.893 | 0.873 | - | 0.288 | 0.905 |
-**0.949** | | VRDU AD Buy | Simple | 0.402 | 0.553 | 0.640 | 0.510 | 0.386 |
-0.577 | | | Latin Prompting | 0.389 | 0.586 | - | 0.556 | 0.435 | 0.608 | | |
-SFT (Ours) | 0.661 | **0.770** | - | 0.685 | 0.594 | 0.633 | | VRDU
-Registration | Simple | 0.659 | 0.676 | 0.665 | 0.699 | 0.579 | 0.685 | | |
-Latin Prompting | 0.693 | 0.673 | - | 0.740 | 0.587 | 0.715 | | | SFT (Ours) |
-**0.723** | 0.711 | - | 0.720 | 0.639 | 0.705 | ### How To Execute 1. Install
-all dependencies via `pip install -r requirements_dev.txt` 2. Setup the keys -
-OpenAI: Ensure that your OpenAI API key is set as environment variable
-`OPENAI_API_KEY`. - Gemini: Ensure that your VertexAI setup is correct in case
-you wanna benchmark gemini-pro too. - Mistral: Setup the `MISTRAL_API_KEY` env
-variable as well as `MISTRAL_ENDPOINT` (Azure) - Anthropic: Setup the
-`ANTHROPIC_API_KEY` env variable 3. Download all datasets - the download link
-is provided when executing the benchmark script for the first time. Please note
-that the `datasets` folder should be on the same level as the repository
-folder. 4. Execute the corresponding benchmark script. For example: ```bash
-python3 src/benchmark_doc_vqa.py "gpt-3.5-turbo-16k" "simple" ``` The following
-models are benchmarked: - `gpt-3.5-turbo-16k` (Version `gpt-3.5-turbo-16k-0613`
-) - `gpt-4-turbo` (Version `gpt-4-1106-preview`) - `gemini-pro` (Version 1.0) -
-`mistral-large` (Version 03/2024) - `claude-3` (Version `claude-3-opus-
-20240229`) - `gpt-4-vision-preview` (Version `gpt-4-1106-vision-preview `) The
-following prompt methods are supported: - `simple` - Simple text concatenation
-after OCR with GooleOCR - `latin` - Method as introduced by [Wang et al.]
-(https://arxiv.org/abs/2306.00526) - `sft` - DeepOpinion internal only -
-`vision` - If images should directly be used. Requires a model with vision
-capabilities e.g. gpt-4-vision 5. The final ANLS* is shown on the console. ##
-How to Execute all Unit Tests To run all unit tests simply execute `pytest` ##
-Packaging See https://packaging.python.org/en/latest/tutorials/packaging-
-projects/
+gemini-v1.0-pro | gemini-v1.5-pro | mistral-large | claude-3 | | --------------
+--- | --------------- | ----------------- | ----------- | ------------ | ------
+--------- | --------------- | -------------- | --------- | | DocVQA | Simple |
+0.576 | 0.607 | 0.759 | 0.586 | 0.647 | 0.445 | 0.768 | | | Latin Prompting |
+0.62 | 0.699 | - | 0.676 | 0.668 | 0.447 | 0.762 | | | SFT (Ours) | 0.768 |
+0.790 | - | 0.741 | 0.737 | 0.648 | **0.831** | | MPDocVQA | Simple | 0.507 |
+0.635 | 0.708 | 0.603 | 0.627 | 0.364 | 0.636 | | | Latin Prompting | 0.489 |
+0.739 | - | 0.502 | 0.726 | 0.335 | 0.438 | | | SFT (Ours) | 0.724 | 0.781 | -
+| 0.616 | **0.794** | 0.476 | 0.575 | | Kleister Charity | Simple | 0.527 |
+0.743 | 0.751 | 0.583 | 0.764 | 0.652 | **0.800** | | | Latin Prompting | 0.477
+| 0.735 | - | 0.478 | 0.763 | 0.576 | 0.787 | | | SFT (Ours) | 0.534 | 0.763 |
+- | 0.633 | 0.779 | 0.657 | 0.786 | | Kleister NDA | Simple | 0.361 | 0.695 |
+0.664 | 0.623 | 0.722 | 0.637 | 0.673 | | | Latin Prompting | 0.412 | 0.705 | -
+| 0.599 | 0.707 | 0.624 | 0.67 | | | SFT (Ours) | 0.315 | 0.703 | - | 0.552 |
+**0.715** | 0.641 | 0.677 | | SROIE | Simple | 0.509 | 0.835 | 0.834 | 0.263 |
+0.594 | 0.855 | 0.933 | | | Latin Prompting | 0.723 | 0.851 | - | 0.371 | 0.623
+| 0.863 | 0.926 | | | SFT (Ours) | 0.792 | 0.873 | - | 0.288 | 0.623 | 0.905 |
+**0.949** | | VRDU AD Buy | Simple | 0.414 | 0.553 | 0.640 | 0.510 | 0.645 |
+0.386 | 0.577 | | | Latin Prompting | 0.424 | 0.586 | - | 0.556 | 0.686 | 0.435
+| 0.608 | | | SFT (Ours) | 0.676 | **0.770** | - | 0.685 | 0.765 | 0.594 |
+0.633 | | VRDU Registration | Simple | 0.586 | 0.676 | 0.665 | 0.699 | 0.730 |
+0.579 | 0.685 | | | Latin Prompting | 0.606 | 0.673 | - | 0.740 | 0.749 | 0.587
+| 0.715 | | | SFT (Ours) | 0.637 | 0.711 | - | 0.720 | **0.780** | 0.639 |
+0.705 | ### How To Execute 1. Install all dependencies via `pip install -
+r requirements_dev.txt` 2. Setup the keys - OpenAI: Ensure that your OpenAI API
+key is set as environment variable `OPENAI_API_KEY`. - Gemini: Ensure that your
+VertexAI setup is correct in case you wanna benchmark gemini-pro too. -
+Mistral: Setup the `MISTRAL_API_KEY` env variable as well as `MISTRAL_ENDPOINT`
+(Azure) - Anthropic: Setup the `ANTHROPIC_API_KEY` env variable 3. Download all
+datasets - the download link is provided when executing the benchmark script
+for the first time. Please note that the `datasets` folder should be on the
+same level as the repository folder. 4. Execute the corresponding benchmark
+script. For example: ```bash python3 src/benchmark_doc_vqa.py "gpt-3.5-turbo-
+16k" "simple" ``` The following model versions are benchmarked: - `gpt-3.5-
+turbo-16k` (Version `gpt-3.5-turbo-16k-0613` ) - `gpt-4-turbo` (Version `gpt-4-
+1106-preview`) - `gemini-v1.0-pro` (Version `gemini-1.0-pro`) - `mistral-large`
+(Version 03/2024) - `claude-3` (Version `claude-3-opus-20240229`) - `gpt-4-
+vision` (Version `gpt-4-1106-vision-preview `) - `gemini-v1.5-pro` (Version
+`gemini-1.5-pro-preview-0409`) The following prompt methods are supported: -
+`simple` - Simple text concatenation after OCR with GooleOCR - `latin` - Method
+as introduced by [Wang et al.](https://arxiv.org/abs/2306.00526) - `sft` -
+DeepOpinion internal only - `vision` - If images should directly be used.
+Requires a model with vision capabilities e.g. gpt-4-vision 5. The final ANLS*
+is shown on the console. ## How to Execute all Unit Tests To run all unit tests
+simply execute `pytest` ## Packaging See https://packaging.python.org/en/
+latest/tutorials/packaging-projects/
```

### Comparing `anls_star-0.0.6/pyproject.toml` & `anls_star-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "anls_star"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="David Peer", email="david.peer@deepopinion.ai" },
 ]
 description = "A universal metric for Generative Large Language Models (GLLMs)"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `anls_star-0.0.6/PKG-INFO` & `anls_star-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: anls_star
-Version: 0.0.6
+Version: 0.0.7
 Summary: A universal metric for Generative Large Language Models (GLLMs)
 Project-URL: Repository, https://github.com/deepopinion/anls_star_metric
 Project-URL: Issues, https://github.com/deepopinion/anls_star_metric/issues
 Project-URL: Paper, https://arxiv.org/abs/2402.03848
 Project-URL: DeepOpinion, https://deepopinion.ai
 Author-email: David Peer <david.peer@deepopinion.ai>
 License-File: LICENSE
@@ -58,37 +58,37 @@
 
 ## Benchmarks
 
 The following table shows the ANLS* score for the different models and prompt methods on different datasets. Note that we evaluate the models and prompt methods on 100 samples for single page datasets and 20 samples for multi page datasets in order to reduce the execution time and costs. Note that the provided validation set is used for the report.
 
 
 <!-- Use the following page to convert to latex for the paper https://tableconvert.com/markdown-to-latex -->
-| Dataset           | Method          | gpt-3.5-turbo-16k | gpt-4-turbo | gpt-4-vision | gemini-pro | mistral-large  | claude-3  |
-| ----------------- | --------------- | ----------------- | ----------- | ------------ | ---------- | -------------- | --------- |
-| DocVQA            | Simple          | 0.586             | 0.607       | 0.759        | 0.586      | 0.445          | 0.768     |
-|                   | Latin Prompting | 0.659             | 0.699       | -            | 0.676      | 0.447          | 0.762     |
-|                   | SFT (Ours)      | 0.809             | 0.790       | -            | 0.741      | 0.648          | **0.831** |
-| MPDocVQA          | Simple          | 0.517             | 0.635       | 0.708        | 0.603      | 0.364          | 0.636     |
-|                   | Latin Prompting | 0.499             | 0.739       | -            | 0.502      | 0.335          | 0.438     |
-|                   | SFT (Ours)      | 0.734             | **0.781**   | -            | 0.616      | 0.476          | 0.575     |
-| Kleister Charity  | Simple          | 0.490             | 0.743       | 0.751        | 0.583      | 0.652          | **0.800** |
-|                   | Latin Prompting | 0.442             | 0.735       | -            | 0.478      | 0.576          | 0.787     |
-|                   | SFT (Ours)      | 0.476             | 0.763       | -            | 0.633      | 0.657          | 0.786     |
-| Kleister NDA      | Simple          | 0.343             | 0.695       | 0.664        | 0.623      | 0.637          | 0.673     |
-|                   | Latin Prompting | 0.434             | **0.705**   | -            | 0.599      | 0.624          | 0.67      |
-|                   | SFT (Ours)      | 0.355             | 0.703       | -            | 0.552      | 0.641          | 0.677     |
-| SROIE             | Simple          | 0.874             | 0.835       | 0.834        | 0.263      | 0.855          | 0.933     |
-|                   | Latin Prompting | 0.849             | 0.851       | -            | 0.371      | 0.863          | 0.926     |
-|                   | SFT (Ours)      | 0.893             | 0.873       | -            | 0.288      | 0.905          | **0.949** |
-| VRDU AD Buy       | Simple          | 0.402             | 0.553       | 0.640        | 0.510      | 0.386          | 0.577     |
-|                   | Latin Prompting | 0.389             | 0.586       | -            | 0.556      | 0.435          | 0.608     |
-|                   | SFT (Ours)      | 0.661             | **0.770**   | -            | 0.685      | 0.594          | 0.633     |
-| VRDU Registration | Simple          | 0.659             | 0.676       | 0.665        | 0.699      | 0.579          | 0.685     |
-|                   | Latin Prompting | 0.693             | 0.673       | -            | 0.740      | 0.587          | 0.715     |
-|                   | SFT (Ours)      | **0.723**         | 0.711       | -            | 0.720      | 0.639          | 0.705     |
+| Dataset           | Method          | gpt-3.5-turbo-16k | gpt-4-turbo | gpt-4-vision | gemini-v1.0-pro | gemini-v1.5-pro | mistral-large  | claude-3  |
+| ----------------- | --------------- | ----------------- | ----------- | ------------ | --------------- | --------------- | -------------- | --------- |
+| DocVQA            | Simple          | 0.576             | 0.607       | 0.759        | 0.586           | 0.647           | 0.445          | 0.768     |
+|                   | Latin Prompting | 0.62              | 0.699       | -            | 0.676           | 0.668           | 0.447          | 0.762     |
+|                   | SFT (Ours)      | 0.768             | 0.790       | -            | 0.741           | 0.737           | 0.648          | **0.831** |
+| MPDocVQA          | Simple          | 0.507             | 0.635       | 0.708        | 0.603           | 0.627           | 0.364          | 0.636     |
+|                   | Latin Prompting | 0.489             | 0.739       | -            | 0.502           | 0.726           | 0.335          | 0.438     |
+|                   | SFT (Ours)      | 0.724             | 0.781       | -            | 0.616           | **0.794**       | 0.476          | 0.575     |
+| Kleister Charity  | Simple          | 0.527             | 0.743       | 0.751        | 0.583           | 0.764           | 0.652          | **0.800** |
+|                   | Latin Prompting | 0.477             | 0.735       | -            | 0.478           | 0.763           | 0.576          | 0.787     |
+|                   | SFT (Ours)      | 0.534             | 0.763       | -            | 0.633           | 0.779           | 0.657          | 0.786     |
+| Kleister NDA      | Simple          | 0.361             | 0.695       | 0.664        | 0.623           | 0.722           | 0.637          | 0.673     |
+|                   | Latin Prompting | 0.412             | 0.705       | -            | 0.599           | 0.707           | 0.624          | 0.67      |
+|                   | SFT (Ours)      | 0.315             | 0.703       | -            | 0.552           | **0.715**       | 0.641          | 0.677     |
+| SROIE             | Simple          | 0.509             | 0.835       | 0.834        | 0.263           | 0.594           | 0.855          | 0.933     |
+|                   | Latin Prompting | 0.723             | 0.851       | -            | 0.371           | 0.623           | 0.863          | 0.926     |
+|                   | SFT (Ours)      | 0.792             | 0.873       | -            | 0.288           | 0.623           | 0.905          | **0.949** |
+| VRDU AD Buy       | Simple          | 0.414             | 0.553       | 0.640        | 0.510           | 0.645           | 0.386          | 0.577     |
+|                   | Latin Prompting | 0.424             | 0.586       | -            | 0.556           | 0.686           | 0.435          | 0.608     |
+|                   | SFT (Ours)      | 0.676             | **0.770**   | -            | 0.685           | 0.765           | 0.594          | 0.633     |
+| VRDU Registration | Simple          | 0.586             | 0.676       | 0.665        | 0.699           | 0.730           | 0.579          | 0.685     |
+|                   | Latin Prompting | 0.606             | 0.673       | -            | 0.740           | 0.749           | 0.587          | 0.715     |
+|                   | SFT (Ours)      | 0.637             | 0.711       | -            | 0.720           | **0.780**       | 0.639          | 0.705     |
 
 
 ### How To Execute
 1. Install all dependencies via `pip install -r requirements_dev.txt`
 2. Setup the keys
  - OpenAI: Ensure that your OpenAI API key is set as environment variable `OPENAI_API_KEY`. 
  - Gemini: Ensure that your VertexAI setup is correct in case you wanna benchmark gemini-pro too.
@@ -97,21 +97,22 @@
 3. Download all datasets - the download link is provided when executing the benchmark script for the first time. Please note that the `datasets` folder should be on the same level as the repository folder.
 4. Execute the corresponding benchmark script. For example:
 
 ```bash
     python3 src/benchmark_doc_vqa.py "gpt-3.5-turbo-16k" "simple"
 ```
 
-The following models are benchmarked:
+The following model versions are benchmarked:
 - `gpt-3.5-turbo-16k`       (Version `gpt-3.5-turbo-16k-0613` )
 - `gpt-4-turbo`             (Version `gpt-4-1106-preview`)
-- `gemini-pro`              (Version 1.0)
+- `gemini-v1.0-pro`         (Version `gemini-1.0-pro`)
 - `mistral-large`           (Version 03/2024)
 - `claude-3`                (Version `claude-3-opus-20240229`)
-- `gpt-4-vision-preview`    (Version `gpt-4-1106-vision-preview	`)
+- `gpt-4-vision`            (Version `gpt-4-1106-vision-preview	`)
+- `gemini-v1.5-pro`         (Version `gemini-1.5-pro-preview-0409`)
 
 The following prompt methods are supported:
 - `simple` - Simple text concatenation after OCR with GooleOCR
 - `latin` - Method as introduced by [Wang et al.](https://arxiv.org/abs/2306.00526)
 - `sft` - DeepOpinion internal only
 - `vision` - If images should directly be used. Requires a model with vision capabilities e.g. gpt-4-vision
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: anls_star Version: 0.0.6 Summary: A universal
+Metadata-Version: 2.3 Name: anls_star Version: 0.0.7 Summary: A universal
 metric for Generative Large Language Models (GLLMs) Project-URL: Repository,
 https://github.com/deepopinion/anls_star_metric Project-URL: Issues, https://
 github.com/deepopinion/anls_star_metric/issues Project-URL: Paper, https://
 arxiv.org/abs/2402.03848 Project-URL: DeepOpinion, https://deepopinion.ai
 Author-email: David Peer
 deepopinion.ai> License-File: LICENSE Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
@@ -38,50 +38,53 @@
 extracting the date and total value from an invoice. Missing keys as well as
 hallucinated keys are penalized. ## Benchmarks The following table shows the
 ANLS* score for the different models and prompt methods on different datasets.
 Note that we evaluate the models and prompt methods on 100 samples for single
 page datasets and 20 samples for multi page datasets in order to reduce the
 execution time and costs. Note that the provided validation set is used for the
 report. | Dataset | Method | gpt-3.5-turbo-16k | gpt-4-turbo | gpt-4-vision |
-gemini-pro | mistral-large | claude-3 | | ----------------- | --------------- |
------------------ | ----------- | ------------ | ---------- | -------------- |
---------- | | DocVQA | Simple | 0.586 | 0.607 | 0.759 | 0.586 | 0.445 | 0.768 |
-| | Latin Prompting | 0.659 | 0.699 | - | 0.676 | 0.447 | 0.762 | | | SFT
-(Ours) | 0.809 | 0.790 | - | 0.741 | 0.648 | **0.831** | | MPDocVQA | Simple |
-0.517 | 0.635 | 0.708 | 0.603 | 0.364 | 0.636 | | | Latin Prompting | 0.499 |
-0.739 | - | 0.502 | 0.335 | 0.438 | | | SFT (Ours) | 0.734 | **0.781** | - |
-0.616 | 0.476 | 0.575 | | Kleister Charity | Simple | 0.490 | 0.743 | 0.751 |
-0.583 | 0.652 | **0.800** | | | Latin Prompting | 0.442 | 0.735 | - | 0.478 |
-0.576 | 0.787 | | | SFT (Ours) | 0.476 | 0.763 | - | 0.633 | 0.657 | 0.786 | |
-Kleister NDA | Simple | 0.343 | 0.695 | 0.664 | 0.623 | 0.637 | 0.673 | | |
-Latin Prompting | 0.434 | **0.705** | - | 0.599 | 0.624 | 0.67 | | | SFT (Ours)
-| 0.355 | 0.703 | - | 0.552 | 0.641 | 0.677 | | SROIE | Simple | 0.874 | 0.835
-| 0.834 | 0.263 | 0.855 | 0.933 | | | Latin Prompting | 0.849 | 0.851 | - |
-0.371 | 0.863 | 0.926 | | | SFT (Ours) | 0.893 | 0.873 | - | 0.288 | 0.905 |
-**0.949** | | VRDU AD Buy | Simple | 0.402 | 0.553 | 0.640 | 0.510 | 0.386 |
-0.577 | | | Latin Prompting | 0.389 | 0.586 | - | 0.556 | 0.435 | 0.608 | | |
-SFT (Ours) | 0.661 | **0.770** | - | 0.685 | 0.594 | 0.633 | | VRDU
-Registration | Simple | 0.659 | 0.676 | 0.665 | 0.699 | 0.579 | 0.685 | | |
-Latin Prompting | 0.693 | 0.673 | - | 0.740 | 0.587 | 0.715 | | | SFT (Ours) |
-**0.723** | 0.711 | - | 0.720 | 0.639 | 0.705 | ### How To Execute 1. Install
-all dependencies via `pip install -r requirements_dev.txt` 2. Setup the keys -
-OpenAI: Ensure that your OpenAI API key is set as environment variable
-`OPENAI_API_KEY`. - Gemini: Ensure that your VertexAI setup is correct in case
-you wanna benchmark gemini-pro too. - Mistral: Setup the `MISTRAL_API_KEY` env
-variable as well as `MISTRAL_ENDPOINT` (Azure) - Anthropic: Setup the
-`ANTHROPIC_API_KEY` env variable 3. Download all datasets - the download link
-is provided when executing the benchmark script for the first time. Please note
-that the `datasets` folder should be on the same level as the repository
-folder. 4. Execute the corresponding benchmark script. For example: ```bash
-python3 src/benchmark_doc_vqa.py "gpt-3.5-turbo-16k" "simple" ``` The following
-models are benchmarked: - `gpt-3.5-turbo-16k` (Version `gpt-3.5-turbo-16k-0613`
-) - `gpt-4-turbo` (Version `gpt-4-1106-preview`) - `gemini-pro` (Version 1.0) -
-`mistral-large` (Version 03/2024) - `claude-3` (Version `claude-3-opus-
-20240229`) - `gpt-4-vision-preview` (Version `gpt-4-1106-vision-preview `) The
-following prompt methods are supported: - `simple` - Simple text concatenation
-after OCR with GooleOCR - `latin` - Method as introduced by [Wang et al.]
-(https://arxiv.org/abs/2306.00526) - `sft` - DeepOpinion internal only -
-`vision` - If images should directly be used. Requires a model with vision
-capabilities e.g. gpt-4-vision 5. The final ANLS* is shown on the console. ##
-How to Execute all Unit Tests To run all unit tests simply execute `pytest` ##
-Packaging See https://packaging.python.org/en/latest/tutorials/packaging-
-projects/
+gemini-v1.0-pro | gemini-v1.5-pro | mistral-large | claude-3 | | --------------
+--- | --------------- | ----------------- | ----------- | ------------ | ------
+--------- | --------------- | -------------- | --------- | | DocVQA | Simple |
+0.576 | 0.607 | 0.759 | 0.586 | 0.647 | 0.445 | 0.768 | | | Latin Prompting |
+0.62 | 0.699 | - | 0.676 | 0.668 | 0.447 | 0.762 | | | SFT (Ours) | 0.768 |
+0.790 | - | 0.741 | 0.737 | 0.648 | **0.831** | | MPDocVQA | Simple | 0.507 |
+0.635 | 0.708 | 0.603 | 0.627 | 0.364 | 0.636 | | | Latin Prompting | 0.489 |
+0.739 | - | 0.502 | 0.726 | 0.335 | 0.438 | | | SFT (Ours) | 0.724 | 0.781 | -
+| 0.616 | **0.794** | 0.476 | 0.575 | | Kleister Charity | Simple | 0.527 |
+0.743 | 0.751 | 0.583 | 0.764 | 0.652 | **0.800** | | | Latin Prompting | 0.477
+| 0.735 | - | 0.478 | 0.763 | 0.576 | 0.787 | | | SFT (Ours) | 0.534 | 0.763 |
+- | 0.633 | 0.779 | 0.657 | 0.786 | | Kleister NDA | Simple | 0.361 | 0.695 |
+0.664 | 0.623 | 0.722 | 0.637 | 0.673 | | | Latin Prompting | 0.412 | 0.705 | -
+| 0.599 | 0.707 | 0.624 | 0.67 | | | SFT (Ours) | 0.315 | 0.703 | - | 0.552 |
+**0.715** | 0.641 | 0.677 | | SROIE | Simple | 0.509 | 0.835 | 0.834 | 0.263 |
+0.594 | 0.855 | 0.933 | | | Latin Prompting | 0.723 | 0.851 | - | 0.371 | 0.623
+| 0.863 | 0.926 | | | SFT (Ours) | 0.792 | 0.873 | - | 0.288 | 0.623 | 0.905 |
+**0.949** | | VRDU AD Buy | Simple | 0.414 | 0.553 | 0.640 | 0.510 | 0.645 |
+0.386 | 0.577 | | | Latin Prompting | 0.424 | 0.586 | - | 0.556 | 0.686 | 0.435
+| 0.608 | | | SFT (Ours) | 0.676 | **0.770** | - | 0.685 | 0.765 | 0.594 |
+0.633 | | VRDU Registration | Simple | 0.586 | 0.676 | 0.665 | 0.699 | 0.730 |
+0.579 | 0.685 | | | Latin Prompting | 0.606 | 0.673 | - | 0.740 | 0.749 | 0.587
+| 0.715 | | | SFT (Ours) | 0.637 | 0.711 | - | 0.720 | **0.780** | 0.639 |
+0.705 | ### How To Execute 1. Install all dependencies via `pip install -
+r requirements_dev.txt` 2. Setup the keys - OpenAI: Ensure that your OpenAI API
+key is set as environment variable `OPENAI_API_KEY`. - Gemini: Ensure that your
+VertexAI setup is correct in case you wanna benchmark gemini-pro too. -
+Mistral: Setup the `MISTRAL_API_KEY` env variable as well as `MISTRAL_ENDPOINT`
+(Azure) - Anthropic: Setup the `ANTHROPIC_API_KEY` env variable 3. Download all
+datasets - the download link is provided when executing the benchmark script
+for the first time. Please note that the `datasets` folder should be on the
+same level as the repository folder. 4. Execute the corresponding benchmark
+script. For example: ```bash python3 src/benchmark_doc_vqa.py "gpt-3.5-turbo-
+16k" "simple" ``` The following model versions are benchmarked: - `gpt-3.5-
+turbo-16k` (Version `gpt-3.5-turbo-16k-0613` ) - `gpt-4-turbo` (Version `gpt-4-
+1106-preview`) - `gemini-v1.0-pro` (Version `gemini-1.0-pro`) - `mistral-large`
+(Version 03/2024) - `claude-3` (Version `claude-3-opus-20240229`) - `gpt-4-
+vision` (Version `gpt-4-1106-vision-preview `) - `gemini-v1.5-pro` (Version
+`gemini-1.5-pro-preview-0409`) The following prompt methods are supported: -
+`simple` - Simple text concatenation after OCR with GooleOCR - `latin` - Method
+as introduced by [Wang et al.](https://arxiv.org/abs/2306.00526) - `sft` -
+DeepOpinion internal only - `vision` - If images should directly be used.
+Requires a model with vision capabilities e.g. gpt-4-vision 5. The final ANLS*
+is shown on the console. ## How to Execute all Unit Tests To run all unit tests
+simply execute `pytest` ## Packaging See https://packaging.python.org/en/
+latest/tutorials/packaging-projects/
```

