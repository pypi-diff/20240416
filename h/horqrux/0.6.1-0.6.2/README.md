# Comparing `tmp/horqrux-0.6.1.tar.gz` & `tmp/horqrux-0.6.2.tar.gz`

## Comparing `horqrux-0.6.1.tar` & `horqrux-0.6.2.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 horqrux-0.6.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 horqrux-0.6.1/README.md
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 horqrux-0.6.1/mkdocs.yml
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 horqrux-0.6.1/setup.py
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 horqrux-0.6.1/.github/workflows/run-tests-and-mypy.yml
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 horqrux-0.6.1/docs/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 horqrux-0.6.1/docs/CONTRIBUTING.md
--rw-r--r--   0        0        0    13456 2020-02-02 00:00:00.000000 horqrux-0.6.1/docs/index.md
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 horqrux-0.6.1/docs/css/mkdocstrings.css
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 horqrux-0.6.1/docs/javascripts/mathjax.js
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 horqrux-0.6.1/horqrux/__init__.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 horqrux-0.6.1/horqrux/adjoint.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 horqrux-0.6.1/horqrux/analog.py
--rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 horqrux-0.6.1/horqrux/apply.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 horqrux-0.6.1/horqrux/matrices.py
--rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 horqrux-0.6.1/horqrux/parametric.py
--rw-r--r--   0        0        0     7708 2020-02-02 00:00:00.000000 horqrux-0.6.1/horqrux/primitive.py
--rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 horqrux-0.6.1/horqrux/utils.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 horqrux-0.6.1/tests/test_adjoint.py
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 horqrux-0.6.1/tests/test_analog.py
--rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 horqrux-0.6.1/tests/test_gates.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 horqrux-0.6.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 horqrux-0.6.1/LICENSE
--rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 horqrux-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 horqrux-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 horqrux-0.6.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 horqrux-0.6.2/README.md
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 horqrux-0.6.2/mkdocs.yml
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 horqrux-0.6.2/setup.py
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 horqrux-0.6.2/.github/workflows/run-tests-and-mypy.yml
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 horqrux-0.6.2/docs/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 horqrux-0.6.2/docs/CONTRIBUTING.md
+-rw-r--r--   0        0        0    12271 2020-02-02 00:00:00.000000 horqrux-0.6.2/docs/index.md
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 horqrux-0.6.2/docs/css/mkdocstrings.css
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 horqrux-0.6.2/docs/javascripts/mathjax.js
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 horqrux-0.6.2/horqrux/__init__.py
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 horqrux-0.6.2/horqrux/adjoint.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 horqrux-0.6.2/horqrux/analog.py
+-rw-r--r--   0        0        0     6018 2020-02-02 00:00:00.000000 horqrux-0.6.2/horqrux/apply.py
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 horqrux-0.6.2/horqrux/circuit.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 horqrux-0.6.2/horqrux/matrices.py
+-rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 horqrux-0.6.2/horqrux/parametric.py
+-rw-r--r--   0        0        0     7708 2020-02-02 00:00:00.000000 horqrux-0.6.2/horqrux/primitive.py
+-rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 horqrux-0.6.2/horqrux/utils.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 horqrux-0.6.2/tests/test_adjoint.py
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 horqrux-0.6.2/tests/test_analog.py
+-rw-r--r--   0        0        0     4295 2020-02-02 00:00:00.000000 horqrux-0.6.2/tests/test_gates.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 horqrux-0.6.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 horqrux-0.6.2/LICENSE
+-rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 horqrux-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 horqrux-0.6.2/PKG-INFO
```

### Comparing `horqrux-0.6.1/.pre-commit-config.yaml` & `horqrux-0.6.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `horqrux-0.6.1/README.md` & `horqrux-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `horqrux-0.6.1/mkdocs.yml` & `horqrux-0.6.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `horqrux-0.6.1/.github/workflows/run-tests-and-mypy.yml` & `horqrux-0.6.2/.github/workflows/run-tests-and-mypy.yml`

 * *Files identical despite different names*

### Comparing `horqrux-0.6.1/docs/CODE_OF_CONDUCT.md` & `horqrux-0.6.2/docs/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `horqrux-0.6.1/docs/CONTRIBUTING.md` & `horqrux-0.6.2/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `horqrux-0.6.1/docs/index.md` & `horqrux-0.6.2/docs/index.md`

 * *Files 8% similar despite different names*

