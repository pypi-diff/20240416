# Comparing `tmp/hiperwalk-2.0b11.tar.gz` & `tmp/hiperwalk-2.0b12.tar.gz`

## Comparing `hiperwalk-2.0b11.tar` & `hiperwalk-2.0b12.tar`

### file list

```diff
@@ -1,160 +1,165 @@
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/.readthedocs.yaml
--rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/build_and_upload_to_pypi
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/deleteme.py
--rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/fit.py
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hypercube.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/memory_test.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/oriented_lat.py
--rw-r--r--   0        0        0   180930 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/output.txt
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/paulomotta.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/plot_max_success_probability.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/plot_optimal_runtime.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/prob_test.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/renato.py
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/ring_of_donuts.py
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/test_state.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/test_t_opt.py
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/.github/workflows/rebuild_project_page.yml
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/config.py
--rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/custom.nbl
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/custom.py
--rwxr-xr-x   0        0        0     1734 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/distance.py
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/dtqw1d.nbl
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/dtqw1d.py
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/dtqw2d.nbl
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/dtqw2d.py
--rw-r--r--   0        0        0    12690 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/gnuplot.py
--rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/hiperwalk.py
--rwxr-xr-x   0        0        0      909 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/install.sh
--rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/ioFunctions.py
--rw-r--r--   0        0        0    22919 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/neblina.py
--rw-r--r--   0        0        0    29012 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/operators.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/parsing.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/run.py
--rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/staggered1d.nbl
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/staggered1d.py
--rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/staggered2d.nbl
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/staggered2d.py
--rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/standardDeviation.py
--rw-r--r--   0        0        0    12276 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/state.py
--rw-r--r--   0        0        0    24726 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/testmode.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/walks.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/examples/coined1D.in
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/examples/coined2D.in
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/examples/custom.in
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/examples/psi0.dat
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/examples/staggered1D.in
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/examples/staggered2D.in
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/examples/u0.dat
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/examples/u1.dat
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/Makefile
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/README.md
--rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/conf.py
--rwxr-xr-x   0        0        0      104 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/go
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/index.rst
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/make.bat
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/requirements.txt
--rwxr-xr-x   0        0        0       13 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/test_docs
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/_templates/autoclass.rst
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/_templates/autofunctions.rst
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/_templates/automodule.rst
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/development/index.rst
--rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/documentation/graph.rst
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/documentation/hpc.rst
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/documentation/index.rst
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/documentation/plot.rst
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/documentation/quantum_walk.rst
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/documentation/graph_constructors/complete.rst
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/documentation/graph_constructors/complete_bipartite.rst
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/documentation/graph_constructors/cycle.rst
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/documentation/graph_constructors/grid.rst
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/documentation/graph_constructors/hypercube.rst
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/documentation/graph_constructors/integer_lattice.rst
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/documentation/graph_constructors/line.rst
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/examples/index.rst
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/graphviz/graph-arcs.dot
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/graphviz/graph-example.dot
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/graphviz/grid/bounded-diagonal.dot
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/graphviz/grid/bounded-diagonal.py
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/graphviz/grid/bounded-natural.dot
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/graphviz/grid/bounded-natural.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/graphviz/grid/diagonal-grid-neigh-order.dot
--rw-r--r--   0        0        0     5932 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/graphviz/grid/even-dim-diagonal.dot
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/graphviz/grid/even-dim-diagonal.py
--rwxr-xr-x   0        0        0      307 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/graphviz/grid/go
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/graphviz/grid/natural-grid-neigh-order.dot
--rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/graphviz/grid/periodic-diagonal.dot
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/graphviz/grid/periodic-diagonal.py
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/graphviz/grid/periodic-natural.dot
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/graphviz/grid/periodic-natural.py
--rw-r--r--   0        0        0     9009 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/install/index.rst
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/tutorial/graph_constructors.rst
--rw-r--r--   0        0        0     6196 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/tutorial/graphs.rst
--rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/tutorial/index.rst
--rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/tutorial/plotting.rst
--rw-r--r--   0        0        0    23410 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/tutorial/quantum_walk_models.rst
--rw-r--r--   0        0        0   348577 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/Untitled-Copy1.ipynb
--rw-r--r--   0        0        0  1644954 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/Untitled.ipynb
--rw-r--r--   0        0        0   765630 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/Untitled1.ipynb
--rw-r--r--   0        0        0  1234252 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/Untitled2.ipynb
--rw-r--r--   0        0        0   429871 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/Untitled3.ipynb
--rw-r--r--   0        0        0   541540 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/Untitled4.ipynb
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/coined-bipartite-search.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/coined-complete-search.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/coined-diagonal-grid.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/coined-grid-search.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/coined-hypercube.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/continuous-cycle.py
--rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/deleteme.py
--rw-r--r--   0        0        0    43772 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/exemplo1.ipynb
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/grid-search.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/grovers-algorithm.py
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/hipercubo-multimarcados.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/hypercube-search.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/issue13.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/new_hypercube.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/square_lattice.py
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/notebooks/CoinedDiagonalLattice.ipynb
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/notebooks/ContinuousCycle.ipynb
--rw-r--r--   0        0        0     5412 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/notebooks/test_load_numpy_matrix.ipynb
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/__init__.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/_constants.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/graph/__init__.py
--rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/graph/_sym_dir_multigraph.py
--rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/graph/complete.py
--rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/graph/complete_bipartite.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/graph/cycle.py
--rw-r--r--   0        0        0    15634 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/graph/graph.py
--rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/graph/grid.py
--rw-r--r--   0        0        0     4860 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/graph/hypercube.py
--rw-r--r--   0        0        0    10212 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/graph/integer_lattice.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/graph/line.py
--rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/graph/multigraph.py
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/graph/weighted_graph.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/plot/__init__.py
--rw-r--r--   0        0        0    36244 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/plot/_plot.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/quantum_walk/__init__.py
--rw-r--r--   0        0        0    12866 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/quantum_walk/_pyneblina_interface.py
--rw-r--r--   0        0        0    39685 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/quantum_walk/coined.py
--rw-r--r--   0        0        0    17212 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/quantum_walk/continuous_time.py
--rw-r--r--   0        0        0    27148 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/quantum_walk/quantum_walk.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/tests/__init__.py
--rwxr-xr-x   0        0        0      120 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/tests/run_all.sh
--rwxr-xr-x   0        0        0      121 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/tests/run_hpc.sh
--rwxr-xr-x   0        0        0      121 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/tests/run_nonhpc.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/tests/unit/__init__.py
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/tests/unit/binary_search_test.py
--rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/tests/unit/coined_cycle.py
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/tests/unit/coined_line.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/tests/unit/complete.py
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/tests/unit/complete_bipartite.py
--rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/tests/unit/continuous_time.py
--rw-r--r--   0        0        0     5370 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/tests/unit/graph.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/tests/unit/hypercube.py
--rw-r--r--   0        0        0     6517 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/tests/unit/multigraph.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/.gitignore
--rw-r--r--   0        0        0     7560 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/LICENSE
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/README.md
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/pyproject.toml
--rw-r--r--   0        0        0    11957 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/PKG-INFO
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/.readthedocs.yaml
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/Untitled.ipynb
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/Untitled1.ipynb
+-rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/build_and_upload_to_pypi
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/deleteme.py
+-rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/fit.py
+-rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/hypercube.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/memory_test.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/oriented_lat.py
+-rw-r--r--   0        0        0   180930 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/output.txt
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/paulomotta.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/plot_max_success_probability.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/plot_optimal_runtime.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/prob_test.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/renato.py
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/ring_of_donuts.py
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/test_state.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/test_t_opt.py
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/.github/workflows/rebuild_project_page.yml
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/Archive/config.py
+-rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/Archive/custom.nbl
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/Archive/custom.py
+-rwxr-xr-x   0        0        0     1734 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/Archive/distance.py
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/Archive/dtqw1d.nbl
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/Archive/dtqw1d.py
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/Archive/dtqw2d.nbl
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/Archive/dtqw2d.py
+-rw-r--r--   0        0        0    12690 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/Archive/gnuplot.py
+-rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/Archive/hiperwalk.py
+-rwxr-xr-x   0        0        0      909 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/Archive/install.sh
+-rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/Archive/ioFunctions.py
+-rw-r--r--   0        0        0    22919 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/Archive/neblina.py
+-rw-r--r--   0        0        0    29012 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/Archive/operators.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/Archive/parsing.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/Archive/run.py
+-rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/Archive/staggered1d.nbl
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/Archive/staggered1d.py
+-rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/Archive/staggered2d.nbl
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/Archive/staggered2d.py
+-rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/Archive/standardDeviation.py
+-rw-r--r--   0        0        0    12276 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/Archive/state.py
+-rw-r--r--   0        0        0    24726 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/Archive/testmode.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/Archive/walks.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/Archive/examples/coined1D.in
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/Archive/examples/coined2D.in
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/Archive/examples/custom.in
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/Archive/examples/psi0.dat
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/Archive/examples/staggered1D.in
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/Archive/examples/staggered2D.in
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/Archive/examples/u0.dat
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/Archive/examples/u1.dat
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/Makefile
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/README.md
+-rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/conf.py
+-rwxr-xr-x   0        0        0      104 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/go
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/index.rst
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/make.bat
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/requirements.txt
+-rwxr-xr-x   0        0        0       13 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/test_docs
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/_templates/autoclass.rst
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/_templates/autofunctions.rst
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/_templates/automodule.rst
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/development/index.rst
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/documentation/graph.rst
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/documentation/hpc.rst
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/documentation/index.rst
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/documentation/plot.rst
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/documentation/quantum_walk.rst
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/documentation/graph_constructors/complete.rst
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/documentation/graph_constructors/complete_bipartite.rst
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/documentation/graph_constructors/cycle.rst
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/documentation/graph_constructors/grid.rst
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/documentation/graph_constructors/hypercube.rst
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/documentation/graph_constructors/integer_lattice.rst
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/documentation/graph_constructors/line.rst
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/examples/index.rst
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/graphviz/graph-arcs.dot
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/graphviz/graph-example.dot
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/graphviz/grid/bounded-diagonal.dot
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/graphviz/grid/bounded-diagonal.py
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/graphviz/grid/bounded-natural.dot
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/graphviz/grid/bounded-natural.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/graphviz/grid/diagonal-grid-neigh-order.dot
+-rw-r--r--   0        0        0     5932 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/graphviz/grid/even-dim-diagonal.dot
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/graphviz/grid/even-dim-diagonal.py
+-rwxr-xr-x   0        0        0      307 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/graphviz/grid/go
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/graphviz/grid/natural-grid-neigh-order.dot
+-rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/graphviz/grid/periodic-diagonal.dot
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/graphviz/grid/periodic-diagonal.py
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/graphviz/grid/periodic-natural.dot
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/graphviz/grid/periodic-natural.py
+-rw-r--r--   0        0        0     9127 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/install/index.rst
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/tutorial/graph_constructors.rst
+-rw-r--r--   0        0        0     6196 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/tutorial/graphs.rst
+-rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/tutorial/index.rst
+-rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/tutorial/plotting.rst
+-rw-r--r--   0        0        0    23683 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/docs/tutorial/quantum_walk_models.rst
+-rw-r--r--   0        0        0   348577 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/examples/Untitled-Copy1.ipynb
+-rw-r--r--   0        0        0  1644954 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/examples/Untitled.ipynb
+-rw-r--r--   0        0        0   765630 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/examples/Untitled1.ipynb
+-rw-r--r--   0        0        0  1234252 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/examples/Untitled2.ipynb
+-rw-r--r--   0        0        0   429871 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/examples/Untitled3.ipynb
+-rw-r--r--   0        0        0   541540 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/examples/Untitled4.ipynb
+-rw-r--r--   0        0        0   269682 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/examples/Untitled5.ipynb
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/examples/coined-bipartite-search.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/examples/coined-complete-search.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/examples/coined-diagonal-grid.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/examples/coined-grid-search.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/examples/coined-hypercube.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/examples/continuous-cycle.py
+-rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/examples/deleteme.py
+-rw-r--r--   0        0        0    43772 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/examples/exemplo1.ipynb
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/examples/grid-search.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/examples/grovers-algorithm.py
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/examples/hipercubo-multimarcados.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/examples/hypercube-search.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/examples/issue13.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/examples/new_hypercube.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/examples/square_lattice.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/examples/untitled
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/examples/notebooks/CoinedDiagonalLattice.ipynb
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/examples/notebooks/ContinuousCycle.ipynb
+-rw-r--r--   0        0        0     5412 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/examples/notebooks/test_load_numpy_matrix.ipynb
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/hiperwalk/__init__.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/hiperwalk/_constants.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/hiperwalk/graph/__init__.py
+-rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/hiperwalk/graph/_sym_dir_multigraph.py
+-rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/hiperwalk/graph/complete.py
+-rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/hiperwalk/graph/complete_bipartite.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/hiperwalk/graph/cycle.py
+-rw-r--r--   0        0        0    15638 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/hiperwalk/graph/graph.py
+-rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/hiperwalk/graph/grid.py
+-rw-r--r--   0        0        0     4860 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/hiperwalk/graph/hypercube.py
+-rw-r--r--   0        0        0    10212 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/hiperwalk/graph/integer_lattice.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/hiperwalk/graph/line.py
+-rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/hiperwalk/graph/multigraph.py
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/hiperwalk/graph/weighted_graph.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/hiperwalk/plot/__init__.py
+-rw-r--r--   0        0        0    36244 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/hiperwalk/plot/_plot.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/hiperwalk/quantum_walk/__init__.py
+-rw-r--r--   0        0        0    12561 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/hiperwalk/quantum_walk/_pyneblina_interface.py
+-rw-r--r--   0        0        0    39927 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/hiperwalk/quantum_walk/coined.py
+-rw-r--r--   0        0        0    17212 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/hiperwalk/quantum_walk/continuous_time.py
+-rw-r--r--   0        0        0    26704 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/hiperwalk/quantum_walk/quantum_walk.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/tests/__init__.py
+-rwxr-xr-x   0        0        0      120 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/tests/run_all.sh
+-rwxr-xr-x   0        0        0      121 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/tests/run_hpc.sh
+-rwxr-xr-x   0        0        0      121 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/tests/run_nonhpc.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/tests/unit/__init__.py
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/tests/unit/binary_search_test.py
+-rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/tests/unit/coined_cycle.py
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/tests/unit/coined_line.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/tests/unit/complete.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/tests/unit/complete_bipartite.py
+-rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/tests/unit/continuous_time.py
+-rw-r--r--   0        0        0   287610 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/tests/unit/examples.py
+-rw-r--r--   0        0        0     5370 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/tests/unit/graph.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/tests/unit/hypercube.py
+-rw-r--r--   0        0        0     6517 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/tests/unit/multigraph.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/.gitignore
+-rw-r--r--   0        0        0     7560 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/LICENSE
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/README.md
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/pyproject.toml
+-rw-r--r--   0        0        0    11957 2020-02-02 00:00:00.000000 hiperwalk-2.0b12/PKG-INFO
```

