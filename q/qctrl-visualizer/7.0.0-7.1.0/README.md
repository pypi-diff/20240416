# Comparing `tmp/qctrl_visualizer-7.0.0.tar.gz` & `tmp/qctrl_visualizer-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qctrl_visualizer-7.0.0.tar", max compression
+gzip compressed data, was "qctrl_visualizer-7.1.0.tar", max compression
```

## Comparing `qctrl_visualizer-7.0.0.tar` & `qctrl_visualizer-7.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    36587 2024-02-05 03:27:46.149646 qctrl_visualizer-7.0.0/LICENSE
--rw-r--r--   0        0        0      754 2024-02-05 03:27:46.149646 qctrl_visualizer-7.0.0/README.md
--rw-r--r--   0        0        0     2481 2024-02-05 03:28:07.013981 qctrl_visualizer-7.0.0/pyproject.toml
--rw-r--r--   0        0        0     2232 2024-02-05 03:28:07.025981 qctrl_visualizer-7.0.0/qctrlvisualizer/__init__.py
--rw-r--r--   0        0        0    23367 2024-02-05 03:27:46.153646 qctrl_visualizer-7.0.0/qctrlvisualizer/bloch.py
--rw-r--r--   0        0        0    14038 2024-02-05 03:27:46.153646 qctrl_visualizer-7.0.0/qctrlvisualizer/confidence_ellipses.py
--rw-r--r--   0        0        0    16085 2024-02-05 03:27:46.153646 qctrl_visualizer-7.0.0/qctrlvisualizer/controls.py
--rw-r--r--   0        0        0     4593 2024-02-05 03:27:46.153646 qctrl_visualizer-7.0.0/qctrlvisualizer/cost_histories.py
--rw-r--r--   0        0        0     7393 2024-02-05 03:27:46.153646 qctrl_visualizer-7.0.0/qctrlvisualizer/density_matrix.py
--rw-r--r--   0        0        0     9848 2024-02-05 03:27:46.153646 qctrl_visualizer-7.0.0/qctrlvisualizer/filter_functions.py
--rw-r--r--   0        0        0     6612 2024-02-05 03:27:46.153646 qctrl_visualizer-7.0.0/qctrlvisualizer/histogram.py
--rw-r--r--   0        0        0    12517 2024-02-05 03:27:46.153646 qctrl_visualizer-7.0.0/qctrlvisualizer/populations.py
--rw-r--r--   0        0        0     4549 2024-02-05 03:27:46.153646 qctrl_visualizer-7.0.0/qctrlvisualizer/style.py
--rw-r--r--   0        0        0     4535 2024-02-05 03:27:46.153646 qctrl_visualizer-7.0.0/qctrlvisualizer/utils.py
--rw-r--r--   0        0        0     5555 2024-02-05 03:27:46.153646 qctrl_visualizer-7.0.0/qctrlvisualizer/wigner_function.py
--rw-r--r--   0        0        0     2699 1970-01-01 00:00:00.000000 qctrl_visualizer-7.0.0/PKG-INFO
+-rw-r--r--   0        0        0    36587 2024-04-16 06:02:29.909304 qctrl_visualizer-7.1.0/LICENSE
+-rw-r--r--   0        0        0      754 2024-04-16 06:02:29.909304 qctrl_visualizer-7.1.0/README.md
+-rw-r--r--   0        0        0     2516 2024-04-16 06:02:54.297332 qctrl_visualizer-7.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2232 2024-04-16 06:02:54.305332 qctrl_visualizer-7.1.0/qctrlvisualizer/__init__.py
+-rw-r--r--   0        0        0    23367 2024-04-16 06:02:29.913304 qctrl_visualizer-7.1.0/qctrlvisualizer/bloch.py
+-rw-r--r--   0        0        0    14010 2024-04-16 06:02:29.913304 qctrl_visualizer-7.1.0/qctrlvisualizer/confidence_ellipses.py
+-rw-r--r--   0        0        0    16082 2024-04-16 06:02:29.913304 qctrl_visualizer-7.1.0/qctrlvisualizer/controls.py
+-rw-r--r--   0        0        0     4660 2024-04-16 06:02:29.913304 qctrl_visualizer-7.1.0/qctrlvisualizer/cost_histories.py
+-rw-r--r--   0        0        0     7731 2024-04-16 06:02:29.913304 qctrl_visualizer-7.1.0/qctrlvisualizer/density_matrix.py
+-rw-r--r--   0        0        0     9996 2024-04-16 06:02:29.913304 qctrl_visualizer-7.1.0/qctrlvisualizer/filter_functions.py
+-rw-r--r--   0        0        0     6661 2024-04-16 06:02:29.913304 qctrl_visualizer-7.1.0/qctrlvisualizer/histogram.py
+-rw-r--r--   0        0        0    12615 2024-04-16 06:02:29.913304 qctrl_visualizer-7.1.0/qctrlvisualizer/populations.py
+-rw-r--r--   0        0        0     4534 2024-04-16 06:02:29.913304 qctrl_visualizer-7.1.0/qctrlvisualizer/style.py
+-rw-r--r--   0        0        0     5241 2024-04-16 06:02:29.913304 qctrl_visualizer-7.1.0/qctrlvisualizer/utils.py
+-rw-r--r--   0        0        0     5623 2024-04-16 06:02:29.913304 qctrl_visualizer-7.1.0/qctrlvisualizer/wigner_function.py
+-rw-r--r--   0        0        0     2699 1970-01-01 00:00:00.000000 qctrl_visualizer-7.1.0/PKG-INFO
```

### Comparing `qctrl_visualizer-7.0.0/LICENSE` & `qctrl_visualizer-7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qctrl_visualizer-7.0.0/README.md` & `qctrl_visualizer-7.1.0/README.md`

 * *Files identical despite different names*

### Comparing `qctrl_visualizer-7.0.0/pyproject.toml` & `qctrl_visualizer-7.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qctrl-visualizer"
-version = "7.0.0"
+version = "7.1.0"
 description = "Q-CTRL Visualizer"
 license = "https://q-ctrl.com/terms"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "README.md"
 homepage = "https://q-ctrl.com"
 documentation = "https://docs.q-ctrl.com/boulder-opal/references/qctrl-visualizer/"
