# Comparing `tmp/keras_generators-1.3.2-py3-none-any.whl.zip` & `tmp/keras_generators-1.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 28287 bytes, number of entries: 16
+Zip file size: 28299 bytes, number of entries: 16
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-08 16:27 examples/__init__.py
 -rw-rw-rw-  2.0 fat     6233 b- defN 23-Apr-13 14:38 examples/predict_stock_price.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-08 16:27 keras_generators/__init__.py
 -rw-rw-rw-  2.0 fat     7068 b- defN 23-Mar-08 16:27 keras_generators/callbacks.py
 -rw-rw-rw-  2.0 fat      520 b- defN 23-Apr-13 14:20 keras_generators/common.py
 -rw-rw-rw-  2.0 fat    10842 b- defN 23-Mar-08 16:27 keras_generators/encoders.py
--rw-rw-rw-  2.0 fat    36086 b- defN 23-May-31 22:45 keras_generators/generators.py
+-rw-rw-rw-  2.0 fat    36106 b- defN 24-Apr-16 20:19 keras_generators/generators.py
 -rw-rw-rw-  2.0 fat     4139 b- defN 23-Mar-08 19:39 keras_generators/splitters.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-08 16:27 keras_generators/model_abstractions/__init__.py
 -rw-rw-rw-  2.0 fat     8063 b- defN 23-Dec-01 13:36 keras_generators/model_abstractions/model_object.py
--rw-rw-rw-  2.0 fat     3188 b- defN 23-Apr-13 14:19 keras_generators/model_abstractions/model_params.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Dec-01 13:39 keras_generators-1.3.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     9873 b- defN 23-Dec-01 13:39 keras_generators-1.3.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Dec-01 13:39 keras_generators-1.3.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       26 b- defN 23-Dec-01 13:39 keras_generators-1.3.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1421 b- defN 23-Dec-01 13:39 keras_generators-1.3.2.dist-info/RECORD
-16 files, 99109 bytes uncompressed, 25901 bytes compressed:  73.9%
+-rw-rw-rw-  2.0 fat     3263 b- defN 24-Apr-16 20:19 keras_generators/model_abstractions/model_params.py
+-rw-rw-rw-  2.0 fat    11558 b- defN 24-Apr-16 20:27 keras_generators-1.4.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     9821 b- defN 24-Apr-16 20:27 keras_generators-1.4.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-16 20:27 keras_generators-1.4.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       26 b- defN 24-Apr-16 20:27 keras_generators-1.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1421 b- defN 24-Apr-16 20:27 keras_generators-1.4.0.dist-info/RECORD
+16 files, 99152 bytes uncompressed, 25913 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: keras_generators/model_abstractions/model_object.py
 Comment: 
 
 Filename: keras_generators/model_abstractions/model_params.py
 Comment: 
 
-Filename: keras_generators-1.3.2.dist-info/LICENSE
+Filename: keras_generators-1.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: keras_generators-1.3.2.dist-info/METADATA
+Filename: keras_generators-1.4.0.dist-info/METADATA
 Comment: 
 
-Filename: keras_generators-1.3.2.dist-info/WHEEL
+Filename: keras_generators-1.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: keras_generators-1.3.2.dist-info/top_level.txt
+Filename: keras_generators-1.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: keras_generators-1.3.2.dist-info/RECORD
+Filename: keras_generators-1.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## keras_generators/generators.py

```diff
@@ -1,21 +1,22 @@
 """
 Reason why not use tf.Dataset:
  - when scaling data, scaling factor aren't saved, so it's impossible to scale during inference in production
 """
+
 import json
 import math
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from typing import Collection, Dict, ForwardRef, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
-from keras.utils import data_utils
 from pydantic import PositiveInt, conint, validate_arguments
 from pydantic.dataclasses import dataclass
+from tensorflow.python.keras.utils import data_utils
 
 from .common import ArbitraryTypes, ImmutableConfig, NumpyArrayEncoder
 from .encoders import ChainedDataEncoder, CompoundDataEncoder, DataEncoder
 from .splitters import OrderedSplitter, TrainValTestSpliter
 
 
 class DataSource(ABC):
```