### Comparing `hiperwalk-2.0b11/deleteme.py` & `hiperwalk-2.0b12/deleteme.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/fit.py` & `hiperwalk-2.0b12/fit.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/hypercube.py` & `hiperwalk-2.0b12/hypercube.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/memory_test.py` & `hiperwalk-2.0b12/memory_test.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/output.txt` & `hiperwalk-2.0b12/output.txt`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/paulomotta.py` & `hiperwalk-2.0b12/paulomotta.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/ring_of_donuts.py` & `hiperwalk-2.0b12/ring_of_donuts.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/test_state.py` & `hiperwalk-2.0b12/test_state.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/test_t_opt.py` & `hiperwalk-2.0b12/test_t_opt.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/.github/workflows/rebuild_project_page.yml` & `hiperwalk-2.0b12/.github/workflows/rebuild_project_page.yml`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/Archive/config.py` & `hiperwalk-2.0b12/Archive/config.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/Archive/custom.nbl` & `hiperwalk-2.0b12/Archive/custom.nbl`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/Archive/custom.py` & `hiperwalk-2.0b12/Archive/custom.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/Archive/distance.py` & `hiperwalk-2.0b12/Archive/distance.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/Archive/dtqw1d.nbl` & `hiperwalk-2.0b12/Archive/dtqw1d.nbl`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/Archive/dtqw1d.py` & `hiperwalk-2.0b12/Archive/dtqw1d.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/Archive/dtqw2d.nbl` & `hiperwalk-2.0b12/Archive/dtqw2d.nbl`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/Archive/dtqw2d.py` & `hiperwalk-2.0b12/Archive/dtqw2d.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/Archive/gnuplot.py` & `hiperwalk-2.0b12/Archive/gnuplot.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/Archive/hiperwalk.py` & `hiperwalk-2.0b12/Archive/hiperwalk.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/Archive/install.sh` & `hiperwalk-2.0b12/Archive/install.sh`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/Archive/ioFunctions.py` & `hiperwalk-2.0b12/Archive/ioFunctions.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/Archive/neblina.py` & `hiperwalk-2.0b12/Archive/neblina.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/Archive/operators.py` & `hiperwalk-2.0b12/Archive/operators.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/Archive/parsing.py` & `hiperwalk-2.0b12/Archive/parsing.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/Archive/run.py` & `hiperwalk-2.0b12/Archive/run.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/Archive/staggered1d.nbl` & `hiperwalk-2.0b12/Archive/staggered1d.nbl`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/Archive/staggered1d.py` & `hiperwalk-2.0b12/Archive/staggered1d.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/Archive/staggered2d.nbl` & `hiperwalk-2.0b12/Archive/staggered2d.nbl`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/Archive/staggered2d.py` & `hiperwalk-2.0b12/Archive/staggered2d.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/Archive/standardDeviation.py` & `hiperwalk-2.0b12/Archive/standardDeviation.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/Archive/state.py` & `hiperwalk-2.0b12/Archive/state.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/Archive/testmode.py` & `hiperwalk-2.0b12/Archive/testmode.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/Archive/walks.py` & `hiperwalk-2.0b12/Archive/walks.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/docs/Makefile` & `hiperwalk-2.0b12/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/docs/conf.py` & `hiperwalk-2.0b12/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/docs/index.rst` & `hiperwalk-2.0b12/docs/index.rst`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/docs/make.bat` & `hiperwalk-2.0b12/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/docs/_templates/automodule.rst` & `hiperwalk-2.0b12/docs/_templates/automodule.rst`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/docs/development/index.rst` & `hiperwalk-2.0b12/docs/development/index.rst`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/docs/documentation/graph.rst` & `hiperwalk-2.0b12/docs/documentation/graph.rst`

 * *Files 6% similar despite different names*

