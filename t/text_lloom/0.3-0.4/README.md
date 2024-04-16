# Comparing `tmp/text_lloom-0.3.tar.gz` & `tmp/text_lloom-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text_lloom-0.3.tar", max compression
+gzip compressed data, was "text_lloom-0.4.tar", max compression
```

## Comparing `text_lloom-0.3.tar` & `text_lloom-0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       39 2024-02-02 13:27:07.282735 text_lloom-0.3/README.md
--rw-r--r--   0        0        0      540 2024-04-05 10:02:22.600059 text_lloom-0.3/pyproject.toml
--rw-r--r--   0        0        0     2002 2024-04-05 09:56:53.952744 text_lloom-0.3/src/text_lloom/__init__.py
--rw-r--r--   0        0        0      738 2024-02-28 09:09:42.891236 text_lloom-0.3/src/text_lloom/concept.py
--rw-r--r--   0        0        0    55984 2024-04-05 06:51:48.640862 text_lloom-0.3/src/text_lloom/concept_induction.py
--rw-r--r--   0        0        0    12290 2024-03-08 09:30:26.443347 text_lloom-0.3/src/text_lloom/llm.py
--rw-r--r--   0        0        0     7784 2024-02-28 01:05:49.223109 text_lloom-0.3/src/text_lloom/prompts.py
--rw-r--r--   0        0        0     1263 2024-04-05 10:01:18.147604 text_lloom-0.3/src/text_lloom/static/index.css
--rw-r--r--   0        0        0   455935 2024-04-05 10:01:18.147575 text_lloom-0.3/src/text_lloom/static/index.js
--rw-r--r--   0        0        0      707 2024-04-05 10:01:15.229780 text_lloom-0.3/src/text_lloom/static/index_select.css
--rw-r--r--   0        0        0    11241 2024-04-05 10:01:15.229781 text_lloom-0.3/src/text_lloom/static/index_select.js
--rw-r--r--   0        0        0    22880 2024-04-05 07:09:01.158345 text_lloom-0.3/src/text_lloom/workbench.py
--rw-r--r--   0        0        0      972 1970-01-01 00:00:00.000000 text_lloom-0.3/PKG-INFO
+-rw-r--r--   0        0        0       39 2024-02-02 13:27:07.282735 text_lloom-0.4/README.md
+-rw-r--r--   0        0        0      552 2024-04-16 09:41:54.316560 text_lloom-0.4/pyproject.toml
+-rw-r--r--   0        0        0     2019 2024-04-16 07:43:43.539102 text_lloom-0.4/src/text_lloom/__init__.py
+-rw-r--r--   0        0        0      738 2024-02-28 09:09:42.891236 text_lloom-0.4/src/text_lloom/concept.py
+-rw-r--r--   0        0        0    57291 2024-04-15 00:44:18.318856 text_lloom-0.4/src/text_lloom/concept_induction.py
+-rw-r--r--   0        0        0    12290 2024-03-08 09:30:26.443347 text_lloom-0.4/src/text_lloom/llm.py
+-rw-r--r--   0        0        0     8416 2024-04-13 23:28:08.093682 text_lloom-0.4/src/text_lloom/prompts.py
+-rw-r--r--   0        0        0     1263 2024-04-15 01:19:42.816858 text_lloom-0.4/src/text_lloom/static/index.css
+-rw-r--r--   0        0        0   455935 2024-04-15 01:19:42.816860 text_lloom-0.4/src/text_lloom/static/index.js
+-rw-r--r--   0        0        0      707 2024-04-15 01:19:38.799003 text_lloom-0.4/src/text_lloom/static/index_select.css
+-rw-r--r--   0        0        0    11241 2024-04-15 01:19:38.799013 text_lloom-0.4/src/text_lloom/static/index_select.js
+-rw-r--r--   0        0        0    24594 2024-04-12 08:12:52.865258 text_lloom-0.4/src/text_lloom/workbench.py
+-rw-r--r--   0        0        0      984 1970-01-01 00:00:00.000000 text_lloom-0.4/PKG-INFO
```

### Comparing `text_lloom-0.3/pyproject.toml` & `text_lloom-0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "text_lloom"
-version = "0.3"
+version = "0.4"
 description = "Concept Induction to analyze unstructured text"
 authors = ["Michelle Lam <mlam4@cs.stanford.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 bertopic = "^0.16.0"
 hdbscan = "^0.8.33"
 openai = "0.28"
-asyncio = "^3.4.3"
 google-generativeai = "^0.3.2"
 langchain = "0.0.271"
-anywidget = "^0.9.0"
+anywidget = "^0.9.7"
 pathos = "^0.3.2"
-ipywidgets = "^7.1.1"
+ipywidgets = "^8.1.2"
 tiktoken = "^0.6.0"
 nltk = "^3.8.1"
+jupyterlab_widgets = "^3.0.10"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `text_lloom-0.3/src/text_lloom/__init__.py` & `text_lloom-0.4/src/text_lloom/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import importlib.metadata
 import pathlib
 
 import anywidget
 import traitlets
 
 import nltk
-nltk.download('punkt')
+nltk.download('punkt', quiet=True)
 
 try:
-    __version__ = importlib.metadata.version("lloom")
+    __version__ = importlib.metadata.version("text_lloom")
 except importlib.metadata.PackageNotFoundError:
     __version__ = "unknown"
 
 _DEV = False # switch to False for production
 
 if _DEV:
   # from `npx vite`
```

### Comparing `text_lloom-0.3/src/text_lloom/concept.py` & `text_lloom-0.4/src/text_lloom/concept.py`

 * *Files identical despite different names*

### Comparing `text_lloom-0.3/src/text_lloom/concept_induction.py` & `text_lloom-0.4/src/text_lloom/concept_induction.py`

 * *Files 1% similar despite different names*

```diff
@@ -403,102 +403,109 @@
     for m in merged:
         orig_concepts = m["original_themes"]
         print(f"[{orig_concepts}] --> {m['merged_theme_name']}: {m['merged_theme_prompt']}")
 
 # Input: concept_df (columns: doc_id, text, concept_id, concept_name, concept_prompt)
 # Parameters: n_concepts
 # Output: 
-# - concepts: dict (concept_id -> concept dict)
+# - concepts: dict (concept_id -> Concept)
 # - concept_df: DataFrame (columns: doc_id, text, concept_id, concept_name, concept_prompt)
-async def review(concepts, concept_df, concept_col, concept_col_prefix, model_name, debug=True, sess=None):
+async def review(concepts, concept_df, concept_col_prefix, model_name, debug=True, sess=None):
     # Model is asked to review the provided set of concepts
-    concepts_out, concept_df_out, removed = await review_remove(concepts, concept_df, concept_col, concept_col_prefix, model_name=model_name, sess=sess)
-    concepts_out, concept_df_out, merged = await review_merge(concepts_out, concept_df_out, concept_col, concept_col_prefix, model_name=model_name, sess=sess)
+    concepts_out, concept_df_out, removed = await review_remove(concepts, concept_df, concept_col_prefix, model_name=model_name, sess=sess)
+    concepts_out, concept_df_out, merged = await review_merge(concepts_out, concept_df_out, concept_col_prefix, model_name=model_name, sess=sess)
 
     if debug:
         print(f"Removed ({len(removed)}):\n{removed}")
         print(f"Merged ({len(merged)}):")
         pretty_print_merge_results(merged)
 
     # TODO: ask model to filter to the "best" N concepts
+    if sess is not None:
+        sess.concepts = concepts_out
     return concepts_out, concept_df_out
 
 
 # Model removes concepts that are too specific or too general
 # Input: concept_df (columns: doc_id, text, concept_id, concept_name, concept_prompt)
 # Parameters: n_concepts
 # Output: 
-# - concepts: dict (concept_id -> concept dict)
+# - concepts: dict (concept_id -> Concept)
 # - concept_df: DataFrame (columns: doc_id, text, concept_id, concept_name, concept_prompt)
-async def review_remove(concepts, concept_df, concept_col, concept_col_prefix, model_name, sess):
+async def review_remove(concepts, concept_df, concept_col_prefix, model_name, sess):
     concepts = concepts.copy()  # Make a copy of the concepts dict to avoid modifying the original
     start = time.time()
     concept_name_col = f"{concept_col_prefix}_name"
 
-    concepts_list = concept_df[concept_col].tolist()
-    concepts_list = [f"- {c}" for c in concepts_list]
+    concepts_list = [f"- Name: {c.name}, Prompt: {c.prompt}" for c in concepts.values()]
     concepts_list_str = "\n".join(concepts_list)
     arg_dicts = [{
         "themes": concepts_list_str,
     }]
 
     # Run prompts
     prompt_template = review_remove_prompt
     res_text, res_full = await multi_query_gpt_wrapper(prompt_template, arg_dicts, model_name)
 
     # Process results
     res = res_text[0]
     concepts_to_remove = json_load(res, top_level_key="remove")
 
-    concept_df_out = concept_df.copy()
-    concept_df_out = concept_df_out[~concept_df_out[concept_name_col].isin(concepts_to_remove)]
+    if concept_df is not None:
+        concept_df_out = concept_df.copy()
+        concept_df_out = concept_df_out[~concept_df_out[concept_name_col].isin(concepts_to_remove)]  # Remove from concept_df
+    else:
+        concept_df_out = None
     c_ids_to_remove = []
     for c_id, c in concepts.items():
-        if c['name'] in concepts_to_remove:
+        if c.name in concepts_to_remove:
             c_ids_to_remove.append(c_id)
     for c_id in c_ids_to_remove:
-        concepts.pop(c_id, None)
+        concepts.pop(c_id, None)  # Remove from concepts dict
 
     save_progress(sess, concept_df_out, step_name="review_remove", start=start, res=res_full, model_name=model_name)
     return concepts, concept_df_out, concepts_to_remove
 
 def get_concept_by_name(concepts, concept_name):
     for c_id, c in concepts.items():
-        if c['name'] == concept_name:
+        if c.name == concept_name:
             return c_id, c
     return None, None
 
 # Model merges concepts that are similar or overlapping
 # Input: concept_df (columns: doc_id, text, concept_id, concept_name, concept_prompt)
 # Parameters: n_concepts
 # Output: 
-# - concepts: dict (concept_id -> concept dict)
+# - concepts: dict (concept_id -> Concept)
 # - concept_df: DataFrame (columns: doc_id, text, concept_id, concept_name, concept_prompt)
-async def review_merge(concepts, concept_df, concept_col, concept_col_prefix, model_name, sess):
+async def review_merge(concepts, concept_df, concept_col_prefix, model_name, sess):
     concepts = concepts.copy()  # Make a copy of the concepts dict to avoid modifying the original
     start = time.time()
+    concept_col = concept_col_prefix
     concept_name_col = f"{concept_col_prefix}_name"
     concept_prompt_col = f"{concept_col_prefix}_prompt"
 
-    concepts_list = concept_df[concept_col].tolist()
-    concepts_list = [f"- {c}" for c in concepts_list]
+    concepts_list = [f"- Name: {c.name}, Prompt: {c.prompt}" for c in concepts.values()]
     concepts_list_str = "\n".join(concepts_list)
     arg_dicts = [{
         "themes": concepts_list_str,
     }]
 
     # Run prompts
     prompt_template = review_merge_prompt
     res_text, res_full = await multi_query_gpt_wrapper(prompt_template, arg_dicts, model_name)
 
     # Process results
     res = res_text[0]
     concepts_to_merge = json_load(res, top_level_key="merge")
 
-    concept_df_out = concept_df.copy()
+    if concept_df is not None:
+        concept_df_out = concept_df.copy()
+    else:
+        concept_df_out = None
 
     # Remove all original concepts
     # Add new merged concepts
     concepts_to_remove = []
     c_ids_to_remove = []
     for merge_result in concepts_to_merge:
         orig_concepts = merge_result["original_themes"]
@@ -515,38 +522,64 @@
 
         # Get original concept IDs and example IDs
         merged_example_ids = []
         for orig_concept in orig_concepts:
             c_id, c = get_concept_by_name(concepts, orig_concept)
             if c is not None:
                 c_ids_to_remove.append(c_id)
-                merged_example_ids.extend(c["example_ids"])
+                merged_example_ids.extend(c.example_ids)
         
         # Create new merged concept in dict
         new_concept_name = merge_result["merged_theme_name"]
         new_concept_prompt = merge_result["merged_theme_prompt"]
         new_concept_id = str(uuid.uuid4())
-        concepts[new_concept_id] = {
-            "name": new_concept_name,
-            "prompt": new_concept_prompt,
-            "example_ids": merged_example_ids,
-        }
+        concepts[new_concept_id] = Concept(name=new_concept_name, prompt=new_concept_prompt, example_ids=merged_example_ids, active=False)
 
         # Replace prior df row with new merged concept
-        for orig_concept in orig_concepts:
-            concept_df_out.loc[concept_df_out[concept_name_col]==orig_concept, concept_name_col] = new_concept_name
-            concept_df_out.loc[concept_df_out[concept_name_col]==orig_concept, concept_prompt_col] = new_concept_prompt
-            concept_df_out.loc[concept_df_out[concept_name_col]==orig_concept, concept_col] = f"{new_concept_name}: {new_concept_prompt}"
+        if concept_df is not None:
+            for orig_concept in orig_concepts:  # Merge in concept_df
+                concept_df_out.loc[concept_df_out[concept_name_col]==orig_concept, concept_name_col] = new_concept_name
+                concept_df_out.loc[concept_df_out[concept_name_col]==orig_concept, concept_prompt_col] = new_concept_prompt
+                concept_df_out.loc[concept_df_out[concept_name_col]==orig_concept, concept_col] = f"{new_concept_name}: {new_concept_prompt}"
         
     for c_id in c_ids_to_remove:
-        concepts.pop(c_id, None)
+        concepts.pop(c_id, None) # Remove from concepts dict
 
     save_progress(sess, concept_df_out, step_name="review_merge", start=start, res=res_full, model_name=model_name)
     return concepts, concept_df_out, concepts_to_merge
 
+# Model selects the best concepts up to `max_concepts`
+# Input: concepts (concept_id -> Concept)
+# Parameters: max_concepts, model_name
+# Output: selected_concepts: dict (concept_id -> Concept)
+async def review_select(concepts, max_concepts, model_name):
+    concepts_list = [f"- Name: {c.name}, Prompt: {c.prompt}" for c in concepts.values()]
+    concepts_list_str = "\n".join(concepts_list)
+    arg_dicts = [{
+        "themes": concepts_list_str,
+        "max_concepts": max_concepts,
+    }]
+
+    # Run prompts
+    prompt_template = review_select_prompt
+    res_text, res_full = await multi_query_gpt_wrapper(prompt_template, arg_dicts, model_name)
+
+    # Process results
+    res = res_text[0]
+    selected_concept_names = json_load(res, top_level_key="selected")
+
+    selected_concepts = []
+    for c_id, c in concepts.items():
+        if c.name in selected_concept_names:
+            selected_concepts.append(c_id)
+
+    if len(selected_concepts) > max_concepts:
+        selected_concepts = selected_concepts[:max_concepts]
+    return selected_concepts
+
 
 def get_ex_batch_args(df, text_col, doc_id_col, concept_name, concept_prompt):
     ex = get_examples_dict(df, text_col, doc_id_col)
     examples_json = dict_to_json(ex)
     arg_dict = {
         "examples_json": examples_json,
         "pattern_name": concept_name,
```

### Comparing `text_lloom-0.3/src/text_lloom/llm.py` & `text_lloom-0.4/src/text_lloom/llm.py`

 * *Files identical despite different names*

### Comparing `text_lloom-0.3/src/text_lloom/prompts.py` & `text_lloom-0.4/src/text_lloom/prompts.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 """
 
 # Synthesize ========================
 synthesize_prompt = """
 I have this set of bullet point summaries of text examples:
 {examples}
 
-Please write a summary of {n_concepts_phrase} for these examples. {seed_phrase} For each high-level pattern, write a 2-4 word NAME for the pattern and an associated 1-sentence ChatGPT PROMPT that could take in a new text example and determine whether the relevant pattern applies. Also include 1-2 example_ids for items that BEST exemplify the pattern. Please respond ONLY with a valid JSON in the following format:
+Please write a summary of {n_concepts_phrase} for these examples {seed_phrase} For each high-level pattern, write a 2-4 word NAME for the pattern and an associated 1-sentence ChatGPT PROMPT that could take in a new text example and determine whether the relevant pattern applies. Also include 1-2 example_ids for items that BEST exemplify the pattern. Please respond ONLY with a valid JSON in the following format:
 {{
     "patterns": [ 
         {{"name": "<PATTERN_NAME_1>", "prompt": "<PATTERN_PROMPT_1>", "example_ids": ["<EXAMPLE_ID_1>", "<EXAMPLE_ID_2>"]}},
         {{"name": "<PATTERN_NAME_2>", "prompt": "<PATTERN_PROMPT_2>", "example_ids": ["<EXAMPLE_ID_1>", "<EXAMPLE_ID_2>"]}},
     ]
 }}
 """
@@ -73,14 +73,29 @@
             "merged_theme_name": "<THEME_NAME_CD>",
             "merged_theme_prompt": "<THEME_PROMPT_CD>",
         }}
     ]
 }}
 """
 
+review_select_prompt = """
+I have this set of themes generated from text examples:
+{themes}
+
+Please select AT MOST {max_concepts} themes to include in the final set of themes. These themes should be the highest quality themes in the set: (1) NOT too generic or vague (should not describe most examples), (2) NOT too specific (should not only describe a small set of examples), and (3) NOT overlapping with other selected themes (they should capture a range of different patterns).
+Please respond ONLY with a valid JSON in the following format:
+
+{{
+    "selected": [ 
+        "<THEME_NAME_1>",
+        "<THEME_NAME_2>",
+    ]
+}}
+"""
+
 # Score ========================
 score_no_highlight_prompt = """
 CONTEXT: 
     I have the following text examples in a JSON:
     {examples_json}
 
     I also have a pattern named {pattern_name} with the following PROMPT:
