# Comparing `tmp/nvidia_ammo-0.9.3.tar.gz` & `tmp/nvidia_ammo-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia_ammo-0.9.3.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
+gzip compressed data, was "nvidia_ammo-0.9.4.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
```

## Comparing `nvidia_ammo-0.9.3.tar` & `nvidia_ammo-0.9.4.tar`

### PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-ammo
-Version: 0.9.3
+Version: 0.9.4
 Summary: Ammo: a unified algorithmic model optimization and deployment toolkit.
 Author-email: "Nvidia, Inc." <ammo-support@exchange.nvidia.com>
 License: NVIDIA Proprietary Software
 Project-URL: Homepage, https://nvidia.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