```diff
@@ -74,14 +74,16 @@
    <https://docs.python.org/3/reference/datamodel.html#object.__init__>`_
    and `generator
    <https://docs.python.org/3/glossary.html#term-generator>`_
    are words that already have consolidated meanings.
    Thus, we decided to use the word *constructor* because
    it conveys the idea that an instance is going to be returned.
 
+.. _docs_documentation_list_of_graph_constructors:
+
 List of Graph Constructors
 **************************
 
 The following is the list of all available graph constructors.
 
 .. toctree::
    :maxdepth: 1
```

### Comparing `hiperwalk-2.0b11/docs/graphviz/graph-arcs.dot` & `hiperwalk-2.0b12/docs/graphviz/graph-arcs.dot`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/docs/graphviz/grid/bounded-diagonal.dot` & `hiperwalk-2.0b12/docs/graphviz/grid/bounded-diagonal.dot`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/docs/graphviz/grid/bounded-diagonal.py` & `hiperwalk-2.0b12/docs/graphviz/grid/bounded-diagonal.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/docs/graphviz/grid/bounded-natural.dot` & `hiperwalk-2.0b12/docs/graphviz/grid/bounded-natural.dot`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/docs/graphviz/grid/bounded-natural.py` & `hiperwalk-2.0b12/docs/graphviz/grid/bounded-natural.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/docs/graphviz/grid/diagonal-grid-neigh-order.dot` & `hiperwalk-2.0b12/docs/graphviz/grid/diagonal-grid-neigh-order.dot`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/docs/graphviz/grid/even-dim-diagonal.dot` & `hiperwalk-2.0b12/docs/graphviz/grid/even-dim-diagonal.dot`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/docs/graphviz/grid/even-dim-diagonal.py` & `hiperwalk-2.0b12/docs/graphviz/grid/even-dim-diagonal.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/docs/graphviz/grid/natural-grid-neigh-order.dot` & `hiperwalk-2.0b12/docs/graphviz/grid/natural-grid-neigh-order.dot`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/docs/graphviz/grid/periodic-diagonal.dot` & `hiperwalk-2.0b12/docs/graphviz/grid/periodic-diagonal.dot`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/docs/graphviz/grid/periodic-diagonal.py` & `hiperwalk-2.0b12/docs/graphviz/grid/periodic-diagonal.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/docs/graphviz/grid/periodic-natural.dot` & `hiperwalk-2.0b12/docs/graphviz/grid/periodic-natural.dot`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/docs/graphviz/grid/periodic-natural.py` & `hiperwalk-2.0b12/docs/graphviz/grid/periodic-natural.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/docs/tutorial/graph_constructors.rst` & `hiperwalk-2.0b12/docs/tutorial/graph_constructors.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,65 @@
 ==================
 Graph Constructors
 ==================
 