@@ -60,27 +60,28 @@
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.12"
 matplotlib = ">=3.6.3"
 numpy = "^1.23.5"
 scipy = ">=1.9.3"
-qctrl-commons = "^21.2.4"
+qctrl-commons = "^22.1.0"
 
 [tool.poetry.dev-dependencies]
-black = "^23.7.0"
+black = "^24.3.0"
 docopt = "~0.6.2"
 isort = "^5.12.0"
-mypy = "^1.4.1"
+mypy = "^1.9.0"
 pre-commit = "^3.3.3"
 pylint = "^2.17.5"
 pytest = "^7.4.0"
 sphinx = "^5.3.0"
 qctrl-sphinx-theme = "^2.1.4"
 tomli = "^2.0.1"
+sphinx-markdown-builder = "^0.6.6"
 
 [[tool.poetry.source]]
 name = "PyPI"
 priority = "supplemental"
 
 [[tool.poetry.source]]
 name = 'Q-CTRL PyPI'
```

### Comparing `qctrl_visualizer-7.0.0/qctrlvisualizer/__init__.py` & `qctrl_visualizer-7.1.0/qctrlvisualizer/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,8 +65,8 @@
     "plot_population_dynamics",
     "plot_population_distributions",
     "plot_bitstring_probabilities_histogram",
     "plot_sequences",
     "plot_wigner_function",
 ]
 
-__version__ = "7.0.0"
+__version__ = "7.1.0"
```

### Comparing `qctrl_visualizer-7.0.0/qctrlvisualizer/bloch.py` & `qctrl_visualizer-7.1.0/qctrlvisualizer/bloch.py`

 * *Files identical despite different names*

### Comparing `qctrl_visualizer-7.0.0/qctrlvisualizer/confidence_ellipses.py` & `qctrl_visualizer-7.1.0/qctrlvisualizer/confidence_ellipses.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,44 +14,42 @@
 """
 Functions for plotting confidence ellipses.
 """
 from __future__ import annotations
 
 from typing import Optional
 
