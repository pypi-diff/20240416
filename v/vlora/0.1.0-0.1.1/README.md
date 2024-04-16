# Comparing `tmp/vlora-0.1.0.tar.gz` & `tmp/vlora-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vlora-0.1.0.tar", max compression
+gzip compressed data, was "vlora-0.1.1.tar", max compression
```

## Comparing `vlora-0.1.0.tar` & `vlora-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rwxr-xr-x   0        0        0        0 2024-04-09 15:09:36.480210 vlora-0.1.0/README.md
--rwxr-xr-x   0        0        0      321 2024-04-14 04:10:27.211887 vlora-0.1.0/pyproject.toml
--rwxr-xr-x   0        0        0       43 2024-04-14 01:56:08.076961 vlora-0.1.0/vlora/__init__.py
--rwxr-xr-x   0        0        0       40 2024-04-14 01:56:59.509112 vlora-0.1.0/vlora/models/__init__.py
--rwxr-xr-x   0        0        0     1891 2024-04-14 01:50:51.837177 vlora-0.1.0/vlora/models/vit.py
--rwxr-xr-x   0        0        0       29 2024-04-14 01:57:24.608672 vlora-0.1.0/vlora/utils/__init__.py
--rwxr-xr-x   0        0        0     3685 2024-04-14 01:54:54.810885 vlora-0.1.0/vlora/utils/vlorafy.py
--rw-r--r--   0        0        0      506 1970-01-01 00:00:00.000000 vlora-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0        0 2024-04-09 15:09:36.480210 vlora-0.1.1/README.md
+-rwxr-xr-x   0        0        0      342 2024-04-16 04:16:25.884929 vlora-0.1.1/pyproject.toml
+-rwxr-xr-x   0        0        0       43 2024-04-14 01:56:08.076961 vlora-0.1.1/vlora/__init__.py
+-rwxr-xr-x   0        0        0       40 2024-04-14 01:56:59.509112 vlora-0.1.1/vlora/models/__init__.py
+-rwxr-xr-x   0        0        0     1891 2024-04-15 21:50:48.301291 vlora-0.1.1/vlora/models/vit.py
+-rwxr-xr-x   0        0        0       29 2024-04-14 01:57:24.608672 vlora-0.1.1/vlora/utils/__init__.py
+-rwxr-xr-x   0        0        0     3473 2024-04-16 02:25:33.962030 vlora-0.1.1/vlora/utils/vlorafy.py
+-rw-r--r--   0        0        0      429 1970-01-01 00:00:00.000000 vlora-0.1.1/PKG-INFO
```

### Comparing `vlora-0.1.0/vlora/models/vit.py` & `vlora-0.1.1/vlora/models/vit.py`

 * *Files identical despite different names*

### Comparing `vlora-0.1.0/vlora/utils/vlorafy.py` & `vlora-0.1.1/vlora/utils/vlorafy.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,85 +2,86 @@
 from torch import nn
 import torch.nn.utils.parametrize as parametrize
 
 
 def vlorafy(
     base: type[nn.Module],
 ):
-    class vlorafiedClass(base):
-        def __init__(
-            self,
-            *args,
-            vl_base_module: nn.Module,
-            vl_param_name: str | list[str],
-            vl_rank: int | list[int],
-            vl_alpha: int | list[int] = 1,
-            vl_enabled: bool = True,
-            **kwargs,
-        ):
-            super().__init__(*args, **kwargs)
-
-            if isinstance(vl_param_name, str):
-                vl_param_name = [vl_param_name]
-            if isinstance(vl_rank, int):
-                vl_rank = [vl_rank] * len(vl_param_name)
-            if isinstance(vl_alpha, int):
-                vl_alpha = [vl_alpha] * len(vl_param_name)
-            assert len(vl_param_name) == len(vl_rank) == len(vl_alpha)
-            name2param = dict(vl_base_module.named_parameters())
-            assert all(
-                name in name2param for name in vl_param_name
-            ), f"{vl_param_name}\n{list(name2param.keys())}"
-            for name, r, a in zip(vl_param_name, vl_rank, vl_alpha):
-                *mod_names, param_name = name.split(".")
-                base_mod, self_mod = vl_base_module, self
-                for mod_name in mod_names:
-                    base_mod = base_mod.__getattr__(mod_name)
-                    self_mod = self_mod.__getattr__(mod_name)
-                param = base_mod.__getattr__(param_name)
-                self_mod.__setattr__(param_name, param)
-                if len(param.shape) == 1:
-                    parametrize.register_parametrization(
-                        self_mod,
-                        param_name,
-                        VLoRAParam1D(
-                            param.shape[0], param.dtype, param.device, vl_enabled
-                        ),
-                    )
-                elif len(param.shape) == 2:
-                    dim_out, dim_in = param.shape
-                    parametrize.register_parametrization(
-                        self_mod,
-                        param_name,
-                        VLoRAParam2D(
-                            dim_in, dim_out, r, param.dtype, param.device, a, vl_enabled
-                        ),
-                    )
-                else:
-                    raise NotImplementedError
+    return type("_vlorafied", (base,), {"__init__": init_fn})
 