## keras_generators/model_abstractions/model_params.py

```diff
@@ -1,50 +1,49 @@
 #!/usr/bin/env python
 # Author: ASU --<andrei.suiu@gmail.com>
 
 import json
 from pathlib import Path
-from typing import Optional, List
+from typing import Annotated, List, Literal, Optional
 
-from pydantic import constr, conint, PositiveInt, confloat
+from pydantic import Field, PositiveInt, StringConstraints
 from pyxtension.models import ImmutableExtModel
-from typing_extensions import Literal
 
 
 class ModelParams(ImmutableExtModel):
     """
     This class is a base class used to encode the parameters of a model.
     It's easy serializable and deserializable to/from a file.
     It's immutable, and versioned. It won't deserialize an instance of a class with a different version.
     Feel free to extend this class and add more hyper-parameters and architecture parameters for your model like:
         - number of Dense layers
         - type of RNN layer (LSTM, GRU or RNN)
         - add different versions of the ModelParams
         - etc.
     """
-    version: constr(regex=r"^v1\.0\.0$", strict=True) = "v1.0.0"
 
-    batch_size: conint(ge=-1) = 64
+    version: Annotated[str, StringConstraints(pattern=r"^v1\.0\.0$", strict=True)] = "v1.0.0"
+
+    batch_size: Annotated[int, Field(strict=True, ge=-1)] = 64
     val_batch_size: PositiveInt = 64
-    train_size_ratio: confloat(ge=0, le=1) = 0.6
-    val_size_ratio: confloat(ge=0, le=1) = 0.2
-    split_policy: Literal["random", "sequential"] = 'random'  # The policy for splitting dataset
+    train_size_ratio: Annotated[float, Field(ge=0, le=1)] = 0.6
+    val_size_ratio: Annotated[float, Field(ge=0, le=1)] = 0.2
+    split_policy: Literal["random", "sequential"] = "random"  # The policy for splitting dataset
 
     # Maximum number of epochs to train the model
     max_epochs: PositiveInt = 100
 
     # Total number of steps (batches of samples) before declaring one epoch finished and starting the next epoch.
     steps_per_epoch: Optional[int] = None
-    early_stop_patience: Optional[
-        PositiveInt] = None  # The number of epochs with no improvement after which training will be stopped
+    early_stop_patience: Optional[PositiveInt] = None  # The number of epochs with no improvement after which training will be stopped
     rop_patience: Optional[PositiveInt] = None  # Reduce on plateau patience
-    learning_rate: confloat(ge=0, le=1) = 0.003
+    learning_rate: Annotated[float, Field(ge=0, le=1)] = 0.003
 
-    loss: Literal['mse'] = 'mse'
-    metrics: List[Literal['mse']] = ['mse']
+    loss: Literal["mse"] = "mse"
+    metrics: List[Literal["mse"]] = ["mse"]
 
     input_name: str = "input"  # Name of the main input layer
     target_name: str = "target"  # Name of the main target layer
 
     def get_config(self):
         """Returns the config dictionary for a `ModelParams` instance."""
         return {"data": self.json()}
@@ -70,12 +69,12 @@
 
     @classmethod
     def from_config(cls, config):
         d = json.loads(config["data"])
         return cls(**d)
 
     @classmethod
-    def from_file(cls, fpath: Path) -> 'ModelParams':
+    def from_file(cls, fpath: Path) -> "ModelParams":
         with fpath.open("rt") as f:
             d = json.load(f)
             mp = cls(**d)
             return mp
```

## Comparing `keras_generators-1.3.2.dist-info/LICENSE` & `keras_generators-1.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `keras_generators-1.3.2.dist-info/METADATA` & `keras_generators-1.4.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 Metadata-Version: 2.1
 Name: keras-generators