```diff
@@ -107,89 +107,69 @@
 import optax
 from functools import reduce, partial
 from operator import add
 from typing import Any, Callable
 from uuid import uuid4
 
 from horqrux.adjoint import adjoint_expectation
+from horqrux.circuit import Circuit, hea
 from horqrux.primitive import Primitive
+from horqrux.parametric import Parametric
 from horqrux import Z, RX, RY, NOT, zero_state, apply_gate
 
 
 n_qubits = 5
 n_params = 3
 n_layers = 3
 
 # Lets define a sequence of rotations
-def ansatz_w_params(n_qubits: int, n_layers: int) -> tuple[list, list]:
-    all_ops = []
-    param_names = []
-    rots_fns = [RX ,RY, RX]
-    for _ in range(n_layers):
-        for i in range(n_qubits):
-            ops = [fn(str(uuid4()), qubit) for fn, qubit in zip(rots_fns, [i for _ in range(len(rots_fns))])]
-            param_names += [op.param for op in ops]
-            ops += [NOT((i+1) % n_qubits, i % n_qubits) for i in range(n_qubits)]
-            all_ops += ops
-
-    return all_ops, param_names
 
 #  We need a function to fit and use it to produce training data
 fn = lambda x, degree: .05 * reduce(add, (jnp.cos(i*x) + jnp.sin(i*x) for i in range(degree)), 0)
 x = jnp.linspace(0, 10, 100)
 y = fn(x, 5)
 
-@dataclass
-class Circuit:
-    n_qubits: int
-    n_layers: int
 
+class DQC(Circuit):
     def __post_init__(self) -> None:
-        # We will use a featuremap of RX rotations to encode some classical data
-        self.feature_map: list[Primitive] = [RX('phi', i) for i in range(self.n_qubits)]
-        self.ansatz, self.param_names = ansatz_w_params(self.n_qubits, self.n_layers)
         self.observable: list[Primitive] = [Z(0)]
+        self.state = zero_state(self.n_qubits)
 
     @partial(vmap, in_axes=(None, None, 0))
     def __call__(self, param_values: Array, x: Array) -> Array:
-        state = zero_state(self.n_qubits)
         param_dict = {name: val for name, val in zip(self.param_names, param_values)}
-        return adjoint_expectation(state, self.feature_map + self.ansatz, self.observable, {**param_dict, **{'phi': x}})
-
+        return adjoint_expectation(self.state, self.feature_map + self.ansatz, self.observable, {**param_dict, **{'phi': x}})
 
-    @property
-    def n_vparams(self) -> int:
-        return len(self.param_names)
 
-circ = Circuit(n_qubits, n_layers)
+circ = DQC(n_qubits=n_qubits, feature_map=[RX('phi', i) for i in range(n_qubits)], ansatz=hea(n_qubits, n_layers))
 # Create random initial values for the parameters
 key = jax.random.PRNGKey(42)
 param_vals = jax.random.uniform(key, shape=(circ.n_vparams,))
 # Check the initial predictions using randomly initialized parameters
 y_init = circ(param_vals, x)
 
 optimizer = optax.adam(learning_rate=0.01)
 opt_state = optimizer.init(param_vals)
 
 # Define a loss function
-def loss_fn(param_vals: Array, x: Array, y: Array) -> Array:
+def loss_fn(param_vals: Array) -> Array:
     y_pred = circ(param_vals, x)
     return jnp.mean(optax.l2_loss(y_pred, y))
 
 
 def optimize_step(param_vals: Array, opt_state: Array, grads: Array) -> tuple:
     updates, opt_state = optimizer.update(grads, opt_state)
     param_vals = optax.apply_updates(param_vals, updates)
     return param_vals, opt_state
 
 @jit
 def train_step(i: int, paramvals_w_optstate: tuple
 ) -> tuple:
     param_vals, opt_state = paramvals_w_optstate
-    loss, grads = value_and_grad(loss_fn)(param_vals, x, y)
+    loss, grads = value_and_grad(loss_fn)(param_vals)
     param_vals, opt_state = optimize_step(param_vals, opt_state, grads)
     return param_vals, opt_state
 
 
 n_epochs = 200
 param_vals, opt_state = jax.lax.fori_loop(0, n_epochs, train_step, (param_vals, opt_state))
 y_final = circ(param_vals, x)
@@ -217,169 +197,143 @@
 ```python exec="on" source="material-block" html="1"
 from __future__ import annotations
 
 from dataclasses import dataclass
 from functools import reduce
 from itertools import product
 from operator import add