```

### Comparing `text_lloom-0.3/src/text_lloom/static/index.css` & `text_lloom-0.4/src/text_lloom/static/index.css`

 * *Files identical despite different names*

### Comparing `text_lloom-0.3/src/text_lloom/static/index.js` & `text_lloom-0.4/src/text_lloom/static/index.js`

 * *Files identical despite different names*

### Comparing `text_lloom-0.3/src/text_lloom/static/index_select.css` & `text_lloom-0.4/src/text_lloom/static/index_select.css`

 * *Files identical despite different names*

### Comparing `text_lloom-0.3/src/text_lloom/static/index_select.js` & `text_lloom-0.4/src/text_lloom/static/index_select.js`

 * *Files identical despite different names*

### Comparing `text_lloom-0.3/src/text_lloom/workbench.py` & `text_lloom-0.4/src/text_lloom/workbench.py`

 * *Files 4% similar despite different names*

```diff
@@ -144,17 +144,22 @@
 
         # Synthesize: create n_concepts for each of the est_n_clusters
         n_bullets_per_cluster = (params["summ_n_bullets"] * len(self.in_df)) / est_n_clusters
         synth_prompt_tokens = get_token_estimate(synthesize_prompt, self.synth_model_name)
         synth_in_tokens = np.sum([(synth_prompt_tokens + (est_bullet_tokens * n_bullets_per_cluster)) for _ in range(est_n_clusters)])
         synth_out_tokens = params["synth_n_concepts"] * est_n_clusters * est_concept_tokens
         est_cost["synthesize"] = calc_cost_by_tokens(self.synth_model_name, synth_in_tokens, synth_out_tokens)
