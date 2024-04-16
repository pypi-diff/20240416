# Comparing `tmp/welford-torch-0.2.3.tar.gz` & `tmp/welford_torch-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "welford-torch-0.2.3.tar", last modified: Tue Feb 27 15:26:50 2024, max compression
+gzip compressed data, was "welford_torch-0.2.4.tar", last modified: Tue Apr 16 17:12:43 2024, max compression
```

## Comparing `welford-torch-0.2.3.tar` & `welford_torch-0.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-02-27 15:26:50.231409 welford-torch-0.2.3/
--rw-r--r--   0 mac        (501) staff       (20)     1065 2022-12-19 15:38:18.000000 welford-torch-0.2.3/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)     5896 2024-02-27 15:26:50.231284 welford-torch-0.2.3/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     5489 2023-09-16 00:16:42.000000 welford-torch-0.2.3/README.md
--rw-r--r--   0 mac        (501) staff       (20)       38 2024-02-27 15:26:50.231450 welford-torch-0.2.3/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      677 2024-02-27 15:24:31.000000 welford-torch-0.2.3/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-02-27 15:26:50.230313 welford-torch-0.2.3/welford_torch/
--rw-r--r--   0 mac        (501) staff       (20)       61 2023-09-15 20:48:31.000000 welford-torch-0.2.3/welford_torch/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     9712 2023-09-15 23:31:31.000000 welford-torch-0.2.3/welford_torch/covariance_torch.py
--rw-r--r--   0 mac        (501) staff       (20)     2043 2022-12-19 16:43:52.000000 welford-torch-0.2.3/welford_torch/example.py
--rw-r--r--   0 mac        (501) staff       (20)     7671 2023-09-15 23:38:45.000000 welford-torch-0.2.3/welford_torch/test_covariance.py
--rw-r--r--   0 mac        (501) staff       (20)     7523 2023-09-15 20:36:11.000000 welford-torch-0.2.3/welford_torch/test_welford.py
--rw-r--r--   0 mac        (501) staff       (20)     6979 2024-02-27 15:23:56.000000 welford-torch-0.2.3/welford_torch/welford_torch.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-02-27 15:26:50.231098 welford-torch-0.2.3/welford_torch.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     5896 2024-02-27 15:26:50.000000 welford-torch-0.2.3/welford_torch.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      389 2024-02-27 15:26:50.000000 welford-torch-0.2.3/welford_torch.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2024-02-27 15:26:50.000000 welford-torch-0.2.3/welford_torch.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)        6 2024-02-27 15:26:50.000000 welford-torch-0.2.3/welford_torch.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       14 2024-02-27 15:26:50.000000 welford-torch-0.2.3/welford_torch.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:12:43.434419 welford_torch-0.2.4/
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-04-16 15:55:57.000000 welford_torch-0.2.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5939 2024-04-16 17:12:43.434419 welford_torch-0.2.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5489 2024-04-16 15:55:57.000000 welford_torch-0.2.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 17:12:43.434419 welford_torch-0.2.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      687 2024-04-16 17:12:15.000000 welford_torch-0.2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:12:43.434419 welford_torch-0.2.4/welford_torch/
+-rw-r--r--   0 root         (0) root         (0)       61 2024-04-16 15:55:57.000000 welford_torch-0.2.4/welford_torch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10426 2024-04-16 17:11:00.000000 welford_torch-0.2.4/welford_torch/covariance_torch.py
+-rw-r--r--   0 root         (0) root         (0)     2043 2024-04-16 15:55:57.000000 welford_torch-0.2.4/welford_torch/example.py
+-rw-r--r--   0 root         (0) root         (0)    10307 2024-04-16 17:10:07.000000 welford_torch-0.2.4/welford_torch/test_covariance.py
+-rw-r--r--   0 root         (0) root         (0)     7523 2024-04-16 15:55:57.000000 welford_torch-0.2.4/welford_torch/test_welford.py
+-rw-r--r--   0 root         (0) root         (0)     6979 2024-04-16 15:55:57.000000 welford_torch-0.2.4/welford_torch/welford_torch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:12:43.434419 welford_torch-0.2.4/welford_torch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5939 2024-04-16 17:12:43.000000 welford_torch-0.2.4/welford_torch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      389 2024-04-16 17:12:43.000000 welford_torch-0.2.4/welford_torch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 17:12:43.000000 welford_torch-0.2.4/welford_torch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-16 17:12:43.000000 welford_torch-0.2.4/welford_torch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-16 17:12:43.000000 welford_torch-0.2.4/welford_torch.egg-info/top_level.txt
```

### Comparing `welford-torch-0.2.3/LICENSE` & `welford_torch-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `welford-torch-0.2.3/PKG-INFO` & `welford_torch-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: welford-torch
-Version: 0.2.3
+Version: 0.2.4
 Summary: Online Pytorch implementation to get Standard Deviation, Covariance, Correlation and Whitening.
 Home-page: https://github.com/pesvut/welford-torch
 Author: Nicky Pochinkov
 Author-email: work@nicky.pro
 License: MIT
 Keywords: statistics,online,welford,torch,covariance,correlation
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: torch
+Requires-Dist: einops
 
 # Welford
 Python (Pytorch) implementation calculating Standard Deviation, Variance,
 Covariance Matrix, and Whitening Matrix online and in parallel. This makes it
 more memory efficient than computing in the standard way.
 
 This implementation uses Welford's algorithm for variance, and standard
```