-You can use graph constructors to create instances of
-specific, well-known graphs.
-
-Specific Graphs
----------------
-
-Hiperwalk includes classes for well-known specific graphs,
+Hiperwalk has specific commands (graph constructors) to
+generate instances of well-known specific graphs,
 such as Line, Cycle, and Grid.
-For a complete list of specific graphs,
-refer to :ref:`docs_documentation_graph`.
+For a complete list of graph constructors,
+refer to :ref:`docs_documentation_list_of_graph_constructors`.
 
 The key difference between creating an
-arbitrary graph and a specific graph is
+arbitrary graph and using a graph constructor is
 that for the former, you must explicitly provide the adjacency matrix.
 However, for the latter, the adjacency matrix is automatically generated
-based on the number of vertices.
-Consequently, you can create a line with 10 vertices,
+based on specific graph parameters such as the number of vertices.
+Nevertheless,
+the order of neighbors is automatically embedded in
+the generated adjacency matrix.
+
+For example, you can create a line with 10 vertices,
 a cycle with 10 vertices,
 and a grid of dimensions :math:`10 \times 10` using
 valid commands, respectively.
 
 >>> hpw.Line(10) #doctest: +SKIP
 <hiperwalk.graph.line.Line object at 0x7f0a6bb700d0>
 >>> hpw.Cycle(10) #doctest: +SKIP
 <hiperwalk.graph.cycle.Cycle object at 0x7f0a6bbb32e0>
 >>> hpw.Grid(10) #doctest: +SKIP
 <hiperwalk.graph.grid.Grid object at 0x7f0a6bbb2da0>
 
 Naturally, you can create specific graphs using NetworkX and
 the :class:`hiperwalk.Graph` class.