-import matplotlib.pyplot as plt
 import numpy as np
-from qctrlcommons.preconditions import (
-    check_argument,
-    check_argument_positive_integer,
-)
+from matplotlib.figure import Figure
+from qctrlcommons.preconditions import check_argument
 from scipy.linalg import fractional_matrix_power
 from scipy.special import betaincinv
 
 from .style import (
     FIG_HEIGHT,
     QCTRL_STYLE_COLORS,
     qctrl_style,
 )
 from .utils import (
+    check_positive_scalar,
     create_axes,
     create_figure,
     get_units,
 )
 
 
 @qctrl_style()
 def plot_confidence_ellipses(
     ellipse_matrix: np.ndarray,
     estimated_parameters: np.ndarray,
     actual_parameters: Optional[np.ndarray] = None,
     parameter_names: Optional[list[str]] = None,
     parameter_units: str | list[str] = "Hz",
     *,
-    figure: Optional[plt.Figure] = None,
+    figure: Optional[Figure] = None,
 ):
     r"""
     Create an array of confidence ellipse plots.
 
     From an (N,N) matrix transformation and N estimated parameters,
     plots the confidence ellipse for each pair of parameters.
 
@@ -340,15 +338,15 @@
         hessian.shape == (parameter_count, parameter_count),
         "Hessian must be a square matrix.",
         {"hessian": hessian},
     )
 
     check_argument(cost > 0, "The cost must be positive.", {"cost": cost})
 
-    check_argument_positive_integer(measurement_count, "measurement_count")
+    check_positive_scalar(measurement_count, "measurement_count")
 
     check_argument(
         0 < confidence_fraction < 1,
         "The confidence fraction must be between 0 and 1.",
         {"confidence_fraction": confidence_fraction},
     )
```

### Comparing `qctrl_visualizer-7.0.0/qctrlvisualizer/controls.py` & `qctrl_visualizer-7.1.0/qctrlvisualizer/controls.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 
 from collections import namedtuple
 from typing import (
     Any,
     Optional,
 )
 
-import matplotlib.pyplot as plt
 import numpy as np
+from matplotlib.figure import Figure
 from qctrlcommons.preconditions import check_argument
 
 from .style import (
     FIG_WIDTH,
     qctrl_style,
 )
 from .utils import (
@@ -42,15 +42,15 @@
 def plot_controls(
     controls: dict,
     polar: bool = True,
     smooth: bool = False,
     unit_symbol: str = "Hz",
     two_pi_factor: bool = True,
     *,
-    figure: Optional[plt.Figure] = None,
+    figure: Optional[Figure] = None,
 ):
     """
     Create a plot of the specified controls.
 
     Parameters
     ----------
     controls : dict
@@ -290,15 +290,15 @@
             values=np.imag(scaled_values) / prefix_scaling_y,
             ylabel=f"{scaled_name}\nQ\n({prefix_y}{unit_symbol})",
         ),
     ]
 
 
 @qctrl_style()
-def plot_sequences(sequences: dict, *, figure: Optional[plt.Figure] = None):
+def plot_sequences(sequences: dict, *, figure: Optional[Figure] = None):
     """
     Create a plot of dynamical decoupling sequences.
 
     Parameters
     ----------
     sequences : dict
         The dictionary of sequences to plot. Works the same as the dictionary for
```

### Comparing `qctrl_visualizer-7.0.0/qctrlvisualizer/cost_histories.py` & `qctrl_visualizer-7.1.0/qctrlvisualizer/cost_histories.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,29 +15,30 @@
 Functions for plotting cost vs iterations.
 """
 
 from __future__ import annotations
 
 from typing import Optional
 
