# Comparing `tmp/step_kit-0.2.0.tar.gz` & `tmp/step_kit-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "step_kit-0.2.0.tar", max compression
+gzip compressed data, was "step_kit-0.2.1.tar", max compression
```

## Comparing `step_kit-0.2.0.tar` & `step_kit-0.2.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0    11357 2024-04-14 11:50:19.928369 step_kit-0.2.0/LICENSE
--rw-r--r--   0        0        0     1468 2024-04-14 13:51:36.476519 step_kit-0.2.0/README.md
--rw-r--r--   0        0        0     1737 2024-04-15 06:04:29.593771 step_kit-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      138 2024-04-14 11:50:19.933514 step_kit-0.2.0/step/__init__.py
--rw-r--r--   0        0        0        0 2024-04-14 11:50:19.933611 step_kit-0.2.0/step/functionality/__init__.py
--rw-r--r--   0        0        0     4705 2024-04-15 05:59:16.479789 step_kit-0.2.0/step/functionality/base.py
--rw-r--r--   0        0        0        0 2024-04-14 11:50:19.933908 step_kit-0.2.0/step/functionality/comps/__init__.py
--rw-r--r--   0        0        0    18935 2024-04-14 12:22:44.709635 step_kit-0.2.0/step/functionality/comps/model_ops.py
--rw-r--r--   0        0        0    28629 2024-04-15 05:59:16.480343 step_kit-0.2.0/step/functionality/comps/trainer.py
--rw-r--r--   0        0        0    41400 2024-04-15 05:59:16.480907 step_kit-0.2.0/step/functionality/cross_funcmodel.py
--rw-r--r--   0        0        0    18452 2024-04-15 05:59:16.481504 step_kit-0.2.0/step/functionality/sc_funcmodel.py
--rw-r--r--   0        0        0    19728 2024-04-15 05:59:16.482134 step_kit-0.2.0/step/functionality/st_funcmodel.py
--rw-r--r--   0        0        0    19342 2024-04-14 18:41:45.322451 step_kit-0.2.0/step/integration.py
--rw-r--r--   0        0        0     1151 2024-04-15 05:59:16.482328 step_kit-0.2.0/step/manager/__init__.py
--rw-r--r--   0        0        0     2765 2024-04-15 05:59:16.482478 step_kit-0.2.0/step/manager/save.py
--rwxr-xr-x   0        0        0        0 2024-04-14 11:50:19.935557 step_kit-0.2.0/step/models/__init__.py
--rw-r--r--   0        0        0     1846 2024-04-14 11:50:19.935690 step_kit-0.2.0/step/models/clust.py
--rw-r--r--   0        0        0    14675 2024-04-14 12:22:44.709167 step_kit-0.2.0/step/models/deconv.py
--rw-r--r--   0        0        0    15639 2024-04-14 11:50:19.936096 step_kit-0.2.0/step/models/distributions.py
--rw-r--r--   0        0        0    12710 2024-04-15 05:59:16.483032 step_kit-0.2.0/step/models/extension.py
--rw-r--r--   0        0        0    17561 2024-04-15 05:59:16.483633 step_kit-0.2.0/step/models/geneformer.py
--rw-r--r--   0        0        0     2307 2024-04-14 12:22:44.709047 step_kit-0.2.0/step/models/knn_map.py
--rw-r--r--   0        0        0      678 2024-04-14 11:50:19.936662 step_kit-0.2.0/step/models/nnls.py
--rw-r--r--   0        0        0        0 2024-04-14 11:50:19.936752 step_kit-0.2.0/step/modules/__init__.py
--rw-r--r--   0        0        0     6811 2024-04-15 05:59:16.484198 step_kit-0.2.0/step/modules/decoder.py
--rw-r--r--   0        0        0     1848 2024-04-14 11:50:19.937054 step_kit-0.2.0/step/modules/gnn.py
--rw-r--r--   0        0        0     3090 2024-04-14 11:50:19.937162 step_kit-0.2.0/step/modules/transformer.py
--rw-r--r--   0        0        0    10647 2024-04-15 05:59:16.484405 step_kit-0.2.0/step/scmodel.py
--rw-r--r--   0        0        0    16647 2024-04-14 18:42:53.390640 step_kit-0.2.0/step/stmodel.py
--rw-r--r--   0        0        0        0 2024-04-14 11:50:19.937755 step_kit-0.2.0/step/utils/__init__.py
--rw-r--r--   0        0        0    41256 2024-04-14 12:22:44.708893 step_kit-0.2.0/step/utils/dataset.py
--rw-r--r--   0        0        0     2853 2024-04-15 05:59:16.484585 step_kit-0.2.0/step/utils/gbolt.py
--rw-r--r--   0        0        0     1454 2024-04-14 11:50:19.938205 step_kit-0.2.0/step/utils/metrics.py
--rwxr-xr-x   0        0        0    14616 2024-04-15 06:00:06.656239 step_kit-0.2.0/step/utils/misc.py
--rw-r--r--   0        0        0    16000 2024-04-15 05:59:16.485008 step_kit-0.2.0/step/utils/plotting.py
--rw-r--r--   0        0        0        0 2024-04-14 11:50:19.938694 step_kit-0.2.0/step/utils/synthetics/__init__.py
--rw-r--r--   0        0        0    22670 2024-04-14 12:22:44.700905 step_kit-0.2.0/step/utils/synthetics/pseudo_st.py
--rw-r--r--   0        0        0     3187 1970-01-01 00:00:00.000000 step_kit-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-14 11:50:19.928369 step_kit-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3016 2024-04-16 07:34:41.018373 step_kit-0.2.1/README.md
+-rw-r--r--   0        0        0     1737 2024-04-16 08:18:29.082467 step_kit-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      138 2024-04-14 11:50:19.933514 step_kit-0.2.1/step/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-14 11:50:19.933611 step_kit-0.2.1/step/functionality/__init__.py
+-rw-r--r--   0        0        0     4705 2024-04-15 05:59:16.479789 step_kit-0.2.1/step/functionality/base.py
+-rw-r--r--   0        0        0        0 2024-04-14 11:50:19.933908 step_kit-0.2.1/step/functionality/comps/__init__.py
+-rw-r--r--   0        0        0    18935 2024-04-14 12:22:44.709635 step_kit-0.2.1/step/functionality/comps/model_ops.py
+-rw-r--r--   0        0        0    28629 2024-04-15 05:59:16.480343 step_kit-0.2.1/step/functionality/comps/trainer.py
+-rw-r--r--   0        0        0    41985 2024-04-16 07:34:41.020583 step_kit-0.2.1/step/functionality/cross_funcmodel.py
+-rw-r--r--   0        0        0    18452 2024-04-15 05:59:16.481504 step_kit-0.2.1/step/functionality/sc_funcmodel.py
+-rw-r--r--   0        0        0    19728 2024-04-15 05:59:16.482134 step_kit-0.2.1/step/functionality/st_funcmodel.py
+-rw-r--r--   0        0        0    19342 2024-04-14 18:41:45.322451 step_kit-0.2.1/step/integration.py
+-rw-r--r--   0        0        0     1151 2024-04-15 05:59:16.482328 step_kit-0.2.1/step/manager/__init__.py
+-rw-r--r--   0        0        0     2765 2024-04-15 05:59:16.482478 step_kit-0.2.1/step/manager/save.py
+-rwxr-xr-x   0        0        0        0 2024-04-14 11:50:19.935557 step_kit-0.2.1/step/models/__init__.py
+-rw-r--r--   0        0        0     1846 2024-04-14 11:50:19.935690 step_kit-0.2.1/step/models/clust.py
+-rw-r--r--   0        0        0    14598 2024-04-16 07:34:41.021749 step_kit-0.2.1/step/models/deconv.py
+-rw-r--r--   0        0        0    15639 2024-04-14 11:50:19.936096 step_kit-0.2.1/step/models/distributions.py
+-rw-r--r--   0        0        0    12710 2024-04-15 05:59:16.483032 step_kit-0.2.1/step/models/extension.py
+-rw-r--r--   0        0        0    17561 2024-04-15 05:59:16.483633 step_kit-0.2.1/step/models/geneformer.py
+-rw-r--r--   0        0        0     2307 2024-04-14 12:22:44.709047 step_kit-0.2.1/step/models/knn_map.py
+-rw-r--r--   0        0        0      678 2024-04-14 11:50:19.936662 step_kit-0.2.1/step/models/nnls.py
+-rw-r--r--   0        0        0        0 2024-04-14 11:50:19.936752 step_kit-0.2.1/step/modules/__init__.py
+-rw-r--r--   0        0        0     6941 2024-04-16 07:34:41.022554 step_kit-0.2.1/step/modules/decoder.py
+-rw-r--r--   0        0        0     1848 2024-04-14 11:50:19.937054 step_kit-0.2.1/step/modules/gnn.py
+-rw-r--r--   0        0        0     3090 2024-04-14 11:50:19.937162 step_kit-0.2.1/step/modules/transformer.py
+-rw-r--r--   0        0        0    10647 2024-04-15 05:59:16.484405 step_kit-0.2.1/step/scmodel.py
+-rw-r--r--   0        0        0    16647 2024-04-14 18:42:53.390640 step_kit-0.2.1/step/stmodel.py
+-rw-r--r--   0        0        0        0 2024-04-14 11:50:19.937755 step_kit-0.2.1/step/utils/__init__.py
+-rw-r--r--   0        0        0    41256 2024-04-14 12:22:44.708893 step_kit-0.2.1/step/utils/dataset.py
+-rw-r--r--   0        0        0     2853 2024-04-15 05:59:16.484585 step_kit-0.2.1/step/utils/gbolt.py
+-rw-r--r--   0        0        0     1454 2024-04-14 11:50:19.938205 step_kit-0.2.1/step/utils/metrics.py
+-rwxr-xr-x   0        0        0    14616 2024-04-15 06:00:06.656239 step_kit-0.2.1/step/utils/misc.py
+-rw-r--r--   0        0        0    16000 2024-04-15 05:59:16.485008 step_kit-0.2.1/step/utils/plotting.py
+-rw-r--r--   0        0        0        0 2024-04-14 11:50:19.938694 step_kit-0.2.1/step/utils/synthetics/__init__.py
+-rw-r--r--   0        0        0    22670 2024-04-14 12:22:44.700905 step_kit-0.2.1/step/utils/synthetics/pseudo_st.py
+-rw-r--r--   0        0        0     4735 1970-01-01 00:00:00.000000 step_kit-0.2.1/PKG-INFO
```

### Comparing `step_kit-0.2.0/LICENSE` & `step_kit-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.0/pyproject.toml` & `step_kit-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "step-kit"
-version = "0.2.0"
+version = "0.2.1"
 description = "STEP, an acronym for Spatial Transcriptomics Embedding Procedure, is a deep learning-based tool for the analysis of single-cell RNA (scRNA-seq) and spatially resolved transcriptomics (SRT) data. STEP introduces a unified approach to process and analyze multiple samples of scRNA-seq data as well as align several sections of SRT data, disregarding location relationships. Furthermore, STEP conducts integrative analysis across different modalities like scRNA-seq and SRT."
 authors = ["SGGb0nd <lilounan1997@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [
     {include = "step"}
 ]