-However, this approach is not recommended, especially when dealing with
-coined quantum walks, as it may result in undesirable behavior.
+Just be aware that the order of neighbors may vary,
+which may result in undesirable behavior,
+especially when dealing with coined quantum walks.
 
 As an example, let's consider a Line with 10 vertices.
 First, we create the line using the :class:`hiperwalk.Graph` class.
 
 .. testsetup::
 
    import networkx as nx
    import hiperwalk as hpw
 
 >>> path = nx.path_graph(10)
 >>> adj_matrix = nx.adjacency_matrix(path)
 >>> arbitrary_line = hpw.Graph(adj_matrix)
 
-Next, we create the line using the :class:`hiperwalk.Line` class.
+Next, we create the line using the :class:`hiperwalk.Line`
+graph constructor.
 
->>> specific_line = hpw.Line(10)
+>>> graph_constructor_line = hpw.Line(10)
 
-In a simple graph, we associate each edge with two arcs. Suppose we wish
-to know the label of the arc that links vertex 1 to 2. This information
-can be obtained using the :meth:`hiperwalk.Graph.arc_number` method.
-Observe the following results:
-
-For further details on arc labels for each graph, refer to the Notes
-section of each graph class, in this case,
-:class:`hiperwalk.Graph` and :class:`hiperwalk.Line`.
+The order of neighbors os these two instances is different.
+For ``arbitrary_line``,
+the neighbors are listed in ascending order,
+while for ``graph_constructor_line``,
+the neighbors are listed in descending order
+(righmost neighbor followed by the leftmost neighbor).
+
+>>> arbitrary_line.neighbors(1)
+array([0, 2])
+>>> graph_constructor_line.neighbors(1)
+array([2, 0], dtype=int32)
```

### Comparing `hiperwalk-2.0b11/docs/tutorial/graphs.rst` & `hiperwalk-2.0b12/docs/tutorial/graphs.rst`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/docs/tutorial/index.rst` & `hiperwalk-2.0b12/docs/tutorial/index.rst`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/docs/tutorial/plotting.rst` & `hiperwalk-2.0b12/docs/tutorial/plotting.rst`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/docs/tutorial/quantum_walk_models.rst` & `hiperwalk-2.0b12/docs/tutorial/quantum_walk_models.rst`

 * *Files 3% similar despite different names*

```diff
@@ -37,29 +37,33 @@
 <hiperwalk.graph.graph.Graph object at 0x7f657268c0d0>
 
 Since ``cycle`` is an instance of :class:`hiperwalk.Graph`,
 we can pass ``cycle`` to the quantum walk constructor.
 
 Coined Model
 ''''''''''''
-To create a coined quantum walk, we execute
+A coined quantum walk can be created by passing an instance of
+:class:`hiperwalk.Graph` or :class:`hiperwalk.Multigraph`.
+To create a coined quantum walk on the cycle, we execute
 
 >>> coined = hpw.Coined(graph=cycle)
 >>> coined #doctest: +SKIP
 <hiperwalk.quantum_walk.coined_walk.Coined object at 0x7f655b0cd900>
 
 The Hilbert space of the coined quantum walk has dimension
 :math:`2|E|`, i.e. the number of arcs.
 
 >>> coined.hilbert_space_dimension() == 2*cycle.number_of_edges()
 True
 
 Continuous-time Model
 '''''''''''''''''''''
-To create a continuous-time quantum walk,
+A coined quantum walk can be created by passing an instance of
+:class:`hiperwalk.Graph` or :class:`hiperwalk.WeightedGraph`.
+To create a continuous-time quantum walk on the cycle,
 we execute an analogous command.
 
 >>> continuous = hpw.ContinuousTime(graph=cycle)
 >>> continuous #doctest: +SKIP
 <hiperwalk.quantum_walk.continuous_time.ContinuousTime object at 0x7098fe80eef0>
 
 The Hilbert space of the continuous-time quantum walk has dimension
```