-import matplotlib.pyplot as plt
+from matplotlib.axes import Axes
+from matplotlib.figure import Figure
 from qctrlcommons.preconditions import check_argument
 
 from .style import qctrl_style
 from .utils import create_figure
 
 
 @qctrl_style()
 def plot_cost_histories(
     cost_histories: list,
     labels: Optional[list[str]] = None,
     y_axis_log: bool = False,
     initial_iteration: int = 1,
     *,
-    figure: Optional[plt.Figure] = None,
+    figure: Optional[Figure] = None,
 ):
     """
     Create a plot of the cost against iterations for either a single cost history or
     a set of cost histories.
 
     Parameters
     ----------
@@ -92,14 +93,15 @@
         plot_cost_histories(
             cost_histories=cost_histories, labels=["CMA-ES", "Simulated annealing"]
         )
         plt.tight_layout()
     """
     figure = create_figure(figure)
     axs = figure.subplots(nrows=1, ncols=1)
+    assert isinstance(axs, Axes)
 
     check_argument(
         isinstance(cost_histories, list),
         "The cost histories must be in a list.",
         {"cost_histories": cost_histories},
     )
```

### Comparing `qctrl_visualizer-7.0.0/qctrlvisualizer/density_matrix.py` & `qctrl_visualizer-7.1.0/qctrlvisualizer/density_matrix.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,19 +17,17 @@
 """
 from __future__ import annotations
 
 from typing import Optional
 
 import matplotlib.pyplot as plt
 import numpy as np
-from qctrlcommons.preconditions import (
-    check_argument,
-    check_argument_hermitian,
-    check_numeric_numpy_array,
-)
+from matplotlib.axes import Axes
+from matplotlib.figure import Figure
+from qctrlcommons.preconditions import check_argument
 
 from .style import (
     BORDER_COLOR,
     QCTRL_SEQUENTIAL_COLORMAP,
     qctrl_style,
 )
 from .utils import (
@@ -41,15 +39,15 @@
 
 @qctrl_style()
 def plot_density_matrix(
     density_matrix: np.ndarray,
     basis_labels: Optional[list[str]] = None,
     rotate_column_labels: bool = False,
     *,
-    figure: Optional[plt.Figure] = None,
+    figure: Optional[Figure] = None,
 ):
     """
     Create a heatmap with the absolute values of a density matrix's elements.
 
     Parameters
     ----------
     density_matrix : np.ndarray
@@ -103,14 +101,15 @@
     """
     figure = create_figure(figure)
     absolute_density_matrix = _validate_density_matrix(density_matrix)
     dimension = len(absolute_density_matrix)
     row_labels, col_labels = _validate_basis_labels(basis_labels, dimension)
 
     axes = figure.subplots(nrows=1, ncols=1)
+    assert isinstance(axes, Axes)
 
     if rotate_column_labels:
         rotation = 90
     else:
         rotation = 0
     axes.set_yticks(np.arange(dimension), labels=row_labels)
     axes.set_xticks(np.arange(dimension), labels=col_labels, rotation=rotation)
@@ -121,15 +120,15 @@
     )
 
     pixels = 1 / plt.rcParams["figure.dpi"]
     bbox = axes.get_window_extent().transformed(figure.dpi_scale_trans.inverted())
     width = bbox.width
     legend_distance = 16 * pixels / width
 
-    color_bar = axes.figure.colorbar(density_plot, ax=axes, pad=legend_distance)
+    color_bar = axes.figure.colorbar(density_plot, ax=axes, pad=legend_distance)  # type: ignore
     color_bar.ax.set_ylabel(
         "Absolute values of matrix elements", rotation=-90, labelpad=16, va="bottom"
     )
     color_bar.ax.yaxis.set_tick_params(pad=8)
 
     plt.hlines(
         y=np.arange(0, dimension) + 0.5,
@@ -149,20 +148,28 @@
 
 def _validate_density_matrix(density_matrix: np.ndarray) -> np.ndarray:
     """
     Validate the input density matrix and compute its element-wise absolute values.
     """
 
     check_argument(
-        isinstance(density_matrix, np.ndarray),
-        "The density matrix has to be a NumPy array.",
+        isinstance(density_matrix, np.ndarray) and density_matrix.dtype.kind in "iufc",
+        "The density matrix must be a numeric NumPy array.",
+        {"density_matrix": density_matrix},
+    )
+    check_argument(
+        density_matrix.ndim == 2 and density_matrix.shape[0] == density_matrix.shape[1],
+        "The density matrix must be square.",
+        {"density_matrix": density_matrix},
+    )
+    check_argument(
+        np.allclose(density_matrix, density_matrix.T.conj()),
+        "The density matrix must be Hermitian, but does not equal its Hermitian conjugate.",
         {"density_matrix": density_matrix},
     )
-
-    check_numeric_numpy_array(density_matrix, "density_matrix")
 
     diagonal_elements = np.diagonal(density_matrix)
     check_argument(
         all(np.isreal(diagonal_elements)),
         "The diagonal elements of the density matrix must be real.",
         {"density_matrix": density_matrix},
         extras={"diag(density_matrix)": diagonal_elements},
@@ -179,19 +186,15 @@
     check_argument(
         np.isclose(sum(diagonal_elements), 1),
         "The trace of the density matrix must be 1.",
         {"density_matrix": density_matrix},
         extras={"trace(density_matrix)": sum(diagonal_elements)},
     )
 
-    check_argument_hermitian(density_matrix, "density_matrix")
-
-    absolute_density_matrix = np.absolute(density_matrix)
-
-    return absolute_density_matrix
+    return np.absolute(density_matrix)
 
 
 def _validate_basis_labels(
     basis_labels: Optional[list[str]], dimension
 ) -> tuple[list[str], list[str]]:
     """
     Validate the input `basis_labels` if passed and set to default if not.
