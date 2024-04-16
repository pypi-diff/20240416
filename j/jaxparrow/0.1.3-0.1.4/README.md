# Comparing `tmp/jaxparrow-0.1.3.tar.gz` & `tmp/jaxparrow-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxparrow-0.1.3.tar", last modified: Sat Mar 30 10:55:23 2024, max compression
+gzip compressed data, was "jaxparrow-0.1.4.tar", last modified: Tue Apr 16 07:10:56 2024, max compression
```

## Comparing `jaxparrow-0.1.3.tar` & `jaxparrow-0.1.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 10:55:23.774732 jaxparrow-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11353 2024-03-30 10:55:17.000000 jaxparrow-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-03-30 10:55:23.774732 jaxparrow-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-03-30 10:55:17.000000 jaxparrow-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 10:55:23.770732 jaxparrow-0.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-03-30 10:55:17.000000 jaxparrow-0.1.3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 10:55:23.770732 jaxparrow-0.1.3/jaxparrow/
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-30 10:55:17.000000 jaxparrow-0.1.3/jaxparrow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-03-30 10:55:17.000000 jaxparrow-0.1.3/jaxparrow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17167 2024-03-30 10:55:17.000000 jaxparrow-0.1.3/jaxparrow/cyclogeostrophy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-03-30 10:55:17.000000 jaxparrow-0.1.3/jaxparrow/geostrophy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 10:55:23.770732 jaxparrow-0.1.3/jaxparrow/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 10:55:17.000000 jaxparrow-0.1.3/jaxparrow/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-03-30 10:55:17.000000 jaxparrow-0.1.3/jaxparrow/tools/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     8799 2024-03-30 10:55:17.000000 jaxparrow-0.1.3/jaxparrow/tools/kinematics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-03-30 10:55:17.000000 jaxparrow-0.1.3/jaxparrow/tools/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-03-30 10:55:17.000000 jaxparrow-0.1.3/jaxparrow/tools/sanitize.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-30 10:55:17.000000 jaxparrow-0.1.3/jaxparrow/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 10:55:23.770732 jaxparrow-0.1.3/jaxparrow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-03-30 10:55:23.000000 jaxparrow-0.1.3/jaxparrow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-03-30 10:55:23.000000 jaxparrow-0.1.3/jaxparrow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 10:55:23.000000 jaxparrow-0.1.3/jaxparrow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-30 10:55:23.000000 jaxparrow-0.1.3/jaxparrow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-30 10:55:23.000000 jaxparrow-0.1.3/jaxparrow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-30 10:55:23.000000 jaxparrow-0.1.3/jaxparrow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 10:55:23.770732 jaxparrow-0.1.3/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-03-30 10:55:17.000000 jaxparrow-0.1.3/notebooks/duacs_visualisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-03-30 10:55:17.000000 jaxparrow-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 10:55:23.774732 jaxparrow-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 10:55:23.770732 jaxparrow-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-03-30 10:55:17.000000 jaxparrow-0.1.3/tests/gaussian_eddy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-03-30 10:55:17.000000 jaxparrow-0.1.3/tests/test_velocities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:10:56.683470 jaxparrow-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11353 2024-04-16 07:10:49.000000 jaxparrow-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-04-16 07:10:56.683470 jaxparrow-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-04-16 07:10:49.000000 jaxparrow-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:10:56.679470 jaxparrow-0.1.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-16 07:10:49.000000 jaxparrow-0.1.4/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:10:56.679470 jaxparrow-0.1.4/jaxparrow/
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-16 07:10:49.000000 jaxparrow-0.1.4/jaxparrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-04-16 07:10:49.000000 jaxparrow-0.1.4/jaxparrow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16446 2024-04-16 07:10:49.000000 jaxparrow-0.1.4/jaxparrow/cyclogeostrophy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-16 07:10:49.000000 jaxparrow-0.1.4/jaxparrow/geostrophy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:10:56.683470 jaxparrow-0.1.4/jaxparrow/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:10:49.000000 jaxparrow-0.1.4/jaxparrow/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-16 07:10:49.000000 jaxparrow-0.1.4/jaxparrow/tools/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-04-16 07:10:49.000000 jaxparrow-0.1.4/jaxparrow/tools/kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-04-16 07:10:49.000000 jaxparrow-0.1.4/jaxparrow/tools/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-04-16 07:10:49.000000 jaxparrow-0.1.4/jaxparrow/tools/sanitize.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 07:10:49.000000 jaxparrow-0.1.4/jaxparrow/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:10:56.683470 jaxparrow-0.1.4/jaxparrow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-04-16 07:10:56.000000 jaxparrow-0.1.4/jaxparrow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-16 07:10:56.000000 jaxparrow-0.1.4/jaxparrow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 07:10:56.000000 jaxparrow-0.1.4/jaxparrow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-16 07:10:56.000000 jaxparrow-0.1.4/jaxparrow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-16 07:10:56.000000 jaxparrow-0.1.4/jaxparrow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-16 07:10:56.000000 jaxparrow-0.1.4/jaxparrow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:10:56.683470 jaxparrow-0.1.4/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-04-16 07:10:49.000000 jaxparrow-0.1.4/notebooks/duacs_visualisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-16 07:10:49.000000 jaxparrow-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 07:10:56.683470 jaxparrow-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:10:56.683470 jaxparrow-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-16 07:10:49.000000 jaxparrow-0.1.4/tests/gaussian_eddy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-04-16 07:10:49.000000 jaxparrow-0.1.4/tests/test_velocities.py
```

### Comparing `jaxparrow-0.1.3/LICENSE` & `jaxparrow-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxparrow-0.1.3/PKG-INFO` & `jaxparrow-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxparrow
-Version: 0.1.3
+Version: 0.1.4
 Summary: Computes the inversion of the cyclogeostrophic balance based on a variational formulation approach, using JAX
 Author-email: Vadim Bertrand <vadim.bertrand@univ-grenoble-alpes.fr>, Victor E V Z De Almeida <victorzaia@outlook.com>, Julien Le Sommer <julien.lesommer@univ-grenoble-alpes.fr>, Emmanuel Cosme <emmanuel.cosme@univ-grenoble-alpes.fr>
 License: Apache-2.0
 Project-URL: Homepage, https://jaxparrow.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/meom-group/jaxparrow/issues
 Keywords: cyclogeostrophy,eddy,flow,geostrophy,jax,swirl,velocity
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jaxparrow-0.1.3/README.md` & `jaxparrow-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `jaxparrow-0.1.3/docs/conf.py` & `jaxparrow-0.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaxparrow-0.1.3/jaxparrow/__main__.py` & `jaxparrow-0.1.4/jaxparrow/__main__.py`

 * *Files identical despite different names*