### Comparing `hiperwalk-2.0b11/examples/Untitled-Copy1.ipynb` & `hiperwalk-2.0b12/examples/Untitled-Copy1.ipynb`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/examples/Untitled.ipynb` & `hiperwalk-2.0b12/examples/Untitled.ipynb`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/examples/Untitled1.ipynb` & `hiperwalk-2.0b12/examples/Untitled1.ipynb`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/examples/Untitled2.ipynb` & `hiperwalk-2.0b12/examples/Untitled2.ipynb`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/examples/Untitled3.ipynb` & `hiperwalk-2.0b12/examples/Untitled3.ipynb`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/examples/Untitled4.ipynb` & `hiperwalk-2.0b12/examples/Untitled4.ipynb`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/examples/coined-diagonal-grid.py` & `hiperwalk-2.0b12/examples/coined-diagonal-grid.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/examples/deleteme.py` & `hiperwalk-2.0b12/examples/deleteme.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/examples/exemplo1.ipynb` & `hiperwalk-2.0b12/examples/exemplo1.ipynb`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/examples/hipercubo-multimarcados.py` & `hiperwalk-2.0b12/examples/hipercubo-multimarcados.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/examples/hypercube-search.py` & `hiperwalk-2.0b12/examples/hypercube-search.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/examples/issue13.py` & `hiperwalk-2.0b12/examples/issue13.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/examples/notebooks/CoinedDiagonalLattice.ipynb` & `hiperwalk-2.0b12/examples/notebooks/CoinedDiagonalLattice.ipynb`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/examples/notebooks/ContinuousCycle.ipynb` & `hiperwalk-2.0b12/examples/notebooks/ContinuousCycle.ipynb`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/examples/notebooks/test_load_numpy_matrix.ipynb` & `hiperwalk-2.0b12/examples/notebooks/test_load_numpy_matrix.ipynb`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/hiperwalk/graph/_sym_dir_multigraph.py` & `hiperwalk-2.0b12/hiperwalk/graph/_sym_dir_multigraph.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/hiperwalk/graph/complete.py` & `hiperwalk-2.0b12/hiperwalk/graph/complete.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/hiperwalk/graph/complete_bipartite.py` & `hiperwalk-2.0b12/hiperwalk/graph/complete_bipartite.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/hiperwalk/graph/cycle.py` & `hiperwalk-2.0b12/hiperwalk/graph/cycle.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/hiperwalk/graph/graph.py` & `hiperwalk-2.0b12/hiperwalk/graph/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,16 +221,16 @@
         # this function is reimplemented because data=None
         # to use less memory
         u = self.vertex_number(u)
         v = self.vertex_number(v)
         A = self._adj_matrix
 
         if A.has_sorted_indices:
-            i = self._binary_search(A.indices, v, start=A[u],
-                                    end=A[u + 1])
+            i = _binary_search(A.indices, v, start=A.indptr[u],
+                               end=A.indptr[u + 1])
             return i != -1
 
         return v in A.indices[A.indptr[u]:A.indptr[u+1]]
         return v in A.indices[A.indptr[u]:A.indptr[u+1]]
 
     def _entry(self, lin, col):
         entry = self._adj_matrix.indptr[lin] + 1
```

### Comparing `hiperwalk-2.0b11/hiperwalk/graph/grid.py` & `hiperwalk-2.0b12/hiperwalk/graph/grid.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/hiperwalk/graph/hypercube.py` & `hiperwalk-2.0b12/hiperwalk/graph/hypercube.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/hiperwalk/graph/integer_lattice.py` & `hiperwalk-2.0b12/hiperwalk/graph/integer_lattice.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/hiperwalk/graph/line.py` & `hiperwalk-2.0b12/hiperwalk/graph/line.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/hiperwalk/graph/multigraph.py` & `hiperwalk-2.0b12/hiperwalk/graph/multigraph.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/hiperwalk/graph/weighted_graph.py` & `hiperwalk-2.0b12/hiperwalk/graph/weighted_graph.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/hiperwalk/plot/_plot.py` & `hiperwalk-2.0b12/hiperwalk/plot/_plot.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/hiperwalk/quantum_walk/_pyneblina_interface.py` & `hiperwalk-2.0b12/hiperwalk/quantum_walk/_pyneblina_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,21 +124,14 @@
     I think an auxiliary vector is beign created,
     thus twice the memory needed is being used
     """
 
     # TODO: check if complex automatically?
     is_complex = isinstance(v.dtype, complex)
 
-    if not is_complex:
-        warn(
-            "Real multiplication not implemented. "
-            + "Treating entries as complex."
-        )
-    is_complex = True
-
     n = v.shape[0]
     # TODO: needs better support from pyneblina to
     # use next instruction (commented).
     # For example: neblina.vector_set works, but in the real case,
     # it should not be needed to pass the imaginary part as argument.
     # In addition,
     # there should be a way to return a vector and automatically
@@ -268,20 +261,15 @@
             neblina.matrix_set(mat, i, j, M[i, j].real, M[i, j].imag)
 
     neblina.move_matrix_device(mat)
 
     return PyNeblinaMatrix(mat, M.shape, is_complex, False)
 
 def send_matrix(M):
-    if not isinstance(M.dtype, complex):
-        warn(
-            "Real multiplication not implemented. "
-            + "Treating entries as complex."
-        )
-    is_complex = True
+    is_complex = isinstance(M.dtype, complex)
 
     if scipy.sparse.issparse(M):
         return _send_sparse_matrix(M, is_complex)
 
     return _send_dense_matrix(M, is_complex)
 
 def retrieve_matrix(pynbl_mat):
```

### Comparing `hiperwalk-2.0b11/hiperwalk/quantum_walk/coined.py` & `hiperwalk-2.0b12/hiperwalk/quantum_walk/coined.py`

 * *Files 5% similar despite different names*

```diff
@@ -845,32 +845,34 @@
         # TODO: Check if matrices are deleted from memory and GPU.
         U = None
 
         S = self.get_shift()
         C = self.get_coin()
 
         if nbl.get_hpc() is not None:
-            # TODO: implement sparse matrix multiplication with hpc
-            S = S.todense()
-            C = C.todense()
-
-            nbl_S = nbl.send_matrix(S)
-            del S
-            nbl_C = nbl.send_matrix(C)
-            del C
-            nbl_C = nbl.multiply_matrices(nbl_S, nbl_C)
-
-            del nbl_S
-
-            U = nbl.retrieve_matrix(nbl_C)
-            del nbl_C
-            U = scipy.sparse.csr_array(U)
+            from warnings import warn
+            warn('HPC sparse matrix multiplication is not implemented. '
+                 + 'Using standard scipy multiplication instead.')
+            # # TODO: implement sparse matrix multiplication with hpc
+            # S = S.todense()
+            # C = C.todense()
+
+            # nbl_S = nbl.send_matrix(S)
+            # del S
+            # nbl_C = nbl.send_matrix(C)
+            # del C
+            # nbl_C = nbl.multiply_matrices(nbl_S, nbl_C)
+
+            # del nbl_S
+
+            # U = nbl.retrieve_matrix(nbl_C)
+            # del nbl_C
+            # U = scipy.sparse.csr_array(U)
 
-        else:
-            U = S @ C
+        U = S @ C
 
         self._evolution = U
         return U
 
     def set_evolution(self, **kwargs):
         """
         Set the evolution operator.