+
+        # Review: pass all names and prompts
+        rev_in_tokens = synth_out_tokens * 2  # For both review_remove and review_merge
+        rev_out_tokens = rev_in_tokens * 0.5  # Conservatively assume half size
+        est_cost["review"] = calc_cost_by_tokens(self.synth_model_name, rev_in_tokens, rev_out_tokens)
         
         total_cost = np.sum([c[0] + c[1] for c in est_cost.values()])
-        print(f"Estimated cost: {np.round(total_cost, 2)}")
+        print(f"\n\nEstimated cost: {np.round(total_cost, 2)}")
         print("**Please note that this is only an approximate cost estimate**")
 
         if verbose:
             print(f"\nEstimated cost breakdown:")
             for step_name, cost in est_cost.items():
                 total_cost = np.sum(cost)
                 print(f"\t{step_name}: {total_cost:0.4f}")
@@ -177,15 +182,15 @@
         n_batches = math.ceil(len(self.in_df) / batch_size)
         all_doc_tokens = np.sum([get_token_estimate(doc, self.score_model_name) for doc in self.df_to_score[self.doc_col].tolist()])  # Tokens to encode all documents
         score_in_tokens = all_doc_tokens + (n_batches * (score_prompt_tokens + est_concept_tokens))
         score_out_tokens = est_score_json_tokens * n_concepts * len(self.in_df)
         est_cost = calc_cost_by_tokens(self.score_model_name, score_in_tokens, score_out_tokens)
 
         total_cost = np.sum(est_cost)
