# Comparing `tmp/xztrainer-0.9.7.tar.gz` & `tmp/xztrainer-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xztrainer-0.9.7.tar", max compression
+gzip compressed data, was "xztrainer-1.0.0.tar", max compression
```

## Comparing `xztrainer-0.9.7.tar` & `xztrainer-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,11 @@
--rw-r--r--   0        0        0      894 2023-05-13 21:40:29.683483 xztrainer-0.9.7/pyproject.toml
--rw-r--r--   0        0        0       46 1970-01-01 00:00:00.000000 xztrainer-0.9.7/src/xztrainer/__init__.py
--rw-r--r--   0        0        0      256 2023-03-14 15:54:26.631822 xztrainer-0.9.7/src/xztrainer/functional.py
--rw-r--r--   0        0        0     1414 1970-01-01 00:00:00.000000 xztrainer-0.9.7/src/xztrainer/logger/__init__.py
--rw-r--r--   0        0        0     1590 1970-01-01 00:00:00.000000 xztrainer-0.9.7/src/xztrainer/logger/compose.py
--rw-r--r--   0        0        0      384 1970-01-01 00:00:00.000000 xztrainer-0.9.7/src/xztrainer/logger/null.py
--rw-r--r--   0        0        0     1094 1970-01-01 00:00:00.000000 xztrainer-0.9.7/src/xztrainer/logger/stream.py
--rw-r--r--   0        0        0     1259 1970-01-01 00:00:00.000000 xztrainer-0.9.7/src/xztrainer/logger/tensorboard.py
--rw-r--r--   0        0        0     1652 2023-05-07 23:51:35.263746 xztrainer-0.9.7/src/xztrainer/model.py
--rw-r--r--   0        0        0      743 2023-03-10 15:49:26.715934 xztrainer-0.9.7/src/xztrainer/rng.py
--rw-r--r--   0        0        0     1060 1970-01-01 00:00:00.000000 xztrainer-0.9.7/src/xztrainer/sampler.py
--rw-r--r--   0        0        0      409 2023-03-10 15:49:26.707934 xztrainer-0.9.7/src/xztrainer/setup_helper.py
--rw-r--r--   0        0        0    24446 2023-05-13 21:39:53.718697 xztrainer-0.9.7/src/xztrainer/xztrainer.py
--rw-r--r--   0        0        0      830 1970-01-01 00:00:00.000000 xztrainer-0.9.7/PKG-INFO
+-rw-r--r--   0        0        0      717 2024-04-16 19:16:14.863721 xztrainer-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      120 2024-04-16 19:30:48.767471 xztrainer-1.0.0/src/xztrainer/__init__.py
+-rw-r--r--   0        0        0     2179 2024-04-16 19:36:30.205719 xztrainer-1.0.0/src/xztrainer/context.py
+-rw-r--r--   0        0        0      256 2023-03-14 15:54:26.631822 xztrainer-1.0.0/src/xztrainer/functional.py
+-rw-r--r--   0        0        0     1097 2024-04-15 19:29:59.339126 xztrainer-1.0.0/src/xztrainer/logger.py
+-rw-r--r--   0        0        0     1574 2024-04-16 19:23:13.155752 xztrainer-1.0.0/src/xztrainer/model.py
+-rw-r--r--   0        0        0      248 2024-04-16 19:36:30.233718 xztrainer-1.0.0/src/xztrainer/setup_helper.py
+-rw-r--r--   0        0        0     1391 2024-04-15 21:51:39.289037 xztrainer-1.0.0/src/xztrainer/tensor_helper.py
+-rw-r--r--   0        0        0     1343 2024-04-15 21:13:46.348654 xztrainer-1.0.0/src/xztrainer/trainable.py
+-rw-r--r--   0        0        0    16312 2024-04-16 19:36:30.224718 xztrainer-1.0.0/src/xztrainer/trainer.py
+-rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 xztrainer-1.0.0/PKG-INFO
```

### Comparing `xztrainer-0.9.7/pyproject.toml` & `xztrainer-1.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 [tool.poetry]
 name = "xztrainer"