```

### Comparing `qctrl_visualizer-7.0.0/qctrlvisualizer/filter_functions.py` & `qctrl_visualizer-7.1.0/qctrlvisualizer/filter_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,17 @@
 Functions for plotting filter functions.
 """
 
 from __future__ import annotations
 
 from typing import Optional
 
-import matplotlib.pyplot as plt
 import numpy as np
+from matplotlib.axes import Axes
+from matplotlib.figure import Figure
 from qctrlcommons.preconditions import check_argument
 
 from .style import qctrl_style
 from .utils import (
     create_figure,
     get_units,
 )
@@ -32,15 +33,15 @@
 @qctrl_style()
 def plot_filter_functions(
     filter_functions: dict,
     show_legend: bool = True,
     x_axis_log: bool = True,
     y_axis_log: bool = True,
     *,
-    figure: Optional[plt.Figure] = None,
+    figure: Optional[Figure] = None,
 ):
     r"""
     Create a plot of the specified filter functions.
 
     Parameters
     ----------
     filter_functions : dict
@@ -161,30 +162,33 @@
     check_argument(
         filter_functions,
         "At least one filter function must be provided.",
         {"filter_functions": filter_functions},
     )
 
     axes = figure.subplots(nrows=1, ncols=1)
+    assert isinstance(axes, Axes)
 
     all_frequencies = []
     all_inverse_powers = []
     all_uncertainties = []
     for name, filter_function in filter_functions.items():
         if isinstance(filter_function, list):
             frequencies, inverse_powers, inverse_power_uncertainties = np.array(
                 list(
                     zip(
                         *[
                             (
                                 sample["frequency"],
                                 sample["inverse_power"],
-                                sample["inverse_power_uncertainty"]
-                                if "inverse_power_uncertainty" in sample
-                                else sample.get("inverse_power_precision", 0.0),
+                                (
+                                    sample["inverse_power_uncertainty"]
+                                    if "inverse_power_uncertainty" in sample
+                                    else sample.get("inverse_power_precision", 0.0)
+                                ),
                             )
                             for sample in filter_function
                         ]
                     )
                 )
             )
         else:
```

### Comparing `qctrl_visualizer-7.0.0/qctrlvisualizer/histogram.py` & `qctrl_visualizer-7.1.0/qctrlvisualizer/histogram.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,31 +7,31 @@
 #
 #    https://q-ctrl.com/terms
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 
-
 """
 Function for plotting histograms.
 """
 from __future__ import annotations
 
 from typing import Optional
 
-import matplotlib.pyplot as plt
 import numpy as np