-    return vlorafiedClass
+
+def init_fn(
+    self,
+    *args,
+    vl_base_module: nn.Module,
+    vl_param_name: str | list[str],
+    vl_rank: int | list[int],
+    vl_alpha: int | list[int] = 1,
+    vl_enabled: bool = True,
+    **kwargs,
+):
+    super(self.__class__, self).__init__(*args, **kwargs)
+
+    if isinstance(vl_param_name, str):
+        vl_param_name = [vl_param_name]
+    if isinstance(vl_rank, int):
+        vl_rank = [vl_rank] * len(vl_param_name)
+    if isinstance(vl_alpha, int):
+        vl_alpha = [vl_alpha] * len(vl_param_name)
+    assert len(vl_param_name) == len(vl_rank) == len(vl_alpha)
+    name2param = dict(vl_base_module.named_parameters())
+    assert all(
+        name in name2param for name in vl_param_name
+    ), f"{vl_param_name}\n{list(name2param.keys())}"
+    for name, r, a in zip(vl_param_name, vl_rank, vl_alpha):
+        *mod_names, param_name = name.split(".")
+        base_mod, self_mod = vl_base_module, self
+        for mod_name in mod_names:
+            base_mod = base_mod.__getattr__(mod_name)
+            self_mod = self_mod.__getattr__(mod_name)
+        param = base_mod.__getattr__(param_name)
+        self_mod.__setattr__(param_name, param)
+        if len(param.shape) == 1:
+            parametrize.register_parametrization(
+                self_mod,
+                param_name,
+                VLoRAParam1D(param.shape[0], param.dtype, param.device, vl_enabled),
+            )
+        elif len(param.shape) == 2:
+            dim_out, dim_in = param.shape
+            parametrize.register_parametrization(
+                self_mod,
+                param_name,
+                VLoRAParam2D(
+                    dim_in, dim_out, r, param.dtype, param.device, a, vl_enabled
+                ),
+            )
+        else:
+            raise NotImplementedError
 
 
 class VLoRAParam1D(nn.Module):
     def __init__(
         self,
         dim: int,
         dtype: torch.dtype,
         device: torch.device | str,
         enabled: bool = True,
     ):
         super().__init__()
         self.enabled = enabled
         self.A = nn.Parameter(torch.zeros(dim, dtype=dtype, device=device))
+        self.reset_parameters()
+
+    def reset_parameters(self):
         nn.init.zero_(self.A)
 
     def forward(self, param: torch.Tensor) -> torch.Tensor:
         if self.enabled:
-            return param.clone().detach() + self.A
+            return param.detach() + self.A
         return param
 
 
 class VLoRAParam2D(nn.Module):
     def __init__(
         self,
         dim_in: int,
@@ -94,13 +95,17 @@
         assert rank <= dim_in and rank <= dim_out
         super().__init__()
         self.rank = rank
         self.alpha = alpha
         self.enabled = enabled
         self.A = nn.Parameter(torch.zeros((rank, dim_in), dtype=dtype, device=device))
         self.B = nn.Parameter(torch.zeros((rank, dim_out), dtype=dtype, device=device))
+        self.reset_parameters()
+
+    def reset_parameters(self):
         nn.init.kaiming_uniform_(self.A, a=5**0.5)
+        nn.init.kaiming_uniform_(self.B, a=5**0.5)
 
     def forward(self, param: torch.Tensor) -> torch.Tensor:
         if self.enabled:
-            return param.clone().detach() + self.B.T @ self.A
+            return param.detach() + (self.B.T @ self.A) * (self.alpha / self.rank)
         return param
```