-from uuid import uuid4
+from typing import Callable
 
 import jax
 import jax.numpy as jnp
 import matplotlib.pyplot as plt
 import numpy as np
 import optax
 from jax import Array, jit, value_and_grad, vmap
 from numpy.random import uniform
 
+from horqrux.apply import group_by_index
+from horqrux.circuit import Circuit, hea
 from horqrux import NOT, RX, RY, Z, apply_gate, zero_state
 from horqrux.primitive import Primitive
+from horqrux.parametric import Parametric
 from horqrux.utils import inner
 
 LEARNING_RATE = 0.01
 N_QUBITS = 4
 DEPTH = 3
 VARIABLES = ("x", "y")
-X_POS = 0
-Y_POS = 1
-N_POINTS = 150
+NUM_VARIABLES = len(VARIABLES)
+X_POS, Y_POS = [i for i in range(NUM_VARIABLES)]
+BATCH_SIZE = 150
 N_EPOCHS = 1000
 
+def total_magnetization(n_qubits:int) -> Callable:
+    paulis = [Z(i) for i in range(n_qubits)]
 
-def ansatz_w_params(n_qubits: int, n_layers: int) -> tuple[list, list]:
-    all_ops = []
-    param_names = []
-    rots_fns = [RX, RY, RX]
-    for _ in range(n_layers):
-        for i in range(n_qubits):
-            ops = [
-                fn(str(uuid4()), qubit)
-                for fn, qubit in zip(rots_fns, [i for _ in range(len(rots_fns))])
-            ]
-            param_names += [op.param for op in ops]
-            ops += [NOT((i + 1) % n_qubits, i % n_qubits) for i in range(n_qubits)]
-            all_ops += ops
-
-    return all_ops, param_names
-
-
-@dataclass
-class TotalMagnetization:
-    n_qubits: int
-
-    def __post_init__(self) -> None:
-        self.paulis = [Z(i) for i in range(self.n_qubits)]
-
-    def __call__(self, state: Array, values: dict) -> Array:
-        return reduce(add, [apply_gate(state, pauli, values) for pauli in self.paulis])
-
+    def _total_magnetization(out_state: Array, values: dict[str, Array]) -> Array:
+        projected_state = reduce(
+            add, [apply_gate(out_state, pauli, values) for pauli in paulis]
+        )
+        return inner(out_state, projected_state).real
+    return _total_magnetization
 
-@dataclass
-class Circuit:
-    n_qubits: int
-    n_layers: int
 
+class DQC(Circuit):
     def __post_init__(self) -> None:
-        self.feature_map: list[Primitive] = [RX("x", i) for i in range(self.n_qubits // 2)] + [
-            RX("y", i) for i in range(self.n_qubits // 2, self.n_qubits)
-        ]
-        self.ansatz, self.param_names = ansatz_w_params(self.n_qubits, self.n_layers)
-        self.observable = TotalMagnetization(self.n_qubits)
+        self.ansatz = group_by_index(self.ansatz)
+        self.observable = total_magnetization(self.n_qubits)
+        self.state = zero_state(self.n_qubits)
 
     def __call__(self, param_vals: Array, x: Array, y: Array) -> Array:
-        state = zero_state(self.n_qubits)
         param_dict = {name: val for name, val in zip(self.param_names, param_vals)}
         out_state = apply_gate(
-            state, self.feature_map + self.ansatz, {**param_dict, **{"x": x, "y": y}}
+            self.state, self.feature_map + self.ansatz, {**param_dict, **{"x": x, "y": y}}
         )
-        projected_state = self.observable(state, param_dict)
-        return jnp.real(inner(out_state, projected_state))
+        return self.observable(out_state, {})
 
-    @property
-    def n_vparams(self) -> int:
-        return len(self.param_names)
 
-
-circ = Circuit(N_QUBITS, DEPTH)
+fm =  [RX("x", i) for i in range(N_QUBITS // 2)] + [
+            RX("y", i) for i in range(N_QUBITS // 2, N_QUBITS)
+        ]
+ansatz = hea(N_QUBITS, DEPTH)
+circ = DQC(N_QUBITS, fm, ansatz)
 # Create random initial values for the parameters
 key = jax.random.PRNGKey(42)
 param_vals = jax.random.uniform(key, shape=(circ.n_vparams,))
 
 optimizer = optax.adam(learning_rate=0.01)
 opt_state = optimizer.init(param_vals)
 
 
-def exp_fn(param_vals: Array, x: Array, y: Array) -> Array:
-    return circ(param_vals, x, y)
-
-
-def loss_fn(param_vals: Array, x: Array, y: Array) -> Array:
-    def pde_loss(x: float, y: float) -> Array:
-        l_b, r_b, t_b, b_b = list(
-            map(
-                lambda xy: exp_fn(param_vals, *xy),
-                [
-                    [jnp.zeros((1, 1)), y],  # u(0,y)=0
-                    [jnp.ones((1, 1)), y],  # u(L,y)=0
-                    [x, jnp.ones((1, 1))],  # u(x,H)=0
-                    [x, jnp.zeros((1, 1))],  # u(x,0)=f(x)
-                ],
-            )
+def loss_fn(param_vals: Array) -> Array:
+    def pde_loss(x: Array, y: Array) -> Array:
+        x = x.reshape(-1, 1)
+        y = y.reshape(-1, 1)
+        left = (jnp.zeros_like(y), y)  # u(0,y)=0
+        right = (jnp.ones_like(y), y)  # u(L,y)=0
+        top = (x, jnp.ones_like(x))  # u(x,H)=0
+        bottom = (x, jnp.zeros_like(x))  # u(x,0)=f(x)
+        terms = jnp.dstack(list(map(jnp.hstack, [left, right, top, bottom])))
+        loss_left, loss_right, loss_top, loss_bottom = vmap(lambda xy: circ(param_vals, xy[:, 0], xy[:, 1]), in_axes=(2,))(
+            terms
         )
-        b_b -= jnp.sin(jnp.pi * x)
-        hessian = jax.hessian(lambda xy: exp_fn(param_vals, xy[0], xy[1]))(
+        loss_bottom -= jnp.sin(jnp.pi * x)
+        hessian = jax.hessian(lambda xy: circ(param_vals, xy[0], xy[1]))(
             jnp.concatenate(
                 [
                     x.reshape(
                         1,
                     ),
                     y.reshape(
                         1,
                     ),
                 ]
             )
         )
-        interior = hessian[X_POS][X_POS] + hessian[Y_POS][Y_POS]  # uxx+uyy=0
-        return reduce(add, list(map(lambda term: jnp.power(term, 2), [l_b, r_b, t_b, b_b, interior])))
+        loss_interior = hessian[X_POS][X_POS] + hessian[Y_POS][Y_POS]  # uxx+uyy=0
+        return jnp.sum(
+            jnp.concatenate(
+                list(
+                    map(
+                        lambda term: jnp.power(term, 2).reshape(-1, 1),
+                        [loss_left, loss_right, loss_top, loss_bottom, loss_interior],
+                    )
+                )
+            )
+        )
 
-    return jnp.mean(vmap(pde_loss, in_axes=(0, 0))(x, y))
+    return jnp.mean(vmap(pde_loss, in_axes=(0, 0))(*uniform(0, 1.0, (NUM_VARIABLES, BATCH_SIZE))))
 
 
 def optimize_step(param_vals: Array, opt_state: Array, grads: dict[str, Array]) -> tuple:
     updates, opt_state = optimizer.update(grads, opt_state, param_vals)
     param_vals = optax.apply_updates(param_vals, updates)
     return param_vals, opt_state
 
 
-# collocation points sampling and training
-def sample_points(n_in: int, n_p: int) -> Array:
-    return uniform(0, 1.0, (n_in, n_p))
-
-
 @jit
 def train_step(i: int, paramvals_w_optstate: tuple) -> tuple:
     param_vals, opt_state = paramvals_w_optstate
-    x, y = sample_points(2, N_POINTS)
-    loss, grads = value_and_grad(loss_fn)(param_vals, x, y)
+    loss, grads = value_and_grad(loss_fn)(param_vals)
     return optimize_step(param_vals, opt_state, grads)
 
 
 param_vals, opt_state = jax.lax.fori_loop(0, N_EPOCHS, train_step, (param_vals, opt_state))
 # compare the solution to known ground truth
-single_domain = jnp.linspace(0, 1, num=N_POINTS)
+single_domain = jnp.linspace(0, 1, num=BATCH_SIZE)
 domain = jnp.array(list(product(single_domain, single_domain)))
 # analytical solution
 analytic_sol = (
-    (np.exp(-np.pi * domain[:, 0]) * np.sin(np.pi * domain[:, 1])).reshape(N_POINTS, N_POINTS).T
+    (np.exp(-np.pi * domain[:, 0]) * np.sin(np.pi * domain[:, 1])).reshape(BATCH_SIZE, BATCH_SIZE).T
 )
 # DQC solution
-
-dqc_sol = vmap(lambda domain: exp_fn(param_vals, domain[0], domain[1]), in_axes=(0,))(domain).reshape(
-    N_POINTS, N_POINTS
-)
+dqc_sol = vmap(lambda domain: circ(param_vals, domain[0], domain[1]), in_axes=(0,))(
+    domain
+).reshape(BATCH_SIZE, BATCH_SIZE)
 # # plot results
 fig, ax = plt.subplots(1, 2, figsize=(7, 7))
 ax[0].imshow(analytic_sol, cmap="turbo")
 ax[0].set_xlabel("x")
 ax[0].set_ylabel("y")
 ax[0].set_title("Analytical solution u(x,y)")
 ax[1].imshow(dqc_sol, cmap="turbo")
```

### Comparing `horqrux-0.6.1/horqrux/adjoint.py` & `horqrux-0.6.2/horqrux/adjoint.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,51 +1,59 @@
 from __future__ import annotations
 
 from typing import Tuple
 
 from jax import Array, custom_vjp
-from jax.numpy import real as jnpreal
 
 from horqrux.apply import apply_gate
 from horqrux.parametric import Parametric
 from horqrux.primitive import Primitive
 from horqrux.utils import OperationType, inner
 
 
 def expectation(
     state: Array, gates: list[Primitive], observable: list[Primitive], values: dict[str, float]
 ) -> Array:
+    """
+    Run 'state' through a sequence of 'gates' given parameters 'values'
+    and compute the expectation given an observable.
+    """
     out_state = apply_gate(state, gates, values, OperationType.UNITARY)
     projected_state = apply_gate(out_state, observable, values, OperationType.UNITARY)
-    return jnpreal(inner(out_state, projected_state))
+    return inner(out_state, projected_state).real
 
 
 @custom_vjp
 def adjoint_expectation(
     state: Array, gates: list[Primitive], observable: list[Primitive], values: dict[str, float]
 ) -> Array:
     return expectation(state, gates, observable, values)
 
 
 def adjoint_expectation_fwd(
     state: Array, gates: list[Primitive], observable: list[Primitive], values: dict[str, float]
 ) -> Tuple[Array, Tuple[Array, Array, list[Primitive], dict[str, float]]]:
     out_state = apply_gate(state, gates, values, OperationType.UNITARY)
     projected_state = apply_gate(out_state, observable, values, OperationType.UNITARY)
-    return jnpreal(inner(out_state, projected_state)), (out_state, projected_state, gates, values)
+    return inner(out_state, projected_state).real, (out_state, projected_state, gates, values)
 
 
 def adjoint_expectation_bwd(
     res: Tuple[Array, Array, list[Primitive], dict[str, float]], tangent: Array
 ) -> tuple:
+    """Implementation of Algorithm 1 of https://arxiv.org/abs/2009.02823
+    which computes the vector-jacobian product in O(P) time using O(1) state vectors
+    where P=number of parameters in the circuit.
+    """
+
     out_state, projected_state, gates, values = res
     grads = {}
     for gate in gates[::-1]:
         out_state = apply_gate(out_state, gate, values, OperationType.DAGGER)
         if isinstance(gate, Parametric):
             mu = apply_gate(out_state, gate, values, OperationType.JACOBIAN)
-            grads[gate.param] = tangent * 2 * jnpreal(inner(mu, projected_state))
+            grads[gate.param] = tangent * 2 * inner(mu, projected_state).real
         projected_state = apply_gate(projected_state, gate, values, OperationType.DAGGER)
     return (None, None, None, grads)
 
 
 adjoint_expectation.defvjp(adjoint_expectation_fwd, adjoint_expectation_bwd)
```

### Comparing `horqrux-0.6.1/horqrux/analog.py` & `horqrux-0.6.2/horqrux/analog.py`

 * *Files identical despite different names*

### Comparing `horqrux-0.6.1/horqrux/matrices.py` & `horqrux-0.6.2/horqrux/matrices.py`

 * *Files identical despite different names*

### Comparing `horqrux-0.6.1/horqrux/parametric.py` & `horqrux-0.6.2/horqrux/parametric.py`

 * *Files identical despite different names*

### Comparing `horqrux-0.6.1/horqrux/primitive.py` & `horqrux-0.6.2/horqrux/primitive.py`

 * *Files identical despite different names*

### Comparing `horqrux-0.6.1/horqrux/utils.py` & `horqrux-0.6.2/horqrux/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -119,30 +119,30 @@
 
 
 def inner(state: Array, projection: Array) -> Array:
     return jnp.dot(jnp.conj(state.flatten()), projection.flatten())
 
 
 def overlap(state: Array, projection: Array) -> Array:
-    return jnp.real(jnp.power(inner(state, projection), 2))
+    return jnp.power(inner(state, projection), 2).real
 
 
 def uniform_state(
     n_qubits: int,
 ) -> Array:
     state = jnp.ones(2**n_qubits, dtype=jnp.complex128)
     state = state / jnp.sqrt(jnp.array(2**n_qubits, dtype=jnp.complex128))
     return state.reshape([2] * n_qubits)
 
 
-def is_controlled(qs: Tuple[int | None, ...] | int | None) -> bool:
-    if isinstance(qs, int):
+def is_controlled(qubit_support: Tuple[int | None, ...] | int | None) -> bool:
+    if isinstance(qubit_support, int):
         return True
-    elif isinstance(qs, tuple):
-        return any(is_controlled(q) for q in qs)
+    elif isinstance(qubit_support, tuple):
+        return any(is_controlled(q) for q in qubit_support)
     return False
 
 
 def random_state(n_qubits: int) -> Array:
     def _normalize(wf: Array) -> Array:
         return wf / jnp.sqrt((jnp.sum(jnp.abs(wf) ** 2)))
```

### Comparing `horqrux-0.6.1/tests/test_adjoint.py` & `horqrux-0.6.2/tests/test_adjoint.py`

 * *Files identical despite different names*

### Comparing `horqrux-0.6.1/tests/test_analog.py` & `horqrux-0.6.2/tests/test_analog.py`

 * *Files identical despite different names*

### Comparing `horqrux-0.6.1/tests/test_gates.py` & `horqrux-0.6.2/tests/test_gates.py`

 * *Files 15% similar despite different names*

```diff
@@ -98,7 +98,23 @@
     ],
 )
 def test_swap_gate(inputs: tuple[str, str, Array]) -> None:
     bitstring, expected_bitstring, op = inputs
     state = product_state(bitstring)
     out_state = apply_gate(state, op)
     assert equivalent_state(out_state, product_state(expected_bitstring))
+
+
+def test_merge_gates() -> None:
+    gates = [RX("a", 0), RZ("b", 1), RY("c", 0), NOT(1, 2), RX("a", 0, 3), RZ("c", 3)]
+    values = {
+        "a": np.random.uniform(0.1, 2 * np.pi),
+        "b": np.random.uniform(0.1, 2 * np.pi),
+        "c": np.random.uniform(0.1, 2 * np.pi),
+    }
+    state_grouped = apply_gate(
+        product_state("0000"), gates, values, "unitary", group_gates=True, merge_ops=True
+    )
+    state = apply_gate(
+        product_state("0000"), gates, values, "unitary", group_gates=False, merge_ops=False
+    )
+    assert jnp.allclose(state_grouped, state)
```

### Comparing `horqrux-0.6.1/.gitignore` & `horqrux-0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `horqrux-0.6.1/LICENSE` & `horqrux-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `horqrux-0.6.1/pyproject.toml` & `horqrux-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 authors = [
     { name = "Gert-Jan Both" , email = "gert-jan.both@pasqal.com" },
     { name = "Dominik Seitz", email = "dominik.seitz@pasqal.com" },
 ]
 requires-python = ">=3.8,<3.13"
 license = {text = "Apache 2.0"}
 
-version = "0.6.1"
+version = "0.6.2"
 
 classifiers=[
     "License :: Other/Proprietary License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
```

### Comparing `horqrux-0.6.1/PKG-INFO` & `horqrux-0.6.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: horqrux
-Version: 0.6.1
+Version: 0.6.2
 Summary: Jax-based quantum state vector simulator.
 Author-email: Gert-Jan Both <gert-jan.both@pasqal.com>, Dominik Seitz <dominik.seitz@pasqal.com>
 License: Apache 2.0
 License-File: LICENSE
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