### Comparing `welford-torch-0.2.3/README.md` & `welford_torch-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `welford-torch-0.2.3/setup.py` & `welford_torch-0.2.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 with open("README.md") as f:
     readme = f.read()
 
 kwargs = {
     "name": "welford-torch",
-    "version": "0.2.3",
+    "version": "0.2.4",
     "description": "Online Pytorch implementation to get Standard Deviation, Covariance, Correlation and Whitening.",
     "author": "Nicky Pochinkov",
     "author_email": "work@nicky.pro",
     "url": "https://github.com/pesvut/welford-torch",
     "license": "MIT",
     "keywords": ["statistics", "online", "welford", "torch", "covariance", "correlation"],
-    "install_requires": ["torch"],
+    "install_requires": ["torch", "einops"],
     "packages": ["welford_torch"],
     "long_description": readme,
     "long_description_content_type": "text/markdown",
 }
 
 setup(**kwargs)
```

### Comparing `welford-torch-0.2.3/welford_torch/covariance_torch.py` & `welford_torch-0.2.4/welford_torch/covariance_torch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Source: https://carstenschelp.github.io/2019/05/12/Online_Covariance_Algorithm_002.html
 
 import torch
+import einops
 
 class OnlineCovariance:
     """
     A class to calculate the mean and the covariance matrix
     of the incrementally added, n-dimensional data.
     """
     def __init__(self, elements=None, dtype=torch.float32, device=None):
@@ -149,36 +150,62 @@
         if self.__shape is None:
             self.init_zeros(observation, device=self.__device)
 
         assert observation.shape == self.__order
         observation = observation.to(self.__dtype).to(self.__device)
 
         self.__count += 1
-        delta_at_nMin1 = observation - self.__mean
-        self.__mean += delta_at_nMin1 / self.__count
-        weighted_delta_at_n = (observation - self.__mean) / self.__count
+        delta_x = observation - self.__mean
+        self.__mean += delta_x / self.__count
+        delta_x_2_weighted = (observation - self.__mean) / self.__count
+
+        ein_string = "... pos_i, ... pos_j -> ... pos_i pos_j"
+        D = einops.einsum(delta_x, delta_x_2_weighted, ein_string)
 
-        D_at_n = self.__expand_last_dim(weighted_delta_at_n).transpose(-2, -1)
-        D = (self.__expand_last_dim(delta_at_nMin1) * self.__identity) @ D_at_n
         self.__cov = self.__cov * (self.__count - 1) / self.__count + D
 
-    def add_all(self, elements):
+    def add_all(self, xs):
         """ add_all
 
         add multiple data samples.
 
         Args:
             elements (array(S, D)): data samples.
             backup_flg (boolean): if True, backup previous state for rollbacking.
 
         """