### Comparing `jaxparrow-0.1.3/jaxparrow/cyclogeostrophy.py` & `jaxparrow-0.1.4/jaxparrow/cyclogeostrophy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from collections.abc import Callable
 from functools import partial
-import numbers
 from typing import Literal, Union
 
 from jax import jit, lax, value_and_grad
 import jax.numpy as jnp
 import jax.scipy as jsp
 from jaxtyping import Array, Float, Scalar
 import optax
@@ -37,15 +36,14 @@
         lon_t: Float[Array, "lat lon"],
         mask: Float[Array, "lat lon"] = None,
         method: Literal["variational", "iterative"] = "variational",
         n_it: int = None,
         optim: Union[optax.GradientTransformation, str] = "sgd",
         optim_kwargs: dict = None,
         res_eps: float = RES_EPS_IT,
-        res_init: Union[float, Literal["same"]] = RES_INIT_IT,
         use_res_filter: bool = False,
         res_filter_size: int = RES_FILTER_SIZE_IT,
         return_geos: bool = False,
         return_grids: bool = True,
         return_losses: bool = False
 ) -> [Float[Array, "lat lon"], ...]:
     """
@@ -86,20 +84,14 @@
 
         If `None`, only the learning rate is enforced to ``LR_VAR``
     res_eps : float, optional
         Residual tolerance of the iterative approach.
         When residuals are smaller, the iterative approach considers local convergence to cyclogeostrophy.
 
         Defaults to ``RES_EPS_IT``
-    res_init : Union[float | Literal["same"]], optional
-        Residual initial value of the iterative approach.
-        When residuals are larger at the first iteration,
-        the iterative approach considers local divergence to cyclogeostrophy.
-
-        If equals to `same` (default) absolute values of the geostrophic velocities are used
     use_res_filter : bool, optional
         Use of a convolution filter for the iterative approach when computing the residuals [3]_ or not [2]_.
 
         Defaults to `False`
     res_filter_size : int, optional
         Size of the convolution filter of the iterative approach, when ``use_res_filter=True``.
 
@@ -155,19 +147,30 @@
     dy_u = sanitize.sanitize_data(dy_u, jnp.nan, mask)
     dx_v = sanitize.sanitize_data(dx_v, jnp.nan, mask)
     dy_v = sanitize.sanitize_data(dy_v, jnp.nan, mask)
     coriolis_factor_u = sanitize.sanitize_data(coriolis_factor_u, jnp.nan, mask)
     coriolis_factor_v = sanitize.sanitize_data(coriolis_factor_v, jnp.nan, mask)
 
     if method == "variational":
+        if n_it is None:
+            n_it = N_IT_VAR
+        if isinstance(optim, str):
+            if optim_kwargs is None:
+                optim_kwargs = {"learning_rate": LR_VAR}
+            optim = getattr(optax, optim)(**optim_kwargs)
+        elif not isinstance(optim, optax.GradientTransformation):
+            raise TypeError("optim should be an optax.GradientTransformation optimizer, or a string referring to such "
+                            "an optimizer.")
         res = _variational(u_geos_u, v_geos_v, dx_u, dx_v, dy_u, dy_v, coriolis_factor_u, coriolis_factor_v, mask,
-                           n_it, optim, optim_kwargs, return_losses)
+                           n_it, optim, return_losses)
     elif method == "iterative":
+        if n_it is None:
+            n_it = N_IT_IT
         res = _iterative(u_geos_u, v_geos_v, dx_u, dx_v, dy_u, dy_v, coriolis_factor_u, coriolis_factor_v, mask,
-                         n_it, res_eps, res_init, use_res_filter, res_filter_size, return_losses)
+                         n_it, res_eps, use_res_filter, res_filter_size, return_losses)
     else:
         raise ValueError("method should be one of [\"variational\", \"iterative\"]")
 
     # Handle masked data
     u_cyclo_u, v_cyclo_v, losses = res
     u_cyclo_u = sanitize.sanitize_data(u_cyclo_u, jnp.nan, mask)
     v_cyclo_v = sanitize.sanitize_data(v_cyclo_v, jnp.nan, mask)
@@ -213,14 +216,15 @@
     # next it
     u_adv_v, v_adv_u = kinematics.advection(u_cyclo, v_cyclo, dx_u, dy_u, dx_v, dy_v, mask)
     u_np1 = u_geos_u - v_adv_u / coriolis_factor_u
     v_np1 = v_geos_v + u_adv_v / coriolis_factor_v
 
     # compute dist to u_cyclo and v_cyclo
     res_np1 = jnp.abs(u_np1 - u_cyclo) + jnp.abs(v_np1 - v_cyclo)
+    res_np1 = sanitize.sanitize_data(res_np1, 0., mask)
     res_np1 = lax.cond(
         use_res_filter,  # apply filter
         lambda operands: jsp.signal.convolve(operands[0], operands[1], mode="same", method="fft") / operands[2],
         lambda operands: operands[0],
         (res_np1, res_filter, res_weights)
     )
     # compute intermediate masks
@@ -244,41 +248,31 @@
     res_n = res_np1
 
     i += 1
 
     return u_cyclo, v_cyclo, mask_it, res_n, losses, i
 
 
-@partial(jit, static_argnames=("n_it", "res_init", "res_filter_size"))
+@partial(jit, static_argnames=("n_it", "res_filter_size"))
 def _iterative(
         u_geos_u: Float[Array, "lat lon"],
         v_geos_v: Float[Array, "lat lon"],
         dx_u: Float[Array, "lat lon"],
         dx_v: Float[Array, "lat lon"],
         dy_u: Float[Array, "lat lon"],
         dy_v: Float[Array, "lat lon"],
         coriolis_factor_u: Float[Array, "lat lon"],
         coriolis_factor_v: Float[Array, "lat lon"],
         mask: Float[Array, "lat lon"],
-        n_it: Union[int, None],
+        n_it: int,
         res_eps: float,
-        res_init: Union[float, str],
         use_res_filter: bool,
         res_filter_size: int,
         return_losses: bool
 ) -> [Float[Array, "lat lon"], ...]:
-    if n_it is None:
-        n_it = N_IT_IT
-    if res_init == "same":
-        res_n = jnp.maximum(jnp.abs(u_geos_u), jnp.abs(v_geos_v))
-    elif isinstance(res_init, numbers.Number):
-        res_n = res_init * jnp.ones_like(u_geos_u)
-    else:
-        raise ValueError("res_init should be equal to \"same\" or be a number.")
-
     # used if applying a filter when computing stopping criteria
     res_filter = jnp.ones((res_filter_size, res_filter_size))
     res_weights = jsp.signal.convolve(jnp.ones_like(u_geos_u), res_filter, mode="same", method="fft")
 
     # define step partial: freeze constant over iterations
     def step_fn(pytree):
         return _it_step(
@@ -290,15 +284,16 @@
             *pytree
         )
 
     # apply updates
     u_cyclo, v_cyclo, _, _, losses, _ = lax.while_loop(  # noqa
         lambda args: (args[-1] < n_it) | jnp.any(args[2] != 1),
         step_fn,
-        (u_geos_u, v_geos_v, mask.astype(int), res_n, jnp.ones(n_it) * jnp.nan, 0)
+        (u_geos_u, v_geos_v, mask.astype(int), jnp.maximum(jnp.abs(u_geos_u), jnp.abs(v_geos_v)),
+         jnp.ones(n_it) * jnp.nan, 0)
     )
 
     return u_cyclo, v_cyclo, losses
 
 
 # =============================================================================
 # Variational method
@@ -373,40 +368,29 @@
         step_fn,
         (u_geos_u, v_geos_v, optim.init((u_geos_u, v_geos_v)), jnp.ones(n_it) * jnp.nan, 0)
     )
 
     return u_cyclo_u, v_cyclo_v, losses
 
 
-@partial(jit, static_argnames=("n_it", "optim", "optim_kwargs"))
+@partial(jit, static_argnames=("n_it", "optim"))
 def _variational(
         u_geos_u: Float[Array, "lat lon"],
         v_geos_v: Float[Array, "lat lon"],
         dx_u: Float[Array, "lat lon"],
         dx_v: Float[Array, "lat lon"],
         dy_u: Float[Array, "lat lon"],
         dy_v: Float[Array, "lat lon"],
         coriolis_factor_u: Float[Array, "lat lon"],
         coriolis_factor_v: Float[Array, "lat lon"],
         mask: Float[Array, "lat lon"],
-        n_it: Union[int, None],
-        optim: Union[optax.GradientTransformation, str],
-        optim_kwargs: Union[dict, None],
+        n_it: int,
+        optim: optax.GradientTransformation,
         return_losses: bool
 ) -> [Float[Array, "lat lon"], ...]:
-    if n_it is None:
-        n_it = N_IT_VAR
-    if isinstance(optim, str):
-        if optim_kwargs is None:
-            optim_kwargs = {"learning_rate": LR_VAR}
-        optim = getattr(optax, optim)(**optim_kwargs)
-    elif not isinstance(optim, optax.GradientTransformation):
-        raise TypeError("optim should be an optax.GradientTransformation optimizer, or a string referring to such an "
-                        "optimizer.")
-
     # define loss partial: freeze constant over iterations
     loss_fn = partial(
         _var_loss_fn,
         u_geos_u, v_geos_v, dx_u, dx_v, dy_u, dy_v, coriolis_factor_u, coriolis_factor_v, mask
     )
 
     return _solve(u_geos_u, v_geos_v, mask, loss_fn, n_it, optim, return_losses)
```

### Comparing `jaxparrow-0.1.3/jaxparrow/geostrophy.py` & `jaxparrow-0.1.4/jaxparrow/geostrophy.py`

 * *Files identical despite different names*

### Comparing `jaxparrow-0.1.3/jaxparrow/tools/geometry.py` & `jaxparrow-0.1.4/jaxparrow/tools/geometry.py`

 * *Files identical despite different names*

### Comparing `jaxparrow-0.1.3/jaxparrow/tools/kinematics.py` & `jaxparrow-0.1.4/jaxparrow/tools/kinematics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import jax.numpy as jnp
 from jaxtyping import Array, Float
 
 from .geometry import compute_spatial_step, compute_coriolis_factor
 from .operators import derivative, interpolation
-from .sanitize import sanitize_data
+from .sanitize import init_mask, sanitize_data
 
 
 def advection(
         u: Float[Array, "lat lon"],
         v: Float[Array, "lat lon"],
         dx_u: Float[Array, "lat lon"],
         dy_u: Float[Array, "lat lon"],
@@ -171,14 +171,17 @@
 
     Returns
     -------
     w : Float[Array, "lat lon"]
         The normalised relative vorticity,
         on the F grid (if ``interpolate=False``), or the T grid (if ``interpolate=True``)
     """