@@ -1033,15 +1035,14 @@
 
     def state(self, entries):
         """
         Generates a valid state.
 
         The state corresponds to the walker being in a superposition
         of the ``entries``.
-        For instance, click on :meth:`qwalk.coined.Graph`.
         The final state is normalized in order to be a unit vector.
 
         Parameters
         ----------
         entries : list of entry
             Each entry is a tuple (or array).
             An entry can be specified in two different ways:
@@ -1093,15 +1094,16 @@
         True
         >>> np.all(psi1 == psi2)
         True
         """
         if len(entries) == 0:
             raise TypeError("Entries were not specified.")
 
-        state = np.zeros(self.hilb_dim)
+        dtype = np.array([entry[0] for entry in entries]).dtype
+        state = np.zeros(self.hilb_dim, dtype=dtype)
 
         for ampl, arc in entries:
             state[self._graph.arc_number(arc)] = ampl
 
         return self._normalize(state)
 
     def ket(self, arc):
@@ -1126,40 +1128,40 @@
             valid examples
         """
         ket = np.zeros(self.hilb_dim, dtype=float)
         ket[self._graph.arc_number(arc)] = 1
 
         return ket
 
-    def _prepare_engine(self, state, hpc):
-        if hpc is not None:
-            S = nbl.send_matrix(self.get_shift())
-            C = nbl.send_matrix(self.get_coin())
-            self._simul_mat = (C, S)
-            self._simul_vec = nbl.send_vector(state)
-
-            dtype = (complex if (S.is_complex or C.is_complex
-                                 or np.iscomplex(state.dtype))
-                     else np.double)
-
-            return dtype
-
-        return super()._prepare_engine(state, hpc)
-
-
-    def _simulate_step(self, step, hpc):
-        if hpc is not None:
-            for i in range(step):
-                self._simul_vec = nbl.multiply_matrix_vector(
-                    self._simul_mat[0], self._simul_vec)
-
-                self._simul_vec = nbl.multiply_matrix_vector(
-                    self._simul_mat[1], self._simul_vec)
-        else:
-            super()._simulate_step(step, hpc)
+    # def _prepare_engine(self, state, hpc):
+    #     if hpc is not None:
+    #         S = nbl.send_matrix(self.get_shift())
+    #         C = nbl.send_matrix(self.get_coin())
+    #         self._simul_mat = (C, S)
+    #         self._simul_vec = nbl.send_vector(state)
+
+    #         dtype = (complex if (S.is_complex or C.is_complex
+    #                              or np.iscomplex(state.dtype))
+    #                  else np.double)
+
+    #         return dtype
+
+    #     return super()._prepare_engine(state, hpc)
+
+
+    # def _simulate_step(self, step, hpc):
+    #     if hpc is not None:
+    #         for i in range(step):
+    #             self._simul_vec = nbl.multiply_matrix_vector(
+    #                 self._simul_mat[0], self._simul_vec)
+
+    #             self._simul_vec = nbl.multiply_matrix_vector(
+    #                 self._simul_mat[1], self._simul_vec)
+    #     else:
+    #         super()._simulate_step(step, hpc)
 
     def probability(self, states, vertices):
         r"""
         Computes the sum of probabilities for the specified vertices.
         
         Computes the probability of the walker being located on a
         vertex within the set of provided vertices, given that the walk
```

### Comparing `hiperwalk-2.0b11/hiperwalk/quantum_walk/continuous_time.py` & `hiperwalk-2.0b12/hiperwalk/quantum_walk/continuous_time.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/hiperwalk/quantum_walk/quantum_walk.py` & `hiperwalk-2.0b12/hiperwalk/quantum_walk/quantum_walk.py`

 * *Files 3% similar despite different names*

```diff
@@ -414,15 +414,16 @@
         True
         >>> np.all(psi2 == psi3)
         True
         """
         if len(entries) == 0:
             raise TypeError("Entries were not specified.")
 
-        state = np.zeros(self.hilb_dim)
+        dtype = np.array([entry[0] for entry in entries]).dtype
+        state = np.zeros(self.hilb_dim, dtype=dtype)
 
         for ampl, vertex in entries:
             state[self._graph.vertex_number(vertex)] = ampl
 
         return self._normalize(state)
 
     def ket(self, label):
@@ -494,15 +495,15 @@
         else:
             ret = self._simul_vec
 
         return ret
 
 
 
-    def simulate(self, time=None, state=None, initial_state=None):
+    def simulate(self, time=None, state=None):
         r"""
         Simulates the quantum walk.
 
         The simulation progresses by iteratively applying 
         the evolution operator to the outcome of its prior 
         application, initiating from the specified initial state.
 
@@ -525,20 +526,14 @@
                 to ``end`` (inclusive)
                 that is a multiple of ``step``.
 
         state : :class:`numpy.array`, default=None
             The starting state onto which the evolution operator
             will be applied.
 
