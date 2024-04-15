# Comparing `tmp/pcdr-0.4.8b1.tar.gz` & `tmp/pcdr-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcdr-0.4.8b1.tar", last modified: Mon Feb 26 03:09:57 2024, max compression
+gzip compressed data, was "pcdr-1.0.0a1.tar", last modified: Mon Apr 15 23:29:26 2024, max compression
```

## Comparing `pcdr-0.4.8b1.tar` & `pcdr-1.0.0a1.tar`

### file list

```diff
@@ -1,42 +1,48 @@
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-02-26 03:09:57.312424 pcdr-0.4.8b1/
--rw-r--r--   0 j         (1000) j         (1000)       72 2023-08-09 21:29:02.000000 pcdr-0.4.8b1/LICENSE
--rw-r--r--   0 j         (1000) j         (1000)      801 2024-02-26 03:09:57.308424 pcdr-0.4.8b1/PKG-INFO
--rw-r--r--   0 j         (1000) j         (1000)      262 2023-08-09 22:06:58.000000 pcdr-0.4.8b1/README.md
--rw-r--r--   0 j         (1000) j         (1000)      623 2024-02-26 03:09:17.000000 pcdr-0.4.8b1/pyproject.toml
--rw-r--r--   0 j         (1000) j         (1000)       38 2024-02-26 03:09:57.312424 pcdr-0.4.8b1/setup.cfg
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-02-26 03:09:57.304423 pcdr-0.4.8b1/src/
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-02-26 03:09:57.308424 pcdr-0.4.8b1/src/pcdr/
--rw-r--r--   0 j         (1000) j         (1000)     2342 2024-02-26 03:09:33.000000 pcdr-0.4.8b1/src/pcdr/__abandoned.py
--rw-r--r--   0 j         (1000) j         (1000)     1404 2024-02-26 03:09:33.000000 pcdr-0.4.8b1/src/pcdr/__init__.py
--rw-r--r--   0 j         (1000) j         (1000)     3989 2024-02-26 03:09:33.000000 pcdr-0.4.8b1/src/pcdr/basictermplot.py
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-02-26 03:09:57.308424 pcdr-0.4.8b1/src/pcdr/eventual_ideas/
--rw-r--r--   0 j         (1000) j         (1000)      385 2024-02-26 03:09:33.000000 pcdr-0.4.8b1/src/pcdr/eventual_ideas/samples.py
--rw-r--r--   0 j         (1000) j         (1000)     1540 2024-02-26 03:09:33.000000 pcdr-0.4.8b1/src/pcdr/fileio.py
--rw-r--r--   0 j         (1000) j         (1000)     2982 2024-02-26 03:09:33.000000 pcdr-0.4.8b1/src/pcdr/function.py
--rw-r--r--   0 j         (1000) j         (1000)     1783 2024-02-26 03:09:33.000000 pcdr-0.4.8b1/src/pcdr/gnuradio_misc.py
--rw-r--r--   0 j         (1000) j         (1000)     3154 2024-02-26 03:09:33.000000 pcdr-0.4.8b1/src/pcdr/gnuradio_receiver.py
--rw-r--r--   0 j         (1000) j         (1000)     6559 2024-02-26 03:09:33.000000 pcdr-0.4.8b1/src/pcdr/gnuradio_sender.py
--rw-r--r--   0 j         (1000) j         (1000)     7980 2024-02-26 03:09:33.000000 pcdr-0.4.8b1/src/pcdr/gui.py
--rw-r--r--   0 j         (1000) j         (1000)     9644 2024-02-26 03:09:33.000000 pcdr-0.4.8b1/src/pcdr/helpers.py
--rw-r--r--   0 j         (1000) j         (1000)     5009 2024-02-26 03:09:33.000000 pcdr-0.4.8b1/src/pcdr/modulators.py
--rw-r--r--   0 j         (1000) j         (1000)     1909 2024-02-26 03:09:33.000000 pcdr-0.4.8b1/src/pcdr/osmocom_queued_rx_flowgraph.py
--rw-r--r--   0 j         (1000) j         (1000)     3849 2024-02-26 03:09:33.000000 pcdr-0.4.8b1/src/pcdr/osmocom_queued_tx_flowgraph.py
--rw-r--r--   0 j         (1000) j         (1000)     6689 2024-02-26 03:09:33.000000 pcdr-0.4.8b1/src/pcdr/our_GR_blocks.py
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-02-26 03:09:57.308424 pcdr-0.4.8b1/src/pcdr/queue/
--rw-r--r--   0 j         (1000) j         (1000)       51 2024-02-26 03:09:33.000000 pcdr-0.4.8b1/src/pcdr/queue/__init__.py
--rw-r--r--   0 j         (1000) j         (1000)     6324 2024-02-26 03:09:33.000000 pcdr-0.4.8b1/src/pcdr/queue/sink.py
--rw-r--r--   0 j         (1000) j         (1000)     1182 2024-02-26 03:09:33.000000 pcdr-0.4.8b1/src/pcdr/queue/source.py
--rw-r--r--   0 j         (1000) j         (1000)     2429 2024-02-26 03:09:33.000000 pcdr-0.4.8b1/src/pcdr/queue_to_guisink_flowgraph.py
--rwxr-xr-x   0 j         (1000) j         (1000)     5347 2024-02-26 03:09:33.000000 pcdr-0.4.8b1/src/pcdr/queue_to_waterfall_flowgraph.py
--rw-r--r--   0 j         (1000) j         (1000)     4106 2024-02-26 03:09:33.000000 pcdr-0.4.8b1/src/pcdr/simple.py
--rw-r--r--   0 j         (1000) j         (1000)      493 2024-02-26 03:09:33.000000 pcdr-0.4.8b1/src/pcdr/types_and_contracts.py
--rw-r--r--   0 j         (1000) j         (1000)     3013 2024-02-26 03:09:33.000000 pcdr-0.4.8b1/src/pcdr/vector_to_guisink_flowgraph.py
--rw-r--r--   0 j         (1000) j         (1000)     3367 2024-02-26 03:09:33.000000 pcdr-0.4.8b1/src/pcdr/vector_tx_flowgraphs.py
--rw-r--r--   0 j         (1000) j         (1000)    44660 2024-02-26 03:09:33.000000 pcdr-0.4.8b1/src/pcdr/wavegen.py
--rw-r--r--   0 j         (1000) j         (1000)     1441 2024-02-26 03:09:33.000000 pcdr-0.4.8b1/src/pcdr/wrapped_GR_blocks.py
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-02-26 03:09:57.308424 pcdr-0.4.8b1/src/pcdr.egg-info/
--rw-r--r--   0 j         (1000) j         (1000)      801 2024-02-26 03:09:57.000000 pcdr-0.4.8b1/src/pcdr.egg-info/PKG-INFO
--rw-r--r--   0 j         (1000) j         (1000)      915 2024-02-26 03:09:57.000000 pcdr-0.4.8b1/src/pcdr.egg-info/SOURCES.txt
--rw-r--r--   0 j         (1000) j         (1000)        1 2024-02-26 03:09:57.000000 pcdr-0.4.8b1/src/pcdr.egg-info/dependency_links.txt
--rw-r--r--   0 j         (1000) j         (1000)       26 2024-02-26 03:09:57.000000 pcdr-0.4.8b1/src/pcdr.egg-info/requires.txt
--rw-r--r--   0 j         (1000) j         (1000)        5 2024-02-26 03:09:57.000000 pcdr-0.4.8b1/src/pcdr.egg-info/top_level.txt
+drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-15 23:29:26.770252 pcdr-1.0.0a1/
+-rw-r--r--   0 j         (1000) j         (1000)    35149 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/LICENSE
+-rw-r--r--   0 j         (1000) j         (1000)     1757 2024-04-15 23:29:26.770252 pcdr-1.0.0a1/PKG-INFO
+-rw-r--r--   0 j         (1000) j         (1000)     1191 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/README.md
+-rw-r--r--   0 j         (1000) j         (1000)      613 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/pyproject.toml
+-rw-r--r--   0 j         (1000) j         (1000)       38 2024-04-15 23:29:26.770252 pcdr-1.0.0a1/setup.cfg
+drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-15 23:29:26.762252 pcdr-1.0.0a1/src/
+drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-15 23:29:26.766252 pcdr-1.0.0a1/src/pcdr/
+-rw-r--r--   0 j         (1000) j         (1000)      768 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/__init__.py
+drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-15 23:29:26.766252 pcdr-1.0.0a1/src/pcdr/_beta/
+-rw-r--r--   0 j         (1000) j         (1000)     3106 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_beta/gnuradio_receiver.py
+-rw-r--r--   0 j         (1000) j         (1000)     7122 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_beta/gnuradio_sendlike.py
+-rw-r--r--   0 j         (1000) j         (1000)     1774 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_beta/osmocom_queued_rx_flowgraph.py
+-rw-r--r--   0 j         (1000) j         (1000)     3866 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_beta/osmocom_queued_tx_flowgraph.py
+-rw-r--r--   0 j         (1000) j         (1000)     9152 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_flow_impl.py
+-rw-r--r--   0 j         (1000) j         (1000)     2807 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_helpers.py
+drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-15 23:29:26.770252 pcdr-1.0.0a1/src/pcdr/_internal/
+-rw-r--r--   0 j         (1000) j         (1000)     3989 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_internal/basictermplot.py
+-rw-r--r--   0 j         (1000) j         (1000)     1565 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_internal/fileio.py
+-rw-r--r--   0 j         (1000) j         (1000)    13243 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_internal/misc.py
+-rw-r--r--   0 j         (1000) j         (1000)     7650 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_internal/our_GR_blocks.py
+-rw-r--r--   0 j         (1000) j         (1000)     2456 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_internal/queue_to_guisink_flowgraph.py
+-rwxr-xr-x   0 j         (1000) j         (1000)     5357 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_internal/queue_to_waterfall_flowgraph.py
+-rw-r--r--   0 j         (1000) j         (1000)      657 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_internal/types_and_contracts.py
+-rw-r--r--   0 j         (1000) j         (1000)     3013 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_internal/vector_to_guisink_flowgraph.py
+-rw-r--r--   0 j         (1000) j         (1000)     3430 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_internal/vector_tx_flowgraphs.py
+-rw-r--r--   0 j         (1000) j         (1000)     1451 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_internal/wrapped_GR_blocks.py
+-rw-r--r--   0 j         (1000) j         (1000)     5022 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_modulators.py
+drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-15 23:29:26.770252 pcdr-1.0.0a1/src/pcdr/_queue/
+-rw-r--r--   0 j         (1000) j         (1000)       51 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_queue/__init__.py
+-rw-r--r--   0 j         (1000) j         (1000)     6343 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_queue/sink.py
+-rw-r--r--   0 j         (1000) j         (1000)     1199 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_queue/source.py
+-rw-r--r--   0 j         (1000) j         (1000)    45382 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_wavegen.py
+-rw-r--r--   0 j         (1000) j         (1000)      141 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/flow.py
+drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-15 23:29:26.770252 pcdr-1.0.0a1/src/pcdr.egg-info/
+-rw-r--r--   0 j         (1000) j         (1000)     1757 2024-04-15 23:29:26.000000 pcdr-1.0.0a1/src/pcdr.egg-info/PKG-INFO
+-rw-r--r--   0 j         (1000) j         (1000)     1189 2024-04-15 23:29:26.000000 pcdr-1.0.0a1/src/pcdr.egg-info/SOURCES.txt
+-rw-r--r--   0 j         (1000) j         (1000)        1 2024-04-15 23:29:26.000000 pcdr-1.0.0a1/src/pcdr.egg-info/dependency_links.txt
+-rw-r--r--   0 j         (1000) j         (1000)       40 2024-04-15 23:29:26.000000 pcdr-1.0.0a1/src/pcdr.egg-info/requires.txt
+-rw-r--r--   0 j         (1000) j         (1000)        5 2024-04-15 23:29:26.000000 pcdr-1.0.0a1/src/pcdr.egg-info/top_level.txt
+drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-15 23:29:26.770252 pcdr-1.0.0a1/tests/
+-rw-r--r--   0 j         (1000) j         (1000)      838 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/tests/test_gnuradio_vector_tx_flowgraphs.py
+-rw-r--r--   0 j         (1000) j         (1000)      939 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/tests/test_gnuradio_write_file_and_read_file.py
+-rw-r--r--   0 j         (1000) j         (1000)      308 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/tests/test_helpers.py
+-rw-r--r--   0 j         (1000) j         (1000)     2988 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/tests/test_multiple.py
+-rw-r--r--   0 j         (1000) j         (1000)     5648 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/tests/test_other__blocks_for_testing.py
+-rw-r--r--   0 j         (1000) j         (1000)     2498 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/tests/test_our_GR_blocks.py
+-rw-r--r--   0 j         (1000) j         (1000)     1705 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/tests/test_simple.py
```

### Comparing `pcdr-0.4.8b1/pyproject.toml` & `pcdr-1.0.0a1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools>=42.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "pcdr"
-version = "0.4.8b1"
-# authors = [
-#   { name="james-pcdr" },
-# ]
-description = "GNU Radio-based transmit and receive wrapper functions and more"
+version = "1.0.0a1"
+authors = [
+  { name="james-pcdr" },
+]
+description = "GNU Radio-based transmit and receive wrappers and more"
 readme = "README.md"
 requires-python = ">=3.8"