-version = "0.9.7"
+version = "1.0.0"
 description = "A customizable training pipeline for PyTorch"
 authors = ["Maxim Afanasyev <mr.applexz@gmail.com>"]
 license = "MPL-2.0"
 
 [tool.poetry.dependencies]
-python = ">=3.8"
+python = ">=3.9"
 tqdm = ">=4.62.3"
-tensorboard = {version = ">=2.8.0", optional = true}
-torch = {version = ">=1.10.0", optional = true}
-packaging = ">=23.0"
-setuptools = ">=67.6.0"
 numpy = {version = ">=1.24.2", optional = true}
+torch = {version = ">=1.10.0", optional = true}
+accelerate = {version = ">=0.29.2", optional = true}
+torchmetrics = {version = ">=1.3.0", optional = true}
 
-[tool.poetry.dev-dependencies]
-poethepoet = "*"
-light-the-torch = "*"
-pytest = ">=6.2.5"
-scikit-learn = ">=1.0.2"
-line-profiler-pycharm = ">=1.1.0"
+[tool.poetry.group.dev.dependencies]
+scikit-learn = "^1.4.2"
+tensorboard = "^2.16.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.extras]
-tensorboard = ["tensorboard"]
-torch = ["torch"]
+torch = ["torch", "accelerate", "torchmetrics"]
 numpy = ["numpy"]
-
-[tool.poe.tasks]
-install-torch = "python3 -m light_the_torch install --upgrade torch torchaudio torchvision torchmetrics"
```

### Comparing `xztrainer-0.9.7/src/xztrainer/logger/__init__.py` & `xztrainer-1.0.0/src/xztrainer/logger.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,34 @@
-from abc import ABCMeta, abstractmethod
-from contextlib import AbstractContextManager
-from types import TracebackType
-from typing import Union, Iterable, Optional, Type
+from abc import abstractmethod
+from typing import Union, Iterable
+
+from accelerate import Accelerator
 
 ClassifierType = Union[str, Iterable[str]]
 
 
 def convert_classifier(classifier: ClassifierType) -> Iterable[str]:
     if isinstance(classifier, str):
         return classifier,
     elif isinstance(classifier, Iterable):
         return tuple(classifier)
     else:
         raise ValueError(f'Invalid classifier type: {type(classifier)}')
 
 
-class LoggingEngine(AbstractContextManager, metaclass=ABCMeta):
-    def __init__(self):
+class AccelerateLogger:
+    def __init__(self, accelerator: Accelerator):
         self._time_step = 0
         self._top_classifier = ()
+        self._accelerator = accelerator
 
     @abstractmethod
     def log_scalar(self, classifier: ClassifierType, value: float):
-        ...
-
-    @abstractmethod
-    def flush(self):
-        ...
+        classifier = '/'.join(self._top_classifier + convert_classifier(classifier))
+        step = self._time_step
+        self._accelerator.log({classifier: value}, step=step)
 
     def update_time_step(self, time_step: int):
         self._time_step = time_step
 
     def update_top_classifier(self, classifier: ClassifierType):
         self._top_classifier = convert_classifier(classifier)
-
-    def __enter__(self) -> 'LoggingEngine':
-        return self
-
-    def __exit__(self, __exc_type: Optional[Type[BaseException]], __exc_value: Optional[BaseException],
-                 __traceback: Optional[TracebackType]):
-        pass
-
-
-class LoggingEngineConfig(metaclass=ABCMeta):
-    @abstractmethod
-    def create_engine(self, experiment_name: str) -> LoggingEngine:
-        pass
```

### Comparing `xztrainer-0.9.7/src/xztrainer/model.py` & `xztrainer-1.0.0/src/xztrainer/model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,60 @@
+import logging
 import multiprocessing
 from dataclasses import dataclass, field
 from enum import Enum