```

### Comparing `step_kit-0.2.0/step/functionality/base.py` & `step_kit-0.2.1/step/functionality/base.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.0/step/functionality/comps/model_ops.py` & `step_kit-0.2.1/step/functionality/comps/model_ops.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.0/step/functionality/comps/trainer.py` & `step_kit-0.2.1/step/functionality/comps/trainer.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.0/step/functionality/cross_funcmodel.py` & `step_kit-0.2.1/step/functionality/cross_funcmodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,14 +121,16 @@
         self,
         n_dec_layers=1,
         decoder_type="zinb",
         single_st=True,
         dec_norm="batch",
         use_st_decoder=False,
         st_batches=None,
+        activation: Literal['softmax', 'softplus'] = 'softplus',
+        use_l_scale=True,
     ):
         """
         Initialize the st specific decoder.
 
         Args:
             n_dec_layers (int): Number of hidden layers in the decoder.
             decoder_type (str): Type of decoder distribution.
@@ -137,29 +139,34 @@
             use_st_decoder (bool): Whether to use a separate st specific decoder.
 
         Returns:
             None
         """
 
         if use_st_decoder:
-            args: dict = self.model.decoder.args  # type:ignore
+            args: dict = dict(**self.model.decoder.args)  # type:ignore
             args["use_skip"] = False
             args["n_hidden_layers"] = n_dec_layers
             args["norm"] = dec_norm
             args["dist"] = decoder_type
