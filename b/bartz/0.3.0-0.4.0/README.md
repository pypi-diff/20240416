# Comparing `tmp/bartz-0.3.0.tar.gz` & `tmp/bartz-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bartz-0.3.0.tar", max compression
+gzip compressed data, was "bartz-0.4.0.tar", max compression
```

## Comparing `bartz-0.3.0.tar` & `bartz-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1073 2024-03-19 21:21:09.679092 bartz-0.3.0/LICENSE
--rw-r--r--   0        0        0     3678 2024-04-08 04:46:18.271175 bartz-0.3.0/README.md
--rw-r--r--   0        0        0     3643 2024-04-08 06:08:10.021098 bartz-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    16862 2024-04-08 05:01:06.834203 bartz-0.3.0/src/bartz/BART.py
--rw-r--r--   0        0        0     1448 2024-03-31 06:56:42.369415 bartz-0.3.0/src/bartz/__init__.py
--rw-r--r--   0        0        0       22 2024-04-08 06:08:57.994671 bartz-0.3.0/src/bartz/_version.py
--rw-r--r--   0        0        0     5314 2024-03-25 19:59:40.459274 bartz-0.3.0/src/bartz/debug.py
--rw-r--r--   0        0        0     8500 2024-04-08 05:03:57.628481 bartz-0.3.0/src/bartz/grove.py
--rw-r--r--   0        0        0    12033 2024-04-08 05:07:50.118723 bartz-0.3.0/src/bartz/jaxext.py
--rw-r--r--   0        0        0     7634 2024-04-08 05:09:44.969044 bartz-0.3.0/src/bartz/mcmcloop.py
--rw-r--r--   0        0        0    54221 2024-04-08 05:51:36.476838 bartz-0.3.0/src/bartz/mcmcstep.py
--rw-r--r--   0        0        0     5818 2024-04-08 05:55:33.596178 bartz-0.3.0/src/bartz/prepcovars.py
--rw-r--r--   0        0        0     4500 1970-01-01 00:00:00.000000 bartz-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-03-19 21:21:09.679092 bartz-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3678 2024-04-08 04:46:18.271175 bartz-0.4.0/README.md
+-rw-r--r--   0        0        0     3721 2024-04-16 20:35:06.701537 bartz-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    16862 2024-04-08 05:01:06.834203 bartz-0.4.0/src/bartz/BART.py
+-rw-r--r--   0        0        0     1448 2024-03-31 06:56:42.369415 bartz-0.4.0/src/bartz/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-16 20:35:21.927403 bartz-0.4.0/src/bartz/_version.py
+-rw-r--r--   0        0        0     5314 2024-03-25 19:59:40.459274 bartz-0.4.0/src/bartz/debug.py
+-rw-r--r--   0        0        0     8500 2024-04-08 05:03:57.628481 bartz-0.4.0/src/bartz/grove.py
+-rw-r--r--   0        0        0    12033 2024-04-08 05:07:50.118723 bartz-0.4.0/src/bartz/jaxext.py
+-rw-r--r--   0        0        0     7634 2024-04-08 05:09:44.969044 bartz-0.4.0/src/bartz/mcmcloop.py
+-rw-r--r--   0        0        0    54987 2024-04-16 21:14:18.743408 bartz-0.4.0/src/bartz/mcmcstep.py
+-rw-r--r--   0        0        0     5818 2024-04-08 05:55:33.596178 bartz-0.4.0/src/bartz/prepcovars.py
+-rw-r--r--   0        0        0     4500 1970-01-01 00:00:00.000000 bartz-0.4.0/PKG-INFO
```

### Comparing `bartz-0.3.0/LICENSE` & `bartz-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bartz-0.3.0/README.md` & `bartz-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `bartz-0.3.0/pyproject.toml` & `bartz-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "bartz"
-version = "0.3.0"
+version = "0.4.0"
 description = "A JAX implementation of BART"
 authors = ["Giacomo Petrillo <info@giacomopetrillo.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Gattocrucco/bartz"
 packages = [
     { include = "bartz", from = "src" },
@@ -52,14 +52,17 @@
 ipython = "^8.22.2"
 matplotlib = "^3.8.3"
 appnope = "^0.1.4"
 tomli = "^2.0.1"
 packaging = "^24.0"
 xgboost = "^2.0.3"
 pre-commit = "^3.7.0"
+polars = "^0.20.19"
+scikit-learn = "^1.4.2"
+matplotlib-label-lines = "^0.7.0"
 
 [tool.poetry.group.test.dependencies]
 coverage = "^7.4.3"
 pytest = "^8.1.1"
 
 [tool.poetry.group.docs.dependencies]
 Sphinx = "^7.2.6"
```

### Comparing `bartz-0.3.0/src/bartz/BART.py` & `bartz-0.4.0/src/bartz/BART.py`

 * *Files identical despite different names*

### Comparing `bartz-0.3.0/src/bartz/__init__.py` & `bartz-0.4.0/src/bartz/__init__.py`

 * *Files identical despite different names*

### Comparing `bartz-0.3.0/src/bartz/debug.py` & `bartz-0.4.0/src/bartz/debug.py`

 * *Files identical despite different names*

### Comparing `bartz-0.3.0/src/bartz/grove.py` & `bartz-0.4.0/src/bartz/grove.py`

 * *Files identical despite different names*

### Comparing `bartz-0.3.0/src/bartz/jaxext.py` & `bartz-0.4.0/src/bartz/jaxext.py`

 * *Files identical despite different names*

### Comparing `bartz-0.3.0/src/bartz/mcmcloop.py` & `bartz-0.4.0/src/bartz/mcmcloop.py`

 * *Files identical despite different names*

### Comparing `bartz-0.3.0/src/bartz/mcmcstep.py` & `bartz-0.4.0/src/bartz/mcmcstep.py`

 * *Files 22% similar despite different names*