-        print(f"Scoring {n_concepts} concepts for {len(self.in_df)} documents")
+        print(f"\n\nScoring {n_concepts} concepts for {len(self.in_df)} documents")
         print(f"Estimated cost: {np.round(total_cost, 2)}")
         print("**Please note that this is only an approximate cost estimate**")
 
         if verbose:
             print(f"\nEstimated cost breakdown:")
             for step_name, cost in zip(["Input", "Output"], est_cost):
                 print(f"\t{step_name}: {cost:0.4f}")
@@ -214,43 +219,43 @@
         params = {
             "filter_n_quotes": filter_n_quotes,
             "summ_n_bullets": summ_n_bullets,
             "synth_n_concepts": synth_n_concepts,
         }
         return params
     
-    def summary(self, show_detail=True):
+    def summary(self, verbose=True):
         # Time
         total_time = np.sum(list(self.time.values()))
         print(f"Total time: {total_time:0.2f} sec ({(total_time/60):0.2f} min)")
-        if show_detail:
+        if verbose:
             for step_name, time in self.time.items():
                 print(f"\t{step_name}: {time:0.2f} sec")
 
         # Cost
         total_cost = np.sum(list(self.cost.values()))
         print(f"\n\nTotal cost: {total_cost:0.2f}")
-        if show_detail:
+        if verbose:
             for step_name, cost in self.cost.items():