+    # Make sure the mask is initialized
+    mask = init_mask(u, mask)
+
     # Compute spatial step and Coriolis factor
     _, dy_u = compute_spatial_step(lat_u, lon_u)
     dx_v, _ = compute_spatial_step(lat_v, lon_v)
     f_u = compute_coriolis_factor(lat_u)
 
     # Handle spurious data and apply mask
     dy_u = sanitize_data(dy_u, jnp.nan, mask)
@@ -198,21 +201,21 @@
         w = w_f
 
     w = sanitize_data(w, jnp.nan, mask)
 
     return w
 
 
-def eddy_kinetic_energy(
+def kinetic_energy(
         u: Float[Array, "lat lon"],
         v: Float[Array, "lat lon"],
         interpolate: bool = True
 ) -> Float[Array, "lat lon"]:
     """
-    Computes the Eddy Kinetic Energy (EKE) of a velocity field,
+    Computes the Kinetic Energy (KE) of a velocity field,
     possibly on a C-grid (following NEMO convention [1]_) if ``interpolate=True``.
 
     Parameters
     ----------
     u : Float[Array, "lat lon"]
         U component of the velocity field (on the U grid)
     v : Float[Array, "lat lon"]
@@ -223,15 +226,15 @@
         If `False`, the velocity components are assumed to be located on the T grid, and interpolation is not needed.
 
         Defaults to `True`
 
     Returns
     -------
     eke : Float[Array, "lat lon"]
-        The Eddy Kinetic Energy on the T grid
+        The Kinetic Energy on the T grid
     """
     if interpolate:
         # interpolate to the T point
         u_t = interpolation(u, axis=1, padding="left")  # (U(i), U(i+1)) -> T(i+1)
         v_t = interpolation(v, axis=0, padding="left")  # (V(j), V(j+1)) -> T(j+1)
     else:
         u_t, v_t = u, v
```

### Comparing `jaxparrow-0.1.3/jaxparrow/tools/operators.py` & `jaxparrow-0.1.4/jaxparrow/tools/operators.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,34 +101,34 @@
         (the midpoint between $T_i$ and $T_{i+1}$ corresponds to $U_i$)
 
     Returns
     -------
     field : Float[Array, "lat lon"]
         Interpolated field
     """
-    def do_derivate(field_b, field_f, pad_left):
+    def do_differentiate(field_b, field_f, pad_left):
         field_b, field_f = handle_land_boundary(field_b, field_f, pad_left)
         return field_f - field_b
 
     def axis0(_field, pad_left):
         field_b, field_f = _field[:-1, :], _field[1:, :]
-        midpoint_values = do_derivate(field_b, field_f, pad_left)
+        midpoint_values = do_differentiate(field_b, field_f, pad_left)
 
         _field = lax.cond(
             pad_left,
             lambda operand: jnp.pad(operand, pad_width=((1, 0), (0, 0)), mode="edge"),
             lambda operand: jnp.pad(operand, pad_width=((0, 1), (0, 0)), mode="edge"),
             midpoint_values
         )
 
         return _field
 
     def axis1(_field, pad_left):
         field_b, field_f = _field[:, :-1], _field[:, 1:]
-        midpoint_values = do_derivate(field_b, field_f, pad_left)
+        midpoint_values = do_differentiate(field_b, field_f, pad_left)
 
         _field = lax.cond(
             pad_left,
             lambda operand: jnp.pad(operand, pad_width=((0, 0), (1, 0)), mode="edge"),
             lambda operand: jnp.pad(operand, pad_width=((0, 0), (0, 1)), mode="edge"),
             midpoint_values
         )
```

### Comparing `jaxparrow-0.1.3/jaxparrow/tools/sanitize.py` & `jaxparrow-0.1.4/jaxparrow/tools/sanitize.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,22 +64,25 @@
         field2: Float[Array, "lat lon"],
         pad_left: bool
 ) -> [Float[Array, "lat lon"], Float[Array, "lat lon"]]:
     """
     Replaces the non-finite values of ``field1`` (``field2``) with values of ``field2`` (``field1``), element-wise.
 
     It allows to introduce less non-finite values when applying grid operators.
-    In such cases, ``field1`` and ``field2`` are left and right shifted versions of a field.
+    In such cases, ``field1`` and ``field2`` are left and right shifted versions of a field (along one of the axes).
 
     Parameters
     ----------
     field1 : Float[Array, "lat lon"]
         A field
     field2 : Float[Array, "lat lon"]
         Another field
+    pad_left : bool
+        If `True`, apply padding in the `left` direction (i.e. `West` or `South`) ;
+        if `False`, apply padding in the `right` direction (i.e. `East` or `North`).
 
     Returns
     -------
     field1 : Float[Array, "lat lon"]
         A field whose non-finite values have been replaced with the ones from ``field2``
     field2 : Float[Array, "lat lon"]
         A field whose non-finite values have been replaced with the ones from ``field1``
@@ -98,16 +101,16 @@
         lon: Float[Array, "lat lon"],
         mask: Float[Array, "lat lon"] = None
 ) -> [Float[Array, "lat lon"], Float[Array, "lat lon"]]:
     """
     Sanitizes (unstructured) grids by interpolated and extrapolated `nan` or masked values to avoid spurious
     (`0`, `nan`, `inf`) spatial steps and Coriolis factors.
 
-    Helper function written using ``numpy`` and ``scipy``, and as such not used internally,
-    because incompatible with ``jax.vmap``.
+    Helper function written using pure ``numpy`` and ``scipy``, and as such not used internally,
+    because incompatible with ``jax.vmap`` and likes.
     Should be used before calling ``jaxparrow.geostrophy`` or ``jaxparrow.cyclogeostrophy``
     in case of suspicious latitudes or longitudes T grids.
 
     Caution: because it uses ``scipy.interpolate.RBFInterpolator``,
     it's memory usage grows quadratically with the number of grid points.
 
     Parameters
```

### Comparing `jaxparrow-0.1.3/jaxparrow.egg-info/PKG-INFO` & `jaxparrow-0.1.4/jaxparrow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxparrow
-Version: 0.1.3
+Version: 0.1.4
 Summary: Computes the inversion of the cyclogeostrophic balance based on a variational formulation approach, using JAX
 Author-email: Vadim Bertrand <vadim.bertrand@univ-grenoble-alpes.fr>, Victor E V Z De Almeida <victorzaia@outlook.com>, Julien Le Sommer <julien.lesommer@univ-grenoble-alpes.fr>, Emmanuel Cosme <emmanuel.cosme@univ-grenoble-alpes.fr>
 License: Apache-2.0
 Project-URL: Homepage, https://jaxparrow.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/meom-group/jaxparrow/issues
 Keywords: cyclogeostrophy,eddy,flow,geostrophy,jax,swirl,velocity
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jaxparrow-0.1.3/jaxparrow.egg-info/SOURCES.txt` & `jaxparrow-0.1.4/jaxparrow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaxparrow-0.1.3/notebooks/duacs_visualisation.py` & `jaxparrow-0.1.4/notebooks/duacs_visualisation.py`

 * *Files identical despite different names*

### Comparing `jaxparrow-0.1.3/pyproject.toml` & `jaxparrow-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jaxparrow-0.1.3/tests/gaussian_eddy.py` & `jaxparrow-0.1.4/tests/gaussian_eddy.py`

 * *Files identical despite different names*

### Comparing `jaxparrow-0.1.3/tests/test_velocities.py` & `jaxparrow-0.1.4/tests/test_velocities.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from jaxparrow.cyclogeostrophy import _iterative, _variational
+import optax
+
+from jaxparrow.cyclogeostrophy import _iterative, _variational, LR_VAR
 from jaxparrow.geostrophy import _geostrophy
 from jaxparrow.tools.operators import interpolation
 from jaxparrow.tools.sanitize import init_mask
 
 import gaussian_eddy as ge
 
 
@@ -19,41 +21,42 @@
     def test_cyclogeostrophy_penven(self):
         mask = init_mask(self.u_geos)
         u_geos_u = interpolation(self.u_geos, axis=1, padding="right")
         v_geos_v = interpolation(self.v_geos, axis=0, padding="right")
         u_cyclo_est, v_cyclo_est, _ = _iterative(u_geos_u, v_geos_v,
                                                  self.dXY, self.dXY, self.dXY, self.dXY,
                                                  self.coriolis_factor, self.coriolis_factor, mask,
-                                                 20, 0.01, "same", False, 3, False)
+                                                 20, 0.01, False, 3, False)
         u_cyclo_est_t = interpolation(u_cyclo_est, axis=1, padding="left")
         v_cyclo_est_t = interpolation(v_cyclo_est, axis=0, padding="left")
         cyclo_rmse = self.compute_rmse(self.u_cyclo, self.v_cyclo, u_cyclo_est_t, v_cyclo_est_t)  # around .0035
         assert cyclo_rmse < .004
 
     def test_cyclogeostrophy_ioannou(self):
         mask = init_mask(self.u_geos)
         u_geos_u = interpolation(self.u_geos, axis=1, padding="right")
         v_geos_v = interpolation(self.v_geos, axis=0, padding="right")
         u_cyclo_est, v_cyclo_est, _ = _iterative(u_geos_u, v_geos_v,
                                                  self.dXY, self.dXY, self.dXY, self.dXY,
                                                  self.coriolis_factor, self.coriolis_factor, mask,
-                                                 20, 0.01, "same", True, 3, False)
+                                                 20, 0.01, True, 3, False)
         u_cyclo_est_t = interpolation(u_cyclo_est, axis=1, padding="left")
         v_cyclo_est_t = interpolation(v_cyclo_est, axis=0, padding="left")
         cyclo_rmse = self.compute_rmse(self.u_cyclo, self.v_cyclo, u_cyclo_est_t, v_cyclo_est_t)  # around .0035
         assert cyclo_rmse < .004
 
     def test_cyclogeostrophy_variational(self):
         mask = init_mask(self.u_geos)
         u_geos_u = interpolation(self.u_geos, axis=1, padding="right")
         v_geos_v = interpolation(self.v_geos, axis=0, padding="right")
+        optim = optax.sgd(learning_rate=LR_VAR)
         u_cyclo_est, v_cyclo_est, _ = _variational(u_geos_u, v_geos_v,
                                                    self.dXY, self.dXY, self.dXY, self.dXY,
                                                    self.coriolis_factor, self.coriolis_factor, mask,
-                                                   20, "sgd", None, False)
+                                                   20, optim, False)
         u_cyclo_est_t = interpolation(u_cyclo_est, axis=1, padding="left")
         v_cyclo_est_t = interpolation(v_cyclo_est, axis=0, padding="left")
         cyclo_rmse = self.compute_rmse(self.u_cyclo, self.v_cyclo, u_cyclo_est_t, v_cyclo_est_t)  # around .0035
         assert cyclo_rmse < .004
 
     @staticmethod
     def compute_rmse(u, v, u_est, v_est) -> float:
```