-from qctrlcommons.preconditions import (
-    check_argument,
-    check_argument_non_negative_scalar,
-)
+from matplotlib.axes import Axes
+from matplotlib.figure import Figure
+from qctrlcommons.preconditions import check_argument
 
 from .style import qctrl_style
-from .utils import create_figure
+from .utils import (
+    check_non_negative_scalar,
+    create_figure,
+)
 
 
 def _validate_bitstring_counts(bitstring_counts: dict[str, dict[str, int]]) -> int:
     """
     Validate the input arguments of `plot_bitstring_probabilities_histogram`.
 
     Parameters
@@ -66,15 +66,15 @@
         )
 
     first_key = next(iter(bitstring_counts))
     bitstring_length = len(next(iter(bitstring_counts[first_key])))
 
     for experiment, counts in bitstring_counts.items():
         for bitstring, count in counts.items():
-            check_argument_non_negative_scalar(
+            check_non_negative_scalar(
                 count, f'bitstring_counts["{experiment}"]["{bitstring}"]'
             )
             check_argument(
                 len(bitstring) == bitstring_length,
                 "The length of all bitstrings must be the same.",
                 {"bitstring_counts": bitstring_counts},
                 extras={"first bitstring length": bitstring_length},
@@ -86,15 +86,15 @@
 @qctrl_style()
 def plot_bitstring_probabilities_histogram(
     bitstring_counts: dict[str, dict[str, int]],
     show_legend: bool = True,
     rotate_x_axis_labels: bool = True,
     display_all_bitstrings: bool = False,
     *,
-    figure: Optional[plt.Figure] = None,
+    figure: Optional[Figure] = None,
 ):
     """
     Create a histogram of the specified counts.
 
     Parameters
     ----------
     bitstring_counts : dict[str, dict[str,int]]
@@ -152,14 +152,15 @@
             np.binary_repr(i, bitstring_length) for i in range(2**bitstring_length)
         ]
     else:
         # Sort the bitstring labels.
         sorted_bitstrings = sorted(set().union(*list(bitstring_counts.values())))
 
     axes = figure.subplots(nrows=1, ncols=1)
+    assert isinstance(axes, Axes)
 
     default_bar_width = 0.8
     bar_width = default_bar_width / len(bitstring_counts)
 
     x_axis = np.arange(len(sorted_bitstrings))
 
     for bar_shift_index, (experiment, counts) in enumerate(bitstring_counts.items()):
```

### Comparing `qctrl_visualizer-7.0.0/qctrlvisualizer/populations.py` & `qctrl_visualizer-7.1.0/qctrlvisualizer/populations.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,30 +17,31 @@
 """
 from __future__ import annotations
 
 import warnings
 from collections import namedtuple
 from typing import Optional
 
-import matplotlib.pyplot as plt
 import numpy as np
+from matplotlib.axes import Axes
+from matplotlib.figure import Figure
 from qctrlcommons.preconditions import check_argument
 
 from .style import qctrl_style
 from .utils import (
     create_figure,
     get_units,
     safe_greater_than,
     safe_less_than,
 )
 
 
 @qctrl_style()
 def plot_population_dynamics(
-    sample_times: np.ndarray, populations: dict, *, figure: Optional[plt.Figure] = None
+    sample_times: np.ndarray, populations: dict, *, figure: Optional[Figure] = None
 ):
     r"""
     Create a plot of the dynamics of the specified populations.
 
     Parameters
     ----------
     sample_times : np.ndarray
@@ -116,14 +117,15 @@
         plt.tight_layout()
     """
 
     figure = create_figure(figure)
     population_data = _create_population_data(sample_times, populations)
 
     axes = figure.subplots(nrows=1, ncols=1)
+    assert isinstance(axes, Axes)
 
     scale, prefix = get_units(sample_times)
     for data in population_data:
         axes.plot(sample_times / scale, data.values, label=data.label)
 
     axes.set_xlabel(f"Time ({prefix}s)")
     axes.set_ylabel("Probability")
@@ -198,15 +200,15 @@
 @qctrl_style()
 def plot_population_distributions(
     populations: dict[str, np.ndarray],
     basis_labels: Optional[list[str]] = None,
     rotate_x_axis_labels: bool = False,
     show_legend: bool = True,
     *,
-    figure: Optional[plt.Figure] = None,
+    figure: Optional[Figure] = None,
 ):
     """
     Create a bar graph of the given population distributions.
 
     Parameters
     ----------
     populations : dict[str, np.ndarray]