+            args["activation"] = activation
+            args["use_l_scale"] = use_l_scale
+            args["num_batches"] = len(st_batches) if st_batches is not None else 1
             self.st_decoder = ProbDecoder(**args,)
             setattr(self, "st_decoder_type", decoder_type)
             setattr(self, "single_st", single_st)
             self.model.args["st_decoder"] = {  # type:ignore
                 "n_dec_layers": n_dec_layers,
                 "decoder_type": decoder_type,
                 "single_st": single_st,
                 "dec_norm": dec_norm,
                 "use_st_decoder": use_st_decoder,
                 "st_batches": st_batches,
+                "activation": activation,
+                "use_l_scale": use_l_scale,
             }
         else:
             self.st_decoder = self.model.decoder
             setattr(self, "st_decoder_type", self.model.decoder.args["dist"])
             setattr(self, "single_st", single_st)
         self._get_px_r = self.model.get_px_r
 
@@ -491,14 +498,15 @@
         n_glayers=2,
         dec_norm="batch",
         key_added: str = "X_smoothed",
         use_st_decoder=False,
         graph_batch_size=2,
         kl_cutoff=None,
         logging=False,
+        **kwargs,
     ):
         """Generates domains for the given dataset using the specified parameters.
 
         Args:
             adata (AnnData): The annotated data object.
             dataset (CrossDataset): The cross dataset object.
             decoder_type (str): The type of decoder to use. Default is 'zinb'.
@@ -549,14 +557,15 @@
         self._init_st_decoder(
             use_st_decoder=use_st_decoder,
             n_dec_layers=n_dec_layers,
             decoder_type=decoder_type,
             single_st=single_st,
             dec_norm=dec_norm,
             st_batches=st_batches,
+            **kwargs,
         )
 
         self.model.to(self.device)
         self.st_decoder.to(self.device)
         if use_st_decoder:
             self.optimizer = torch.optim.Adam(
                 self.st_decoder.parameters(), lr=lr
@@ -701,15 +710,15 @@
         single_st = dataset.num_st_batches == 1
         if not hasattr(self, "st_decoder"):
             self._init_st_decoder(
                 use_st_decoder=False,
                 single_st=single_st,
             )
 
-        _get_px_r, st_decoder = self._set_st_counts(adata, dataset, library_size, use_raw, batch_used)
+        _get_px_r, st_decoder, st_decoder_type = self._set_st_counts(adata, dataset, library_size, use_raw, batch_used)
 
         if cell_type_key is None:
             cell_type_key = dataset.class_key
 
         signatures, batch_used_code, celltypes = self._get_ct_sig(adata, dataset, cell_type_key, use_raw, batch_used)
 
         self._init_mixer(
@@ -758,14 +767,15 @@
             norm=False,
             colnames=celltypes,
             rownames=st_adata.obs_names,
         )
         dataset.switch_layer(dataset.layer_key)
         self._get_px_r = _get_px_r
         self.st_decoder = st_decoder
+        self.st_decoder_type = st_decoder_type
         self.model.to('cpu')
         self.st_decoder.to('cpu')
         self.mixer.to('cpu')
 
     def _make_collate_fn(self, batch_used_code, use_raw):
         if use_raw is False:
             return _collate_fn(batch_used_code)
@@ -822,22 +832,24 @@
                 dataset.set_rep(rep)
         assert rep is not None, "No representation found"
         return rep
 
     def _set_st_counts(self, adata, dataset, library_size, use_raw, batch_used):
         _get_px_r = self._get_px_r
         st_decoder = self.st_decoder
+        st_decoder_type = self.st_decoder_type
         if use_raw is False:
             logger.info("Using corrected counts for ST data")
             self.regress_out(adata, dataset, library_size=library_size, batch_used=batch_used)
             self.st_decoder = self.model.decoder
+            self.st_decoder_type = self.model.decoder_type
             dataset.switch_layer("corrected_counts")
         else:
             logger.info("Using raw counts for ST data")
-        return _get_px_r, st_decoder
+        return _get_px_r, st_decoder, st_decoder_type
 
     def nnls_deconv(
         self,
         adata: AnnData,
         dataset: CrossDataset,
         cell_type_key: Optional[str] = None,
         batch_used: Optional[str | int] = 0,
```

### Comparing `step_kit-0.2.0/step/functionality/sc_funcmodel.py` & `step_kit-0.2.1/step/functionality/sc_funcmodel.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.0/step/functionality/st_funcmodel.py` & `step_kit-0.2.1/step/functionality/st_funcmodel.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.0/step/integration.py` & `step_kit-0.2.1/step/integration.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.0/step/manager/__init__.py` & `step_kit-0.2.1/step/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.0/step/manager/save.py` & `step_kit-0.2.1/step/manager/save.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.0/step/models/clust.py` & `step_kit-0.2.1/step/models/clust.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.0/step/models/deconv.py` & `step_kit-0.2.1/step/models/deconv.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,14 +188,15 @@
         self.st_scale = nn.Sequential(
             nn.Linear(hidden_dim, 1),
         )
         self.ct_scale = nn.Parameter(torch.randn(1, self.n_celltypes))
 
         self.domain_wise = domain_wise
         self.hyperparams = kwargs
+        self.T = kwargs.get("T", math.sqrt(input_dim))
         self.args = dict(
             hidden_dim=hidden_dim,
             solver=solver,
             n_spots=n_spots,
             smoother=smoother,
             use_smoother=use_smoother,
             n_glayers=n_glayers,
@@ -354,18 +355,16 @@
             anchors (torch.Tensor): Tensor of shape (batch_size, num_anchors, embedding_dim) representing the anchors.
             indices (torch.Tensor): Tensor of shape (batch_size,) representing the indices of the positive anchors.
 
         Returns:
             torch.Tensor: The consistency loss.
 
         """