-                print(f"\t{step_name}: {cost:0.2f}")
+                print(f"\t{step_name}: {cost:0.3f}")
 
         # Tokens
         in_tokens = np.sum(self.tokens["in_tokens"])
         out_tokens = np.sum(self.tokens["out_tokens"])
         total_tokens =  in_tokens + out_tokens
         print(f"\n\nTokens: total={total_tokens}, in={in_tokens}, out={out_tokens}")
 
     def show_selected(self):
         active_concepts = self.__get_active_concepts()
-        print(f"Active concepts (n={len(active_concepts)}):")
+        print(f"\n\nActive concepts (n={len(active_concepts)}):")
         for c_id, c in active_concepts.items():
             print(f"- {c.name}: {c.prompt}")
 
     # HELPER FUNCTIONS ================================
-    async def gen(self, seed=None, params=None, n_synth=1, debug=True):
+    async def gen(self, seed=None, params=None, n_synth=1, auto_review=True, debug=True):
         if params is None:
             params = self.auto_suggest_parameters(debug=debug)
             if debug:
                 print(f"Auto-suggested parameters: {params}")
         
         # Run cost estimation
         self.estimate_gen_cost(params)
@@ -322,14 +327,18 @@
                 concept_col_prefix=concept_col_prefix,
                 n_concepts=synth_n_concepts,
                 pattern_phrase="unique topic",
                 seed=seed,
                 sess=self,
             )
 