-        # backup for rollbacking
-        elements = elements.to(dtype=self.__dtype, device=self.__device)
-        for elem in elements:
-            self.add(elem)
+        # check init
+        if self.__order is None:
+            self.init_zeros(xs[0])
+
+        # Move to device
+        xs = xs.to(dtype=self.__dtype, device=self.__device)
+
+        # Check counts and keep track
+        n = xs.shape[0]
+        assert xs.shape[1:] == self.__order
+
+        self.__count += n
+
+        # update means for X and Z
+        old_mean = self.__mean.clone()
+        old_count = int(self.__count)
+        delta_xs   = xs - old_mean
+
+        self.__mean.add_(delta_xs.sum(dim=0)/self.__count)
+        new_mean = self.__mean
+        delta_xs_2 = xs - new_mean
+
+        # Update Covariance Matrices
+        ein_string = "n_tokens ... pos_i, n_tokens ... pos_j -> ... pos_i pos_j"
+        batch_cov_update = einops.einsum(delta_xs, delta_xs_2, ein_string) / self.__count
+        self.__cov.mul_((self.__count-n)/self.__count)
+        self.__cov.add_(batch_cov_update)
+
+        return self
 
     def merge(self, other):
         """
         Merges the current object and the given other object into the current object.
 
         Parameters
         ----------
@@ -239,14 +266,15 @@
 
         Example: tensor [2, 3, 4] (__order) -> expanded_tensor [2, 3, 4, 4] (__shape)
         """
         shape = tensor.shape # __order
         repeat_shape = ( *( [1]*len(shape) ), shape[-1] ) # 1, ..., 1, n
         return tensor.unsqueeze(-1).repeat(repeat_shape)
 