-Version: 1.3.2
+Version: 1.4.0
 Summary: Multi-dimensional/Multi-input/Multi-output Data preprocessing and Batch Generators for Keras models
 Home-page: https://github.com/asuiu/keras-generators
 Author: Andrei Suiu
 Author-email: andrei.suiu@gmail.com
 License: Apache License 2.0
 Keywords: ML,DataGenerators,Keras,tensorflow
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy >=1.20
 Requires-Dist: pip >=22.1.2
-Requires-Dist: pydantic >=1.10.2
+Requires-Dist: pydantic >=2.0
+Requires-Dist: pyxtension >=1.15.0
 Requires-Dist: scikit-learn >=0.22.2
 Requires-Dist: setuptools >=63.4.1
-Requires-Dist: tensorflow >=2.8.0
+Requires-Dist: tensorflow >=2.16
 Requires-Dist: tsx >=0.1.1
 Requires-Dist: wheel >=0.37.1
-Requires-Dist: pyxtension >=1.15.0
 Provides-Extra: tests
 
 # keras-generators
 
 Multi-dimensional/Multi-input/Multi-output Data preprocessing and Batch Generators for Tensorflow models
 
 ## Installation
```

## Comparing `keras_generators-1.3.2.dist-info/RECORD` & `keras_generators-1.4.0.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 examples/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 examples/predict_stock_price.py,sha256=OLhlvKkctYf12kGk7QgxSWKVWM61EI6r0NzXwSKOuAY,6233
 keras_generators/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 keras_generators/callbacks.py,sha256=fGCSRg13d7oPutoXVnSA2R72ri9kGcZnj47LdNCCcvs,7068
 keras_generators/common.py,sha256=sFcCpVV8dJBrWG3Ry9MhpNZC0l-MZAMBdUBJNwlZYs4,520
 keras_generators/encoders.py,sha256=WwviJAdT_mYwjSIn9wqzt3-DEjLNl7jbliKC2jjlYik,10842
-keras_generators/generators.py,sha256=L9pWUa9xasgawVa73yIphI8zCP9JMz5LUCPoLqXyWhc,36086
+keras_generators/generators.py,sha256=DGdpqFQ5DngMqGWLRzE4UBrfriQnF7_qHF4aZ9YG14E,36106
 keras_generators/splitters.py,sha256=O7AKehcoPiQNjv1kuZWOoax-yvnjTFPuOkwLjox-qMw,4139
 keras_generators/model_abstractions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 keras_generators/model_abstractions/model_object.py,sha256=TkkAcMJQ6S9Onzueret5xNwMZN0eLqqtocbpZEkUZxs,8063
-keras_generators/model_abstractions/model_params.py,sha256=-Dr1zxdO4NaJ9ibYq0IsQg3n79AJyiGv4aaPma67__E,3188
-keras_generators-1.3.2.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-keras_generators-1.3.2.dist-info/METADATA,sha256=SappkfC5rNsdwlnxtwl1ZH8Ygnkqzijcdl-u3C0Ka5Y,9873
-keras_generators-1.3.2.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-keras_generators-1.3.2.dist-info/top_level.txt,sha256=6h3qtPKTpHlh7dFVHfOuDDRxVzXpjgb3hL-O3LMXK2w,26
-keras_generators-1.3.2.dist-info/RECORD,,
+keras_generators/model_abstractions/model_params.py,sha256=114iJ1gi15XEUhhU5vZnBgvfL1GY2ozhEsIiXf7rwTE,3263
+keras_generators-1.4.0.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+keras_generators-1.4.0.dist-info/METADATA,sha256=Fx1195gHaQBTtfL-czLzltBMITN4opxGXNDEG5g_LwA,9821
+keras_generators-1.4.0.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+keras_generators-1.4.0.dist-info/top_level.txt,sha256=6h3qtPKTpHlh7dFVHfOuDDRxVzXpjgb3hL-O3LMXK2w,26
+keras_generators-1.4.0.dist-info/RECORD,,
```