+            # Review current concepts (remove low-quality, merge similar)
+            if auto_review:
+                _, df_concepts = await review(concepts=self.concepts, concept_df=df_concepts, concept_col_prefix=concept_col_prefix, model_name=self.synth_model_name, sess=self)
+
             self.concept_history[i] = self.concepts
             if debug:
                 # Print results
                 print(f"synthesize {i + 1}: (n={len(self.concepts)})")
                 for k, c in self.concepts.items():
                     print(f'- Concept {k}:\n\t{c.name}\n\t- Prompt: {c.prompt}')
             
@@ -352,14 +361,28 @@
     
     def select(self):
         concepts_json = self.__concepts_to_json()
         w = get_select_widget(concepts_json)
         self.select_widget = w
         return w
 
+    async def select_auto(self, max_concepts):
+        # Select the best concepts up to max_concepts
+        selected_concepts = await review_select(self.concepts, max_concepts, self.synth_model_name)
+
+        # Handle if selection failed
+        if len(selected_concepts) == 0:
+            concept_ids = list(self.concepts.keys())
+            selected_concepts = random.sample(concept_ids, max_concepts)
+
+        # Activate only the selected concepts
+        for c_id in selected_concepts:
+            if c_id in self.concepts:
+                self.concepts[c_id].active = True
+
     def __get_active_concepts(self):
         # Update based on widget
         if self.select_widget is not None:
             widget_data = json.loads(self.select_widget.data)
             for c_id, c in self.concepts.items():
                 widget_active = widget_data[c_id]["active"]
                 c.active = widget_active