-        initial_state :
-            .. deprecated: 2.0
-                ``initial_state`` will be removed in version 2.1,
-                it is replaced by ``state`` because
-                the latter is more concise.
-
         Returns
         -------
         states : :class:`numpy.ndarray`.
             States retained during the simulation where
             ``states[i]`` is the ``i``-th saved state.
 
         Raises
@@ -586,21 +581,14 @@
         ############################################
         if time is None:
             raise ValueError(
                 "``time` not specified`. "
                 + "Must be an int or tuple of int."
             )
 
-        if initial_state is not None:
-            warn("``initial_state`` will be removed in version 2.1,"
-                 + "it is replaced by ``state`` because"
-                 + "the latter is more concise.")
-            if state is None:
-                state = initial_state
-
         if state is None:
             raise ValueError(
                 "``state`` not specified. "
                 + "Expected a np.array."
             )
 
         if len(state) != self.hilb_dim:
```

### Comparing `hiperwalk-2.0b11/tests/unit/binary_search_test.py` & `hiperwalk-2.0b12/tests/unit/binary_search_test.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/tests/unit/coined_cycle.py` & `hiperwalk-2.0b12/tests/unit/coined_cycle.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,38 +75,38 @@
     @unittest.skipIf(not TEST_HPC, 'Skipping hpc tests.')
     def test_hpc_clockwise_roundabout(self):
         hpw.set_hpc('cpu')
         self.qw.set_shift('persistent')
         self.qw.set_coin('I')
         self.qw.set_marked([])
 
-        init_state = self.qw.state([1, (0, 1)])
+        init_state = self.qw.ket((0, 1))
 
         num_steps = self.num_vert
         final_state = self.qw.simulate(num_steps, init_state)[0]
 
         self.assertTrue(np.all(init_state == final_state))
 
     @unittest.skipIf(not TEST_HPC, 'Skipping hpc tests.')
     def test_hpc_anticlockwise_roundabout(self):
         hpw.set_hpc('cpu')
         self.qw.set_shift('persistent')
         self.qw.set_coin('I')
         self.qw.set_marked([])
 
-        init_state = self.qw.state([1, (0, self.num_vert - 1)])
+        init_state = self.qw.ket((0, self.num_vert - 1))
 
         num_steps = self.num_vert
         final_state = self.qw.simulate(num_steps, init_state)[0]
 
         self.assertTrue(np.all(init_state == final_state))
 
     @unittest.skipIf(not TEST_HPC, 'Skipping hpc tests.')
     def test_hpc_evolution_operator_matches_nonhpc(self):
-        init_state = self.qw.state([1, (0, 1)])
+        init_state = self.qw.ket((0, 1))
         num_steps = 2*self.num_vert
 
         hpw.set_hpc(None)
         states = self.qw.simulate((num_steps, 1), init_state)
 
         hpw.set_hpc('cpu')
         hpc_states = self.qw.simulate((num_steps, 1), init_state)
```

### Comparing `hiperwalk-2.0b11/tests/unit/coined_line.py` & `hiperwalk-2.0b12/tests/unit/coined_line.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     @unittest.skipIf(not TEST_HPC, 'Skipping hpc tests.')
     def test_hpc_default_evolution_operator(self):
 
         num_steps = self.num_vert // 2
         center = self.num_vert // 2
         entries = [[1, (center, center + 1)],
                    [-1j, (center, center - 1)]]
-        init_state = self.qw.state(*entries)
+        init_state = self.qw.state(entries)
 
         hpw.set_hpc(None)
         states = self.qw.simulate((num_steps, 1), init_state)
         hpw.set_hpc('cpu')
         hpc_states = self.qw.simulate((num_steps, 1), init_state)
 
         self.assertTrue(
```

### Comparing `hiperwalk-2.0b11/tests/unit/complete.py` & `hiperwalk-2.0b12/tests/unit/complete.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/tests/unit/complete_bipartite.py` & `hiperwalk-2.0b12/tests/unit/complete_bipartite.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/tests/unit/continuous_time.py` & `hiperwalk-2.0b12/tests/unit/continuous_time.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/tests/unit/graph.py` & `hiperwalk-2.0b12/tests/unit/graph.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/tests/unit/hypercube.py` & `hiperwalk-2.0b12/tests/unit/hypercube.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/tests/unit/multigraph.py` & `hiperwalk-2.0b12/tests/unit/multigraph.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/.gitignore` & `hiperwalk-2.0b12/.gitignore`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/LICENSE` & `hiperwalk-2.0b12/LICENSE`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/README.md` & `hiperwalk-2.0b12/README.md`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b11/pyproject.toml` & `hiperwalk-2.0b12/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hiperwalk"
-version = "2.0b11"
+version = "2.0b12"
 description = "High-Performance Quantum Walk Simulator"
 license = {file="LICENSE"}
 readme = "README.md"
 authors = [
   { name="Gustavo Bezerra", email="gbezerra@posgrad.lncc.br" },
   { name="Paulo Motta", email="prmottajr@gmail.com" },
   { name="Renato Portugal", email="portugal@lncc.br" },
```

### Comparing `hiperwalk-2.0b11/PKG-INFO` & `hiperwalk-2.0b12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hiperwalk
-Version: 2.0b11
+Version: 2.0b12
 Summary: High-Performance Quantum Walk Simulator
 Project-URL: homepage, http://qubit.lncc.br/qwalk/
 Project-URL: documentation, https://hiperwalk.readthedocs.io/
 Project-URL: source, https://github.com/hiperwalk/hiperwalk
 Author-email: Gustavo Bezerra <gbezerra@posgrad.lncc.br>, Paulo Motta <prmottajr@gmail.com>, Renato Portugal <portugal@lncc.br>
 Maintainer-email: Hiperwalk Organization <hiperwalk@gmail.com>
 License: GNU Lesser General Public License
```