+
     def __compute_eig(self):
         """
         Compute the eigenvalues and eigenvectors of the covariance matrix.
 
         Returns:
             eigenvalues: tensor, The eigenvalues of the covariance matrix.
             eigenvectors: tensor, The eigenvectors of the covariance matrix.
```

### Comparing `welford-torch-0.2.3/welford_torch/example.py` & `welford_torch-0.2.4/welford_torch/example.py`

 * *Files identical despite different names*

### Comparing `welford-torch-0.2.3/welford_torch/test_covariance.py` & `welford_torch-0.2.4/welford_torch/test_covariance.py`

 * *Files 18% similar despite different names*

```diff
@@ -112,14 +112,72 @@
     assert torch.allclose(conventional_mean_2, ocov.mean[1]), \
         "Mean should be the same with both approaches."
     assert np.allclose(conventional_cov_2, torch_to_np(ocov.cov[1]), atol=1e-3), \
         "Covariance-matrix should be the same with both approaches."
     assert np.allclose(conventional_corrcoef_2, torch_to_np(ocov.corrcoef[1])), \
         "Pearson-Correlationcoefficient-matrix should be the same with both approaches."
 
+def test_add_all():
+    "Demonstrate OnlineCovariance.add(observation)"
+
+    # COVARIANCE MATRIX shape [3] -> [3, 3]
+    data = create_correlated_dataset(
+        10000, (2.2, 4.4, 1.5), torch.tensor([[0.2, 0.5, 0.7],[0.3, 0.2, 0.2],[0.5,0.3,0.1]]), (1, 5, 3)
+    )
+
+    # CONVENTIONAL COVARIANCE MATRIX
+    conventional_mean, conventional_cov, conventional_corrcoef = calculate_conventional(data)
+
+    # ONLINE COVARIANCE MATRIX
+    ocov = OnlineCovariance()
+    import einops
+    for data_frac in einops.rearrange(data, "(k ten) ... -> k ten ...", k=1000, ten=10):
+        ocov.add_all(data_frac)
+
+    assert torch.allclose(conventional_mean, ocov.mean), \
+        "Mean should be the same with both approaches."
+
+    assert np.allclose(conventional_cov, torch_to_np(ocov.cov), atol=1e-3), \
+        "Covariance-matrix should be the same with both approaches."
+
+    assert np.allclose(conventional_corrcoef, torch_to_np(ocov.corrcoef)), \
+        "Pearson-Correlationcoefficient-matrix should be the same with both approaches."
+
+    # ONLINE COVARIANCE MATRICES shape [2, 3] -> [2, 3, 3]
+    data_2 = create_correlated_dataset(
+        10000, (6.6, 1.1, 2.5), torch.tensor([[0.9, 0.2, 0.3],[0.3, 0.1, 0.2],[0.2,0.3,0.5]]), (2, 7, 5)
+    )
+
+    # CONVENTIONAL COVARIANCE
+    conventional_mean_2, conventional_cov_2, conventional_corrcoef_2 = calculate_conventional(data_2)
+
+    # ONLINE COVARIANCE MATRIX
+    zipped_data = []
+    for obs_1, obs_2 in zip(data, data_2):
+        zipped_data.append(torch.stack([obs_1, obs_2]))
+    zipped_data = torch.stack(zipped_data)
+
+    ocov = OnlineCovariance()
+    for data_frac in einops.rearrange(zipped_data, "(k ten) ... -> k ten ...", k=1000, ten=10):
+        ocov.add_all(data_frac)
+
+    assert torch.allclose(conventional_mean, ocov.mean[0]), \
+        "Mean should be the same with both approaches."
+    assert np.allclose(conventional_cov, torch_to_np(ocov.cov[0]), atol=1e-3), \
+        "Covariance-matrix should be the same with both approaches."
+    assert np.allclose(conventional_corrcoef, torch_to_np(ocov.corrcoef[0])), \
+        "Pearson-Correlationcoefficient-matrix should be the same with both approaches."
+
+    assert torch.allclose(conventional_mean_2, ocov.mean[1]), \
+        "Mean should be the same with both approaches."
+    assert np.allclose(conventional_cov_2, torch_to_np(ocov.cov[1]), atol=1e-3), \
+        "Covariance-matrix should be the same with both approaches."
+    assert np.allclose(conventional_corrcoef_2, torch_to_np(ocov.corrcoef[1])), \
+        "Pearson-Correlationcoefficient-matrix should be the same with both approaches."
+
 
 def test_merge():
     "Demonstrate OnlineCovariance.merge()"
 
     data_part1 = create_correlated_dataset(500, (2.2, 4.4, 1.5), torch.tensor([[0.2, 0.5, 0.7],[0.3, 0.2, 0.2],[0.5,0.3,0.1]]), (1, 5, 3))
     data_part2 = create_correlated_dataset(1000, (5, 6, 2), torch.tensor([[0.2, 0.5, 0.7],[0.3, 0.2, 0.2],[0.5,0.3,0.1]]), (1, 5, 3))
     ocov_part1 = OnlineCovariance()
@@ -179,14 +237,15 @@
     assert torch.allclose(whitened_ocov.cov, whitened_ocov.identity, atol=1e-3), \
         "Whitening data should lead Covariance Matrix to look like the Identity matrix in this dataset."
 
 def test_all():
     tests = [
         test_init,
         test_add,
+        test_add_all,
         test_merge,
         test_whitening,
     ]
     for test in tests:
         try:
             print(f"# Running test {test.__name__}...")
             test()
```

### Comparing `welford-torch-0.2.3/welford_torch/test_welford.py` & `welford_torch-0.2.4/welford_torch/test_welford.py`

 * *Files identical despite different names*

### Comparing `welford-torch-0.2.3/welford_torch/welford_torch.py` & `welford_torch-0.2.4/welford_torch/welford_torch.py`

 * *Files identical despite different names*

### Comparing `welford-torch-0.2.3/welford_torch.egg-info/PKG-INFO` & `welford_torch-0.2.4/welford_torch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: welford-torch
-Version: 0.2.3
+Version: 0.2.4
 Summary: Online Pytorch implementation to get Standard Deviation, Covariance, Correlation and Whitening.
 Home-page: https://github.com/pesvut/welford-torch
 Author: Nicky Pochinkov
 Author-email: work@nicky.pro
 License: MIT
 Keywords: statistics,online,welford,torch,covariance,correlation
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: torch
+Requires-Dist: einops
 
 # Welford
 Python (Pytorch) implementation calculating Standard Deviation, Variance,
 Covariance Matrix, and Whitening Matrix online and in parallel. This makes it
 more memory efficient than computing in the standard way.
 
 This implementation uses Welford's algorithm for variance, and standard
```