-dependencies = ["numpy", "termcolor", "typeguard"]
+dependencies = ["numpy", "termcolor", "typeguard", "attrs>=21.1.0"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/python-can-define-radio/sdr-course"
-"Bug Tracker" = "https://github.com/python-can-define-radio/sdr-course/issues"
+"Homepage" = "https://github.com/python-can-define-radio/pcdr"
+"Bug Tracker" = "https://github.com/python-can-define-radio/pcdr/issues"
```

### Comparing `pcdr-0.4.8b1/src/pcdr/basictermplot.py` & `pcdr-1.0.0a1/src/pcdr/_internal/basictermplot.py`

 * *Files identical despite different names*

### Comparing `pcdr-0.4.8b1/src/pcdr/fileio.py` & `pcdr-1.0.0a1/src/pcdr/_internal/fileio.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from _typeshed import FileDescriptorOrPath
 
 import numpy as np
 
-from pcdr.types_and_contracts import TRealNum
+from pcdr._internal.types_and_contracts import TRealNum
 
 
 
 def writeRealCSV(filename, data_to_write):
     # type: (FileDescriptorOrPath, Iterable[TRealNum]) -> None
     with open(filename, "w") as outfile:
         for item in data_to_write:
@@ -25,22 +25,22 @@
             quad = item.imag
             outfile.write(f"{inphase},{quad}\n")
 
 
 def __readCSV(filename_csv: str, samp_rate: float, type_: Callable) -> Tuple[np.ndarray, np.ndarray]:
     
     ## This import must be here to avoid circular imports.
-    from pcdr.wavegen import createTimestamps
+    from pcdr._wavegen import make_timestamps_seconds
 
     with open(filename_csv) as f:
         contents = f.read().splitlines()
     
     num_samples = len(contents)
     max_time = num_samples / samp_rate
-    timestamps = createTimestamps(max_time, num_samples)
+    timestamps = make_timestamps_seconds(max_time, num_samples)
     contents_as_numbers = np.array(list(map(type_, contents)))
     return timestamps, contents_as_numbers
 
 
 def readRealCSV(filename_csv: str, samp_rate: float) -> Tuple[np.ndarray, np.ndarray]:
     __readCSV(filename_csv, samp_rate, float)
```

### Comparing `pcdr-0.4.8b1/src/pcdr/gnuradio_receiver.py` & `pcdr-1.0.0a1/src/pcdr/_beta/gnuradio_receiver.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from typing import List, Tuple
 import numpy as np
 import time
 from gnuradio import gr
 
-from pcdr.osmocom_queued_rx_flowgraph import osmocom_source_to_queue_sink, file_source_to_queue_sink
-from pcdr.gnuradio_misc import configure_graceful_exit
-from pcdr.helpers import queue_to_list, validate_hack_rf_receive
-from pcdr.types_and_contracts import SupportsQueueSink
+from pcdr._beta.osmocom_queued_rx_flowgraph import osmocom_source_to_queue_sink, file_source_to_queue_sink
+from pcdr._internal.misc import configure_graceful_exit
+from pcdr._internal.types_and_contracts import SupportsQueueSink
 
 
 
 
 def __run_block_and_return_queue_contents(tb: SupportsQueueSink, seconds: float):
     """Note: if seconds=-1, that means 'read till done'.
     Don't use seconds=-1 for the osmocom, as it will never finish."""
```

### Comparing `pcdr-0.4.8b1/src/pcdr/gnuradio_sender.py` & `pcdr-1.0.0a1/src/pcdr/_beta/gnuradio_sendlike.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,81 @@
+from distutils.version import StrictVersion
+from queue import Empty
+import signal
+import sys
 from typing import List, Optional, Sequence, TypeVar, Union
+
 import numpy as np
-from queue import Empty
-from pcdr.helpers import SimpleQueueTypeWrapped, queue_to_list, prepend_zeros_
-from pcdr.osmocom_queued_tx_flowgraph import queue_to_osmocom_sink, queue_to_print_sink, queue_to_string_file_sink, queue_to_file_sink
-from pcdr.vector_tx_flowgraphs import vector_to_file_sink, vector_to_osmocom_sink
-from pcdr.gnuradio_misc import configure_graceful_exit
-from pcdr.types_and_contracts import TRealNum, TRealOrComplexNum
-from pcdr.osmocom_queued_tx_flowgraph import queue_to_zmqpub_sink
-from pcdr.queue_to_guisink_flowgraph import queue_to_guisink
-from pcdr.vector_to_guisink_flowgraph import vector_to_guisink
-from pcdr.gnuradio_misc import configure_and_run_gui_flowgraph
+from gnuradio import gr
+
+from pcdr._beta.osmocom_queued_tx_flowgraph import queue_to_osmocom_sink, queue_to_print_sink, queue_to_string_file_sink, queue_to_file_sink, queue_to_zmqpub_sink
+from pcdr._internal.misc import SimpleQueueTypeWrapped, queue_to_list, prepend_zeros_, configure_graceful_exit
+from pcdr._internal.vector_tx_flowgraphs import vector_to_file_sink, vector_to_osmocom_sink
+from pcdr._internal.types_and_contracts import TRealNum, TRealOrComplexNum
+from pcdr._internal.queue_to_guisink_flowgraph import queue_to_guisink
+from pcdr._internal.vector_to_guisink_flowgraph import vector_to_guisink
+
+
+
+try:
+    ## Why this import is here:
+    ## We don't want Qt to be required for ALL pcdr uses;
+    ## just graphical ones.
+    from PyQt5 import Qt
+
+
+    def _configure_and_run_gui_flowgraph(top_block_cls, args):
+        """The portion of GNU Radio boilerplate that 
+        sets up the QT GUI Application."""
+        if StrictVersion("4.5.0") <= StrictVersion(Qt.qVersion()) < StrictVersion("5.0.0"):
+            style = gr.prefs().get_string('qtgui', 'style', 'raster')
+            Qt.QApplication.setGraphicsSystem(style)
+        qapp = Qt.QApplication(sys.argv)
+
+        tb = top_block_cls(*args)
+        tb.start()
+        tb.show()
+
+        def sig_handler(sig=None, frame=None):
+            Qt.QApplication.quit()
+
+        signal.signal(signal.SIGINT, sig_handler)
+        signal.signal(signal.SIGTERM, sig_handler)
 
+        timer = Qt.QTimer()
+        timer.start(500)
+        timer.timeout.connect(lambda: None)
 
-T = TypeVar('T')
+        def quitting():
+            tb.stop()
+            tb.wait()
+        qapp.aboutToQuit.connect(quitting)
+        qapp.exec_()
 
+except ModuleNotFoundError:
+    pass
 
 
-def pad_chunk_queue(data: np.ndarray, chunk_size: int) -> SimpleQueueTypeWrapped:
+def _pad_chunk_queue(data: np.ndarray, chunk_size: int) -> SimpleQueueTypeWrapped:
     """
     - numpy-ify
     - Pad `data` to a multiple of `chunk_size`
     - Split into chunks of that size
     - Convert to a queue of numpy arrays for gnuradio use
     
     Examples:
     >>> testdata = np.array([1, 2, 3], dtype=np.uint8)
-    >>> pcq = pad_chunk_queue(testdata, 2)
+    >>> pcq = _pad_chunk_queue(testdata, 2)
     >>> pcq.get()
     array([1.+0.j, 2.+0.j], dtype=complex64)
     >>> pcq.get()
     array([3.+0.j, 0.+0.j], dtype=complex64)
 
     >>> testdata = np.array([1, 2, 3], dtype=np.uint8)
-    >>> pcq = pad_chunk_queue(testdata, 5)
+    >>> pcq = _pad_chunk_queue(testdata, 5)
     >>> nparry = np.array(queue_to_list(pcq))
     >>> should_be = np.array([[1, 2, 3, 0, 0]], dtype=np.complex64)
     >>> assert (nparry == should_be).all()
     """
     assert 0 < chunk_size
     assert len(data.shape) == 1  # Require 1-dimensional array (`shape` has only one item, that is, one dimension)
     npdata = np.array(data, dtype=np.complex64)
@@ -54,115 +93,101 @@
     q = SimpleQueueTypeWrapped(np.ndarray, np.complex64, chunk_size)
     for item in chunked:
         q.put(item)
     assert issubclass(q.qtype, np.ndarray)
     return q
 
 
-def gnuradio_guisink_using_queue_impl(data: np.ndarray,
+def _gnuradio_guisink_using_queue_impl(data: np.ndarray,
                   center_freq: float,
                   samp_rate: float,
                   prepend_zeros: int = 0,
                   chunk_size: int = 1024):
     """Display using a GNU Radio QT GUI Sink."""
     prepended = np.concatenate([np.zeros(prepend_zeros, dtype=data.dtype), data])
     assert prepended.dtype == data.dtype
     assert (prepended[prepend_zeros:] == data).all()
-    q = pad_chunk_queue(prepended, chunk_size)
+    q = _pad_chunk_queue(prepended, chunk_size)
 
-    configure_and_run_gui_flowgraph(queue_to_guisink, [center_freq, samp_rate, q, chunk_size])
+    _configure_and_run_gui_flowgraph(queue_to_guisink, [center_freq, samp_rate, q, chunk_size])
 
 
 def gnuradio_guisink(data: np.ndarray,
                   center_freq: float,
                   samp_rate: float,
                   prepend_zeros: int = 0):
     """Display using a GNU Radio QT GUI Sink."""
     prepended = prepend_zeros_(data, prepend_zeros)
     normal_py_data = tuple(map(complex, prepended))  # GNURadio type issues. Eventually, fix this for efficiency
-    configure_and_run_gui_flowgraph(vector_to_guisink, [center_freq, samp_rate, normal_py_data])
+    _configure_and_run_gui_flowgraph(vector_to_guisink, [center_freq, samp_rate, normal_py_data])
 
 
-def gnuradio_print_using_queue_impl(data: np.ndarray, print_delay: float = 0.5, chunk_size: int = 1024):
+def _gnuradio_print_using_queue_impl(data: np.ndarray, print_delay: float = 0.5, chunk_size: int = 1024):
     """Sends data to a print block."""
-    q = pad_chunk_queue(data, chunk_size)
+    q = _pad_chunk_queue(data, chunk_size)
     tb = queue_to_print_sink(print_delay, q, chunk_size)
     configure_graceful_exit(tb)
     tb.start()
     tb.wait()
 
 
-def gnuradio_print():
-    raise NotImplementedError()
+# def gnuradio_print():
+#     raise NotImplementedError()
 
 
-def gnuradio_write_text_file():
-    raise NotImplementedError()
+# def gnuradio_write_text_file():
+#     raise NotImplementedError()
 
 
-def gnuradio_write_text_file_using_queue_impl(data: np.ndarray, filename: str, chunk_size: int = 1024):
+def _gnuradio_write_text_file_using_queue_impl(data: np.ndarray, filename: str, chunk_size: int = 1024):
     """Writes data to a file named `filename`, encoded as text.
-    NOTE: Based on issues experienced with gnuradio_write_file, this may not write the entire file."""
-    q = pad_chunk_queue(data, chunk_size)
+    NOTE: Based on issues experienced with _gnuradio_write_file, this may not write the entire file."""
+    q = _pad_chunk_queue(data, chunk_size)
     tb = queue_to_string_file_sink(filename, q, chunk_size)
     configure_graceful_exit(tb)
     tb.start()
     tb.wait()
 
 
-def gnuradio_write_file_using_queue_impl(data: np.ndarray, filename: str, chunk_size: int = 1024):
+def _gnuradio_write_file_using_queue_impl(data: np.ndarray, filename: str, chunk_size: int = 1024):
     """Writes data to a file named `filename`, encoded as np.complex64.
     NOTE: There seem to be unresolved issues in which this does not write a full file."""
-    q = pad_chunk_queue(data, chunk_size)
+    q = _pad_chunk_queue(data, chunk_size)
     tb = queue_to_file_sink(filename, q, chunk_size)
     configure_graceful_exit(tb)
     tb.start()
     tb.wait()
 
 
-def gnuradio_write_file(data: np.ndarray, filename: str):
+def _gnuradio_write_file(data: np.ndarray, filename: str):
     """Writes data to a file named `filename`, encoded as np.complex64.
     NOTE: There seem to be an unresolved issue in which this does not write a full file."""
     normal_py_data = tuple(map(complex, data))  # GNURadio type issues. Eventually, fix this for efficiency
     tb = vector_to_file_sink(normal_py_data, filename)
     configure_graceful_exit(tb)
     tb.start()
     tb.wait()
 
 
-def gnuradio_network_pub(data: np.ndarray, port: int = 8008, chunk_size: int = 1024):
+def _gnuradio_network_pub(data: np.ndarray, port: int = 8008, chunk_size: int = 1024):
     """NOT FULLY TESTED. 
     Use a TCP socket to transmit data to a host on the network (also works for localhost).
     (Note: implemented using ZeroMQ.)"""
-    q = pad_chunk_queue(data, chunk_size)
+    q = _pad_chunk_queue(data, chunk_size)
     tb = queue_to_zmqpub_sink(port, q, chunk_size)
     configure_graceful_exit(tb)
     tb.start()
     tb.wait()
 
 
-def gnuradio_send(data: np.ndarray,
-                  center_freq: float,
-                  samp_rate: float,
-                  if_gain: int = 16,
-                  device_args: str = "hackrf=0",
-                  repeat: bool = False):
-    """Sends `data` to osmocom sink."""
-    normal_py_data = tuple(map(complex, data))  # GNURadio type issues. Eventually, fix this for efficiency
-    tb = vector_to_osmocom_sink(normal_py_data, center_freq, samp_rate, if_gain, device_args, repeat)
-    configure_graceful_exit(tb)
-    tb.start()
-    tb.wait()
-
-
-def gnuradio_send_using_queue_impl(data: np.ndarray,
+def _gnuradio_send_using_queue_impl(data: np.ndarray,
                   center_freq: float,
                   samp_rate: float,
                   if_gain: int = 16,
                   device_args: str = "hackrf=0",
                   chunk_size: int = 1024):
     """Sends `data` to osmocom sink."""
-    q = pad_chunk_queue(data, chunk_size)
+    q = _pad_chunk_queue(data, chunk_size)
     tb = queue_to_osmocom_sink(center_freq, samp_rate, chunk_size, if_gain, q, device_args)
     configure_graceful_exit(tb)
     tb.start()
     tb.wait()
```

### Comparing `pcdr-0.4.8b1/src/pcdr/modulators.py` & `pcdr-1.0.0a1/src/pcdr/_modulators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import List, Iterable, TypeVar, Tuple
+
 import numpy as np
 
 
 T = TypeVar('T')
 
 
 
@@ -33,15 +34,15 @@
     This returns None:
     >>> __must_be_binary([1, 0, 1])
 
     This raises:
     >>> __must_be_binary("101")
     Traceback (most recent call last):
         ...
-    pcdr.modulators.NonBitError: ...
+    pcdr._modulators.NonBitError: ...
     """
     if not all(map(lambda x: x in [1, 0], bits)):
         raise NonBitError('`bits` must be of type List[int], and all of those integers'
                          ' must be either 0 or 1. It cannot be a string, such as "1010".')
 
 
 def ook_modulate(bits: List[int], bit_length: int, dtype=np.uint8) -> np.ndarray:
@@ -65,15 +66,15 @@
 
 
 def ook_modulate_at_frequency(bits: List[int], bit_length: int, samp_rate: float, freq: float) -> Tuple[np.ndarray, np.ndarray]:
     """
     OOK Modulate at a given frequency. Returns the timestamps and the modulated data.
 
     Examples:
-    >>> from pcdr.basictermplot import plot
+    >>> from pcdr._internal.basictermplot import plot
     >>> timestamps, data = ook_modulate_at_frequency([1, 0, 1, 1], bit_length=20, samp_rate=40, freq=2)
     >>> plot(timestamps, data.real, 80, 10)
     xmin: 0.00
     xmax: 1.98
     ymin: -1.00
     ymax: 1.00
     ~o███████████████████████████████████████o███████████████████o███████████████████
@@ -86,15 +87,15 @@
     ~████████████████████████████████████████████████████████████████████████████████
     ~███████o█████o█████████████████████████████████o█████o█████████████o█████o██████
     ~████████ooooo███████████████████████████████████ooooo███████████████ooooo███████
     """
     __must_be_binary(bits)
     ## TODO: place this import better.
     ## For now, this import must be here due to circular imports
-    from pcdr.wavegen import multiply_by_complex_wave
+    from pcdr._wavegen import multiply_by_complex_wave
 
     baseband_sig = ook_modulate(bits, bit_length)
     result = multiply_by_complex_wave(baseband_sig, samp_rate, freq)
     assert result[0].dtype == np.float64
     assert result[1].dtype == np.complex64
     assert len(result[0]) == len(result[1]) == (len(bits) * bit_length)
     return result
```

### Comparing `pcdr-0.4.8b1/src/pcdr/osmocom_queued_rx_flowgraph.py` & `pcdr-1.0.0a1/src/pcdr/_beta/osmocom_queued_rx_flowgraph.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 from gnuradio import gr, blocks
 import pmt
 import numpy as np
 import osmosdr
 from typing import List, Protocol
 
-from pcdr.our_GR_blocks import queue_sink
-from pcdr.helpers import validate_hack_rf_receive
+from pcdr._internal.our_GR_blocks import queue_sink
 
 
 
 
-## Bizarre GNU Radio variable-rename issues
-
-_osmocom_source_to_queuequeue_sink = queue_sink
-
-
 
 class osmocom_source_to_queue_sink(gr.top_block):
 
     
     def __init__(self, center_freq: float, samp_rate: float, chunk_size: int, device_args: str, if_gain: int = 32, bb_gain: int = 42):
         gr.top_block.__init__(self, "Top block")
```

### Comparing `pcdr-0.4.8b1/src/pcdr/osmocom_queued_tx_flowgraph.py` & `pcdr-1.0.0a1/src/pcdr/_beta/osmocom_queued_tx_flowgraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 import numpy as np
 from gnuradio import gr
 from gnuradio import blocks
 import osmosdr
 import time
 from queue import SimpleQueue, Empty
-from pcdr.our_GR_blocks import queue_source, string_file_sink, print_sink
-from pcdr.helpers import validate_hack_rf_transmit
+from pcdr._internal.our_GR_blocks import queue_source, string_file_sink, print_sink
+from pcdr._internal.misc import validate_hack_rf_transmit
 from gnuradio import zeromq
 
 
 
 
 ## Bizarre GNU Radio variable-rename issues
```

### Comparing `pcdr-0.4.8b1/src/pcdr/our_GR_blocks.py` & `pcdr-1.0.0a1/src/pcdr/_internal/our_GR_blocks.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import numpy as np
 from gnuradio import gr
 from gnuradio import blocks
 import osmosdr
 import time
 from queue import Empty, SimpleQueue, LifoQueue
-from pcdr.helpers import SimpleQueueTypeWrapped, QueueTypeWrapped, queue_to_list
+from pcdr._internal.misc import (
+    SimpleQueueTypeWrapped, QueueTypeWrapped,
+    queue_to_list, getSize
+)
 from typing import List, Optional
 from typeguard import typechecked
 
 
 
 class queue_source(gr.sync_block):
     ## TODO: Is this used anywhere? Let's start using Blk_queue_source instead
@@ -180,15 +183,15 @@
     def __init__(self):
         raise NotImplementedError()
 
 
 
 class Blk_strength_at_freq(gr.sync_block):
     @typechecked
-    def __init__(self, samp_rate: float, freq_of_interest: float, fft_size: int, avg_count: int = 1):
+    def __init__(self, samp_rate: float, freq_of_interest: float, fft_size: int):
         gr.sync_block.__init__(self,
             name='Python Block: Strength at frequency',
             in_sig=[(np.complex64, fft_size)],
             out_sig=[]
         )
         assert 0 <= freq_of_interest < samp_rate / 2
         maxval = samp_rate/2 - samp_rate/fft_size
@@ -207,7 +210,39 @@
         #     fft_val = float(self._fft[self._idx])
         #     self.__last_few.append(fft_val)
         # else:
         #     avg = sum(self.__last_few) / len(self.__last_few)
         #     self._deq.append(avg)
         #     self.__last_few = []
         return 1
+
+
+class Blk_SingleItemStack(gr.sync_block):
+    @typechecked
+    def __init__(self, length: int, type_: type):
+        gr.sync_block.__init__(self,
+            name='Python Block: Single Item Stack',
+            in_sig=[(type_, length)],
+            out_sig=[]
+        )
+        self._reading = SingleItemStack()
+    
+    def work(self, input_items, output_items):
+        dat = input_items[0][0]
+        self._reading.put(dat)
+        return 1
+
+
+class Blk_VecSingleItemStack(gr.hier_block2):
+    @typechecked
+    def __init__(self, type_: type, vecsize: int):
+                
+        itemsize = getSize(type_)
+        gr.hier_block2.__init__(
+            self, 
+            "VecSingleItemStack",
+            gr.io_signature(1, 1, itemsize),
+            gr.io_signature(0, 0, 0)
+        )
+        self.stv = blocks.stream_to_vector(itemsize, vecsize)
+        self.sis = Blk_SingleItemStack(vecsize, type_)
+        self.connect(self, self.stv, self.sis)
```

### Comparing `pcdr-0.4.8b1/src/pcdr/queue/sink.py` & `pcdr-1.0.0a1/src/pcdr/_queue/sink.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 # >>> filesink.wait()
 Queue is empty, block will now report 'done' to GNU Radio flowgraph
 # >>> p.unlink()
 """
 from typeguard import typechecked
 from gnuradio import gr, blocks
 from termcolor import cprint
-from pcdr.helpers import getSize
-from pcdr.our_GR_blocks import Blk_queue_source
-from pcdr.queue import ChunkSizeNonIntegerError
+from pcdr._internal.misc import getSize
+from pcdr._internal.our_GR_blocks import Blk_queue_source
+from pcdr._queue import ChunkSizeNonIntegerError
 import numpy as np
 from typing import Optional
 import osmosdr
 import time
 
 
 @typechecked
@@ -48,15 +48,15 @@
 def _compute_chunk_size(samp_rate: float, chunk_size: Optional[int]) -> int:
     """
     >>> _compute_chunk_size(350, None)
     35
     >>> _compute_chunk_size(321, None)
     Traceback (most recent call last):
       ...
-    pcdr.queue.ChunkSizeNonIntegerError: Chunk size must be specified if samp rate is not divisible by 10.
+    pcdr._queue.ChunkSizeNonIntegerError: Chunk size must be specified if samp rate is not divisible by 10.
 
     If chunk size is specified, simply return it:
     >>> _compute_chunk_size(321, 300)
     300
     """
     if chunk_size != None:
         return chunk_size
```

### Comparing `pcdr-0.4.8b1/src/pcdr/queue/source.py` & `pcdr-1.0.0a1/src/pcdr/_queue/source.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional
 from typeguard import typechecked
 from gnuradio import gr, blocks
-from pcdr.helpers import getSize
-from pcdr.our_GR_blocks import Blk_queue_sink
+from pcdr._internal.misc import getSize
+from pcdr._internal.our_GR_blocks import Blk_queue_sink
 import numpy as np
 
 
 
 class _QueuedSource:
     """
     Sets up a top block that...
```

### Comparing `pcdr-0.4.8b1/src/pcdr/queue_to_guisink_flowgraph.py` & `pcdr-1.0.0a1/src/pcdr/_internal/queue_to_guisink_flowgraph.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 from gnuradio import gr
 import sys
 import signal
 from argparse import ArgumentParser
 from gnuradio.eng_arg import eng_float, intx
 from gnuradio import eng_notation
 from gnuradio import qtgui
-from pcdr.helpers import SimpleQueueTypeWrapped
-from pcdr.our_GR_blocks import queue_source
-from pcdr.wrapped_GR_blocks import qt_gui_init_boilerplate
+from pcdr._internal.misc import SimpleQueueTypeWrapped
+from pcdr._internal.our_GR_blocks import queue_source
+from pcdr._internal.wrapped_GR_blocks import qt_gui_init_boilerplate
 
 
 
 _queue_to_guisink__queue_source = queue_source
 
 class queue_to_guisink(gr.top_block, Qt.QWidget):
```

### Comparing `pcdr-0.4.8b1/src/pcdr/queue_to_waterfall_flowgraph.py` & `pcdr-1.0.0a1/src/pcdr/_internal/queue_to_waterfall_flowgraph.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import signal
 from argparse import ArgumentParser
 from gnuradio.eng_arg import eng_float, intx
 from gnuradio import eng_notation
 from gnuradio import qtgui
 from queue import SimpleQueue
 import numpy as np
-from pcdr.our_GR_blocks import queue_source
+from pcdr._internal.our_GR_blocks import queue_source
 
 
 _queue_to_waterfall__queue_source = queue_source
 
 
 class queue_to_waterfall(gr.top_block, Qt.QWidget):
```

### Comparing `pcdr-0.4.8b1/src/pcdr/vector_to_guisink_flowgraph.py` & `pcdr-1.0.0a1/src/pcdr/_internal/vector_to_guisink_flowgraph.py`

 * *Files identical despite different names*

### Comparing `pcdr-0.4.8b1/src/pcdr/vector_tx_flowgraphs.py` & `pcdr-1.0.0a1/src/pcdr/_internal/vector_tx_flowgraphs.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,34 +8,36 @@
 # Title: Osmocom helper
 # GNU Radio version: 3.8.1.0
 
 import numpy as np
 from gnuradio import gr
 from gnuradio import blocks
 import osmosdr
-from pcdr.our_GR_blocks import print_sink, string_file_sink
+from pcdr._internal.our_GR_blocks import print_sink, string_file_sink
 from gnuradio import zeromq
-from typing import Tuple
-from pcdr.helpers import validate_hack_rf_transmit
+from typing import List
+from pcdr._internal.misc import validate_hack_rf_transmit
+from typeguard import typechecked
 
 
 ## Bizarre GNU Radio variable-rename issues
 
 # _queue_to_print_sink__queue_source = queue_source
 # _queue_to_string_file_sink__queue_source = queue_source
 # _queue_to_osmocom_sink__queue_source = queue_source
 # _queue_to_string_file_sink__string_file_sink = string_file_sink
 # _queue_to_print_sink__print_sink = print_sink
 # _queue_to_zmqpub_sink__queue_source = queue_source
 
 
 class vector_to_osmocom_sink(gr.top_block):
 
+    @typechecked
     def __init__(self,
-                 data: Tuple[complex],
+                 data: List[complex],
                  center_freq: float,
                  samp_rate: float,
                  if_gain: int,
                  device_args: str,
                  repeat: bool):
         """device_args: "hackrf=0" is common."""
 
@@ -53,32 +55,32 @@
         self.osmosdr_sink.set_if_gain(if_gain)
         self.osmosdr_sink.set_bb_gain(0)
 
         self.connect(self.vector_source, self.osmosdr_sink)
 
 
 class vector_to_print_sink(gr.top_block):
-    def __init__(self, print_delay: float, data: Tuple[complex], repeat: bool):
+    def __init__(self, print_delay: float, data: List[complex], repeat: bool):
         gr.top_block.__init__(self, "Top block")
         self.vector_source = blocks.vector_source_c(data, repeat)
         self.print_sink = print_sink(print_delay)
         self.connect(self.vector_source, self.print_sink)
 
 
 class vector_to_string_file_sink(gr.top_block):
-    def __init__(self, filename: str, data: Tuple[complex]):
+    def __init__(self, filename: str, data: List[complex]):
         assert isinstance(filename, str)
         gr.top_block.__init__(self, "Top block")
         self.vector_source = blocks.vector_source_c(data)
         self.string_file_sink = string_file_sink(filename)
         self.connect(self.vector_source, self.string_file_sink)
 
 
 class vector_to_file_sink(gr.top_block):
-    def __init__(self, data: Tuple[complex], filename: str):
+    def __init__(self, data: List[complex], filename: str):
         assert isinstance(filename, str)
         gr.top_block.__init__(self, "Top block")
         self.vector_source = blocks.vector_source_c(data)
         self.file_sink = blocks.file_sink(gr.sizeof_gr_complex, filename, append=False)
         self.file_sink.set_unbuffered(False)
         self.connect(self.vector_source, self.file_sink)
```

### Comparing `pcdr-0.4.8b1/src/pcdr/wavegen.py` & `pcdr-1.0.0a1/src/pcdr/_wavegen.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-import numpy as np
 import random
 from typing import Optional, List, Tuple, Literal
-from pcdr.fileio import writeRealCSV, writeComplexCSV
-from pcdr.modulators import ook_modulate
-from pcdr.helpers import str_to_bin_list
+
+import numpy as np
 from typeguard import typechecked
 
+from pcdr._internal.fileio import writeRealCSV, writeComplexCSV
+from pcdr._modulators import ook_modulate
+from pcdr._helpers import str_to_bin_list
 
 
-def createTimestamps(seconds: float, num_samples: int, dtype=np.float64) -> np.ndarray:
+
+def make_timestamps_seconds(seconds: float, num_samples: int, dtype=np.float64) -> np.ndarray:
     """Creates timestamps from zero up to the given maximum number of seconds.
     Implemented using np.linspace().
     
     Note: We use np.float64 as the default dtype because np.float32 was causing float rounding issues
     that became worse with larger time values (as float rounding issues usually do).
     
     Example:
-    >>> createTimestamps(2, 10)
+    >>> make_timestamps_seconds(2, 10)
     array([0. , 0.2, 0.4, 0.6, 0.8, 1. , 1.2, 1.4, 1.6, 1.8])
     """
     assert 0 <= seconds
     assert 0 <= num_samples
     result = np.linspace(
         start=0,
         stop=seconds,
@@ -30,23 +32,23 @@
     )
     assert result.dtype == dtype
     assert len(result) == num_samples
     assert (0 <= result).all()
     return result
 
 
-def createTimestamps_samprate(samp_rate: float, num_samples: int, dtype=np.float64) -> np.ndarray:
+def make_timestamps_samprate(samp_rate: float, num_samples: int, dtype=np.float64) -> np.ndarray:
     """Creates `num_samples` timestamps spaced by `1/samp_rate`.
     Implemented using np.linspace().
     
     Examples:
-    >>> createTimestamps_samprate(5, 10)
+    >>> make_timestamps_samprate(5, 10)
     array([0. , 0.2, 0.4, 0.6, 0.8, 1. , 1.2, 1.4, 1.6, 1.8])
 
-    >>> createTimestamps_samprate(10, 4)
+    >>> make_timestamps_samprate(10, 4)
     array([0. , 0.1, 0.2, 0.3])
 
     Note: We use np.float64 as the default dtype because np.float32 was causing float rounding issues
     that became worse with larger time values (as float rounding issues usually do)."""
     assert 0 < samp_rate
     assert 0 <= num_samples
     
@@ -61,14 +63,17 @@
     assert result.dtype == dtype
     assert len(result) == num_samples
     assert (0 <= result).all()
 
     return result
 
 
+def make_timestamps():
+    raise NotImplementedError("Intended purpose: run either make_timestamps_seconds or make_timestamps_samprate based on provided arguments")
+
 #### This is something we may do eventually.
 # @overload
 # def makeRealWave(samp_rate: float,
 #                  freq: float,
 #                  num_samples: int,
 #                  allowAliasing: bool = False) -> Tuple[np.ndarray, np.ndarray]: ...
 # @overload
@@ -82,16 +87,16 @@
 #     return something
 
 
 def makeRealWave_basic(timestamps: np.ndarray, freq: float) -> np.ndarray:
     """Return a sine wave.
     
     Example:
-    >>> from pcdr.basictermplot import plot
-    >>> timestamps = createTimestamps(1, 50)
+    >>> from pcdr._internal.basictermplot import plot
+    >>> timestamps = make_timestamps_seconds(1, 50)
     >>> wave = makeRealWave_basic(timestamps, 2)
     >>> plot(timestamps, wave)
     xmin: 0.00
     xmax: 0.98
     ymin: -1.00
     ymax: 1.00
     ~██████o████████████████████████o██████████████████
@@ -110,16 +115,16 @@
 
 def makeComplexWave_basic(timestamps: np.ndarray, freq: float) -> np.ndarray:
     """Return a complex wave.
     
     The real part is cosine (starts at 1); the imaginary part is sine (starts at 0).
     
     Example:
-    >>> from pcdr.basictermplot import plot
-    >>> timestamps = createTimestamps(1, 50)
+    >>> from pcdr._internal.basictermplot import plot
+    >>> timestamps = make_timestamps_seconds(1, 50)
     >>> wave = makeComplexWave_basic(timestamps, 2)
     >>> plot(timestamps, wave.real)
     xmin: 0.00
     xmax: 0.98
     ymin: -0.99
     ymax: 1.00
     ~o████████████████████████o████████████████████████
@@ -155,52 +160,52 @@
 
 
 class AliasError(ValueError):
     pass
 
 
 
-def isAliasingWhenDisallowed(allowAliasing: bool, freq: float, samp_rate: float) -> bool:
+def _isAliasingWhenDisallowed(allowAliasing: bool, freq: float, samp_rate: float) -> bool:
     """
     Examples:
 
     >>> allowAliasing = False
     >>> samp_rate = 5
     >>> too_high_freq = 4
     >>> acceptable_freq = 2
-    >>> isAliasingWhenDisallowed(allowAliasing, too_high_freq, samp_rate)
+    >>> _isAliasingWhenDisallowed(allowAliasing, too_high_freq, samp_rate)
     True
-    >>> isAliasingWhenDisallowed(allowAliasing, acceptable_freq, samp_rate)
+    >>> _isAliasingWhenDisallowed(allowAliasing, acceptable_freq, samp_rate)
     False
     >>> allowAliasing = True
-    >>> isAliasingWhenDisallowed(allowAliasing, too_high_freq, samp_rate)
+    >>> _isAliasingWhenDisallowed(allowAliasing, too_high_freq, samp_rate)
     False
-    >>> isAliasingWhenDisallowed(allowAliasing, acceptable_freq, samp_rate)
+    >>> _isAliasingWhenDisallowed(allowAliasing, acceptable_freq, samp_rate)
     False
     """
     return (not allowAliasing) and (abs(freq) > samp_rate/2)
 
 
-def aliasingError(allowAliasing: bool, freq: float, samp_rate: float) -> None:
+def _aliasingError(allowAliasing: bool, freq: float, samp_rate: float) -> None:
     """Gives a detailed Aliasing error message if it's aliasing when it shouldn't.
     :raises AliasError:"""
-    if isAliasingWhenDisallowed(allowAliasing, freq, samp_rate):
+    if _isAliasingWhenDisallowed(allowAliasing, freq, samp_rate):
         raise AliasError(f"For a sample rate of {samp_rate}, the highest frequency that can be faithfully represented is {samp_rate/2}. The specified freq, {freq}, is greater than the limit specified by Shannon/Nyquist/Kotelnikov/Whittaker (commonly called the Nyquist frequency).")
 
 
 def makeComplexWave_numsamps(num_samples: int, samp_rate: float, freq: float, allowAliasing: bool = False) -> Tuple[np.ndarray, np.ndarray]:
     """
     Returns a tuple (timestamps, wave).
     
     The real part of the wave is cosine (starts at 1); the imaginary part is sine (starts at 0).
 
-    :raises AliasError: if isAliasingWhenDisallowed
+    :raises AliasError: if _isAliasingWhenDisallowed
     
     Example:
-    >>> from pcdr.basictermplot import plot
+    >>> from pcdr._internal.basictermplot import plot
     >>> timestamps, wave = makeComplexWave_numsamps(50, 50, 2)
     >>> plot(timestamps, wave.real)
     xmin: 0.00
     xmax: 0.98
     ymin: -0.99
     ymax: 1.00
     ~o████████████████████████o████████████████████████
@@ -223,30 +228,30 @@
     ~o███████████oo███████████o███████████oo███████████
     ~██████████████o█████████o██████████████o█████████o
     ~███████████████o██████oo████████████████o██████oo█
     ~████████████████oooooo███████████████████oooooo███
     """
     assert 0 < samp_rate
     assert 0 <= num_samples
-    aliasingError(allowAliasing, freq, samp_rate)
+    _aliasingError(allowAliasing, freq, samp_rate)
     t = num_samples / samp_rate
-    timestamps = createTimestamps(seconds=t, num_samples=num_samples)
+    timestamps = make_timestamps_seconds(seconds=t, num_samples=num_samples)
     wave = makeComplexWave_basic(timestamps, freq)
     assert len(timestamps) == len(wave) == num_samples
     return timestamps, wave
 
 
 def makeRealWave_numsamps(num_samples: int, samp_rate: float, freq: float, allowAliasing: bool = False) -> Tuple[np.ndarray, np.ndarray]:
     """
     Return a Real wave.
 
-    :raises AliasError: if isAliasingWhenDisallowed
+    :raises AliasError: if _isAliasingWhenDisallowed
     
     Example:
-    >>> from pcdr.basictermplot import plot
+    >>> from pcdr._internal.basictermplot import plot
     >>> timestamps, wave = makeRealWave_numsamps(50, 50, 2)
     >>> plot(timestamps, wave)
     xmin: 0.00
     xmax: 0.98
     ymin: -1.00
     ymax: 1.00
     ~██████o████████████████████████o██████████████████
@@ -256,32 +261,32 @@
     ~o███████████oo███████████o███████████oo███████████
     ~██████████████o█████████o██████████████o█████████o
     ~███████████████o██████oo████████████████o██████oo█
     ~████████████████oooooo███████████████████oooooo███
     """
     assert 0 < samp_rate
     assert 0 <= num_samples
-    aliasingError(allowAliasing, freq, samp_rate)
+    _aliasingError(allowAliasing, freq, samp_rate)
     t = num_samples / samp_rate
-    timestamps = createTimestamps(seconds=t, num_samples=num_samples)
+    timestamps = make_timestamps_seconds(seconds=t, num_samples=num_samples)
     wave = makeRealWave_basic(timestamps, freq)
     assert len(timestamps) == len(wave) == num_samples
     return timestamps, wave
 
 
 def makeComplexWave_time(seconds: float, samp_rate: float, freq: float, allowAliasing: bool = False) -> Tuple[np.ndarray, np.ndarray]:
     """
     Returns a tuple (timestamps, wave).
     
     The real part of the wave is cosine (starts at 1); the imaginary part is sine (starts at 0).
 
-    :raises AliasError: if isAliasingWhenDisallowed
+    :raises AliasError: if _isAliasingWhenDisallowed
     
     Example:
-    >>> from pcdr.basictermplot import plot
+    >>> from pcdr._internal.basictermplot import plot
     >>> timestamps, wave = makeComplexWave_time(1, 50, 2)
     >>> plot(timestamps, wave.real)
     xmin: 0.00
     xmax: 0.98
     ymin: -0.99
     ymax: 1.00
     ~o████████████████████████o████████████████████████
@@ -303,30 +308,30 @@
     ~█o█████████o██████████████o█████████o█████████████
     ~o███████████oo███████████o███████████oo███████████
     ~██████████████o█████████o██████████████o█████████o
     ~███████████████o██████oo████████████████o██████oo█
     ~████████████████oooooo███████████████████oooooo███
     """
     assert 0 < samp_rate
-    aliasingError(allowAliasing, freq, samp_rate)
+    _aliasingError(allowAliasing, freq, samp_rate)
     num_samples = int(samp_rate * seconds)
-    timestamps = createTimestamps(seconds, num_samples)
+    timestamps = make_timestamps_seconds(seconds, num_samples)
     wave = makeComplexWave_basic(timestamps, freq)
     assert len(timestamps) == len(wave) == num_samples
     return timestamps, wave
 
 
 def makeRealWave_time(seconds: float, samp_rate: float, freq: float, allowAliasing: bool = False) -> Tuple[np.ndarray, np.ndarray]:
     """
     Return a Real wave.
 
-    :raises AliasError: if isAliasingWhenDisallowed
+    :raises AliasError: if _isAliasingWhenDisallowed
     
     Example:
-    >>> from pcdr.basictermplot import plot
+    >>> from pcdr._internal.basictermplot import plot
     >>> timestamps, wave = makeRealWave_time(1, 50, 2)
     >>> plot(timestamps, wave.real)
     xmin: 0.00
     xmax: 0.98
     ymin: -1.00
     ymax: 1.00
     ~██████o████████████████████████o██████████████████
@@ -335,37 +340,37 @@
     ~█o█████████o██████████████o█████████o█████████████
     ~o███████████oo███████████o███████████oo███████████
     ~██████████████o█████████o██████████████o█████████o
     ~███████████████o██████oo████████████████o██████oo█
     ~████████████████oooooo███████████████████oooooo███
     """
     assert 0 < samp_rate
-    aliasingError(allowAliasing, freq, samp_rate)
+    _aliasingError(allowAliasing, freq, samp_rate)
     num_samples = int(samp_rate * seconds)
-    timestamps = createTimestamps(seconds, num_samples)
+    timestamps = make_timestamps_seconds(seconds, num_samples)
     wave = makeRealWave_basic(timestamps, freq)
     assert len(timestamps) == len(wave) == num_samples
     return timestamps, wave
 
 
 @typechecked
-def makeWave(samp_rate: float,
+def make_wave(samp_rate: float,
              freq: float,
              type_: Literal["real", "complex"],
              *, seconds: Optional[float] = None,
              num: Optional[float] = None,
              allowAliasing: bool = False) -> Tuple[np.ndarray, np.ndarray]:
     """
     TODO:
      - finish writing tests
      - Write implementation that makes these tests pass
      - Change lessons to use makeWave
      - Add @typechecked to all funcs in this file
     
-    >>> from pcdr.basictermplot import plot
+    >>> from pcdr._internal.basictermplot import plot
     >>> timestamps, wave = makeWave(50, 3, "real", seconds=1)
     >>> plot(timestamps, wave)
     xmin: 0.00
     xmax: 0.98
     ymin: -1.00
     ymax: 1.00
     ~████o████████████████o████████████████████████████
@@ -480,17 +485,21 @@
             return makeRealWave_numsamps(num, samp_rate, freq, allowAliasing)
         elif type_ == "complex":
             return makeComplexWave_numsamps(num, samp_rate, freq, allowAliasing)
         else:
             raise ValueError("This will never happen if the @typechecked works")
     else:
         raise Exception("Impossible case")
-    
 
-def waveAndWrite(basename: str, timestamps: np.ndarray, freq, complex_or_real: Literal["c", "r"]):
+
+makeWave = make_wave
+
+
+
+def wave_and_write(basename: str, timestamps: np.ndarray, freq, complex_or_real: Literal["c", "r"]):
     if complex_or_real == "r":
         data = makeRealWave_basic(timestamps, freq)
         writeRealCSV(basename + ".csv", data)
         data.tofile(basename + ".float32")
     elif complex_or_real == "c":
         data = makeComplexWave_basic(timestamps, freq)
         writeComplexCSV(basename + ".csv", data)
@@ -516,21 +525,21 @@
 
     freq = float(input("What frequency wave would you like to generate (Hz)? "))
     complex_or_real = input("Complex or Real wave? Enter c or r. ")
     filename = input("Filename? (Press enter to choose the default name, 'generated_data'.) ")
     if filename.strip() == "":
         filename = "generated_data"
 
-    timestamps = createTimestamps(max_time, num_samples)
+    timestamps = make_timestamps_seconds(max_time, num_samples)
     print("------------------")
     print(f"Going to generate {int(num_samples)} samples.")
     print("Simulated samples were taken at these times (units are seconds):")
     print(timestamps)
 
-    waveAndWrite(filename, timestamps, freq, complex_or_real)
+    wave_and_write(filename, timestamps, freq, complex_or_real)
     print("Done writing files.")
 
 
 def wave_file_gen(samp_rate: float, max_time: float, freq: float, complex_or_real: str, filename: str = 'generated_data'):
     """Units:
     samp_rate: samples per sec
     max_time: seconds
@@ -539,25 +548,25 @@
     """
     
     num_samples = samp_rate * max_time
 
     if int(num_samples) != num_samples:
         raise ValueError(f"The number of samples would be {num_samples}, but a partial sample is meaningless.\nPlease pick a sample rate and an amount of time whose product is an integer.")
 
-    timestamps = createTimestamps(max_time, num_samples)
+    timestamps = make_timestamps_seconds(max_time, num_samples)
 
-    waveAndWrite(filename, timestamps, freq, complex_or_real)
+    wave_and_write(filename, timestamps, freq, complex_or_real)
 
 
 def multiply_by_complex_wave(baseband_sig: np.ndarray, samp_rate: float, freq: float, allowAliasing: bool = False) -> Tuple[np.ndarray, np.ndarray]:
     """
     Returns a tuple (timestamps, mult).
 
-    >>> from pcdr.basictermplot import plot
-    >>> from pcdr.wavegen import multiply_by_complex_wave, ook_modulate
+    >>> from pcdr._internal.basictermplot import plot
+    >>> from pcdr import multiply_by_complex_wave, ook_modulate
     >>> baseband_sig = ook_modulate([1, 0], 32)
     >>> timestamps, mult = multiply_by_complex_wave(baseband_sig, 64, 2)
     >>> plot(timestamps, mult.real)
     xmin: 0.00
     xmax: 0.98
     ymin: -1.00
     ymax: 1.00
@@ -578,16 +587,16 @@
     return timestamps, mult
 
 
 def multiply_by_real_wave(baseband_sig: np.ndarray, samp_rate: float, freq: float, allowAliasing: bool = False) -> Tuple[np.ndarray, np.ndarray]:
     """
     Returns a tuple (timestamps, mult).
 
-    >>> from pcdr.basictermplot import plot
-    >>> from pcdr.wavegen import multiply_by_real_wave, ook_modulate
+    >>> from pcdr._internal.basictermplot import plot
+    >>> from pcdr import multiply_by_real_wave, ook_modulate
     >>> baseband_sig = ook_modulate([1, 0], 32)
     >>> timestamps, wave = multiply_by_real_wave(baseband_sig, 64, 2)
     >>> plot(timestamps, wave)
     xmin: 0.00
     xmax: 0.98
     ymin: -1.00
     ymax: 1.00
@@ -653,15 +662,15 @@
     elif data.dtype == np.complex64:
         randnoisereal = np.complex64(random_normal(len(data), dtype=np.float32, seed=seed))
         randnoiseimag = np.complex64(random_normal(len(data), dtype=np.float32, seed=seed))
         randnoise = randnoisereal + (1j * randnoiseimag)
     else:
         raise NotImplementedError("Currently, this only works for these dtypes: float32, complex64.")
     assert randnoise.dtype == data.dtype
-    result = data + randnoise
+    result = data + amplitude * randnoise
     assert result.dtype == data.dtype
     return result
 
 
 def generate_ook_modulated_example_data(noise: bool = False, message_delay: bool = False, text_source: Optional[str] = None) -> np.ndarray:
     """
     Generate a file with the given `output_filename`.
@@ -683,15 +692,16 @@
         message = random.choice(sentences) + "."
         
         
     samp_rate = random.randrange(100, 700, 100)
     bit_length = random.randrange(50, 3000, 10)
     freq = random.randrange(10, samp_rate // 5)
     
-    bits = str_to_bin_list(message)
+    with_preamb = "«" + message
+    bits = str_to_bin_list(with_preamb)
     baseband_sig = ook_modulate(bits, bit_length)
     timestamps, fully_modded = multiply_by_complex_wave(baseband_sig, samp_rate, freq)
     if message_delay:
         fully_modded = np.concatenate([
             np.zeros(random.randint(100, 1500), dtype=np.complex64),
             fully_modded
         ])
@@ -722,55 +732,93 @@
 
 def make_fft_positive_freqs_only(sig: np.ndarray, samp_rate: float) -> Tuple[np.ndarray, np.ndarray]:
     """
     Computes an fft, returns only the positive frequencies.
     Return value is a tuple: (sample_freqs, fft_mag).
     `sample_freqs` ranges from 0 to approximately samp_rate/2
 
-    >>> from pcdr.basictermplot import plot
-    >>> from pcdr.wavegen import makeWave, make_fft_positive_freqs_only
+    >>> from pcdr._internal.basictermplot import plot
+    >>> from pcdr import make_wave, make_fft_positive_freqs_only
     >>> samp_rate = 50
-    >>> timestamps, wave = makeWave(samp_rate, 5, "complex", seconds=2)
+    >>> timestamps, wave = make_wave(samp_rate, 5, "complex", seconds=2)
     >>> sample_freqs, fft_mag = make_fft_positive_freqs_only(wave, samp_rate)
     >>> plot(sample_freqs, fft_mag, youtputsize=4)
     xmin: 0.00
     xmax: 24.50
     ymin: 0.00
-    ymax: 53.54
+    ymax: ...
     ~██████████o███████████████████████████████████████
     ~██████████████████████████████████████████████████
     ~█████████o█o██████████████████████████████████████
     ~ooooooooo███oooooooooooooooooooooooooooooooooooooo
+
+    >>> timestamps, wave = makeWave(samp_rate, 5, "complex", seconds=0.2)
+    >>> sample_freqs, fft_mag = make_fft_positive_freqs_only(wave, samp_rate)
+    >>> plot(sample_freqs, fft_mag, youtputsize=4)
+    xmin: 0.00
+    xmax: 20.00
+    ymin: 0.06
+    ymax: ...
+    ~█o███
+    ~█████
+    ~o█o██
+    ~███oo
     """
     sample_freqs, fft_mag = make_fft(sig, samp_rate)
     halfway = len(sample_freqs) // 2
     return sample_freqs[halfway:], fft_mag[halfway:]
 
 
 def make_fft(sig: np.ndarray, samp_rate: float) -> Tuple[np.ndarray, np.ndarray]:
     """
     Returns a tuple of (sample_freqs, fft_mag).
     `sample_freqs` ranges from approximately `-samp_rate/2` to approximately `samp_rate/2`.
 
-    >>> from pcdr.basictermplot import plot
-    >>> from pcdr.wavegen import makeComplexWave_time, make_fft
-    >>> timestamps, wave = makeComplexWave_time(1, 50, 10)
-    >>> sample_freqs, fft_mag = make_fft(wave, 50)
-    >>> plot(sample_freqs, fft_mag)
+    >>> from pcdr._internal.basictermplot import plot
+    >>> from pcdr import make_wave, make_fft
+    >>> seconds = 0.2
+    >>> samp_rate = 50
+    >>> freq = 5
+    >>> timestamps, wave = make_wave(samp_rate, freq, "complex", seconds=seconds)
+    >>> sample_freqs, fft_mag = make_fft(wave, samp_rate)
+    >>> sample_freqs
+    array([-25., -20., -15., -10.,  -5.,   0.,   5.,  10.,  15.,  20.])
+
+    >>> plot(sample_freqs, fft_mag, youtputsize=2)
     xmin: -25.00
-    xmax: 24.00
+    xmax: 20.00
     ymin: 0.00
-    ymax: 26.54
-    ~███████████████████████████████████o██████████████
-    ~██████████████████████████████████████████████████
-    ~██████████████████████████████████████████████████
-    ~██████████████████████████████████████████████████
-    ~██████████████████████████████████o█o█████████████
-    ~██████████████████████████████████████████████████
-    ~██████████████████████████████████████████████████
-    ~oooooooooooooooooooooooooooooooooo███ooooooooooooo
+    ymax: ...
+    ~██████o███
+    ~oooooo█ooo
+
+    >>> seconds = 0.8
+    >>> samp_rate = 10
+    >>> freq = 2
+    >>> timestamps, wave = makeComplexWave_time(seconds, samp_rate, freq)
+    >>> sample_freqs, fft_mag = make_fft(wave, samp_rate)
+    >>> sample_freqs
+    array([-5.  , -3.75, -2.5 , -1.25,  0.  ,  1.25,  2.5 ,  3.75])
+
+    >>> plot(sample_freqs, fft_mag, youtputsize=2)
+    xmin: -5.00
+    xmax: 3.75
+    ymin: 0.01
+    ymax: ...
+    ~██████o█
+    ~oooooo█o
+
+    Notice that the lowest sample frequency is not necessarily `samp_rate / 2`:
+    >>> seconds = 0.9
+    >>> samp_rate = 10
+    >>> freq = 2
+    >>> timestamps, wave = makeComplexWave_time(seconds, samp_rate, freq)
+    >>> sample_freqs, fft_mag = make_fft(wave, samp_rate)
+    >>> sample_freqs
+    array([-4.44444444, -3.33333333, -2.22222222, -1.11111111,  0.        ,
+            1.11111111,  2.22222222,  3.33333333,  4.44444444])
     """
     windowed = sig * np.hamming(len(sig))
     fft_result = np.fft.fftshift(np.fft.fft(windowed))
     sample_freqs = np.fft.fftshift(np.fft.fftfreq(len(windowed), 1/samp_rate))
     fft_mag = abs(fft_result)
     return sample_freqs, fft_mag
```

### Comparing `pcdr-0.4.8b1/src/pcdr/wrapped_GR_blocks.py` & `pcdr-1.0.0a1/src/pcdr/_internal/wrapped_GR_blocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 - Hier blocks with a similar purpose
 """
 
 from distutils.version import StrictVersion
 
 from gnuradio import gr
 from PyQt5 import Qt
-from pcdr.types_and_contracts import top_block_and_widget
+from pcdr._internal.types_and_contracts import top_block_and_widget
 from gnuradio import qtgui
 
 
 
 def qt_gui_init_boilerplate(tb: top_block_and_widget, classname: str):
     Qt.QWidget.__init__(tb)
     tb.setWindowTitle("Not titled yet")
```

### Comparing `pcdr-0.4.8b1/src/pcdr.egg-info/SOURCES.txt` & `pcdr-1.0.0a1/src/pcdr.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 LICENSE
 README.md
 pyproject.toml
-src/pcdr/__abandoned.py
 src/pcdr/__init__.py
-src/pcdr/basictermplot.py
-src/pcdr/fileio.py
-src/pcdr/function.py
-src/pcdr/gnuradio_misc.py
-src/pcdr/gnuradio_receiver.py
-src/pcdr/gnuradio_sender.py
-src/pcdr/gui.py
-src/pcdr/helpers.py
-src/pcdr/modulators.py
-src/pcdr/osmocom_queued_rx_flowgraph.py
-src/pcdr/osmocom_queued_tx_flowgraph.py
-src/pcdr/our_GR_blocks.py
-src/pcdr/queue_to_guisink_flowgraph.py
-src/pcdr/queue_to_waterfall_flowgraph.py
-src/pcdr/simple.py
-src/pcdr/types_and_contracts.py
-src/pcdr/vector_to_guisink_flowgraph.py
-src/pcdr/vector_tx_flowgraphs.py
-src/pcdr/wavegen.py
-src/pcdr/wrapped_GR_blocks.py
+src/pcdr/_flow_impl.py
+src/pcdr/_helpers.py
+src/pcdr/_modulators.py
+src/pcdr/_wavegen.py
+src/pcdr/flow.py
 src/pcdr.egg-info/PKG-INFO
 src/pcdr.egg-info/SOURCES.txt
 src/pcdr.egg-info/dependency_links.txt
 src/pcdr.egg-info/requires.txt
 src/pcdr.egg-info/top_level.txt
-src/pcdr/eventual_ideas/samples.py
-src/pcdr/queue/__init__.py
-src/pcdr/queue/sink.py
-src/pcdr/queue/source.py
+src/pcdr/_beta/gnuradio_receiver.py
+src/pcdr/_beta/gnuradio_sendlike.py
+src/pcdr/_beta/osmocom_queued_rx_flowgraph.py
+src/pcdr/_beta/osmocom_queued_tx_flowgraph.py
+src/pcdr/_internal/basictermplot.py
+src/pcdr/_internal/fileio.py
+src/pcdr/_internal/misc.py
+src/pcdr/_internal/our_GR_blocks.py
+src/pcdr/_internal/queue_to_guisink_flowgraph.py
+src/pcdr/_internal/queue_to_waterfall_flowgraph.py
+src/pcdr/_internal/types_and_contracts.py
+src/pcdr/_internal/vector_to_guisink_flowgraph.py
+src/pcdr/_internal/vector_tx_flowgraphs.py
+src/pcdr/_internal/wrapped_GR_blocks.py
+src/pcdr/_queue/__init__.py
+src/pcdr/_queue/sink.py
+src/pcdr/_queue/source.py
+tests/test_gnuradio_vector_tx_flowgraphs.py
+tests/test_gnuradio_write_file_and_read_file.py
+tests/test_helpers.py
+tests/test_multiple.py
+tests/test_other__blocks_for_testing.py
+tests/test_our_GR_blocks.py
+tests/test_simple.py
```