-        # top_n_anchors = F.normalize(top_n_anchors, dim=-1)
-        # anchors = F.normalize(anchors, dim=-1)
         logits = torch.einsum("bd,nd->bn", top_n_anchors, anchors)
-        logits = logits / math.sqrt(anchors.shape[-1])
+        logits = logits / self.T
         labels = indices
         loss = F.cross_entropy(logits, labels)
         return loss
 
     def p_hat(self, coef, logits):
         ct_scale = self.ct_scale
         return ct_scale.exp() * coef  # * self.st_scale(logits).exp()
```

### Comparing `step_kit-0.2.0/step/models/distributions.py` & `step_kit-0.2.1/step/models/distributions.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.0/step/models/extension.py` & `step_kit-0.2.1/step/models/extension.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.0/step/models/geneformer.py` & `step_kit-0.2.1/step/models/geneformer.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.0/step/models/knn_map.py` & `step_kit-0.2.1/step/models/knn_map.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.0/step/models/nnls.py` & `step_kit-0.2.1/step/models/nnls.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.0/step/modules/decoder.py` & `step_kit-0.2.1/step/modules/decoder.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,28 +101,31 @@
             hidden_dim = hidden_dim * (2 ** (n_hidden_layers - 1))
         self.px_scale_decoder = nn.Sequential(
             nn.Linear(hidden_dim, output_dim),
             _get_activation(activation, norm),
         )
         self.px_dropout_decoder = (
             nn.Linear(
-                hidden_dim, output_dim) if dist == "zinb" else lambda _: None
+                hidden_dim, output_dim) if dist == "zinb" else (lambda _: None)
         )
         self.px_r = nn.Parameter(torch.randn(num_batches, output_dim).squeeze(0))
 
         if num_batches > 1:
             self.get_px_r = lambda batch_label: self.px_r[batch_label]
         else:
             self.get_px_r = lambda _: self.px_r
 
