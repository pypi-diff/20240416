# Comparing `tmp/pyquil_grpc_web-4.9.0rc3.tar.gz` & `tmp/pyquil_grpc_web-4.9.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyquil_grpc_web-4.9.0rc3.tar", max compression
+gzip compressed data, was "pyquil_grpc_web-4.9.1rc0.tar", max compression
```

## Comparing `pyquil_grpc_web-4.9.0rc3.tar` & `pyquil_grpc_web-4.9.1rc0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0    11358 2024-04-12 19:00:24.562604 pyquil_grpc_web-4.9.0rc3/LICENSE
--rw-r--r--   0        0        0     1779 2024-04-12 19:00:24.562604 pyquil_grpc_web-4.9.0rc3/NOTICE.md
--rw-r--r--   0        0        0     8944 2024-04-12 19:00:24.562604 pyquil_grpc_web-4.9.0rc3/README.md
--rw-r--r--   0        0        0     3113 2024-04-12 19:00:39.758609 pyquil_grpc_web-4.9.0rc3/pyproject.toml
--rw-r--r--   0        0        0      159 2024-04-12 19:00:24.802604 pyquil_grpc_web-4.9.0rc3/pyquil/__init__.py
--rw-r--r--   0        0        0     1088 2024-04-12 19:00:39.758609 pyquil_grpc_web-4.9.0rc3/pyquil/_version.py
--rw-r--r--   0        0        0     2129 2024-04-12 19:00:24.802604 pyquil_grpc_web-4.9.0rc3/pyquil/api/__init__.py
--rw-r--r--   0        0        0     8884 2024-04-12 19:00:24.802604 pyquil_grpc_web-4.9.0rc3/pyquil/api/_abstract_compiler.py
--rw-r--r--   0        0        0     7377 2024-04-12 19:00:24.802604 pyquil_grpc_web-4.9.0rc3/pyquil/api/_benchmark.py
--rw-r--r--   0        0        0     9942 2024-04-12 19:00:24.802604 pyquil_grpc_web-4.9.0rc3/pyquil/api/_compiler.py
--rw-r--r--   0        0        0     5554 2024-04-12 19:00:24.802604 pyquil_grpc_web-4.9.0rc3/pyquil/api/_compiler_client.py
--rw-r--r--   0        0        0     4265 2024-04-12 19:00:24.802604 pyquil_grpc_web-4.9.0rc3/pyquil/api/_errors.py
--rw-r--r--   0        0        0     1010 2024-04-12 19:00:24.802604 pyquil_grpc_web-4.9.0rc3/pyquil/api/_logger.py
--rw-r--r--   0        0        0     7568 2024-04-12 19:00:24.802604 pyquil_grpc_web-4.9.0rc3/pyquil/api/_qam.py
--rw-r--r--   0        0        0    11336 2024-04-12 19:00:24.802604 pyquil_grpc_web-4.9.0rc3/pyquil/api/_qpu.py
--rw-r--r--   0        0        0    55258 2024-04-12 19:00:24.802604 pyquil_grpc_web-4.9.0rc3/pyquil/api/_quantum_computer.py
--rw-r--r--   0        0        0     8637 2024-04-12 19:00:24.802604 pyquil_grpc_web-4.9.0rc3/pyquil/api/_qvm.py
--rw-r--r--   0        0        0     5562 2024-04-12 19:00:24.802604 pyquil_grpc_web-4.9.0rc3/pyquil/api/_rewrite_arithmetic.py
--rw-r--r--   0        0        0    10749 2024-04-12 19:00:24.802604 pyquil_grpc_web-4.9.0rc3/pyquil/api/_wavefunction_simulator.py
--rw-r--r--   0        0        0      369 2024-04-12 19:00:24.802604 pyquil_grpc_web-4.9.0rc3/pyquil/diagnostics.py
--rw-r--r--   0        0        0     1371 2024-04-12 19:00:24.802604 pyquil_grpc_web-4.9.0rc3/pyquil/experiment/__init__.py
--rw-r--r--   0        0        0      896 2024-04-12 19:00:24.802604 pyquil_grpc_web-4.9.0rc3/pyquil/experiment/_calibration.py
--rw-r--r--   0        0        0    15705 2024-04-12 19:00:24.802604 pyquil_grpc_web-4.9.0rc3/pyquil/experiment/_group.py
--rw-r--r--   0        0        0    22783 2024-04-12 19:00:24.802604 pyquil_grpc_web-4.9.0rc3/pyquil/experiment/_main.py
--rw-r--r--   0        0        0     8213 2024-04-12 19:00:24.802604 pyquil_grpc_web-4.9.0rc3/pyquil/experiment/_memory.py
--rw-r--r--   0        0        0     5547 2024-04-12 19:00:24.802604 pyquil_grpc_web-4.9.0rc3/pyquil/experiment/_program.py
--rw-r--r--   0        0        0     9047 2024-04-12 19:00:24.802604 pyquil_grpc_web-4.9.0rc3/pyquil/experiment/_result.py
--rw-r--r--   0        0        0     7469 2024-04-12 19:00:24.802604 pyquil_grpc_web-4.9.0rc3/pyquil/experiment/_setting.py
--rw-r--r--   0        0        0      934 2024-04-12 19:00:24.802604 pyquil_grpc_web-4.9.0rc3/pyquil/experiment/_symmetrization.py
--rw-r--r--   0        0        0      282 2024-04-12 19:00:24.802604 pyquil_grpc_web-4.9.0rc3/pyquil/external/README.md
--rw-r--r--   0        0        0        0 2024-04-12 19:00:24.802604 pyquil_grpc_web-4.9.0rc3/pyquil/external/__init__.py
--rw-r--r--   0        0        0     9858 2024-04-12 19:00:24.802604 pyquil_grpc_web-4.9.0rc3/pyquil/external/rpcq.py
--rw-r--r--   0        0        0    42387 2024-04-12 19:00:24.802604 pyquil_grpc_web-4.9.0rc3/pyquil/gates.py
--rw-r--r--   0        0        0      201 2024-04-12 19:00:24.802604 pyquil_grpc_web-4.9.0rc3/pyquil/latex/__init__.py
--rw-r--r--   0        0        0    18720 2024-04-12 19:00:24.802604 pyquil_grpc_web-4.9.0rc3/pyquil/latex/_diagram.py
--rw-r--r--   0        0        0     3452 2024-04-12 19:00:24.802604 pyquil_grpc_web-4.9.0rc3/pyquil/latex/_ipython.py
--rw-r--r--   0        0        0     4041 2024-04-12 19:00:24.802604 pyquil_grpc_web-4.9.0rc3/pyquil/latex/_main.py
--rw-r--r--   0        0        0     1266 2024-04-12 19:00:24.802604 pyquil_grpc_web-4.9.0rc3/pyquil/latex/latex_generation.py
--rw-r--r--   0        0        0    31958 2024-04-12 19:00:24.802604 pyquil_grpc_web-4.9.0rc3/pyquil/noise.py
--rw-r--r--   0        0        0     3346 2024-04-12 19:00:24.802604 pyquil_grpc_web-4.9.0rc3/pyquil/noise_gates.py
--rw-r--r--   0        0        0    15865 2024-04-12 19:00:24.806604 pyquil_grpc_web-4.9.0rc3/pyquil/operator_estimation.py
--rw-r--r--   0        0        0    42310 2024-04-12 19:00:24.806604 pyquil_grpc_web-4.9.0rc3/pyquil/paulis.py
--rw-r--r--   0        0        0        0 2024-04-12 19:00:24.806604 pyquil_grpc_web-4.9.0rc3/pyquil/py.typed
--rw-r--r--   0        0        0    19676 2024-04-12 19:00:24.806604 pyquil_grpc_web-4.9.0rc3/pyquil/pyqvm.py
--rw-r--r--   0        0        0      336 2024-04-12 19:00:24.806604 pyquil_grpc_web-4.9.0rc3/pyquil/quantum_processor/__init__.py
--rw-r--r--   0        0        0     1662 2024-04-12 19:00:24.806604 pyquil_grpc_web-4.9.0rc3/pyquil/quantum_processor/_base.py
--rw-r--r--   0        0        0        0 2024-04-12 19:00:24.806604 pyquil_grpc_web-4.9.0rc3/pyquil/quantum_processor/_isa.py
--rw-r--r--   0        0        0      774 2024-04-12 19:00:24.806604 pyquil_grpc_web-4.9.0rc3/pyquil/quantum_processor/compiler.py
--rw-r--r--   0        0        0     1856 2024-04-12 19:00:24.806604 pyquil_grpc_web-4.9.0rc3/pyquil/quantum_processor/graph.py
--rw-r--r--   0        0        0     2714 2024-04-12 19:00:24.806604 pyquil_grpc_web-4.9.0rc3/pyquil/quantum_processor/qcs.py
--rw-r--r--   0        0        0      417 2024-04-12 19:00:24.806604 pyquil_grpc_web-4.9.0rc3/pyquil/quantum_processor/transformers/__init__.py
--rw-r--r--   0        0        0      331 2024-04-12 19:00:24.806604 pyquil_grpc_web-4.9.0rc3/pyquil/quantum_processor/transformers/compiler_isa_to_graph.py
--rw-r--r--   0        0        0     5279 2024-04-12 19:00:24.806604 pyquil_grpc_web-4.9.0rc3/pyquil/quantum_processor/transformers/graph_to_compiler_isa.py
--rw-r--r--   0        0        0    11791 2024-04-12 19:00:24.806604 pyquil_grpc_web-4.9.0rc3/pyquil/quantum_processor/transformers/qcs_isa_to_compiler_isa.py
--rw-r--r--   0        0        0      224 2024-04-12 19:00:24.806604 pyquil_grpc_web-4.9.0rc3/pyquil/quantum_processor/transformers/qcs_isa_to_graph.py
--rw-r--r--   0        0        0    48378 2024-04-12 19:00:24.806604 pyquil_grpc_web-4.9.0rc3/pyquil/quil.py
--rw-r--r--   0        0        0    44767 2024-04-12 19:00:24.806604 pyquil_grpc_web-4.9.0rc3/pyquil/quilatom.py
--rw-r--r--   0        0        0   103651 2024-04-12 19:00:24.806604 pyquil_grpc_web-4.9.0rc3/pyquil/quilbase.py
--rw-r--r--   0        0        0     4191 2024-04-12 19:00:24.806604 pyquil_grpc_web-4.9.0rc3/pyquil/quiltcalibrations.py
--rw-r--r--   0        0        0    10338 2024-04-12 19:00:24.806604 pyquil_grpc_web-4.9.0rc3/pyquil/quiltwaveforms.py
--rw-r--r--   0        0        0      511 2024-04-12 19:00:24.806604 pyquil_grpc_web-4.9.0rc3/pyquil/simulation/__init__.py
--rw-r--r--   0        0        0    13329 2024-04-12 19:00:24.806604 pyquil_grpc_web-4.9.0rc3/pyquil/simulation/_numpy.py
--rw-r--r--   0        0        0    15815 2024-04-12 19:00:24.806604 pyquil_grpc_web-4.9.0rc3/pyquil/simulation/_reference.py
--rw-r--r--   0        0        0    14218 2024-04-12 19:00:24.806604 pyquil_grpc_web-4.9.0rc3/pyquil/simulation/matrices.py
--rw-r--r--   0        0        0    19105 2024-04-12 19:00:24.806604 pyquil_grpc_web-4.9.0rc3/pyquil/simulation/tools.py
--rw-r--r--   0        0        0     8766 2024-04-12 19:00:24.806604 pyquil_grpc_web-4.9.0rc3/pyquil/wavefunction.py
--rw-r--r--   0        0        0    11078 1970-01-01 00:00:00.000000 pyquil_grpc_web-4.9.0rc3/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-04-16 18:28:15.355920 pyquil_grpc_web-4.9.1rc0/LICENSE
+-rw-r--r--   0        0        0     1779 2024-04-16 18:28:15.355920 pyquil_grpc_web-4.9.1rc0/NOTICE.md
+-rw-r--r--   0        0        0     8944 2024-04-16 18:28:15.355920 pyquil_grpc_web-4.9.1rc0/README.md
+-rw-r--r--   0        0        0     3113 2024-04-16 18:28:31.231907 pyquil_grpc_web-4.9.1rc0/pyproject.toml
+-rw-r--r--   0        0        0      159 2024-04-16 18:28:15.591920 pyquil_grpc_web-4.9.1rc0/pyquil/__init__.py
+-rw-r--r--   0        0        0     1088 2024-04-16 18:28:31.231907 pyquil_grpc_web-4.9.1rc0/pyquil/_version.py
+-rw-r--r--   0        0        0     2129 2024-04-16 18:28:15.591920 pyquil_grpc_web-4.9.1rc0/pyquil/api/__init__.py
+-rw-r--r--   0        0        0     8884 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/api/_abstract_compiler.py
+-rw-r--r--   0        0        0     7377 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/api/_benchmark.py
+-rw-r--r--   0        0        0     9942 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/api/_compiler.py
+-rw-r--r--   0        0        0     5554 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/api/_compiler_client.py
+-rw-r--r--   0        0        0     4265 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/api/_errors.py
+-rw-r--r--   0        0        0     1010 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/api/_logger.py
+-rw-r--r--   0        0        0     7568 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/api/_qam.py
+-rw-r--r--   0        0        0    11336 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/api/_qpu.py
+-rw-r--r--   0        0        0    55258 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/api/_quantum_computer.py
+-rw-r--r--   0        0        0     8637 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/api/_qvm.py
+-rw-r--r--   0        0        0     5562 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/api/_rewrite_arithmetic.py
+-rw-r--r--   0        0        0    10749 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/api/_wavefunction_simulator.py
+-rw-r--r--   0        0        0      369 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/diagnostics.py
+-rw-r--r--   0        0        0     1371 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/experiment/__init__.py
+-rw-r--r--   0        0        0      896 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/experiment/_calibration.py
+-rw-r--r--   0        0        0    15705 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/experiment/_group.py
+-rw-r--r--   0        0        0    22783 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/experiment/_main.py
+-rw-r--r--   0        0        0     8213 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/experiment/_memory.py
+-rw-r--r--   0        0        0     5547 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/experiment/_program.py
+-rw-r--r--   0        0        0     9047 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/experiment/_result.py
+-rw-r--r--   0        0        0     7469 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/experiment/_setting.py
+-rw-r--r--   0        0        0      934 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/experiment/_symmetrization.py
+-rw-r--r--   0        0        0      282 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/external/README.md
+-rw-r--r--   0        0        0        0 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/external/__init__.py
+-rw-r--r--   0        0        0     9858 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/external/rpcq.py
+-rw-r--r--   0        0        0    42387 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/gates.py
+-rw-r--r--   0        0        0      201 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/latex/__init__.py
+-rw-r--r--   0        0        0    18720 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/latex/_diagram.py
+-rw-r--r--   0        0        0     3452 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/latex/_ipython.py
+-rw-r--r--   0        0        0     4041 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/latex/_main.py
+-rw-r--r--   0        0        0     1266 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/latex/latex_generation.py
+-rw-r--r--   0        0        0    31958 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/noise.py
+-rw-r--r--   0        0        0     3346 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/noise_gates.py
+-rw-r--r--   0        0        0    15865 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/operator_estimation.py
+-rw-r--r--   0        0        0    42310 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/paulis.py
+-rw-r--r--   0        0        0        0 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/py.typed
+-rw-r--r--   0        0        0    19676 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/pyqvm.py
+-rw-r--r--   0        0        0      336 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/quantum_processor/__init__.py
+-rw-r--r--   0        0        0     1662 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/quantum_processor/_base.py
+-rw-r--r--   0        0        0        0 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/quantum_processor/_isa.py
+-rw-r--r--   0        0        0      774 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/quantum_processor/compiler.py
+-rw-r--r--   0        0        0     1856 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/quantum_processor/graph.py
+-rw-r--r--   0        0        0     2714 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/quantum_processor/qcs.py
+-rw-r--r--   0        0        0      417 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/quantum_processor/transformers/__init__.py
+-rw-r--r--   0        0        0      331 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/quantum_processor/transformers/compiler_isa_to_graph.py
+-rw-r--r--   0        0        0     5279 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/quantum_processor/transformers/graph_to_compiler_isa.py
+-rw-r--r--   0        0        0    11791 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/quantum_processor/transformers/qcs_isa_to_compiler_isa.py
+-rw-r--r--   0        0        0      224 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/quantum_processor/transformers/qcs_isa_to_graph.py
+-rw-r--r--   0        0        0    48378 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/quil.py
+-rw-r--r--   0        0        0    44831 2024-04-16 18:28:15.595919 pyquil_grpc_web-4.9.1rc0/pyquil/quilatom.py
+-rw-r--r--   0        0        0   103651 2024-04-16 18:28:15.599919 pyquil_grpc_web-4.9.1rc0/pyquil/quilbase.py
+-rw-r--r--   0        0        0     4191 2024-04-16 18:28:15.599919 pyquil_grpc_web-4.9.1rc0/pyquil/quiltcalibrations.py
+-rw-r--r--   0        0        0    10338 2024-04-16 18:28:15.599919 pyquil_grpc_web-4.9.1rc0/pyquil/quiltwaveforms.py
+-rw-r--r--   0        0        0      511 2024-04-16 18:28:15.599919 pyquil_grpc_web-4.9.1rc0/pyquil/simulation/__init__.py
+-rw-r--r--   0        0        0    13329 2024-04-16 18:28:15.599919 pyquil_grpc_web-4.9.1rc0/pyquil/simulation/_numpy.py
+-rw-r--r--   0        0        0    15815 2024-04-16 18:28:15.599919 pyquil_grpc_web-4.9.1rc0/pyquil/simulation/_reference.py
+-rw-r--r--   0        0        0    14218 2024-04-16 18:28:15.599919 pyquil_grpc_web-4.9.1rc0/pyquil/simulation/matrices.py
+-rw-r--r--   0        0        0    19105 2024-04-16 18:28:15.599919 pyquil_grpc_web-4.9.1rc0/pyquil/simulation/tools.py
+-rw-r--r--   0        0        0     8766 2024-04-16 18:28:15.599919 pyquil_grpc_web-4.9.1rc0/pyquil/wavefunction.py
+-rw-r--r--   0        0        0    11078 1970-01-01 00:00:00.000000 pyquil_grpc_web-4.9.1rc0/PKG-INFO
```

### Comparing `pyquil_grpc_web-4.9.0rc3/LICENSE` & `pyquil_grpc_web-4.9.1rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/NOTICE.md` & `pyquil_grpc_web-4.9.1rc0/NOTICE.md`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/README.md` & `pyquil_grpc_web-4.9.1rc0/README.md`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyproject.toml` & `pyquil_grpc_web-4.9.1rc0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [project]
 name = "pyquil-grpc-web"
 
 [tool.poetry]
 name = "pyquil-grpc-web"
