# Comparing `tmp/vbll-0.1.1.tar.gz` & `tmp/vbll-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbll-0.1.1.tar", max compression
+gzip compressed data, was "vbll-0.1.2.tar", max compression
```

## Comparing `vbll-0.1.1.tar` & `vbll-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1518 2024-04-03 21:17:48.496333 vbll-0.1.1/README.md
--rw-r--r--   0        0        0      298 2024-04-03 21:51:43.234850 vbll-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-19 18:57:42.630224 vbll-0.1.1/vbll/layers/__init__.py
--rw-r--r--   0        0        0     9317 2024-03-19 18:57:42.630316 vbll-0.1.1/vbll/layers/classification.py
--rw-r--r--   0        0        0     4413 2024-03-19 18:57:42.630403 vbll-0.1.1/vbll/layers/regression.py
--rw-r--r--   0        0        0     4445 2024-03-19 18:57:42.630508 vbll-0.1.1/vbll/utils/distributions.py
--rw-r--r--   0        0        0     2029 1970-01-01 00:00:00.000000 vbll-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1518 2024-04-03 21:17:48.496333 vbll-0.1.2/README.md
+-rw-r--r--   0        0        0      298 2024-04-16 02:54:37.185805 vbll-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-04-04 02:26:23.181168 vbll-0.1.2/vbll/__init__.py
+-rw-r--r--   0        0        0      100 2024-04-04 02:26:23.181436 vbll-0.1.2/vbll/layers/__init__.py
+-rw-r--r--   0        0        0    10539 2024-04-12 02:48:25.320525 vbll-0.1.2/vbll/layers/classification.py
+-rw-r--r--   0        0        0     4400 2024-04-04 02:26:23.181823 vbll-0.1.2/vbll/layers/regression.py
+-rw-r--r--   0        0        0     4445 2024-03-19 18:57:42.630508 vbll-0.1.2/vbll/utils/distributions.py
+-rw-r--r--   0        0        0     2029 1970-01-01 00:00:00.000000 vbll-0.1.2/PKG-INFO
```

### Comparing `vbll-0.1.1/README.md` & `vbll-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `vbll-0.1.1/vbll/layers/classification.py` & `vbll-0.1.2/vbll/layers/classification.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import torch.nn.functional as F
 import numpy as np
 from dataclasses import dataclass
 from collections.abc import Callable
 import abc
 import warnings
 
-from vbll.vbll.utils.distributions import Normal, DenseNormal, get_parameterization
+from vbll.utils.distributions import Normal, DenseNormal, get_parameterization
 
 def KL(p, q_scale):
     feat_dim = p.mean.shape[-1]
     mse_term = (p.mean ** 2).sum(-1).sum(-1) / q_scale
     trace_term = (p.trace_covariance / q_scale).sum(-1)
     logdet_term = (feat_dim * np.log(q_scale) - p.logdet_covariance).sum(-1)
 
@@ -20,26 +20,39 @@
 @dataclass
 class VBLLReturn():
     predictive: Normal | DenseNormal # Could return distribution or mean/cov
     train_loss_fn: Callable[[torch.Tensor], torch.Tensor]
     val_loss_fn: Callable[[torch.Tensor], torch.Tensor]
     ood_scores: None | Callable[[torch.Tensor], torch.Tensor] = None
 
-class VBLLClassificationD(nn.Module):
+class DiscClassification(nn.Module):
     def __init__(self,
                  in_features,
                  out_features,
                  regularization_weight,
                  parameterization='dense',
                  softmax_bound='jensen',
                  return_ood=False,
                  prior_scale=1.,
                  wishart_scale=1.,
                  dof=1.):
-        super(VBLLClassificationD, self).__init__()
+        """Initailize a DiscClassification model.
+
+        :param in_features: Number of input features
+        :param out_features: Number of output features
+        :param regularization_weight: Weight of regularization term
+        :param parameterization: Parameterization of the last layer distribution.
+        :param softmax_bound: Bound to use for softmax.
+        :param return_ood: Whether to return OOD scores.
+        :param prior_scale: Scale of the prior.
+        :param wishart_scale: Scale of the Wishart distribution.
+        :param dof: Degrees of freedom of the Wishart distribution.
+
+        """
+        super(DiscClassification, self).__init__()
 
         self.wishart_scale = wishart_scale
         self.dof = (dof + out_features + 1.)/2.
         self.regularization_weight = regularization_weight
 
         # define prior, currently fixing zero mean and arbitrarily scaled cov
         self.prior_scale = prior_scale
@@ -131,27 +144,41 @@
         return loss_fn
 
     # ----- OOD metrics
 
     def max_predictive(self, x):
         return torch.max(self.predictive(x), dim=-1)[0]
 
-class VBLLClassificationG(nn.Module):
+class GenClassification(nn.Module):
     # TODO(jamesharrison): add dirichlet
     def __init__(self,
                  in_features,
                  out_features,
                  regularization_weight,
                  parameterization='dense',
                  softmax_bound='jensen',
                  return_ood=False,
                  prior_scale=1.,
                  wishart_scale=1.,
                  dof=1.):
-        super(VBLLClassificationG, self).__init__()
+        """Initailize a GenClassification model.
+
+        :param in_features: Number of input features
+        :param out_features: Number of output features
+        :param regularization_weight: Weight of regularization term
+        :param parameterization: Parameterization of the last layer distribution. 
+        :param softmax_bound: Bound to use for softmax.
+        :param return_ood: Whether to return OOD scores.
+        :param prior_scale: Scale of the prior.
+        :param wishart_scale: Scale of the Wishart distribution.
+        :param dof: Degrees of freedom of the Wishart distribution.
+
+        """
+
+        super(GenClassification, self).__init__()
 
         self.wishart_scale = wishart_scale
         self.dof = (dof + in_features + 1.)/2.
         self.regularization_weight = regularization_weight
 
         # define prior, currently fixing zero mean and arbitrarily scaled cov
         self.prior_scale = prior_scale
```