-        if use_l_scale and num_batches > 1:
-            self.l_scale = nn.Parameter(torch.randn(num_batches, 1))
-            self.get_l_scale = lambda batch_label: 1 + F.sigmoid(
-                self.l_scale[batch_label]
-            )
+        if use_l_scale:
+            self.l_scale = nn.Parameter(torch.randn(num_batches, 1).squeeze(0))
+            if num_batches > 1:
+                self.get_l_scale = lambda batch_label: 1 + F.sigmoid(
+                    self.l_scale[batch_label]
+                )
+            else:
+                self.get_l_scale = (lambda _: 1 + F.sigmoid(self.l_scale))
         else:
             self.get_l_scale = lambda _: 1
 
     def forward(self, z, library, batch_label=None, z_=None):
         """
         Forward pass of the ProbDecoder.
```

### Comparing `step_kit-0.2.0/step/modules/gnn.py` & `step_kit-0.2.1/step/modules/gnn.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.0/step/modules/transformer.py` & `step_kit-0.2.1/step/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.0/step/scmodel.py` & `step_kit-0.2.1/step/scmodel.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.0/step/stmodel.py` & `step_kit-0.2.1/step/stmodel.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.0/step/utils/dataset.py` & `step_kit-0.2.1/step/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.0/step/utils/gbolt.py` & `step_kit-0.2.1/step/utils/gbolt.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.0/step/utils/metrics.py` & `step_kit-0.2.1/step/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.0/step/utils/misc.py` & `step_kit-0.2.1/step/utils/misc.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.0/step/utils/plotting.py` & `step_kit-0.2.1/step/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.0/step/utils/synthetics/pseudo_st.py` & `step_kit-0.2.1/step/utils/synthetics/pseudo_st.py`

 * *Files identical despite different names*