@@ -256,14 +258,15 @@
         plt.tight_layout()
     """
     figure = create_figure(figure)
     dimension = _validate_populations(populations)
     basis_labels = _validate_basis_labels(basis_labels, dimension)
 
     axes = figure.subplots(nrows=1, ncols=1)
+    assert isinstance(axes, Axes)
 
     default_bar_width = 0.8
     bar_width = default_bar_width / len(populations)
 
     x_axis = np.arange(dimension)
 
     for vector_number, (vector_label, population) in enumerate(populations.items()):
```

### Comparing `qctrl_visualizer-7.0.0/qctrlvisualizer/style.py` & `qctrl_visualizer-7.1.0/qctrlvisualizer/style.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,22 +32,21 @@
 DPI = 72
 FIG_WIDTH = 10.0
 FIG_HEIGHT = 5.0
 
 #: A list of colors defined in the Q-CTRL style.
 QCTRL_STYLE_COLORS = [
     "#680CE9",
-    "#D84144",
-    "#32A4A8",
-    "#A2A933",
-    "#D84190",
-    "#4177D8",
-    "#D6722F",
-    "#D543ED",
-    "#32A857",
+    "#E04542",
+    "#2AA1A4",
+    "#B0AA31",
+    "#E54399",
+    "#4B7AD9",
+    "#DF7A30",
+    "#32A859",
 ]
 
 QCTRL_SEQUENTIAL_COLORMAP = LinearSegmentedColormap.from_list(
     "QCTRL_SEQUENTIAL_COLORMAP",
     ["#FFFFFF", "#EDE0FE", "#B482FA", "#680CE9", "#440087"],
     N=200,
 )
```

### Comparing `qctrl_visualizer-7.0.0/qctrlvisualizer/utils.py` & `qctrl_visualizer-7.1.0/qctrlvisualizer/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 
 from __future__ import annotations
 
 from typing import Optional
 
 import matplotlib.pyplot as plt
 import numpy as np
+from matplotlib.figure import Figure
 from matplotlib.ticker import ScalarFormatter
+from qctrlcommons.preconditions import check_argument
 
 from qctrlvisualizer.style import (
     DPI,
     FIG_HEIGHT,
     FIG_WIDTH,
 )
 
@@ -61,23 +63,25 @@
     # [0.001, 1) -> 0.001x/milli,
     # [1, 1000) -> no scaling,
     # [1000, 1e6) -> 1000x/kilo,
     # and so on.
     max_value = max(np.abs(values))
     exponent = float(
         3
-        * np.floor_divide(np.log10(max_value, out=np.zeros(1), where=max_value > 0), 3)
+        * np.floor_divide(
+            np.log10(max_value, out=np.zeros(1), where=max_value > 0), 3
+        ).item()
     )
     # Clip the scaling to the allowable range.
     exponent_clipped = np.clip(exponent, -24, 24)
     return 10**exponent_clipped, prefixes[exponent_clipped]
 
 
 def create_axes(
-    figure: plt.Figure,
+    figure: Figure,
     count_x: int,
     count_y: int,
     width: float,
     height: float,
     share_x: bool = False,
     share_y: bool = False,
 ) -> np.ndarray:
@@ -121,15 +125,15 @@
     for axes in axes_array.flat:
         axes.yaxis.set_major_formatter(ScalarFormatter())
         axes.xaxis.set_major_formatter(ScalarFormatter())
 
     return axes_array
 
 
-def create_figure(figure: Optional[plt.Figure]) -> plt.Figure:
+def create_figure(figure: Optional[Figure]) -> Figure:
     """
     Retun a new Figure object if the input is None.
     Otherwise, mutate it with the default figure settings.
     """
     if figure is None:
         return plt.figure()
 
@@ -153,7 +157,24 @@
 
 def safe_greater_than(array, bound):
     """
     Returns False if any of the elements of array are greater than bound (within rounding error).
     Returns True otherwise.
     """
     return np.any((1 - np.isclose(array, bound)) * (array > bound))
+
+
+def check_non_negative_scalar(value: int | float, name: str) -> None:
+    """
+    Check if a scalar argument >= 0.
+    """
+    check_argument(np.isscalar(value), f"{name} must be scalar.", {name: value})
+    check_argument(np.isreal(value), f"{name} must be real.", {name: value})
+    check_argument(value >= 0, f"{name} must not be negative.", {name: value})
+
+
+def check_positive_scalar(value: int | float, name: str) -> None:
+    """
+    Check if a scalar argument > 0.
+    """
+    check_non_negative_scalar(value, name)
+    check_argument(value != 0, f"{name} cannot be zero.", {name: value})
```

### Comparing `qctrl_visualizer-7.0.0/qctrlvisualizer/wigner_function.py` & `qctrl_visualizer-7.1.0/qctrlvisualizer/wigner_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,18 @@
 Functions for plotting cost vs iterations.
 """
 
 from __future__ import annotations
 
 from typing import Optional
 