-version = "4.9.0-rc.3"
+version = "4.9.1-rc.0"
 description = "A Python library for creating Quantum Instruction Language (Quil) programs."
 authors = [ "Rigetti Computing <softapps@rigetti.com>",]
 readme = "README.md"
 repository = "https://github.com/rigetti/pyquil.git"
 documentation = "https://pyquil-docs.rigetti.com"
 license = "Apache-2.0"
 classifiers = [ "Development Status :: 5 - Production/Stable", "License :: OSI Approved :: Apache Software License", "Programming Language :: Python :: 3.8", "Programming Language :: Python :: 3.9", "Operating System :: OS Independent",]
```

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/_version.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/_version.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/api/__init__.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/api/_abstract_compiler.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/api/_abstract_compiler.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/api/_benchmark.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/api/_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/api/_compiler.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/api/_compiler.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/api/_compiler_client.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/api/_compiler_client.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/api/_errors.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/api/_errors.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/api/_logger.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/api/_logger.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/api/_qam.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/api/_qam.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/api/_qpu.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/api/_qpu.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/api/_quantum_computer.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/api/_quantum_computer.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/api/_qvm.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/api/_qvm.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/api/_rewrite_arithmetic.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/api/_rewrite_arithmetic.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/api/_wavefunction_simulator.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/api/_wavefunction_simulator.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/experiment/__init__.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/experiment/_calibration.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/experiment/_calibration.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/experiment/_group.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/experiment/_group.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/experiment/_main.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/experiment/_main.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/experiment/_memory.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/experiment/_memory.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/experiment/_program.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/experiment/_program.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/experiment/_result.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/experiment/_result.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/experiment/_setting.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/experiment/_setting.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/experiment/_symmetrization.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/experiment/_symmetrization.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/external/rpcq.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/external/rpcq.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/gates.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/gates.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/latex/_diagram.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/latex/_diagram.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/latex/_ipython.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/latex/_ipython.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/latex/_main.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/latex/_main.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/latex/latex_generation.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/latex/latex_generation.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/noise.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/noise.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/noise_gates.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/noise_gates.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/operator_estimation.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/operator_estimation.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/paulis.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/paulis.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/pyqvm.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/pyqvm.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/quantum_processor/_base.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/quantum_processor/_base.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/quantum_processor/compiler.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/quantum_processor/compiler.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/quantum_processor/graph.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/quantum_processor/graph.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/quantum_processor/qcs.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/quantum_processor/qcs.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/quantum_processor/transformers/graph_to_compiler_isa.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/quantum_processor/transformers/graph_to_compiler_isa.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/quantum_processor/transformers/qcs_isa_to_compiler_isa.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/quantum_processor/transformers/qcs_isa_to_compiler_isa.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/quil.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/quil.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/quilatom.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/quilatom.py`

 * *Files 1% similar despite different names*