```diff
@@ -144,28 +144,36 @@
             'large_float' : dtype
                 The dtype for scalars, small arrays, and arrays which require
                 accuracy.
             'require_min_points' : bool
                 Whether the `min_points_per_leaf` parameter is specified.
             'resid_batch_size', 'count_batch_size' : int or None
                 The data batch sizes for computing the sufficient statistics.
+        'ratios' : dict, optional
+            If `save_ratios` is True, this field is present. It has the fields:
+
+            'log_trans_prior' : large_float array (num_trees,)
+                The log transition and prior Metropolis-Hastings ratio for the
+                proposed move on each tree.
+            'log_likelihood' : large_float array (num_trees,)
+                The log likelihood ratio.
     """
 
     p_nonterminal = jnp.asarray(p_nonterminal, large_float)
     p_nonterminal = jnp.pad(p_nonterminal, (0, 1))
     max_depth = p_nonterminal.size
 
     @functools.partial(jax.vmap, in_axes=None, out_axes=0, axis_size=num_trees)
     def make_forest(max_depth, dtype):
         return grove.make_tree(max_depth, dtype)
 
     small_float = jnp.dtype(small_float)
     large_float = jnp.dtype(large_float)
     y = jnp.asarray(y, small_float)
-    resid_batch_size, count_batch_size = _choose_suffstat_batch_size(resid_batch_size, count_batch_size, y)
+    resid_batch_size, count_batch_size = _choose_suffstat_batch_size(resid_batch_size, count_batch_size, y, 2 ** max_depth * num_trees)
     sigma2 = jnp.array(sigma2_beta / sigma2_alpha, large_float)
     sigma2 = jnp.where(jnp.isfinite(sigma2) & (sigma2 > 0), sigma2, 1)
 
     bart = dict(
         leaf_trees=make_forest(max_depth, small_float),
         var_trees=make_forest(max_depth - 1, jaxext.minimal_unsigned_dtype(X.shape[0] - 1)),
         split_trees=make_forest(max_depth - 1, max_split.dtype),
@@ -198,27 +206,21 @@
             resid_batch_size=resid_batch_size,
             count_batch_size=count_batch_size,
         ),
     )
 
     if save_ratios:
         bart['ratios'] = dict(
-            grow=dict(
-                trans_prior=jnp.full(num_trees, jnp.nan),
-                likelihood=jnp.full(num_trees, jnp.nan),
-            ),
-            prune=dict(
-                trans_prior=jnp.full(num_trees, jnp.nan),
-                likelihood=jnp.full(num_trees, jnp.nan),
-            ),
+            log_trans_prior=jnp.full(num_trees, jnp.nan),
+            log_likelihood=jnp.full(num_trees, jnp.nan),
         )
 
     return bart
 
-def _choose_suffstat_batch_size(resid_batch_size, count_batch_size, y):
+def _choose_suffstat_batch_size(resid_batch_size, count_batch_size, y, forest_size):
 
     @functools.cache
     def get_platform():
         try:
             device = y.devices().pop()
         except jax.errors.ConcretizationTypeError:
             device = jax.devices()[0]
@@ -240,14 +242,18 @@
         platform = get_platform()
         if platform == 'cpu':
             count_batch_size = None
         elif platform == 'gpu':
             n = max(1, y.size)
             count_batch_size = 2 ** int(round(math.log2(n) / 2 - 2)) # n^1/2
                 # /4 is good on V100, /2 on L4/T4, still haven't tried A100
+            max_memory = 2 ** 29
+            itemsize = 4
+            min_batch_size = int(math.ceil(forest_size * itemsize * n / max_memory))
+            count_batch_size = max(count_batch_size, min_batch_size)
             count_batch_size = max(1, count_batch_size)
 
     return resid_batch_size, count_batch_size
 
 def step(bart, key):
     """
     Perform one full MCMC step on a BART state.
@@ -285,35 +291,89 @@
         The new BART mcmc state.
 
     Notes
     -----
     This function zeroes the proposal counters.
     """
     key, subkey = random.split(key)
-    grow_moves, prune_moves = sample_moves(bart, subkey)
-    return accept_moves_and_sample_leaves(bart, grow_moves, prune_moves, key)
+    moves = sample_moves(bart, subkey)
+    return accept_moves_and_sample_leaves(bart, moves, key)
 
 def sample_moves(bart, key):
     """
     Propose moves for all the trees.
 
     Parameters
     ----------
     bart : dict
         BART mcmc state.
     key : jax.dtypes.prng_key array
         A jax random key.
 
     Returns
     -------
-    grow_moves, prune_moves : dict
-        The proposals for grow and prune moves. See `grow_move` and `prune_move`.
-    """
-    key = random.split(key, bart['var_trees'].shape[0])
-    return _sample_moves_vmap_trees(bart['var_trees'], bart['split_trees'], bart['affluence_trees'], bart['max_split'], bart['p_nonterminal'], bart['p_propose_grow'], key)
+    moves : dict
+        A dictionary with fields:
+
+        'allowed' : bool array (num_trees,)
+            Whether the move is possible.
+        'grow' : bool array (num_trees,)
+            Whether the move is a grow move or a prune move.
+        'num_growable' : int array (num_trees,)
+            The number of growable leaves in the original tree.
+        'node' : int array (num_trees,)
+            The index of the leaf to grow or node to prune.
+        'left', 'right' : int array (num_trees,)
+            The indices of the children of 'node'.
+        'partial_ratio' : float array (num_trees,)
+            A factor of the Metropolis-Hastings ratio of the move. It lacks
+            the likelihood ratio and the probability of proposing the prune
+            move. If the move is Prune, the ratio is inverted.
+        'grow_var' : int array (num_trees,)
+            The decision axes of the new rules.
+        'grow_split' : int array (num_trees,)
+            The decision boundaries of the new rules.
+        'var_trees' : int array (num_trees, 2 ** (d - 1))
+            The updated decision axes of the trees, valid whatever move.
+        'logu' : float array (num_trees,)
+            The logarithm of a uniform (0, 1] random variable to be used to
+            accept the move. It's in (-oo, 0].
+    """
+    ntree = bart['leaf_trees'].shape[0]
+    key = random.split(key, 1 + ntree)
+    key, subkey = key[0], key[1:]
+
+    # compute moves
+    grow_moves, prune_moves = _sample_moves_vmap_trees(bart['var_trees'], bart['split_trees'], bart['affluence_trees'], bart['max_split'], bart['p_nonterminal'], bart['p_propose_grow'], subkey)
+
+    u, logu = random.uniform(key, (2, ntree), bart['opt']['large_float'])
+
+    # choose between grow or prune
+    grow_allowed = grow_moves['num_growable'].astype(bool)
+    p_grow = jnp.where(grow_allowed & prune_moves['allowed'], 0.5, grow_allowed)
+    grow = u < p_grow # use < instead of <= because u is in [0, 1)
+
+    # compute children indices
+    node = jnp.where(grow, grow_moves['node'], prune_moves['node'])
+    left = node << 1
+    right = left + 1
+
+    return dict(
+        allowed=grow | prune_moves['allowed'],
+        grow=grow,
+        num_growable=grow_moves['num_growable'],
+        node=node,
+        left=left,
+        right=right,
+        partial_ratio=jnp.where(grow, grow_moves['partial_ratio'], prune_moves['partial_ratio']),
+        grow_var=grow_moves['var'],
+        grow_split=grow_moves['split'],
+        var_trees=grow_moves['var_tree'],
+        logu=jnp.log1p(-logu),
+    )
 
 @functools.partial(jaxext.vmap_nodoc, in_axes=(0, 0, 0, None, None, None, 0))
 def _sample_moves_vmap_trees(*args):
     args, key = args[:-1], args[-1]
     key, key1 = random.split(key)
     grow = grow_move(*args, key)
     prune = prune_move(*args, key1)
@@ -350,49 +410,42 @@
         A dictionary with fields:
 
         'num_growable' : int
             The number of growable leaves.
         'node' : int
             The index of the leaf to grow. ``2 ** d`` if there are no growable
             leaves.
-        'left', 'right' : int
-            The indices of the children of 'node'.
         'var', 'split' : int
             The decision axis and boundary of the new rule.
         'partial_ratio' : float
             A factor of the Metropolis-Hastings ratio of the move. It lacks
             the likelihood ratio and the probability of proposing the prune
             move.
-        'var_tree', 'split_tree' : array (2 ** (d - 1),)
-            The updated decision axes and boundaries of the tree.
+        'var_tree' : array (2 ** (d - 1),)
+            The updated decision axes of the tree.
     """
 
     key, key1, key2 = random.split(key, 3)
 
     leaf_to_grow, num_growable, prob_choose, num_prunable = choose_leaf(split_tree, affluence_tree, p_propose_grow, key)
 
     var = choose_variable(var_tree, split_tree, max_split, leaf_to_grow, key1)
     var_tree = var_tree.at[leaf_to_grow].set(var.astype(var_tree.dtype))
 
     split = choose_split(var_tree, split_tree, max_split, leaf_to_grow, key2)
-    split_tree = split_tree.at[leaf_to_grow].set(split.astype(split_tree.dtype))
 
-    ratio = compute_partial_ratio(prob_choose, num_prunable, p_nonterminal, leaf_to_grow, split_tree)
+    ratio = compute_partial_ratio(prob_choose, num_prunable, p_nonterminal, leaf_to_grow)
 
-    left = leaf_to_grow << 1
     return dict(
         num_growable=num_growable,
         node=leaf_to_grow,
-        left=left,
-        right=left + 1,
         var=var,
         split=split,
         partial_ratio=ratio,
         var_tree=var_tree,
-        split_tree=split_tree,
     )
 
 def choose_leaf(split_tree, affluence_tree, p_propose_grow, key):
     """
     Choose a leaf node to grow in a tree.
 
     Parameters
@@ -654,31 +707,29 @@
     split : int
         The split point.
     """
     var = var_tree[leaf_index]
     l, r = split_range(var_tree, split_tree, max_split, leaf_index, var)
     return random.randint(key, (), l, r)
 
-def compute_partial_ratio(prob_choose, num_prunable, p_nonterminal, leaf_to_grow, new_split_tree):
+def compute_partial_ratio(prob_choose, num_prunable, p_nonterminal, leaf_to_grow):
     """
     Compute the product of the transition and prior ratios of a grow move.
 
     Parameters
     ----------
     num_growable : int
         The number of leaf nodes that can be grown.
     num_prunable : int
         The number of leaf parents that could be pruned, after converting the
         leaf to be grown to a non-terminal node.
     p_nonterminal : array (d,)
         The probability of a nonterminal node at each depth.
     leaf_to_grow : int
         The index of the leaf to grow.
-    new_split_tree : array (2 ** (d - 1),)
-        The splitting points of the tree, after the leaf is grown.
 
     Returns
     -------
     ratio : float
         The transition ratio P(new tree -> old tree) / P(old tree -> new tree)
         times the prior ratio P(new tree) / P(old tree), but the transition
         ratio is missing the factor P(propose prune) in the numerator.
@@ -695,15 +746,15 @@
         # leaf to grow is root  -->  the tree can only be a root
         # tree is a root  -->  the only leaf I can grow is root
 
     p_grow = jnp.where(prune_allowed, 0.5, 1)
 
     inv_trans_ratio = p_grow * prob_choose * num_prunable
 
-    depth = grove.tree_depths(new_split_tree.size)[leaf_to_grow]
+    depth = grove.tree_depths(2 ** (p_nonterminal.size - 1))[leaf_to_grow]
     p_parent = p_nonterminal[depth]
     cp_children = 1 - p_nonterminal[depth + 1]
     tree_ratio = cp_children * cp_children * p_parent / (1 - p_parent)
 
     return tree_ratio / inv_trans_ratio
 
 def prune_move(var_tree, split_tree, affluence_tree, max_split, p_nonterminal, p_propose_grow, key):
@@ -732,32 +783,27 @@
     prune_move : dict
         A dictionary with fields:
 
         'allowed' : bool
             Whether the move is possible.
         'node' : int
             The index of the node to prune. ``2 ** d`` if no node can be pruned.
-        'left', 'right' : int
-            The indices of the children of 'node'.
         'partial_ratio' : float
             A factor of the Metropolis-Hastings ratio of the move. It lacks
             the likelihood ratio and the probability of proposing the prune
             move. This ratio is inverted.
     """
     node_to_prune, num_prunable, prob_choose = choose_leaf_parent(split_tree, affluence_tree, p_propose_grow, key)
     allowed = split_tree[1].astype(bool) # allowed iff the tree is not a root
 
-    ratio = compute_partial_ratio(prob_choose, num_prunable, p_nonterminal, node_to_prune, split_tree)
+    ratio = compute_partial_ratio(prob_choose, num_prunable, p_nonterminal, node_to_prune)
 
-    left = node_to_prune << 1
     return dict(
         allowed=allowed,
         node=node_to_prune,
-        left=left,
-        right=left + 1,
         partial_ratio=ratio, # it is inverted in accept_move_and_sample_leaves
     )
 
 def choose_leaf_parent(split_tree, affluence_tree, p_propose_grow, key):
     """
     Pick a non-terminal node with leaf children to prune in a tree.
 
@@ -815,165 +861,155 @@
         A random integer in the range ``[0, n)``, and which satisfies
         ``mask[u] == True``. If all values in the mask are `False`, return `n`.
     """
     ecdf = jnp.cumsum(mask)
     u = random.randint(key, (), 0, ecdf[-1])
     return jnp.searchsorted(ecdf, u, 'right')
 
-def accept_moves_and_sample_leaves(bart, grow_moves, prune_moves, key):
+def accept_moves_and_sample_leaves(bart, moves, key):
     """
     Accept or reject the proposed moves and sample the new leaf values.
 
     Parameters
     ----------
     bart : dict
         A BART mcmc state.
-    grow_moves : dict
-        The proposals for grow moves, batched over the first axis. See
-        `grow_move`.
-    prune_moves : dict
-        The proposals for prune moves, batched over the first axis. See
-        `prune_move`.
+    moves : dict
+        The proposed moves, see `sample_moves`.
     key : jax.dtypes.prng_key array
         A jax random key.
 
     Returns
     -------
     bart : dict
         The new BART mcmc state.
     """
-    bart, grow_moves, prune_moves, count_trees, move_counts, u, z = accept_moves_parallel_stage(bart, grow_moves, prune_moves, key)
-    bart, counts = accept_moves_sequential_stage(bart, count_trees, grow_moves, prune_moves, move_counts, u, z)
-    return accept_moves_final_stage(bart, counts, grow_moves, prune_moves)
+    bart, moves, count_trees, move_counts, prelkv, prelk, prelf = accept_moves_parallel_stage(bart, moves, key)
+    bart, moves = accept_moves_sequential_stage(bart, count_trees, moves, move_counts, prelkv, prelk, prelf)
+    return accept_moves_final_stage(bart, moves)
 
-def accept_moves_parallel_stage(bart, grow_moves, prune_moves, key):
+def accept_moves_parallel_stage(bart, moves, key):
     """
     Pre-computes quantities used to accept moves, in parallel across trees.
 
     Parameters
     ----------
     bart : dict
         A BART mcmc state.
-    grow_moves, prune_moves : dict
-        The proposals for the moves, batched over the first axis. See
-        `grow_move` and `prune_move`.
+    moves : dict
+        The proposed moves, see `sample_moves`.
     key : jax.dtypes.prng_key array
         A jax random key.
 
     Returns
     -------
     bart : dict
         A partially updated BART mcmc state.
-    grow_moves, prune_moves : dict
-        The proposals for the moves, with the field 'partial_ratio' replaced
-        by 'trans_prior_ratio'.
-    count_trees : array (num_trees, 2 ** (d - 1))
+    moves : dict
+        The proposed moves, with the field 'partial_ratio' replaced
+        by 'log_trans_prior_ratio'.
+    count_trees : array (num_trees, 2 ** d)
         The number of points in each potential or actual leaf node.
     move_counts : dict
         The counts of the number of points in the the nodes modified by the
         moves.
-    u : float array (num_trees, 2)
-        Random uniform values used to accept the moves.
-    z : float array (num_trees, 2 ** d)
-        Random standard normal values used to sample the new leaf values.
+    prelkv, prelk, prelf : dict
+        Dictionary with pre-computed terms of the likelihood ratios and leaf
+        samples.
     """
     bart = bart.copy()
 
-    bart['var_trees'] = grow_moves['var_tree']
-        # Since var_tree can contain garbage, I can set the var of leaf to be
-        # grown irrespectively of what move I'm gonna accept in the end.
-
-    bart['leaf_indices'] = apply_grow_to_indices(grow_moves, bart['leaf_indices'], bart['X'])
-
-    count_trees, move_counts = compute_count_trees(bart['leaf_indices'], grow_moves, prune_moves, bart['opt']['count_batch_size'])
-
-    grow_moves, prune_moves = complete_ratio(grow_moves, prune_moves, move_counts, bart['min_points_per_leaf'])
+    # where the move is grow, modify the state like the move was accepted
+    bart['var_trees'] = moves['var_trees']
+    bart['leaf_indices'] = apply_grow_to_indices(moves, bart['leaf_indices'], bart['X'])
+    bart['leaf_trees'] = adapt_leaf_trees_to_grow_indices(bart['leaf_trees'], moves)
 
+    # count number of datapoints per leaf
+    count_trees, move_counts = compute_count_trees(bart['leaf_indices'], moves, bart['opt']['count_batch_size'])
     if bart['opt']['require_min_points']:
-        count_half_trees = count_trees[:, :grow_moves['split_tree'].shape[1]]
+        count_half_trees = count_trees[:, :bart['var_trees'].shape[1]]
         bart['affluence_trees'] = count_half_trees >= 2 * bart['min_points_per_leaf']
 
-    bart['leaf_trees'] = adapt_leaf_trees_to_grow_indices(bart['leaf_trees'], grow_moves)
+    # compute some missing information about moves
+    moves = complete_ratio(moves, move_counts, bart['min_points_per_leaf'])
+    bart['grow_prop_count'] = jnp.sum(moves['grow'])
+    bart['prune_prop_count'] = jnp.sum(moves['allowed'] & ~moves['grow'])
 
-    key, subkey = random.split(key)
-    u = random.uniform(subkey, (len(bart['leaf_trees']), 2), bart['opt']['large_float'])
-    z = random.normal(key, bart['leaf_trees'].shape, bart['opt']['large_float'])
+    prelkv, prelk = precompute_likelihood_terms(count_trees, bart['sigma2'], move_counts)
+    prelf = precompute_leaf_terms(count_trees, bart['sigma2'], key)
 
-    return bart, grow_moves, prune_moves, count_trees, move_counts, u, z
+    return bart, moves, count_trees, move_counts, prelkv, prelk, prelf
 
-def apply_grow_to_indices(grow_moves, leaf_indices, X):
+@functools.partial(jaxext.vmap_nodoc, in_axes=(0, 0, None))
+def apply_grow_to_indices(moves, leaf_indices, X):
     """
     Update the leaf indices to apply a grow move.
 
     Parameters
     ----------
-    grow_moves : dict
-        The proposals for grow moves. See `grow_move`.
+    moves : dict
+        The proposed moves, see `sample_moves`.
     leaf_indices : array (num_trees, n)
         The index of the leaf each datapoint falls into.
     X : array (p, n)
         The predictors matrix.
 
     Returns
     -------
     grow_leaf_indices : array (num_trees, n)
         The updated leaf indices.
     """
-    left_child = grow_moves['node'].astype(leaf_indices.dtype) << 1
-    go_right = X[grow_moves['var'], :] >= grow_moves['split'][:, None]
-    tree_size = jnp.array(2 * grow_moves['split_tree'].shape[1])
-    node_to_update = jnp.where(grow_moves['num_growable'], grow_moves['node'], tree_size)
+    left_child = moves['node'].astype(leaf_indices.dtype) << 1
+    go_right = X[moves['grow_var'], :] >= moves['grow_split']
+    tree_size = jnp.array(2 * moves['var_trees'].size)
+    node_to_update = jnp.where(moves['grow'], moves['node'], tree_size)
     return jnp.where(
-        leaf_indices == node_to_update[:, None],
-        left_child[:, None] + go_right,
+        leaf_indices == node_to_update,
+        left_child + go_right,
         leaf_indices,
     )
 
-def compute_count_trees(grow_leaf_indices, grow_moves, prune_moves, batch_size):
+def compute_count_trees(leaf_indices, moves, batch_size):
     """
     Count the number of datapoints in each leaf.
 
     Parameters
     ----------
     grow_leaf_indices : int array (num_trees, n)
         The index of the leaf each datapoint falls into, if the grow move is
         accepted.
-    grow_moves, prune_moves : dict
-        The proposals for the moves. See `grow_move` and `prune_move`.
+    moves : dict
+        The proposed moves, see `sample_moves`.
     batch_size : int or None
         The data batch size to use for the summation.
 
     Returns
     -------
     count_trees : int array (num_trees, 2 ** (d - 1))
         The number of points in each potential or actual leaf node.
     counts : dict
         The counts of the number of points in the the nodes modified by the
         moves, organized as two dictionaries 'grow' and 'prune', with subfields
         'left', 'right', and 'total'.
     """
 
-    ntree, tree_size = grow_moves['split_tree'].shape
+    ntree, tree_size = moves['var_trees'].shape
     tree_size *= 2
-    counts = dict(grow=dict(), prune=dict())
     tree_indices = jnp.arange(ntree)
 
-    count_trees = count_datapoints_per_leaf(grow_leaf_indices, tree_size, batch_size)
+    count_trees = count_datapoints_per_leaf(leaf_indices, tree_size, batch_size)
 
-    # count datapoints in leaf to grow
-    counts['grow']['left'] = count_trees[tree_indices, grow_moves['left']]
-    counts['grow']['right'] = count_trees[tree_indices, grow_moves['right']]
-    counts['grow']['total'] = counts['grow']['left'] + counts['grow']['right']
-    count_trees = count_trees.at[tree_indices, grow_moves['node']].set(counts['grow']['total'])
-
-    # count datapoints in node to prune
-    counts['prune']['left'] = count_trees[tree_indices, prune_moves['left']]
-    counts['prune']['right'] = count_trees[tree_indices, prune_moves['right']]
-    counts['prune']['total'] = counts['prune']['left'] + counts['prune']['right']
-    count_trees = count_trees.at[tree_indices, prune_moves['node']].set(counts['prune']['total'])
+    # count datapoints in nodes modified by move
+    counts = dict()
+    counts['left'] = count_trees[tree_indices, moves['left']]
+    counts['right'] = count_trees[tree_indices, moves['right']]
+    counts['total'] = counts['left'] + counts['right']
+
+    # write count into non-leaf node
+    count_trees = count_trees.at[tree_indices, moves['node']].set(counts['total'])
 
     return count_trees, counts
 
 def count_datapoints_per_leaf(leaf_indices, tree_size, batch_size):
     """
     Count the number of datapoints in each leaf.
 
@@ -1021,319 +1057,340 @@
     return (jnp
         .zeros((ntree, size, nbatches), dtype)
         .at[tree_indices[:, None], indices, batch_indices]
         .add(values)
         .sum(axis=2)
     )
 
-def complete_ratio(grow_moves, prune_moves, move_counts, min_points_per_leaf):
+def complete_ratio(moves, move_counts, min_points_per_leaf):
     """
     Complete non-likelihood MH ratio calculation.
 
     This functions adds the probability of choosing the prune move.
 
     Parameters
     ----------
-    grow_moves, prune_moves : dict
-        The proposals for the moves. See `grow_move` and `prune_move`.
+    moves : dict
+        The proposed moves, see `sample_moves`.
     move_counts : dict
         The counts of the number of points in the the nodes modified by the
         moves.
     min_points_per_leaf : int or None
         The minimum number of data points in a leaf node.
 
     Returns
     -------
-    grow_moves, prune_moves : dict
-        The proposals for the moves, with the field 'partial_ratio' replaced
-        by 'trans_prior_ratio'.
-    """
-    grow_moves = grow_moves.copy()
-    prune_moves = prune_moves.copy()
-    compute_p_prune_vec = jax.vmap(compute_p_prune, in_axes=(0, 0, 0, None))
-    grow_p_prune, prune_p_prune = compute_p_prune_vec(grow_moves, move_counts['grow']['left'], move_counts['grow']['right'], min_points_per_leaf)
-    grow_moves['trans_prior_ratio'] = grow_moves.pop('partial_ratio') * grow_p_prune
-    prune_moves['trans_prior_ratio'] = prune_moves.pop('partial_ratio') * prune_p_prune
-    return grow_moves, prune_moves
+    moves : dict
+        The updated moves, with the field 'partial_ratio' replaced by
+        'log_trans_prior_ratio'.
+    """
+    moves = moves.copy()
+    p_prune = compute_p_prune(moves, move_counts['left'], move_counts['right'], min_points_per_leaf)
+    moves['log_trans_prior_ratio'] = jnp.log(moves.pop('partial_ratio') * p_prune)
+    return moves
 
-def compute_p_prune(grow_move, grow_left_count, grow_right_count, min_points_per_leaf):
+def compute_p_prune(moves, left_count, right_count, min_points_per_leaf):
     """
     Compute the probability of proposing a prune move.
 
     Parameters
     ----------
-    grow_move : dict
-        The proposal for the grow move, see `grow_move`.
-    grow_left_count, grow_right_count : int
+    moves : dict
+        The proposed moves, see `sample_moves`.
+    left_count, right_count : int
         The number of datapoints in the proposed children of the leaf to grow.
     min_points_per_leaf : int or None
         The minimum number of data points in a leaf node.
 
     Returns
     -------
-    grow_p_prune : float
-        The probability of proposing a prune move, after accepting the grow
-        move.
-    prune_p_prune : float
-        The probability of proposing the prune move.
+    p_prune : float
+        The probability of proposing a prune move. If grow: after accepting the
+        grow move, if prune: right away.
     """
-    other_growable_leaves = grow_move['num_growable'] >= 2
-    new_leaves_growable = grow_move['node'] < grow_move['split_tree'].size // 2
+
+    # calculation in case the move is grow
+    other_growable_leaves = moves['num_growable'] >= 2
+    new_leaves_growable = moves['node'] < moves['var_trees'].shape[1] // 2
     if min_points_per_leaf is not None:
-        any_above_threshold = grow_left_count >= 2 * min_points_per_leaf
-        any_above_threshold |= grow_right_count >= 2 * min_points_per_leaf
+        any_above_threshold = left_count >= 2 * min_points_per_leaf
+        any_above_threshold |= right_count >= 2 * min_points_per_leaf
         new_leaves_growable &= any_above_threshold
     grow_again_allowed = other_growable_leaves | new_leaves_growable
     grow_p_prune = jnp.where(grow_again_allowed, 0.5, 1)
-    prune_p_prune = jnp.where(grow_move['num_growable'], 0.5, 1)
-    return grow_p_prune, prune_p_prune
 
-def adapt_leaf_trees_to_grow_indices(leaf_trees, grow_moves):
+    # calculation in case the move is prune
+    prune_p_prune = jnp.where(moves['num_growable'], 0.5, 1)
+
+    return jnp.where(moves['grow'], grow_p_prune, prune_p_prune)
+
+@jaxext.vmap_nodoc
+def adapt_leaf_trees_to_grow_indices(leaf_trees, moves):
     """
-    Modify leaf values such that the indices of the grow move work on the
+    Modify leaf values such that the indices of the grow moves work on the
     original tree.
 
     Parameters
     ----------
     leaf_trees : float array (num_trees, 2 ** d)
         The leaf values.
-    grow_moves : dict
-        The proposals for grow moves. See `grow_move`.
+    moves : dict
+        The proposed moves, see `sample_moves`.
 
     Returns
     -------
     leaf_trees : float array (num_trees, 2 ** d)
         The modified leaf values. The value of the leaf to grow is copied to
         what would be its children if the grow move was accepted.
     """
-    ntree, _ = leaf_trees.shape
-    tree_indices = jnp.arange(ntree)
-    values_at_node = leaf_trees[tree_indices, grow_moves['node']]
+    values_at_node = leaf_trees[moves['node']]
     return (leaf_trees
-        .at[tree_indices, grow_moves['left']]
+        .at[jnp.where(moves['grow'], moves['left'], leaf_trees.size)]
         .set(values_at_node)
-        .at[tree_indices, grow_moves['right']]
+        .at[jnp.where(moves['grow'], moves['right'], leaf_trees.size)]
         .set(values_at_node)
     )
 
-def accept_moves_sequential_stage(bart, count_trees, grow_moves, prune_moves, move_counts, u, z):
+def precompute_likelihood_terms(count_trees, sigma2, move_counts):
+    """
+    Pre-compute terms used in the likelihood ratio of the acceptance step.
+
+    Parameters
+    ----------
+    count_trees : array (num_trees, 2 ** d)
+        The number of points in each potential or actual leaf node.
+    sigma2 : float
+        The noise variance.
+    move_counts : dict
+        The counts of the number of points in the the nodes modified by the
+        moves.
+
+    Returns
+    -------
+    prelkv : dict
+        Dictionary with pre-computed terms of the likelihood ratio, one per
+        tree.
+    prelk : dict
+        Dictionary with pre-computed terms of the likelihood ratio, shared by
+        all trees.
+    """
+    ntree = len(count_trees)
+    sigma_mu2 = 1 / ntree
+    prelkv = dict()
+    prelkv['sigma2_left'] = sigma2 + move_counts['left'] * sigma_mu2
+    prelkv['sigma2_right'] = sigma2 + move_counts['right'] * sigma_mu2
+    prelkv['sigma2_total'] = sigma2 + move_counts['total'] * sigma_mu2
+    prelkv['sqrt_term'] = jnp.log(
+        sigma2 * prelkv['sigma2_total'] /
+        (prelkv['sigma2_left'] * prelkv['sigma2_right'])
+    ) / 2
+    return prelkv, dict(
+        exp_factor=sigma_mu2 / (2 * sigma2),
+    )
+
+def precompute_leaf_terms(count_trees, sigma2, key):
+    """
+    Pre-compute terms used to sample leaves from their posterior.
+
+    Parameters
+    ----------
+    count_trees : array (num_trees, 2 ** d)
+        The number of points in each potential or actual leaf node.
+    sigma2 : float
+        The noise variance.
+    key : jax.dtypes.prng_key array
+        A jax random key.
+
+    Returns
+    -------
+    prelf : dict
+        Dictionary with pre-computed terms of the leaf sampling, with fields:
+
+        'mean_factor' : float array (num_trees, 2 ** d)
+            The factor to be multiplied by the sum of residuals to obtain the
+            posterior mean.
+        'centered_leaves' : float array (num_trees, 2 ** d)
+            The mean-zero normal values to be added to the posterior mean to
+            obtain the posterior leaf samples.
+    """
+    ntree = len(count_trees)
+    prec_lk = count_trees / sigma2
+    var_post = lax.reciprocal(prec_lk + ntree) # = 1 / (prec_lk + prec_prior)
+    z = random.normal(key, count_trees.shape, sigma2.dtype)
+    return dict(
+        mean_factor=var_post / sigma2, # = mean_lk * prec_lk * var_post / resid_tree
+        centered_leaves=z * jnp.sqrt(var_post),
+    )
+
+def accept_moves_sequential_stage(bart, count_trees, moves, move_counts, prelkv, prelk, prelf):
     """
     The part of accepting the moves that has to be done one tree at a time.
 
     Parameters
     ----------
     bart : dict
         A partially updated BART mcmc state.
-    count_trees : array (num_trees, 2 ** (d - 1))
+    count_trees : array (num_trees, 2 ** d)
         The number of points in each potential or actual leaf node.
-    grow_moves, prune_moves : dict
-        The proposals for the moves, with completed ratios. See `grow_move` and
-        `prune_move`.
+    moves : dict
+        The proposed moves, see `sample_moves`.
     move_counts : dict
         The counts of the number of points in the the nodes modified by the
         moves.
-    u : float array (num_trees, 2)
-        Random uniform values used to for proposal and accept decisions.
-    z : float array (num_trees, 2 ** d)
-        Random standard normal values used to sample the new leaf values.
+    prelkv, prelk, prelf : dict
+        Dictionaries with pre-computed terms of the likelihood ratios and leaf
+        samples.
 
     Returns
     -------
     bart : dict
         A partially updated BART mcmc state.
-    counts : dict
-        The indicators of proposals and acceptances for grow and prune moves.
+    moves : dict
+        The proposed moves, with these additional fields:
+
+        'acc' : bool array (num_trees,)
+            Whether the move was accepted.
+        'to_prune' : bool array (num_trees,)
+            Whether, to reflect the acceptance status of the move, the state
+            should be updated by pruning the leaves involved in the move.
     """
     bart = bart.copy()
+    moves = moves.copy()
 
     def loop(resid, item):
-        resid, leaf_tree, split_tree, counts, ratios = accept_move_and_sample_leaves(
+        resid, leaf_tree, acc, to_prune, ratios = accept_move_and_sample_leaves(
             bart['X'],
             len(bart['leaf_trees']),
             bart['opt']['resid_batch_size'],
             resid,
-            bart['sigma2'],
             bart['min_points_per_leaf'],
             'ratios' in bart,
+            prelk,
             *item,
         )
-        return resid, (leaf_tree, split_tree, counts, ratios)
+        return resid, (leaf_tree, acc, to_prune, ratios)
 
     items = (
         bart['leaf_trees'], count_trees,
-        grow_moves, prune_moves, move_counts,
+        moves, move_counts,
         bart['leaf_indices'],
-        u, z,
+        prelkv, prelf,
     )
-    resid, (leaf_trees, split_trees, counts, ratios) = lax.scan(loop, bart['resid'], items)
+    resid, (leaf_trees, acc, to_prune, ratios) = lax.scan(loop, bart['resid'], items)
 
     bart['resid'] = resid
     bart['leaf_trees'] = leaf_trees
-    bart['split_trees'] = split_trees
     bart.get('ratios', {}).update(ratios)
+    moves['acc'] = acc
+    moves['to_prune'] = to_prune
 
-    return bart, counts
+    return bart, moves
 
-def accept_move_and_sample_leaves(X, ntree, resid_batch_size, resid, sigma2, min_points_per_leaf, save_ratios, leaf_tree, count_tree, grow_move, prune_move, move_counts, grow_leaf_indices, u, z):
+def accept_move_and_sample_leaves(X, ntree, resid_batch_size, resid, min_points_per_leaf, save_ratios, prelk, leaf_tree, count_tree, move, move_counts, leaf_indices, prelkv, prelf):
     """
     Accept or reject a proposed move and sample the new leaf values.
 
     Parameters
     ----------
     X : int array (p, n)
         The predictors.
     ntree : int
         The number of trees in the forest.
     resid_batch_size : int, None
         The batch size for computing the sum of residuals in each leaf.
     resid : float array (n,)
         The residuals (data minus forest value).
-    sigma2 : float
-        The noise variance.
     min_points_per_leaf : int or None
         The minimum number of data points in a leaf node.
     save_ratios : bool
         Whether to save the acceptance ratios.
+    prelk : dict
+        The pre-computed terms of the likelihood ratio which are shared across
+        trees.
     leaf_tree : float array (2 ** d,)
         The leaf values of the tree.
     count_tree : int array (2 ** d,)
         The number of datapoints in each leaf.
-    grow_move, prune_move : dict
-        The proposals for the moves, with completed ratios. See `grow_move` and
-        `prune_move`.
-    grow_leaf_indices : int array (n,)
-        The leaf indices of the tree proposed by the grow move.
-    u : float array (2,)
-        Two uniform random values in [0, 1).
-    z : float array (2 ** d,)
-        Standard normal random values.
+    move : dict
+        The proposed move, see `sample_moves`.
+    leaf_indices : int array (n,)
+        The leaf indices for the largest version of the tree compatible with
+        the move.
+    prelkv, prelf : dict
+        The pre-computed terms of the likelihood ratio and leaf sampling which
+        are specific to the tree.
 
     Returns
     -------
     resid : float array (n,)
         The updated residuals (data minus forest value).
     leaf_tree : float array (2 ** d,)
         The new leaf values of the tree.
-    split_tree : int array (2 ** (d - 1),)
-        The updated decision boundaries of the tree.
-    counts : dict
-        The indicators of proposals and acceptances for grow and prune moves.
+    acc : bool
+        Whether the move was accepted.
+    to_prune : bool
+        Whether, to reflect the acceptance status of the move, the state should
+        be updated by pruning the leaves involved in the move.
     ratios : dict
         The acceptance ratios for the moves. Empty if not to be saved.
     """
 
     # sum residuals and count units per leaf, in tree proposed by grow move
-    resid_tree = sum_resid(resid, grow_leaf_indices, leaf_tree.size, resid_batch_size)
+    resid_tree = sum_resid(resid, leaf_indices, leaf_tree.size, resid_batch_size)
 
     # subtract starting tree from function
     resid_tree += count_tree * leaf_tree
 
-    # get indices of grow move
-    grow_node = grow_move['node']
-    assert grow_node.dtype == jnp.int32
-    grow_left = grow_move['left']
-    grow_right = grow_move['right']
-
-    # sum residuals in leaf to grow
-    grow_resid_left = resid_tree[grow_left]
-    grow_resid_right = resid_tree[grow_right]
-    grow_resid_total = grow_resid_left + grow_resid_right
-    resid_tree = resid_tree.at[grow_node].set(grow_resid_total)
-
-    # get indices of prune move
-    prune_node = prune_move['node']
-    assert prune_node.dtype == jnp.int32
-    prune_left = prune_move['left']
-    prune_right = prune_move['right']
-
-    # sum residuals in node to prune
-    prune_resid_left = resid_tree[prune_left]
-    prune_resid_right = resid_tree[prune_right]
-    prune_resid_total = prune_resid_left + prune_resid_right
-    resid_tree = resid_tree.at[prune_node].set(prune_resid_total)
-
-    # Now resid_tree and count_tree contain correct values whatever move is
-    # accepted.
-
-    # compute likelihood ratios
-    grow_lk_ratio = compute_likelihood_ratio(grow_resid_total, grow_resid_left, grow_resid_right, move_counts['grow']['total'], move_counts['grow']['left'], move_counts['grow']['right'], sigma2, ntree)
-    prune_lk_ratio = compute_likelihood_ratio(prune_resid_total, prune_resid_left, prune_resid_right, move_counts['prune']['total'], move_counts['prune']['left'], move_counts['prune']['right'], sigma2, ntree)
-
-    # compute acceptance ratios
-    grow_ratio = grow_move['trans_prior_ratio'] * grow_lk_ratio
-    if min_points_per_leaf is not None:
-        grow_ratio = jnp.where(move_counts['grow']['left'] >= min_points_per_leaf, grow_ratio, 0)
-        grow_ratio = jnp.where(move_counts['grow']['right'] >= min_points_per_leaf, grow_ratio, 0)
-    prune_ratio = prune_move['trans_prior_ratio'] * prune_lk_ratio
-    prune_ratio = lax.reciprocal(prune_ratio)
-
-    # save acceptance ratios
+    # get indices of move
+    node = move['node']
+    assert node.dtype == jnp.int32
+    left = move['left']
+    right = move['right']
+
+    # sum residuals in parent node modified by move
+    resid_left = resid_tree[left]
+    resid_right = resid_tree[right]
+    resid_total = resid_left + resid_right
+    resid_tree = resid_tree.at[node].set(resid_total)
+
+    # compute acceptance ratio
+    log_lk_ratio = compute_likelihood_ratio(resid_total, resid_left, resid_right, prelkv, prelk)
+    log_ratio = move['log_trans_prior_ratio'] + log_lk_ratio
+    log_ratio = jnp.where(move['grow'], log_ratio, -log_ratio)
     ratios = {}
     if save_ratios:
         ratios.update(
-            grow=dict(
-                trans_prior=grow_move['trans_prior_ratio'],
-                likelihood=grow_lk_ratio,
-            ),
-            prune=dict(
-                trans_prior=lax.reciprocal(prune_move['trans_prior_ratio']),
-                likelihood=lax.reciprocal(prune_lk_ratio),
-            ),
+            log_trans_prior=move['log_trans_prior_ratio'],
+            log_likelihood=log_lk_ratio,
         )
 
-    # determine what move to propose (not proposing anything is an option)
-    grow_allowed = grow_move['num_growable'].astype(bool)
-    p_grow = jnp.where(grow_allowed & prune_move['allowed'], 0.5, grow_allowed)
-    try_grow = u[0] < p_grow # use < instead of <= because coins are in [0, 1)
-    try_prune = prune_move['allowed'] & ~try_grow
-
     # determine whether to accept the move
-    do_grow = try_grow & (u[1] < grow_ratio)
-    do_prune = try_prune & (u[1] < prune_ratio)
-
-    # pick split tree for chosen move
-    split_tree = grow_move['split_tree']
-    split_tree = split_tree.at[jnp.where(do_grow, split_tree.size, grow_node)].set(0)
-    split_tree = split_tree.at[jnp.where(do_prune, prune_node, split_tree.size)].set(0)
-    # I can leave garbage in var_tree, resid_tree, count_tree
+    acc = move['allowed'] & (move['logu'] <= log_ratio)
+    if min_points_per_leaf is not None:
+        acc &= move_counts['left'] >= min_points_per_leaf
+        acc &= move_counts['right'] >= min_points_per_leaf
 
     # compute leaves posterior and sample leaves
-    inv_sigma2 = lax.reciprocal(sigma2)
-    prec_lk = count_tree * inv_sigma2
-    var_post = lax.reciprocal(prec_lk + ntree) # = 1 / (prec_lk + prec_prior)
-    mean_post = resid_tree * inv_sigma2 * var_post # = mean_lk * prec_lk * var_post
     initial_leaf_tree = leaf_tree
-    leaf_tree = mean_post + z * jnp.sqrt(var_post)
+    mean_post = resid_tree * prelf['mean_factor']
+    leaf_tree = mean_post + prelf['centered_leaves']
 
-    # copy leaves around such that the grow leaf indices select the right leaf
-    leaf_tree = (leaf_tree
-        .at[jnp.where(do_prune, prune_left, leaf_tree.size)]
-        .set(leaf_tree[prune_node])
-        .at[jnp.where(do_prune, prune_right, leaf_tree.size)]
-        .set(leaf_tree[prune_node])
-    )
+    # copy leaves around such that the leaf indices select the right leaf
+    to_prune = acc ^ move['grow']
     leaf_tree = (leaf_tree
-        .at[jnp.where(do_grow, leaf_tree.size, grow_left)]
-        .set(leaf_tree[grow_node])
-        .at[jnp.where(do_grow, leaf_tree.size, grow_right)]
-        .set(leaf_tree[grow_node])
+        .at[jnp.where(to_prune, left, leaf_tree.size)]
+        .set(leaf_tree[node])
+        .at[jnp.where(to_prune, right, leaf_tree.size)]
+        .set(leaf_tree[node])
     )
 
     # replace old tree with new tree in function values
-    resid += (initial_leaf_tree - leaf_tree)[grow_leaf_indices]
+    resid += (initial_leaf_tree - leaf_tree)[leaf_indices]
 
-    # pack proposal and acceptance indicators
-    counts = dict(
-        grow_prop_count=try_grow,
-        grow_acc_count=do_grow,
-        prune_prop_count=try_prune,
-        prune_acc_count=do_prune,
-    )
-
-    return resid, leaf_tree, split_tree, counts, ratios
+    return resid, leaf_tree, acc, to_prune, ratios
 
 def sum_resid(resid, leaf_indices, tree_size, batch_size):
     """
     Sum the residuals in each leaf.
 
     Parameters
     ----------
@@ -1365,114 +1422,126 @@
     return (jnp
         .zeros((size, nbatches), dtype)
         .at[indices, batch_indices]
         .add(values)
         .sum(axis=1)
     )
 
-def compute_likelihood_ratio(total_resid, left_resid, right_resid, total_count, left_count, right_count, sigma2, n_tree):
+def compute_likelihood_ratio(total_resid, left_resid, right_resid, prelkv, prelk):
     """
     Compute the likelihood ratio of a grow move.
 
     Parameters
     ----------
     total_resid : float
         The sum of the residuals in the leaf to grow.
     left_resid, right_resid : float
         The sum of the residuals in the left/right child of the leaf to grow.
-    total_count : int
-        The number of datapoints in the leaf to grow.
-    left_count, right_count : int
-        The number of datapoints in the left/right child of the leaf to grow.
-    sigma2 : float
-        The noise variance.
-    n_tree : int
-        The number of trees in the forest.
+    prelkv, prelk : dict
+        The pre-computed terms of the likelihood ratio, see
+        `precompute_likelihood_terms`.
 
     Returns
     -------
     ratio : float
         The likelihood ratio P(data | new tree) / P(data | old tree).
     """
-
-    sigma_mu2 = 1 / n_tree
-    sigma2_left = sigma2 + left_count * sigma_mu2
-    sigma2_right = sigma2 + right_count * sigma_mu2
-    sigma2_total = sigma2 + total_count * sigma_mu2
-
-    sqrt_term = sigma2 * sigma2_total / (sigma2_left * sigma2_right)
-
-    exp_term = sigma_mu2 / (2 * sigma2) * (
-        left_resid * left_resid / sigma2_left +
-        right_resid * right_resid / sigma2_right -
-        total_resid * total_resid / sigma2_total
+    exp_term = prelk['exp_factor'] * (
+        left_resid * left_resid / prelkv['sigma2_left'] +
+        right_resid * right_resid / prelkv['sigma2_right'] -
+        total_resid * total_resid / prelkv['sigma2_total']
     )
+    return prelkv['sqrt_term'] + exp_term
 
-    return jnp.sqrt(sqrt_term) * jnp.exp(exp_term)
-
-def accept_moves_final_stage(bart, counts, grow_moves, prune_moves):
+def accept_moves_final_stage(bart, moves):
     """
     The final part of accepting the moves, in parallel across trees.
 
     Parameters
     ----------
     bart : dict
         A partially updated BART mcmc state.
     counts : dict
         The indicators of proposals and acceptances for grow and prune moves.
-    grow_moves, prune_moves : dict
-        The proposals for the moves. See `grow_move` and `prune_move`.
+    moves : dict
+        The proposed moves (see `sample_moves`) as updated by
+        `accept_moves_sequential_stage`.
 
     Returns
     -------
     bart : dict
         The fully updated BART mcmc state.
     """
     bart = bart.copy()
-
-    for k, v in counts.items():
-        bart[k] = jnp.sum(v, axis=0)
-
-    bart['leaf_indices'] = apply_moves_to_indices(bart['leaf_indices'], counts, grow_moves, prune_moves)
-
+    bart['grow_acc_count'] = jnp.sum(moves['acc'] & moves['grow'])
+    bart['prune_acc_count'] = jnp.sum(moves['acc'] & ~moves['grow'])
+    bart['leaf_indices'] = apply_moves_to_leaf_indices(bart['leaf_indices'], moves)
+    bart['split_trees'] = apply_moves_to_split_trees(bart['split_trees'], moves)
     return bart
 
-def apply_moves_to_indices(leaf_indices, counts, grow_moves, prune_moves):
+@jax.vmap
+def apply_moves_to_leaf_indices(leaf_indices, moves):
     """
     Update the leaf indices to match the accepted move.
 
     Parameters
     ----------
     leaf_indices : int array (num_trees, n)
         The index of the leaf each datapoint falls into, if the grow move was
         accepted.
-    counts : dict
-        The indicators of proposals and acceptances for grow and prune moves.
-    grow_moves, prune_moves : dict
-        The proposals for the moves. See `grow_move` and `prune_move`.
+    moves : dict
+        The proposed moves (see `sample_moves`), as updated by
+        `accept_moves_sequential_stage`.
 
     Returns
     -------
     leaf_indices : int array (num_trees, n)
         The updated leaf indices.
     """
     mask = ~jnp.array(1, leaf_indices.dtype) # ...1111111110
-    cond = (leaf_indices & mask) == grow_moves['left'][:, None]
-    leaf_indices = jnp.where(
-        cond & ~counts['grow_acc_count'][:, None],
-        grow_moves['node'][:, None].astype(leaf_indices.dtype),
-        leaf_indices,
-    )
-    cond = (leaf_indices & mask) == prune_moves['left'][:, None]
+    is_child = (leaf_indices & mask) == moves['left']
     return jnp.where(
-        cond & counts['prune_acc_count'][:, None],
-        prune_moves['node'][:, None].astype(leaf_indices.dtype),
+        is_child & moves['to_prune'],
+        moves['node'].astype(leaf_indices.dtype),
         leaf_indices,
     )
 
+@jax.vmap
+def apply_moves_to_split_trees(split_trees, moves):
+    """
+    Update the split trees to match the accepted move.
+
+    Parameters
+    ----------
+    split_trees : int array (num_trees, 2 ** (d - 1))
+        The cutpoints of the decision nodes in the initial trees.
+    moves : dict
+        The proposed moves (see `sample_moves`), as updated by
+        `accept_moves_sequential_stage`.
+
+    Returns
+    -------
+    split_trees : int array (num_trees, 2 ** (d - 1))
+        The updated split trees.
+    """
+    return (split_trees
+        .at[jnp.where(
+            moves['grow'],
+            moves['node'],
+            split_trees.size,
+        )]
+        .set(moves['grow_split'].astype(split_trees.dtype))
+        .at[jnp.where(
+            moves['to_prune'],
+            moves['node'],
+            split_trees.size,
+        )]
+        .set(0)
+    )
+
 def sample_sigma(bart, key):
     """
     Noise variance sampling step of BART MCMC.
 
     Parameters
     ----------
     bart : dict
```

### Comparing `bartz-0.3.0/src/bartz/prepcovars.py` & `bartz-0.4.0/src/bartz/prepcovars.py`

 * *Files identical despite different names*

### Comparing `bartz-0.3.0/PKG-INFO` & `bartz-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bartz
-Version: 0.3.0
+Version: 0.4.0
 Summary: A JAX implementation of BART
 Home-page: https://github.com/Gattocrucco/bartz
 License: MIT
 Author: Giacomo Petrillo
 Author-email: info@giacomopetrillo.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