-import matplotlib.pyplot as plt
 import numpy as np
+from matplotlib.axes import Axes
 from matplotlib.colors import TwoSlopeNorm
+from matplotlib.figure import Figure
 from qctrlcommons.preconditions import check_argument
 
 from .style import (
     QCTRL_DIVERGENT_COLORMAP,
     qctrl_style,
 )
 from .utils import create_figure
@@ -34,15 +35,15 @@
 @qctrl_style()
 def plot_wigner_function(
     wigner_function: np.ndarray,
     position: np.ndarray,
     momentum: np.ndarray,
     contour_count: int = 100,
     *,
-    figure: Optional[plt.Figure] = None,
+    figure: Optional[Figure] = None,
 ):
     r"""
     Create a contour plot of the specified Wigner function.
 
     Parameters
     ----------
     wigner_function : np.ndarray
@@ -121,14 +122,15 @@
     check_argument(
         isinstance(contour_count, (int, np.integer)) and contour_count > 0,
         "The number of contours must be a positive integer.",
         {"contour_count": contour_count},
     )
 
     axes = figure.subplots(nrows=1, ncols=1)
+    assert isinstance(axes, Axes)
     axes.set_aspect("equal")
 
     # Fix divergent colormap with the central color at 0.
     wigner_max_abs = np.max(np.abs(wigner_function))
     norm = TwoSlopeNorm(vcenter=0.0, vmin=-wigner_max_abs, vmax=wigner_max_abs)
 
     # The Wigner function is a real function, but we only plot the real part
```

### Comparing `qctrl_visualizer-7.0.0/PKG-INFO` & `qctrl_visualizer-7.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qctrl-visualizer
-Version: 7.0.0
+Version: 7.1.0
 Summary: Q-CTRL Visualizer
 Home-page: https://q-ctrl.com
 License: https://q-ctrl.com/terms
 Keywords: black opal,boulder opal,fire opal,nisq,open controls,q control,q ctrl,q-control,q-ctrl,qcontrol,qctrl,quantum,quantum algorithms,quantum circuits,quantum coding,quantum coding software,quantum computing,quantum control,quantum control software,quantum control theory,quantum engineering,quantum error correction,quantum firmware,quantum fundamentals,quantum sensing,qubit,qudit
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
@@ -26,15 +26,15 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Distributed Computing
 Requires-Dist: matplotlib (>=3.6.3)
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
-Requires-Dist: qctrl-commons (>=21.2.4,<22.0.0)
+Requires-Dist: qctrl-commons (>=22.1.0,<23.0.0)
 Requires-Dist: scipy (>=1.9.3)
 Project-URL: Documentation, https://docs.q-ctrl.com/boulder-opal/references/qctrl-visualizer/
 Project-URL: GitHub, https://github.com/qctrl
 Project-URL: Twitter, https://twitter.com/qctrlHQ
 Description-Content-Type: text/markdown
 
 # Q-CTRL Visualizer
```