-from typing import Protocol, Callable, List, Optional, Any, Union, Tuple
+import typing as t
 
-from torch import nn, dtype
+from torch import nn, Tensor
 from torch.optim import Optimizer
-from torch.utils.data.dataloader import default_collate
+from torch.utils.data import default_collate
 
-from xztrainer.logger import LoggingEngineConfig
-from xztrainer.logger.stream import StreamLoggingEngineConfig
 
-
-class SchedulerType(Enum):
-    STEP = 'step'
-    EPOCH = 'epoch'
+ModelOutputType = t.Union[Tensor, list, tuple]
+ModelOutputsType = dict[str, ModelOutputType]
+DataType = t.Union[dict[str, t.Any], t.Iterable]
 
 
 class CheckpointType(Enum):
     MODEL_ONLY = 'model_only'
     XZTRAINER = 'xztrainer'
 
 
-class LRSchedulerProtocol(Protocol):
+class LRSchedulerProtocol(t.Protocol):
     def step(self):
         ...
 
     def state_dict(self):
         ...
 
     def load_state_dict(self, state_dict):
         ...
 
 
 @dataclass
 class XZTrainerConfig:
-    batch_size: int
-    batch_size_eval: int
+    experiment_name: str
+    minibatch_size: int
+    minibatch_size_eval: int
     epochs: int
-    optimizer: Callable[[nn.Module], Optimizer]
-    amp_dtype: Optional[dtype] = None
-    experiment_name: str = 'master'
+    optimizer: t.Callable[[nn.Module], Optimizer]
+    scheduler: t.Callable[[Optimizer, int], LRSchedulerProtocol]
     gradient_clipping: float = 1.0
-    scheduler: Optional[Callable[[Optimizer, int], LRSchedulerProtocol]] = None
-    scheduler_type: Optional[SchedulerType] = None
     dataloader_num_workers: int = multiprocessing.cpu_count()
     dataloader_pin_memory: bool = True
     dataloader_persistent_workers: bool = True
     dataloader_shuffle_train_dataset: bool = True
-    accumulation_batches: int = 1
-    print_steps: int = 100
+    log_steps: int = 100
     eval_steps: int = 0
     skip_nan_loss: bool = True
     save_steps: int = 100
-    save_keep_n: int = -1
-    save_dir: str = 'checkpoint'
-    collate_fn: Callable[[List[object]], Any] = default_collate
-    logger: LoggingEngineConfig = field(default_factory=lambda: StreamLoggingEngineConfig())
+    save_keep_n: int = 3
+    collate_fn: t.Callable[[list[object]], t.Any] = default_collate
+    tracker_config: dict[str, t.Any] = field(default_factory=dict)
+    logging_level: t.Union[int, None] = logging.INFO
+
+
+@t.runtime_checkable
+class MetricMultiOutputNamedProtocol(t.Protocol):
+    @property
+    def multi_output_names(self) -> t.List[str]:
+        ...
```

### Comparing `xztrainer-0.9.7/PKG-INFO` & `xztrainer-1.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: xztrainer
-Version: 0.9.7
+Version: 1.0.0
 Summary: A customizable training pipeline for PyTorch
 License: MPL-2.0
 Author: Maxim Afanasyev
 Author-email: mr.applexz@gmail.com
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: numpy
-Provides-Extra: tensorboard
 Provides-Extra: torch
+Requires-Dist: accelerate (>=0.29.2) ; extra == "torch"
 Requires-Dist: numpy (>=1.24.2) ; extra == "numpy"
-Requires-Dist: packaging (>=23.0)
-Requires-Dist: setuptools (>=67.6.0)
-Requires-Dist: tensorboard (>=2.8.0) ; extra == "tensorboard"
 Requires-Dist: torch (>=1.10.0) ; extra == "torch"
+Requires-Dist: torchmetrics (>=1.3.0) ; extra == "torch"
 Requires-Dist: tqdm (>=4.62.3)
```