```diff
@@ -574,17 +574,19 @@
         Note that expression simplification can be slow for large recursive expressions.
         """
         try:
             if dtype != object:
                 return np.asarray(self._evaluate(), dtype=dtype)
             raise ValueError
         except ValueError:
-            # Note: The `None` here is a placeholder for the expression in the numpy array.
-            # The expression instance will still be accessible in the array.
-            return np.array(None, dtype=object)
+            # np.asarray(self, ...) would cause an infinite recursion error, so we build the array with a
+            # placeholder value, then replace it with self after.
+            array = np.asarray(None, dtype=object)
+            array.flat[0] = self
+            return array
 
 
 ParameterSubstitutionsMapDesignator = Mapping[Union["Parameter", "MemoryReference"], ExpressionValueDesignator]
 
 
 def substitute(expr: ExpressionDesignator, d: ParameterSubstitutionsMapDesignator) -> ExpressionDesignator:
     """
```

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/quilbase.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/quilbase.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/quiltcalibrations.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/quiltcalibrations.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/quiltwaveforms.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/quiltwaveforms.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/simulation/_numpy.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/simulation/_numpy.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/simulation/_reference.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/simulation/_reference.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/simulation/matrices.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/simulation/matrices.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/simulation/tools.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/simulation/tools.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/pyquil/wavefunction.py` & `pyquil_grpc_web-4.9.1rc0/pyquil/wavefunction.py`

 * *Files identical despite different names*

### Comparing `pyquil_grpc_web-4.9.0rc3/PKG-INFO` & `pyquil_grpc_web-4.9.1rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyquil-grpc-web
-Version: 4.9.0rc3
+Version: 4.9.1rc0
 Summary: A Python library for creating Quantum Instruction Language (Quil) programs.
 Home-page: https://github.com/rigetti/pyquil.git
 License: Apache-2.0
 Keywords: quantum,quil,programming,hybrid
 Author: Rigetti Computing
 Author-email: softapps@rigetti.com
 Requires-Python: >=3.8,<=3.12
```