@@ -516,14 +539,32 @@
             del c["example_ids"]
             return c
         active_concepts = self.__get_active_concepts()
         concepts_dict = [format_dict(c.to_dict()) for c_id, c in active_concepts.items()]
         concepts_json = json.dumps(concepts_dict)
         return concepts_json
 
+    async def gen_auto(
+        self,
+        max_concepts=8,
+        seed=None, params=None, n_synth=1,
+        debug=True
+    ):
+        # Runs gen(), select(), and score() all at once
+        # Run generation
+        await self.gen(seed=seed, params=params, n_synth=n_synth, auto_review=True, debug=debug)
+
+        # Select the best concepts
+        await self.select_auto(max_concepts=max_concepts)
+        self.show_selected()
+
+        # Run scoring
+        score_df = await self.score()
+        return score_df
+
     async def add(self, name, prompt, ex_ids=[], get_highlights=True):
         # Add concept
         c = Concept(name=name, prompt=prompt, example_ids=ex_ids, active=True)
         self.concepts[c.id] = c
 
         # Update widget
         self.select_widget = self.select()
```

### Comparing `text_lloom-0.3/PKG-INFO` & `text_lloom-0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: text_lloom
-Version: 0.3
+Version: 0.4
 Summary: Concept Induction to analyze unstructured text
 Author: Michelle Lam
 Author-email: mlam4@cs.stanford.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: anywidget (>=0.9.0,<0.10.0)
-Requires-Dist: asyncio (>=3.4.3,<4.0.0)
+Requires-Dist: anywidget (>=0.9.7,<0.10.0)
 Requires-Dist: bertopic (>=0.16.0,<0.17.0)
 Requires-Dist: google-generativeai (>=0.3.2,<0.4.0)
 Requires-Dist: hdbscan (>=0.8.33,<0.9.0)
-Requires-Dist: ipywidgets (>=7.1.1,<8.0.0)
+Requires-Dist: ipywidgets (>=8.1.2,<9.0.0)
+Requires-Dist: jupyterlab_widgets (>=3.0.10,<4.0.0)
 Requires-Dist: langchain (==0.0.271)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: openai (==0.28)
 Requires-Dist: pathos (>=0.3.2,<0.4.0)
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
 Description-Content-Type: text/markdown
```