### Comparing `vbll-0.1.1/vbll/layers/regression.py` & `vbll-0.1.2/vbll/layers/regression.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import torch
 from dataclasses import dataclass
-from vbll.vbll.utils.distributions import Normal, DenseNormal, get_parameterization
+from vbll.utils.distributions import Normal, DenseNormal, get_parameterization
 from collections.abc import Callable
 import torch.nn as nn
 
 
 def KL(p, q_scale):
     feat_dim = p.mean.shape[-1]
     mse_term = (p.mean ** 2).sum(-1).sum(-1) / q_scale
@@ -18,15 +18,15 @@
 class VBLLReturn():
     predictive: Normal | DenseNormal # Could return distribution or mean/cov
     train_loss_fn: Callable[[torch.Tensor], torch.Tensor]
     val_loss_fn: Callable[[torch.Tensor], torch.Tensor]
     ood_scores: None | Callable[[torch.Tensor], torch.Tensor] = None
 
 
-class VBLLRegression(nn.Module):
+class Regression(nn.Module):
     """
     Variational Bayesian Linear Regression
 
     Parameters
     ----------
     in_features : int
         Number of input features
@@ -47,15 +47,15 @@
                  in_features,
                  out_features,
                  regularization_weight,
                  parameterization='dense',
                  prior_scale=1.,
                  wishart_scale=1e-2,
                  dof=1.):
-        super(VBLLRegression, self).__init__()
+        super(Regression, self).__init__()
 
         self.wishart_scale = wishart_scale
         self.dof = (dof + out_features + 1.)/2.
         self.regularization_weight = regularization_weight
 
         # define prior, currently fixing zero mean and arbitrarily scaled cov
         self.prior_scale = prior_scale
```

### Comparing `vbll-0.1.1/vbll/utils/distributions.py` & `vbll-0.1.2/vbll/utils/distributions.py`

 * *Files identical despite different names*

### Comparing `vbll-0.1.1/PKG-INFO` & `vbll-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: vbll
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: John Willes
 Author-email: johnwilles@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: numpy (>=1.26.0,<2.0.0)
-Requires-Dist: torch (>=2.2.0,<3.0.0)
+Requires-Dist: numpy (>=1.21.0,<2.0.0)
+Requires-Dist: torch (>=1.6.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Variational Bayesian Last Layers (VBLL)
 
 ## Introduction
 VBLL introduces a deterministic variational formulation for training Bayesian last layers in neural networks. This method offers a computationally efficient approach to improving uncertainty estimation in deep learning models. By leveraging this technique, VBLL can be trained and evaluated with quadratic complexity in last layer width, making it nearly computationally free to add to standard architectures. Our work focuses on enhancing predictive accuracy, calibration, and out-of-distribution detection over baselines in both regression and classification.
```

