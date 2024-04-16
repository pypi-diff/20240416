# Comparing `tmp/blenderproc-2.7.0.tar.gz` & `tmp/blenderproc-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/wink_do/PycharmProjects/BlenderProcPip/dist/.tmp-p4xmp18r/blenderproc-2.7.0.tar", last modified: Fri Jan 26 16:26:30 2024, max compression
+gzip compressed data, was "/home/wink_do/PycharmProjects/BlenderProcPip/dist/.tmp-6168m9tc/blenderproc-2.7.1.tar", last modified: Tue Apr 16 09:01:17 2024, max compression
```

## Comparing `blenderproc-2.7.0.tar` & `blenderproc-2.7.1.tar`

### file list

```diff
@@ -1,244 +1,244 @@
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:30.000000 blenderproc-2.7.0/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    35147 2023-08-17 12:19:13.000000 blenderproc-2.7.0/LICENSE
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      102 2023-08-17 12:19:13.000000 blenderproc-2.7.0/MANIFEST.in
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    10163 2024-01-26 16:26:30.000000 blenderproc-2.7.0/PKG-INFO
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     9894 2023-08-17 12:19:13.000000 blenderproc-2.7.0/README.md
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     3258 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/__init__.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      263 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/__main__.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc/api/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/api/__init__.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc/api/camera/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      838 2024-01-26 16:05:01.000000 blenderproc-2.7.0/blenderproc/api/camera/__init__.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc/api/constructor/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)       89 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/api/constructor/__init__.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc/api/filter/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      152 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/api/filter/__init__.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc/api/lighting/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      249 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/api/lighting/__init__.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc/api/loader/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     1212 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/api/loader/__init__.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc/api/material/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      559 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/api/material/__init__.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc/api/math/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      230 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/api/math/__init__.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc/api/object/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      871 2024-01-26 16:05:01.000000 blenderproc-2.7.0/blenderproc/api/object/__init__.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc/api/postprocessing/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      378 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/api/postprocessing/__init__.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc/api/renderer/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      748 2024-01-26 16:05:01.000000 blenderproc-2.7.0/blenderproc/api/renderer/__init__.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc/api/sampler/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      678 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/api/sampler/__init__.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc/api/types/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      423 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/api/types/__init__.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc/api/utility/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      330 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/api/utility/__init__.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc/api/world/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)       90 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/api/world/__init__.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc/api/writer/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      282 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/api/writer/__init__.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    14503 2024-01-26 16:05:01.000000 blenderproc-2.7.0/blenderproc/command_line.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     3819 2024-01-26 16:05:01.000000 blenderproc-2.7.0/blenderproc/debug_startup.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc/external/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/external/__init__.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc/external/vhacd/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/external/vhacd/__init__.py
--rwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)       90 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/external/vhacd/build_linux.sh
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     8333 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/external/vhacd/decompose.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc/python/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/__init__.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc/python/camera/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     5818 2024-01-26 16:05:01.000000 blenderproc-2.7.0/blenderproc/python/camera/CameraProjection.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    18508 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/camera/CameraUtility.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    15546 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/camera/CameraValidation.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    22207 2024-01-26 16:05:01.000000 blenderproc-2.7.0/blenderproc/python/camera/LensDistortionUtility.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/camera/__init__.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc/python/constructor/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    27011 2024-01-26 16:05:01.000000 blenderproc-2.7.0/blenderproc/python/constructor/RandomRoomConstructor.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/constructor/__init__.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc/python/filter/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     7841 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/filter/Filter.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/filter/__init__.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc/python/lighting/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     8702 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/lighting/IntersectingSpotLight.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     7955 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/lighting/SuncgLighting.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     1920 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/lighting/SurfaceLighting.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/lighting/__init__.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc/python/loader/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    18438 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/loader/AMASSLoader.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     8305 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/loader/BlendLoader.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    18085 2024-01-26 16:05:01.000000 blenderproc-2.7.0/blenderproc/python/loader/BopLoader.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    10629 2024-01-26 16:05:01.000000 blenderproc-2.7.0/blenderproc/python/loader/CCMaterialLoader.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    23898 2024-01-26 16:05:01.000000 blenderproc-2.7.0/blenderproc/python/loader/Front3DLoader.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     2969 2024-01-26 16:05:01.000000 blenderproc-2.7.0/blenderproc/python/loader/HavenEnvironmentLoader.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    13427 2024-01-26 16:05:01.000000 blenderproc-2.7.0/blenderproc/python/loader/HavenMaterialLoader.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     8771 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/loader/IKEALoader.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     3290 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/loader/Matterport3DLoader.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     5510 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/loader/ObjectLoader.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     5630 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/loader/Pix3DLoader.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     5849 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/loader/ReplicaLoader.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     5703 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/loader/RockEssentialsRockLoader.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     8313 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/loader/SceneNetLoader.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     7813 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/loader/ShapeNetLoader.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    22816 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/loader/SuncgLoader.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     3590 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/loader/TextureLoader.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    22225 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/loader/URDFLoader.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/loader/__init__.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc/python/material/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     9457 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/material/Dust.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    24897 2024-01-26 16:05:01.000000 blenderproc-2.7.0/blenderproc/python/material/MaterialLoaderUtility.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/material/__init__.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc/python/object/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    16222 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/object/FaceSlicer.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     1181 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/object/ObjectMerging.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     4279 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/object/ObjectPoseSampler.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     6919 2024-01-26 16:05:01.000000 blenderproc-2.7.0/blenderproc/python/object/ObjectReplacer.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     8069 2024-01-26 16:05:01.000000 blenderproc-2.7.0/blenderproc/python/object/OnSurfaceSampler.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    15757 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/object/PhysicsSimulation.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/object/__init__.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc/python/postprocessing/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    24403 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/postprocessing/PostProcessingUtility.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     9305 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/postprocessing/StereoGlobalMatching.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/postprocessing/__init__.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc/python/renderer/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     7836 2024-01-26 16:05:01.000000 blenderproc-2.7.0/blenderproc/python/renderer/FlowRendererUtility.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     4237 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/renderer/NOCSRendererUtility.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    42662 2024-01-26 16:05:01.000000 blenderproc-2.7.0/blenderproc/python/renderer/RendererUtility.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    18538 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/renderer/SegMapRendererUtility.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/renderer/__init__.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc/python/sampler/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     5446 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/sampler/Disk.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     3021 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/sampler/Front3DPointInRoomSampler.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     2577 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/sampler/PartSphere.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     2915 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/sampler/RandomWalk.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     2862 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/sampler/ReplicaPointInRoomSampler.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     3603 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/sampler/Shell.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     1773 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/sampler/Sphere.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     2841 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/sampler/SuncgPointInRoomSampler.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     2168 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/sampler/UniformSO3.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     7022 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/sampler/UpperRegionSampler.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/sampler/__init__.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc/python/tests/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      881 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/tests/SilentMode.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     2058 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/tests/TestsPathManager.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/tests/__init__.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc/python/types/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    11574 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/types/ArmatureUtility.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    11677 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/types/BoneUtility.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    14550 2024-01-26 16:05:01.000000 blenderproc-2.7.0/blenderproc/python/types/EntityUtility.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     2251 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/types/InertialUtility.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    10989 2024-01-26 16:05:01.000000 blenderproc-2.7.0/blenderproc/python/types/LightUtility.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    28270 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/types/LinkUtility.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    24004 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/types/MaterialUtility.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    33599 2024-01-26 16:05:01.000000 blenderproc-2.7.0/blenderproc/python/types/MeshObjectUtility.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     5301 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/types/StructUtility.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      908 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/types/StructUtilityFunctions.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    19000 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/types/URDFUtility.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/types/__init__.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:30.000000 blenderproc-2.7.0/blenderproc/python/utility/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    14810 2024-01-26 16:05:01.000000 blenderproc-2.7.0/blenderproc/python/utility/BlenderUtility.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    10385 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/utility/CollisionUtility.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     1487 2024-01-26 16:05:01.000000 blenderproc-2.7.0/blenderproc/python/utility/DefaultConfig.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     7547 2024-01-26 16:05:01.000000 blenderproc-2.7.0/blenderproc/python/utility/GlobalStorage.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     7242 2024-01-26 16:05:01.000000 blenderproc-2.7.0/blenderproc/python/utility/Initializer.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    12249 2024-01-26 16:05:01.000000 blenderproc-2.7.0/blenderproc/python/utility/InstallUtility.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     3255 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/utility/LabelIdMapping.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    11218 2024-01-26 16:05:01.000000 blenderproc-2.7.0/blenderproc/python/utility/MaterialGetter.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     5855 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/utility/MathUtility.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      941 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/utility/PatternUtility.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    24307 2024-01-26 16:04:59.000000 blenderproc-2.7.0/blenderproc/python/utility/SetupUtility.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    25199 2024-01-26 16:05:01.000000 blenderproc-2.7.0/blenderproc/python/utility/Utility.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/utility/__init__.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:30.000000 blenderproc-2.7.0/blenderproc/python/writer/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    47724 2024-01-26 16:05:01.000000 blenderproc-2.7.0/blenderproc/python/writer/BopWriterUtility.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    20280 2024-01-26 16:05:01.000000 blenderproc-2.7.0/blenderproc/python/writer/CocoWriterUtility.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     7157 2024-01-26 16:04:59.000000 blenderproc-2.7.0/blenderproc/python/writer/GifWriterUtility.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    19757 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/writer/WriterUtility.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/python/writer/__init__.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:30.000000 blenderproc-2.7.0/blenderproc/resources/
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:30.000000 blenderproc-2.7.0/blenderproc/resources/AMASS/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      139 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/resources/AMASS/taxonomy.json
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/resources/__init__.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:30.000000 blenderproc-2.7.0/blenderproc/resources/front_3D/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     1641 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/resources/front_3D/3D_front_mapping.csv
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     1602 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/resources/front_3D/3D_front_nyu_mapping.csv
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/resources/front_3D/__init__.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     3629 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/resources/front_3D/find_all_front_3D_labels.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:30.000000 blenderproc-2.7.0/blenderproc/resources/id_mappings/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      440 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/resources/id_mappings/nyu_idset.csv
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      408 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/resources/id_mappings/old_idset.csv
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc/resources/replica/
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc/resources/replica/height_levels/
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:30.000000 blenderproc-2.7.0/blenderproc/resources/replica/height_levels/apartment_0/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)       15 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/resources/replica/height_levels/apartment_0/height_list_values.txt
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:30.000000 blenderproc-2.7.0/blenderproc/resources/replica/height_levels/apartment_1/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        9 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/resources/replica/height_levels/apartment_1/height_list_values.txt
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:30.000000 blenderproc-2.7.0/blenderproc/resources/replica/height_levels/apartment_2/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        8 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/resources/replica/height_levels/apartment_2/height_list_values.txt
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:30.000000 blenderproc-2.7.0/blenderproc/resources/replica/height_levels/frl_apartment_0/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        8 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/resources/replica/height_levels/frl_apartment_0/height_list_values.txt
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:30.000000 blenderproc-2.7.0/blenderproc/resources/replica/height_levels/frl_apartment_1/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        8 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/resources/replica/height_levels/frl_apartment_1/height_list_values.txt
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:30.000000 blenderproc-2.7.0/blenderproc/resources/replica/height_levels/frl_apartment_2/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        8 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/resources/replica/height_levels/frl_apartment_2/height_list_values.txt
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:30.000000 blenderproc-2.7.0/blenderproc/resources/replica/height_levels/frl_apartment_3/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        8 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/resources/replica/height_levels/frl_apartment_3/height_list_values.txt
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:30.000000 blenderproc-2.7.0/blenderproc/resources/replica/height_levels/frl_apartment_4/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        8 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/resources/replica/height_levels/frl_apartment_4/height_list_values.txt
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:30.000000 blenderproc-2.7.0/blenderproc/resources/replica/height_levels/frl_apartment_5/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        8 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/resources/replica/height_levels/frl_apartment_5/height_list_values.txt
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:30.000000 blenderproc-2.7.0/blenderproc/resources/replica/height_levels/hotel_0/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        9 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/resources/replica/height_levels/hotel_0/height_list_values.txt
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:30.000000 blenderproc-2.7.0/blenderproc/resources/replica/height_levels/office_0/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        9 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/resources/replica/height_levels/office_0/height_list_values.txt
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:30.000000 blenderproc-2.7.0/blenderproc/resources/replica/height_levels/office_1/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        8 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/resources/replica/height_levels/office_1/height_list_values.txt
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:30.000000 blenderproc-2.7.0/blenderproc/resources/replica/height_levels/office_2/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        9 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/resources/replica/height_levels/office_2/height_list_values.txt
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:30.000000 blenderproc-2.7.0/blenderproc/resources/replica/height_levels/office_3/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        8 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/resources/replica/height_levels/office_3/height_list_values.txt
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:30.000000 blenderproc-2.7.0/blenderproc/resources/replica/height_levels/office_4/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        8 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/resources/replica/height_levels/office_4/height_list_values.txt
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:30.000000 blenderproc-2.7.0/blenderproc/resources/replica/height_levels/room_0/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        8 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/resources/replica/height_levels/room_0/height_list_values.txt
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:30.000000 blenderproc-2.7.0/blenderproc/resources/replica/height_levels/room_1/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        8 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/resources/replica/height_levels/room_1/height_list_values.txt
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:30.000000 blenderproc-2.7.0/blenderproc/resources/replica/height_levels/room_2/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        8 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/resources/replica/height_levels/room_2/height_list_values.txt
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:30.000000 blenderproc-2.7.0/blenderproc/resources/scenenet/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      457 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/resources/scenenet/CategoryLabeling.csv
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:30.000000 blenderproc-2.7.0/blenderproc/resources/suncg/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)   159140 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/resources/suncg/Better_labeling_for_NYU.csv
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)   159177 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/resources/suncg/ModelCategoryMapping.csv
--rwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)     5759 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/resources/suncg/light_geometry_compact.txt
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:30.000000 blenderproc-2.7.0/blenderproc/scripts/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/scripts/__init__.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     3927 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/scripts/download_blenderkit.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     4552 2024-01-26 16:05:01.000000 blenderproc-2.7.0/blenderproc/scripts/download_cc_textures.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     6804 2024-01-26 16:05:01.000000 blenderproc-2.7.0/blenderproc/scripts/download_haven.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     7230 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/scripts/download_ikea.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     2041 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/scripts/download_matterport3d.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     1327 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/scripts/download_pix3d.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     1573 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/scripts/download_scenenet.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      866 2024-01-26 16:05:01.000000 blenderproc-2.7.0/blenderproc/scripts/quickstart.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     2590 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/scripts/saveAsImg.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    10952 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/scripts/visHdf5Files.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     4003 2023-08-17 12:19:13.000000 blenderproc-2.7.0/blenderproc/scripts/vis_coco_annotation.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)       70 2024-01-26 16:25:42.000000 blenderproc-2.7.0/blenderproc/version.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc.egg-info/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    10163 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc.egg-info/PKG-INFO
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     7894 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc.egg-info/SOURCES.txt
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        1 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc.egg-info/dependency_links.txt
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)       61 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc.egg-info/entry_points.txt
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)       68 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc.egg-info/requires.txt
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)       12 2024-01-26 16:26:29.000000 blenderproc-2.7.0/blenderproc.egg-info/top_level.txt
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)       38 2024-01-26 16:26:30.000000 blenderproc-2.7.0/setup.cfg
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     1024 2023-08-17 12:19:14.000000 blenderproc-2.7.0/setup.py
-drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-01-26 16:26:30.000000 blenderproc-2.7.0/tests/
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     2189 2023-08-17 12:19:14.000000 blenderproc-2.7.0/tests/testCamera.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     2674 2024-01-26 16:05:01.000000 blenderproc-2.7.0/tests/testCameraProjection.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     4812 2024-01-26 16:05:01.000000 blenderproc-2.7.0/tests/testEntity.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     2408 2023-08-17 12:19:14.000000 blenderproc-2.7.0/tests/testHavenLoader.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     3013 2024-01-26 16:05:01.000000 blenderproc-2.7.0/tests/testLoader.py
--rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     2160 2023-08-17 12:19:14.000000 blenderproc-2.7.0/tests/testUtility.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:17.000000 blenderproc-2.7.1/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    35147 2023-08-17 12:19:13.000000 blenderproc-2.7.1/LICENSE
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      102 2023-08-17 12:19:13.000000 blenderproc-2.7.1/MANIFEST.in
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    10163 2024-04-16 09:01:17.000000 blenderproc-2.7.1/PKG-INFO
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     9894 2023-08-17 12:19:13.000000 blenderproc-2.7.1/README.md
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     3258 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/__init__.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      263 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/__main__.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc/api/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/api/__init__.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc/api/camera/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      870 2024-04-16 08:48:32.000000 blenderproc-2.7.1/blenderproc/api/camera/__init__.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc/api/constructor/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)       89 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/api/constructor/__init__.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc/api/filter/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      152 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/api/filter/__init__.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc/api/lighting/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      249 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/api/lighting/__init__.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc/api/loader/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     1212 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/api/loader/__init__.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc/api/material/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      559 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/api/material/__init__.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc/api/math/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      230 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/api/math/__init__.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc/api/object/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      871 2024-01-26 16:05:01.000000 blenderproc-2.7.1/blenderproc/api/object/__init__.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc/api/postprocessing/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      378 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/api/postprocessing/__init__.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc/api/renderer/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      748 2024-01-26 16:05:01.000000 blenderproc-2.7.1/blenderproc/api/renderer/__init__.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc/api/sampler/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      678 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/api/sampler/__init__.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc/api/types/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      423 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/api/types/__init__.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc/api/utility/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      330 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/api/utility/__init__.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc/api/world/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)       90 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/api/world/__init__.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc/api/writer/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      282 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/api/writer/__init__.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    14503 2024-01-26 16:05:01.000000 blenderproc-2.7.1/blenderproc/command_line.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     3819 2024-01-26 16:05:01.000000 blenderproc-2.7.1/blenderproc/debug_startup.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc/external/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/external/__init__.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc/external/vhacd/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/external/vhacd/__init__.py
+-rwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)       90 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/external/vhacd/build_linux.sh
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     8333 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/external/vhacd/decompose.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc/python/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/__init__.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc/python/camera/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     6931 2024-04-16 08:48:32.000000 blenderproc-2.7.1/blenderproc/python/camera/CameraProjection.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    18508 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/camera/CameraUtility.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    15546 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/camera/CameraValidation.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    22207 2024-01-26 16:05:01.000000 blenderproc-2.7.1/blenderproc/python/camera/LensDistortionUtility.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/camera/__init__.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc/python/constructor/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    27011 2024-01-26 16:05:01.000000 blenderproc-2.7.1/blenderproc/python/constructor/RandomRoomConstructor.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/constructor/__init__.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc/python/filter/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     7841 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/filter/Filter.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/filter/__init__.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc/python/lighting/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     8702 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/lighting/IntersectingSpotLight.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     7955 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/lighting/SuncgLighting.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     1920 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/lighting/SurfaceLighting.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/lighting/__init__.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc/python/loader/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    18438 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/loader/AMASSLoader.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     8330 2024-04-16 08:48:32.000000 blenderproc-2.7.1/blenderproc/python/loader/BlendLoader.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    18085 2024-01-26 16:05:01.000000 blenderproc-2.7.1/blenderproc/python/loader/BopLoader.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    10629 2024-01-26 16:05:01.000000 blenderproc-2.7.1/blenderproc/python/loader/CCMaterialLoader.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    23898 2024-01-26 16:05:01.000000 blenderproc-2.7.1/blenderproc/python/loader/Front3DLoader.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     2969 2024-01-26 16:05:01.000000 blenderproc-2.7.1/blenderproc/python/loader/HavenEnvironmentLoader.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    13427 2024-01-26 16:05:01.000000 blenderproc-2.7.1/blenderproc/python/loader/HavenMaterialLoader.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     8771 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/loader/IKEALoader.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     3290 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/loader/Matterport3DLoader.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     5679 2024-04-16 08:48:32.000000 blenderproc-2.7.1/blenderproc/python/loader/ObjectLoader.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     5630 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/loader/Pix3DLoader.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     5849 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/loader/ReplicaLoader.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     5703 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/loader/RockEssentialsRockLoader.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     8313 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/loader/SceneNetLoader.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     7813 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/loader/ShapeNetLoader.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    22816 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/loader/SuncgLoader.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     3590 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/loader/TextureLoader.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    22225 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/loader/URDFLoader.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/loader/__init__.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc/python/material/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     9457 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/material/Dust.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    24897 2024-01-26 16:05:01.000000 blenderproc-2.7.1/blenderproc/python/material/MaterialLoaderUtility.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/material/__init__.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc/python/object/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    16222 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/object/FaceSlicer.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     1181 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/object/ObjectMerging.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     4279 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/object/ObjectPoseSampler.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     6919 2024-01-26 16:05:01.000000 blenderproc-2.7.1/blenderproc/python/object/ObjectReplacer.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     8069 2024-01-26 16:05:01.000000 blenderproc-2.7.1/blenderproc/python/object/OnSurfaceSampler.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    15757 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/object/PhysicsSimulation.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/object/__init__.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc/python/postprocessing/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    24761 2024-04-16 08:48:32.000000 blenderproc-2.7.1/blenderproc/python/postprocessing/PostProcessingUtility.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     9305 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/postprocessing/StereoGlobalMatching.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/postprocessing/__init__.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc/python/renderer/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     7836 2024-01-26 16:05:01.000000 blenderproc-2.7.1/blenderproc/python/renderer/FlowRendererUtility.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     4237 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/renderer/NOCSRendererUtility.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    42662 2024-01-26 16:05:01.000000 blenderproc-2.7.1/blenderproc/python/renderer/RendererUtility.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    18538 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/renderer/SegMapRendererUtility.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/renderer/__init__.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc/python/sampler/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     5446 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/sampler/Disk.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     3021 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/sampler/Front3DPointInRoomSampler.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     2577 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/sampler/PartSphere.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     2915 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/sampler/RandomWalk.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     2862 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/sampler/ReplicaPointInRoomSampler.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     3603 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/sampler/Shell.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     1773 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/sampler/Sphere.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     2841 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/sampler/SuncgPointInRoomSampler.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     2168 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/sampler/UniformSO3.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     7022 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/sampler/UpperRegionSampler.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/sampler/__init__.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc/python/tests/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      881 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/tests/SilentMode.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     2058 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/tests/TestsPathManager.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/tests/__init__.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc/python/types/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    11574 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/types/ArmatureUtility.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    11677 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/types/BoneUtility.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    14565 2024-04-16 08:48:32.000000 blenderproc-2.7.1/blenderproc/python/types/EntityUtility.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     2251 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/types/InertialUtility.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    10989 2024-01-26 16:05:01.000000 blenderproc-2.7.1/blenderproc/python/types/LightUtility.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    28270 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/types/LinkUtility.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    24004 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/types/MaterialUtility.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    33599 2024-01-26 16:05:01.000000 blenderproc-2.7.1/blenderproc/python/types/MeshObjectUtility.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     5301 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/types/StructUtility.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      908 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/types/StructUtilityFunctions.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    19000 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/types/URDFUtility.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/types/__init__.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:17.000000 blenderproc-2.7.1/blenderproc/python/utility/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    14810 2024-01-26 16:05:01.000000 blenderproc-2.7.1/blenderproc/python/utility/BlenderUtility.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    10385 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/utility/CollisionUtility.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     1487 2024-01-26 16:05:01.000000 blenderproc-2.7.1/blenderproc/python/utility/DefaultConfig.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     7547 2024-01-26 16:05:01.000000 blenderproc-2.7.1/blenderproc/python/utility/GlobalStorage.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     7248 2024-04-16 08:48:32.000000 blenderproc-2.7.1/blenderproc/python/utility/Initializer.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    12249 2024-01-26 16:05:01.000000 blenderproc-2.7.1/blenderproc/python/utility/InstallUtility.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     3255 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/utility/LabelIdMapping.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    11218 2024-01-26 16:05:01.000000 blenderproc-2.7.1/blenderproc/python/utility/MaterialGetter.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     5855 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/utility/MathUtility.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      941 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/utility/PatternUtility.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    24307 2024-01-26 16:04:59.000000 blenderproc-2.7.1/blenderproc/python/utility/SetupUtility.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    25199 2024-01-26 16:05:01.000000 blenderproc-2.7.1/blenderproc/python/utility/Utility.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/utility/__init__.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:17.000000 blenderproc-2.7.1/blenderproc/python/writer/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    47768 2024-04-16 08:48:32.000000 blenderproc-2.7.1/blenderproc/python/writer/BopWriterUtility.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    20280 2024-01-26 16:05:01.000000 blenderproc-2.7.1/blenderproc/python/writer/CocoWriterUtility.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     7158 2024-01-26 16:35:00.000000 blenderproc-2.7.1/blenderproc/python/writer/GifWriterUtility.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    19757 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/writer/WriterUtility.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/python/writer/__init__.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:17.000000 blenderproc-2.7.1/blenderproc/resources/
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:17.000000 blenderproc-2.7.1/blenderproc/resources/AMASS/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      139 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/resources/AMASS/taxonomy.json
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/resources/__init__.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:17.000000 blenderproc-2.7.1/blenderproc/resources/front_3D/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     1641 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/resources/front_3D/3D_front_mapping.csv
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     1602 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/resources/front_3D/3D_front_nyu_mapping.csv
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/resources/front_3D/__init__.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     3629 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/resources/front_3D/find_all_front_3D_labels.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:17.000000 blenderproc-2.7.1/blenderproc/resources/id_mappings/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      440 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/resources/id_mappings/nyu_idset.csv
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      408 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/resources/id_mappings/old_idset.csv
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc/resources/replica/
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc/resources/replica/height_levels/
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:17.000000 blenderproc-2.7.1/blenderproc/resources/replica/height_levels/apartment_0/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)       15 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/resources/replica/height_levels/apartment_0/height_list_values.txt
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:17.000000 blenderproc-2.7.1/blenderproc/resources/replica/height_levels/apartment_1/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        9 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/resources/replica/height_levels/apartment_1/height_list_values.txt
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:17.000000 blenderproc-2.7.1/blenderproc/resources/replica/height_levels/apartment_2/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        8 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/resources/replica/height_levels/apartment_2/height_list_values.txt
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:17.000000 blenderproc-2.7.1/blenderproc/resources/replica/height_levels/frl_apartment_0/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        8 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/resources/replica/height_levels/frl_apartment_0/height_list_values.txt
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:17.000000 blenderproc-2.7.1/blenderproc/resources/replica/height_levels/frl_apartment_1/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        8 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/resources/replica/height_levels/frl_apartment_1/height_list_values.txt
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:17.000000 blenderproc-2.7.1/blenderproc/resources/replica/height_levels/frl_apartment_2/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        8 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/resources/replica/height_levels/frl_apartment_2/height_list_values.txt
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:17.000000 blenderproc-2.7.1/blenderproc/resources/replica/height_levels/frl_apartment_3/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        8 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/resources/replica/height_levels/frl_apartment_3/height_list_values.txt
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:17.000000 blenderproc-2.7.1/blenderproc/resources/replica/height_levels/frl_apartment_4/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        8 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/resources/replica/height_levels/frl_apartment_4/height_list_values.txt
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:17.000000 blenderproc-2.7.1/blenderproc/resources/replica/height_levels/frl_apartment_5/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        8 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/resources/replica/height_levels/frl_apartment_5/height_list_values.txt
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:17.000000 blenderproc-2.7.1/blenderproc/resources/replica/height_levels/hotel_0/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        9 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/resources/replica/height_levels/hotel_0/height_list_values.txt
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:17.000000 blenderproc-2.7.1/blenderproc/resources/replica/height_levels/office_0/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        9 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/resources/replica/height_levels/office_0/height_list_values.txt
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:17.000000 blenderproc-2.7.1/blenderproc/resources/replica/height_levels/office_1/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        8 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/resources/replica/height_levels/office_1/height_list_values.txt
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:17.000000 blenderproc-2.7.1/blenderproc/resources/replica/height_levels/office_2/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        9 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/resources/replica/height_levels/office_2/height_list_values.txt
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:17.000000 blenderproc-2.7.1/blenderproc/resources/replica/height_levels/office_3/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        8 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/resources/replica/height_levels/office_3/height_list_values.txt
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:17.000000 blenderproc-2.7.1/blenderproc/resources/replica/height_levels/office_4/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        8 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/resources/replica/height_levels/office_4/height_list_values.txt
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:17.000000 blenderproc-2.7.1/blenderproc/resources/replica/height_levels/room_0/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        8 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/resources/replica/height_levels/room_0/height_list_values.txt
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:17.000000 blenderproc-2.7.1/blenderproc/resources/replica/height_levels/room_1/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        8 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/resources/replica/height_levels/room_1/height_list_values.txt
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:17.000000 blenderproc-2.7.1/blenderproc/resources/replica/height_levels/room_2/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        8 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/resources/replica/height_levels/room_2/height_list_values.txt
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:17.000000 blenderproc-2.7.1/blenderproc/resources/scenenet/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      457 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/resources/scenenet/CategoryLabeling.csv
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:17.000000 blenderproc-2.7.1/blenderproc/resources/suncg/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)   159140 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/resources/suncg/Better_labeling_for_NYU.csv
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)   159177 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/resources/suncg/ModelCategoryMapping.csv
+-rwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)     5759 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/resources/suncg/light_geometry_compact.txt
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:17.000000 blenderproc-2.7.1/blenderproc/scripts/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/scripts/__init__.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     3927 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/scripts/download_blenderkit.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     4552 2024-01-26 16:05:01.000000 blenderproc-2.7.1/blenderproc/scripts/download_cc_textures.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     6804 2024-01-26 16:05:01.000000 blenderproc-2.7.1/blenderproc/scripts/download_haven.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     7230 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/scripts/download_ikea.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     2041 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/scripts/download_matterport3d.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     1327 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/scripts/download_pix3d.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     1573 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/scripts/download_scenenet.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)      866 2024-01-26 16:05:01.000000 blenderproc-2.7.1/blenderproc/scripts/quickstart.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     2590 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/scripts/saveAsImg.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    10952 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/scripts/visHdf5Files.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     4003 2023-08-17 12:19:13.000000 blenderproc-2.7.1/blenderproc/scripts/vis_coco_annotation.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)       70 2024-04-16 09:00:11.000000 blenderproc-2.7.1/blenderproc/version.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc.egg-info/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)    10163 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc.egg-info/PKG-INFO
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     7894 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc.egg-info/SOURCES.txt
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)        1 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc.egg-info/dependency_links.txt
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)       61 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc.egg-info/entry_points.txt
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)       68 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc.egg-info/requires.txt
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)       12 2024-04-16 09:01:16.000000 blenderproc-2.7.1/blenderproc.egg-info/top_level.txt
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)       38 2024-04-16 09:01:17.000000 blenderproc-2.7.1/setup.cfg
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     1024 2023-08-17 12:19:14.000000 blenderproc-2.7.1/setup.py
+drwxrwx---   0 wink_do  (120347) dlr_wink_do_p (422229)        0 2024-04-16 09:01:17.000000 blenderproc-2.7.1/tests/
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     2189 2023-08-17 12:19:14.000000 blenderproc-2.7.1/tests/testCamera.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     3914 2024-04-16 08:48:32.000000 blenderproc-2.7.1/tests/testCameraProjection.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     4812 2024-01-26 16:05:01.000000 blenderproc-2.7.1/tests/testEntity.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     2408 2023-08-17 12:19:14.000000 blenderproc-2.7.1/tests/testHavenLoader.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     3013 2024-01-26 16:05:01.000000 blenderproc-2.7.1/tests/testLoader.py
+-rw-rw----   0 wink_do  (120347) dlr_wink_do_p (422229)     2160 2023-08-17 12:19:14.000000 blenderproc-2.7.1/tests/testUtility.py
```

### Comparing `blenderproc-2.7.0/LICENSE` & `blenderproc-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/PKG-INFO` & `blenderproc-2.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blenderproc
-Version: 2.7.0
+Version: 2.7.1
 Home-page: https://github.com/DLR-RM/BlenderProc
 Author: Maximilian Denninger, Dominik Winkelbauer, Martin Sundermeyer
 Maintainer: Dominik Winkelbauer
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BlenderProc2
```

### Comparing `blenderproc-2.7.0/README.md` & `blenderproc-2.7.1/README.md`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/__init__.py` & `blenderproc-2.7.1/blenderproc/__init__.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/api/camera/__init__.py` & `blenderproc-2.7.1/blenderproc/api/camera/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 from blenderproc.python.camera.CameraUtility import add_camera_pose, get_camera_pose, rotation_from_forward_vec, \
     set_intrinsics_from_blender_params, set_stereo_parameters, set_intrinsics_from_K_matrix, get_sensor_size, \
     get_view_fac_in_px, get_intrinsics_as_K_matrix, get_fov, add_depth_of_field, set_resolution, \
     get_camera_frustum, get_camera_frustum_as_object, is_point_inside_camera_frustum
 from blenderproc.python.camera.CameraValidation import perform_obstacle_in_view_check, visible_objects, \
     scene_coverage_score, decrease_interest_score, check_novel_pose
 from blenderproc.python.camera.LensDistortionUtility import set_lens_distortion, set_camera_parameters_from_config_file
-from blenderproc.python.camera.CameraProjection import depth_via_raytracing, pointcloud_from_depth, project_points, unproject_points
+from blenderproc.python.camera.CameraProjection import depth_via_raytracing, depth_at_points_via_raytracing, pointcloud_from_depth, project_points, unproject_points
```

### Comparing `blenderproc-2.7.0/blenderproc/api/loader/__init__.py` & `blenderproc-2.7.1/blenderproc/api/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/api/material/__init__.py` & `blenderproc-2.7.1/blenderproc/api/material/__init__.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/api/object/__init__.py` & `blenderproc-2.7.1/blenderproc/api/object/__init__.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/api/renderer/__init__.py` & `blenderproc-2.7.1/blenderproc/api/renderer/__init__.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/api/sampler/__init__.py` & `blenderproc-2.7.1/blenderproc/api/sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/command_line.py` & `blenderproc-2.7.1/blenderproc/command_line.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/debug_startup.py` & `blenderproc-2.7.1/blenderproc/debug_startup.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/external/vhacd/decompose.py` & `blenderproc-2.7.1/blenderproc/external/vhacd/decompose.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/camera/CameraProjection.py` & `blenderproc-2.7.1/blenderproc/python/camera/CameraProjection.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,14 +18,42 @@
 
     :param bvh_tree: The BVH tree to use for raytracing.
     :param frame: The frame number whose assigned camera pose should be used. If None is given, the current frame
                   is used.
     :param return_dist: If True, a distance image instead of a depth image is returned.
     :return: The depth image with shape [H, W].
     """
+    resolution_x = bpy.context.scene.render.resolution_x
+    resolution_y = bpy.context.scene.render.resolution_y
+
+    # Generate 2D coordinates of all pixels
+    y = np.arange(resolution_y)   
+    x = np.arange(resolution_x)
+    points = np.stack(np.meshgrid(x, y), -1).astype(np.float32)
+
+    # Calc depth at points
+    depth = depth_at_points_via_raytracing(bvh_tree, points.reshape(-1, 2), frame, return_dist)
+    
+    # Reshape back into depth image
+    depth = np.reshape(depth, [resolution_y, resolution_x])
+    return depth
+
+
+def depth_at_points_via_raytracing(bvh_tree: BVHTree, points_2d: np.ndarray, frame: Optional[int] = None, return_dist: bool = False) -> np.ndarray:
+    """ Computes the depth values at the given 2D points.
+
+    All points that correspond to rays which do not hit any object are set to inf.
+
+    :param bvh_tree: The BVH tree to use for raytracing.
+    :param points_2d: An array of N 2D points with shape [N, 2].
+    :param frame: The frame number whose assigned camera pose should be used. If None is given, the current frame
+                  is used.
+    :param return_dist: If True, distance values instead of depth are returned.
+    :return: The depth values with shape [N].
+    """
     with KeyFrame(frame):
         cam_ob = bpy.context.scene.camera
         cam = cam_ob.data
 
         cam2world_matrix = cam_ob.matrix_world
         resolution_x = bpy.context.scene.render.resolution_x
         resolution_y = bpy.context.scene.render.resolution_y
@@ -38,32 +66,31 @@
         # Compute vectors along both sides of the plane
         vec_x = frame[3] - frame[0]
         vec_y = frame[1] - frame[0]
 
         dists = []
         # Go in discrete grid-like steps over plane
         position = cam2world_matrix.to_translation()
-        for y in range(0, resolution_y):
-            for x in reversed(range(0, resolution_x)):
-                # Compute current point on plane
-                end = frame[0] + vec_x * (x + 0.5) / float(resolution_x) \
-                        + vec_y * (y + 0.5) / float(resolution_y)
-                # Send ray from the camera position through the current point on the plane
-                _, _, _, dist = bvh_tree.ray_cast(position, end - position)
-                if dist is None:
-                    dist = np.inf
+        for p in points_2d:
+            # Compute current point on plane
+            end = frame[0] + vec_x * (resolution_x - (p[0] + 0.5)) / float(resolution_x) \
+                    + vec_y * (p[1] + 0.5) / float(resolution_y)
+            # Send ray from the camera position through the current point on the plane
+            _, _, _, dist = bvh_tree.ray_cast(position, end - position)
+            if dist is None:
+                dist = np.inf
 
-                dists.append(dist)
+            dists.append(dist)
         dists = np.array(dists)
-        dists = np.reshape(dists, [resolution_y, resolution_x])
 
         if not return_dist:
-            depth = dist2depth(dists)
-        return depth
-
+            return dist2depth(dists, points_2d)
+        else:
+            return dists
+    
 def unproject_points(points_2d: np.ndarray, depth: np.ndarray, frame: Optional[int] = None, depth_cut_off: float = 1e6) -> np.ndarray:
     """ Unproject 2D points into 3D
 
     :param points_2d: An array of N 2D points with shape [N, 2].
     :param depth: A list of depth values corresponding to each 2D point, shape [N].
     :param frame: The frame number whose assigned camera pose should be used. If None is given, the current frame
                   is used.
```

### Comparing `blenderproc-2.7.0/blenderproc/python/camera/CameraUtility.py` & `blenderproc-2.7.1/blenderproc/python/camera/CameraUtility.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/camera/CameraValidation.py` & `blenderproc-2.7.1/blenderproc/python/camera/CameraValidation.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/camera/LensDistortionUtility.py` & `blenderproc-2.7.1/blenderproc/python/camera/LensDistortionUtility.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/constructor/RandomRoomConstructor.py` & `blenderproc-2.7.1/blenderproc/python/constructor/RandomRoomConstructor.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/filter/Filter.py` & `blenderproc-2.7.1/blenderproc/python/filter/Filter.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/lighting/IntersectingSpotLight.py` & `blenderproc-2.7.1/blenderproc/python/lighting/IntersectingSpotLight.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/lighting/SuncgLighting.py` & `blenderproc-2.7.1/blenderproc/python/lighting/SuncgLighting.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/lighting/SurfaceLighting.py` & `blenderproc-2.7.1/blenderproc/python/lighting/SurfaceLighting.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/loader/AMASSLoader.py` & `blenderproc-2.7.1/blenderproc/python/loader/AMASSLoader.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/loader/BlendLoader.py` & `blenderproc-2.7.1/blenderproc/python/loader/BlendLoader.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,16 @@
     :param obj_types: The type of objects to load. This parameter is only relevant when `data_blocks`
                       is set to `"objects"`. Available options are: ['mesh', 'curve', 'hair', 'armature',
                       'empty', 'light', 'camera']
     :param name_regrex: Regular expression representing a name pattern of entities' (everything that can be
                         stored in a .blend file's folders, see Blender's documentation for bpy.types.ID
                         for more info) names.
     :param data_blocks: The data block or a list of data blocks which should be loaded from the given .blend file.
-                        Available options are: ['armatures', 'cameras', 'curves', 'hairs', 'images', 'lights',
-                        'materials', 'meshes', 'objects', 'textures']
+                        Available options are: ['armatures', 'cameras', 'curves', 'hairs', 'hair_curves', 'images',
+                        'lights', 'materials', 'meshes', 'objects', 'textures']
     :param link: whether to link instead of append data blocks from .blend file. Linked objects can not be modified.
     :return: The list of loaded mesh objects.
     """
     if obj_types is None:
         obj_types = ["mesh", "empty"]
     # get a path to a .blend file
     path = resolve_path(path)
@@ -97,16 +97,16 @@
     _BlendLoader.purge_added_orphans(orphans_before, data_to)
     return loaded_objects
 
 
 class _BlendLoader:
     valid_data_blocks = [collection.lower() for collection in dir(bpy.data) if
                         isinstance(getattr(bpy.data, collection), bpy.types.bpy_prop_collection)]
-    valid_object_types = ['mesh', 'curve', 'surface', 'meta', 'font', 'hair', 'pointcloud', 'volume', 'gpencil',
-                          'armature', 'lattice', 'empty', 'light', 'light_probe', 'camera', 'speaker']
+    valid_object_types = ['mesh', 'curve', 'curves', 'surface', 'meta', 'font', 'hair', 'pointcloud', 'volume',
+                          'gpencil', 'armature', 'lattice', 'empty', 'light', 'light_probe', 'camera', 'speaker']
 
     @staticmethod
     def validate_and_standardizes_configured_list(config_value: Union[list, str], allowed_elements: list,
                                                   element_name: str) -> list:
         """ Makes sure the given config value is a list, is lower case and only consists of valid elements.
 
         :param config_value: The configured value that should be standardized and validated.
```

### Comparing `blenderproc-2.7.0/blenderproc/python/loader/BopLoader.py` & `blenderproc-2.7.1/blenderproc/python/loader/BopLoader.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/loader/CCMaterialLoader.py` & `blenderproc-2.7.1/blenderproc/python/loader/CCMaterialLoader.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/loader/Front3DLoader.py` & `blenderproc-2.7.1/blenderproc/python/loader/Front3DLoader.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/loader/HavenEnvironmentLoader.py` & `blenderproc-2.7.1/blenderproc/python/loader/HavenEnvironmentLoader.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/loader/HavenMaterialLoader.py` & `blenderproc-2.7.1/blenderproc/python/loader/HavenMaterialLoader.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/loader/IKEALoader.py` & `blenderproc-2.7.1/blenderproc/python/loader/IKEALoader.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/loader/Matterport3DLoader.py` & `blenderproc-2.7.1/blenderproc/python/loader/Matterport3DLoader.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/loader/ObjectLoader.py` & `blenderproc-2.7.1/blenderproc/python/loader/ObjectLoader.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,14 +101,16 @@
                                 obj not in previously_selected_objects]
         for obj in selected_objects:
             obj.data.materials.append(mat)
     elif filepath.lower().endswith('.fbx'):
         bpy.ops.import_scene.fbx(filepath=filepath)
     elif filepath.lower().endswith('.glb') or filepath.lower().endswith('.gltf'):
         bpy.ops.import_scene.gltf(filepath=filepath)
+    elif filepath.lower().endswith('.usda') or filepath.lower().endswith('.usd') or filepath.lower().endswith('.usdc'):
+        bpy.ops.wm.usd_import(filepath=filepath)
 
     mesh_objects = convert_to_meshes([obj for obj in bpy.context.selected_objects
                                   if obj not in previously_selected_objects])
     # Add model_path cp to all objects
     for obj in mesh_objects:
         obj.set_cp("model_path", filepath)
     return mesh_objects
```

### Comparing `blenderproc-2.7.0/blenderproc/python/loader/Pix3DLoader.py` & `blenderproc-2.7.1/blenderproc/python/loader/Pix3DLoader.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/loader/ReplicaLoader.py` & `blenderproc-2.7.1/blenderproc/python/loader/ReplicaLoader.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/loader/RockEssentialsRockLoader.py` & `blenderproc-2.7.1/blenderproc/python/loader/RockEssentialsRockLoader.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/loader/SceneNetLoader.py` & `blenderproc-2.7.1/blenderproc/python/loader/SceneNetLoader.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/loader/ShapeNetLoader.py` & `blenderproc-2.7.1/blenderproc/python/loader/ShapeNetLoader.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/loader/SuncgLoader.py` & `blenderproc-2.7.1/blenderproc/python/loader/SuncgLoader.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/loader/TextureLoader.py` & `blenderproc-2.7.1/blenderproc/python/loader/TextureLoader.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/loader/URDFLoader.py` & `blenderproc-2.7.1/blenderproc/python/loader/URDFLoader.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/material/Dust.py` & `blenderproc-2.7.1/blenderproc/python/material/Dust.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/material/MaterialLoaderUtility.py` & `blenderproc-2.7.1/blenderproc/python/material/MaterialLoaderUtility.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/object/FaceSlicer.py` & `blenderproc-2.7.1/blenderproc/python/object/FaceSlicer.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/object/ObjectMerging.py` & `blenderproc-2.7.1/blenderproc/python/object/ObjectMerging.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/object/ObjectPoseSampler.py` & `blenderproc-2.7.1/blenderproc/python/object/ObjectPoseSampler.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/object/ObjectReplacer.py` & `blenderproc-2.7.1/blenderproc/python/object/ObjectReplacer.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/object/OnSurfaceSampler.py` & `blenderproc-2.7.1/blenderproc/python/object/OnSurfaceSampler.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/object/PhysicsSimulation.py` & `blenderproc-2.7.1/blenderproc/python/object/PhysicsSimulation.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/postprocessing/PostProcessingUtility.py` & `blenderproc-2.7.1/blenderproc/python/postprocessing/PostProcessingUtility.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,31 +8,36 @@
 import cv2
 from scipy import stats
 
 from blenderproc.python.camera import CameraUtility
 from blenderproc.python.utility.BlenderUtility import get_all_blender_mesh_objects
 
 
-def dist2depth(dist: Union[List[np.ndarray], np.ndarray]) -> Union[List[np.ndarray], np.ndarray]:
+def dist2depth(dist: Union[List[np.ndarray], np.ndarray], points_2d: Optional[np.ndarray] = None) -> Union[List[np.ndarray], np.ndarray]:
     """
-    Maps a distance image to depth image, also works with a list of images.
+    Maps a distance image to depth image, also works with a list of images or a 1-dim array of dist values.
 
     :param dist: The distance data.
+    :param points_2d: Can be used to specify the 2D points corresponding to the given distance values:
+                      Is necessary, if the given distance data is not a full distance image.
     :return: The depth data
     """
 
     dist = trim_redundant_channels(dist)
 
     if isinstance(dist, list) or hasattr(dist, "shape") and len(dist.shape) > 2:
         return [dist2depth(img) for img in dist]
 
     K = CameraUtility.get_intrinsics_as_K_matrix()
     f, cx, cy = K[0, 0], K[0, 2], K[1, 2]
 
-    xs, ys = np.meshgrid(np.arange(dist.shape[1]), np.arange(dist.shape[0]))
+    if points_2d is None:
+        xs, ys = np.meshgrid(np.arange(dist.shape[1]), np.arange(dist.shape[0]))
+    else:
+        xs, ys = points_2d[:, 0], points_2d[:, 1]
 
     # coordinate distances to principal point
     x_opt = np.abs(xs - cx)
     y_opt = np.abs(ys - cy)
 
     # Solve 3 equations in Wolfram Alpha:
     # Solve[{X == (x-c0)/f0*Z, Y == (y-c1)/f0*Z, X*X + Y*Y + Z*Z = d*d}, {X,Y,Z}]
```

### Comparing `blenderproc-2.7.0/blenderproc/python/postprocessing/StereoGlobalMatching.py` & `blenderproc-2.7.1/blenderproc/python/postprocessing/StereoGlobalMatching.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/renderer/FlowRendererUtility.py` & `blenderproc-2.7.1/blenderproc/python/renderer/FlowRendererUtility.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/renderer/NOCSRendererUtility.py` & `blenderproc-2.7.1/blenderproc/python/renderer/NOCSRendererUtility.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/renderer/RendererUtility.py` & `blenderproc-2.7.1/blenderproc/python/renderer/RendererUtility.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/renderer/SegMapRendererUtility.py` & `blenderproc-2.7.1/blenderproc/python/renderer/SegMapRendererUtility.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/sampler/Disk.py` & `blenderproc-2.7.1/blenderproc/python/sampler/Disk.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/sampler/Front3DPointInRoomSampler.py` & `blenderproc-2.7.1/blenderproc/python/sampler/Front3DPointInRoomSampler.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/sampler/PartSphere.py` & `blenderproc-2.7.1/blenderproc/python/sampler/PartSphere.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/sampler/RandomWalk.py` & `blenderproc-2.7.1/blenderproc/python/sampler/RandomWalk.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/sampler/ReplicaPointInRoomSampler.py` & `blenderproc-2.7.1/blenderproc/python/sampler/ReplicaPointInRoomSampler.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/sampler/Shell.py` & `blenderproc-2.7.1/blenderproc/python/sampler/Shell.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/sampler/Sphere.py` & `blenderproc-2.7.1/blenderproc/python/sampler/Sphere.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/sampler/SuncgPointInRoomSampler.py` & `blenderproc-2.7.1/blenderproc/python/sampler/SuncgPointInRoomSampler.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/sampler/UniformSO3.py` & `blenderproc-2.7.1/blenderproc/python/sampler/UniformSO3.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/sampler/UpperRegionSampler.py` & `blenderproc-2.7.1/blenderproc/python/sampler/UpperRegionSampler.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/tests/SilentMode.py` & `blenderproc-2.7.1/blenderproc/python/tests/SilentMode.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/tests/TestsPathManager.py` & `blenderproc-2.7.1/blenderproc/python/tests/TestsPathManager.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/types/ArmatureUtility.py` & `blenderproc-2.7.1/blenderproc/python/types/ArmatureUtility.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/types/BoneUtility.py` & `blenderproc-2.7.1/blenderproc/python/types/BoneUtility.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/types/EntityUtility.py` & `blenderproc-2.7.1/blenderproc/python/types/EntityUtility.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
 
         duplicate_obj = convert_to_entity_subclass(new_entity)
         if type(duplicate_obj) != type(self):
             warnings.warn(f"Duplication is only partly supported for {type(self)}")
 
         if duplicate_children:
             for child in self.get_children():
-                duplicate_child = child.duplicate(duplicate_children=duplicate_children)
+                duplicate_child = child.duplicate(duplicate_children=duplicate_children, linked=linked)
                 duplicate_child.set_parent(duplicate_obj)
 
                 duplicate_child.blender_obj.matrix_basis = child.blender_obj.matrix_basis.copy()
                 duplicate_child.blender_obj.matrix_parent_inverse = child.blender_obj.matrix_parent_inverse.copy()
 
         return duplicate_obj
```

### Comparing `blenderproc-2.7.0/blenderproc/python/types/InertialUtility.py` & `blenderproc-2.7.1/blenderproc/python/types/InertialUtility.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/types/LightUtility.py` & `blenderproc-2.7.1/blenderproc/python/types/LightUtility.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/types/LinkUtility.py` & `blenderproc-2.7.1/blenderproc/python/types/LinkUtility.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/types/MaterialUtility.py` & `blenderproc-2.7.1/blenderproc/python/types/MaterialUtility.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/types/MeshObjectUtility.py` & `blenderproc-2.7.1/blenderproc/python/types/MeshObjectUtility.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/types/StructUtility.py` & `blenderproc-2.7.1/blenderproc/python/types/StructUtility.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/types/StructUtilityFunctions.py` & `blenderproc-2.7.1/blenderproc/python/types/StructUtilityFunctions.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/types/URDFUtility.py` & `blenderproc-2.7.1/blenderproc/python/types/URDFUtility.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/utility/BlenderUtility.py` & `blenderproc-2.7.1/blenderproc/python/utility/BlenderUtility.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/utility/CollisionUtility.py` & `blenderproc-2.7.1/blenderproc/python/utility/CollisionUtility.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/utility/DefaultConfig.py` & `blenderproc-2.7.1/blenderproc/python/utility/DefaultConfig.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/utility/GlobalStorage.py` & `blenderproc-2.7.1/blenderproc/python/utility/GlobalStorage.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/utility/Initializer.py` & `blenderproc-2.7.1/blenderproc/python/utility/Initializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,9 +158,9 @@
                             and block.name == "Camera":
                         continue
                     data_structure.remove(block)
 
     @staticmethod
     def remove_custom_properties():
         """ Remove all custom properties registered at global entities like the scene. """
-        for key in bpy.context.scene.keys():
+        for key in list(bpy.context.scene.keys()):
             del bpy.context.scene[key]
```

### Comparing `blenderproc-2.7.0/blenderproc/python/utility/InstallUtility.py` & `blenderproc-2.7.1/blenderproc/python/utility/InstallUtility.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/utility/LabelIdMapping.py` & `blenderproc-2.7.1/blenderproc/python/utility/LabelIdMapping.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/utility/MaterialGetter.py` & `blenderproc-2.7.1/blenderproc/python/utility/MaterialGetter.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/utility/MathUtility.py` & `blenderproc-2.7.1/blenderproc/python/utility/MathUtility.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/utility/PatternUtility.py` & `blenderproc-2.7.1/blenderproc/python/utility/PatternUtility.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/utility/SetupUtility.py` & `blenderproc-2.7.1/blenderproc/python/utility/SetupUtility.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/utility/Utility.py` & `blenderproc-2.7.1/blenderproc/python/utility/Utility.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/writer/BopWriterUtility.py` & `blenderproc-2.7.1/blenderproc/python/writer/BopWriterUtility.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         os.makedirs(chunks_dir)
     elif not append_to_existing_output:
         raise FileExistsError(f"The output folder already exists: {dataset_dir}")
 
     # Select target objects or objects from the specified dataset or all objects
     if target_objects is not None:
         dataset_objects = target_objects
-        for obj in get_all_mesh_objects():
+        for obj in dataset_objects:
             if obj.is_hidden():
                 print(f"WARNING: The given object {obj.get_name()} is hidden. However, the bop writer will still add "
                       "coco annotations for it. If this is not desired, don't pass the object to the bop writer.")
     elif dataset:
         dataset_objects = []
         for obj in get_all_mesh_objects():
             if "bop_dataset_name" in obj.blender_obj and not obj.is_hidden():
@@ -175,14 +175,18 @@
                                         annotation_scale=annotation_scale, delta=delta, pool=pool)
          
         _BopWriterUtility.calc_gt_info(chunk_dirs=chunk_dirs, starting_frame_id=starting_frame_id,
                                        annotation_scale=annotation_scale, delta=delta, pool=pool)
 
         _BopWriterUtility.calc_gt_coco(chunk_dirs=chunk_dirs, dataset_objects=dataset_objects,
                                        starting_frame_id=starting_frame_id)
+        
+        pool.close()
+        pool.join()
+
 
 
 def bop_pose_to_pyrender_coordinate_system(cam_R_m2c: np.ndarray, cam_t_m2c: np.ndarray) -> np.ndarray:
     """ Converts an object pose in bop format to pyrender camera coordinate system
         (https://pyrender.readthedocs.io/en/latest/examples/cameras.html).
 
     :param cam_R_m2c: 3x3 Rotation matrix.
```

### Comparing `blenderproc-2.7.0/blenderproc/python/writer/CocoWriterUtility.py` & `blenderproc-2.7.1/blenderproc/python/writer/CocoWriterUtility.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/python/writer/GifWriterUtility.py` & `blenderproc-2.7.1/blenderproc/python/writer/GifWriterUtility.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Dict, List, Union
 import os
 
 import bpy
 import numpy as np
 from PIL import Image
 
-from blenderproc.scripts.visHdf5Files import vis_data
+#from blenderproc.scripts.visHdf5Files import vis_data
 from blenderproc.python.utility.Utility import Utility
 
 
 def write_gif_animation(
         output_dir_path: str,
         output_data_dict: Dict[str, List[Union[np.ndarray, list, dict]]],
         append_to_existing_output: bool = False,
```

### Comparing `blenderproc-2.7.0/blenderproc/python/writer/WriterUtility.py` & `blenderproc-2.7.1/blenderproc/python/writer/WriterUtility.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/resources/front_3D/3D_front_mapping.csv` & `blenderproc-2.7.1/blenderproc/resources/front_3D/3D_front_mapping.csv`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/resources/front_3D/3D_front_nyu_mapping.csv` & `blenderproc-2.7.1/blenderproc/resources/front_3D/3D_front_nyu_mapping.csv`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/resources/front_3D/find_all_front_3D_labels.py` & `blenderproc-2.7.1/blenderproc/resources/front_3D/find_all_front_3D_labels.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/resources/suncg/Better_labeling_for_NYU.csv` & `blenderproc-2.7.1/blenderproc/resources/suncg/Better_labeling_for_NYU.csv`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/resources/suncg/ModelCategoryMapping.csv` & `blenderproc-2.7.1/blenderproc/resources/suncg/ModelCategoryMapping.csv`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/resources/suncg/light_geometry_compact.txt` & `blenderproc-2.7.1/blenderproc/resources/suncg/light_geometry_compact.txt`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/scripts/download_blenderkit.py` & `blenderproc-2.7.1/blenderproc/scripts/download_blenderkit.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/scripts/download_cc_textures.py` & `blenderproc-2.7.1/blenderproc/scripts/download_cc_textures.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/scripts/download_haven.py` & `blenderproc-2.7.1/blenderproc/scripts/download_haven.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/scripts/download_ikea.py` & `blenderproc-2.7.1/blenderproc/scripts/download_ikea.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/scripts/download_matterport3d.py` & `blenderproc-2.7.1/blenderproc/scripts/download_matterport3d.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/scripts/download_pix3d.py` & `blenderproc-2.7.1/blenderproc/scripts/download_pix3d.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/scripts/download_scenenet.py` & `blenderproc-2.7.1/blenderproc/scripts/download_scenenet.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/scripts/quickstart.py` & `blenderproc-2.7.1/blenderproc/scripts/quickstart.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/scripts/saveAsImg.py` & `blenderproc-2.7.1/blenderproc/scripts/saveAsImg.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/scripts/visHdf5Files.py` & `blenderproc-2.7.1/blenderproc/scripts/visHdf5Files.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc/scripts/vis_coco_annotation.py` & `blenderproc-2.7.1/blenderproc/scripts/vis_coco_annotation.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/blenderproc.egg-info/PKG-INFO` & `blenderproc-2.7.1/blenderproc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blenderproc
-Version: 2.7.0
+Version: 2.7.1
 Home-page: https://github.com/DLR-RM/BlenderProc
 Author: Maximilian Denninger, Dominik Winkelbauer, Martin Sundermeyer
 Maintainer: Dominik Winkelbauer
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BlenderProc2
```

### Comparing `blenderproc-2.7.0/blenderproc.egg-info/SOURCES.txt` & `blenderproc-2.7.1/blenderproc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/setup.py` & `blenderproc-2.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/tests/testCamera.py` & `blenderproc-2.7.1/tests/testCamera.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/tests/testCameraProjection.py` & `blenderproc-2.7.1/tests/testCameraProjection.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,14 +29,40 @@
         y = np.arange(480)   
         x = np.arange(640)
         pixels_gt = np.stack(np.meshgrid(x, y), -1).astype(np.float32)
         pixels_gt[np.isnan(pixels[..., 0])] = np.nan
 
         np.testing.assert_almost_equal(pixels, pixels_gt, decimal=3)
 
+
+    def test_depth_at_points_via_raytracing(self):
+        """ Test if depth_at_points_via_raytracing leads to the same results as depth_via_raytracing + unproject + project
+        """
+        bproc.clean_up(True)
+        resource_folder = os.path.join("examples", "resources")
+        objs = bproc.loader.load_obj(os.path.join(resource_folder, "scene.obj"))
+
+        cam2world_matrix = np.array([[1.0, 0.0, 0.0, 0.0], [0.0, 0.2674988806247711, -0.9635581970214844, -13.741], [-0.0, 0.9635581970214844, 0.2674988806247711, 4.1242], [0.0, 0.0, 0.0, 1.0]])
+        bproc.camera.add_camera_pose(cam2world_matrix)
+        bproc.camera.set_resolution(640, 480)
+
+        bvh_tree = bproc.object.create_bvh_tree_multi_objects(objs)
+
+        depth = bproc.camera.depth_via_raytracing(bvh_tree)
+        pc = bproc.camera.pointcloud_from_depth(depth)
+        pixels = bproc.camera.project_points(pc.reshape(-1, 3))
+        
+        depth2 = bproc.camera.depth_at_points_via_raytracing(bvh_tree, pixels)
+        depth2[np.isnan(depth2)] = np.inf
+        pc2 = bproc.camera.unproject_points(pixels, depth2)
+
+        np.testing.assert_almost_equal(depth.flatten(), depth2, decimal=3)
+        np.testing.assert_almost_equal(pc.reshape(-1, 3), pc2, decimal=3)
+
+
     def test_depth_via_raytracing(self):
         """ Tests if depth image via raytracing and rendered depth image are identical.
         """
         bproc.clean_up(True)
         resource_folder = os.path.join("examples", "resources")
         objs = bproc.loader.load_obj(os.path.join(resource_folder, "scene.obj"))
 
@@ -55,15 +81,14 @@
         depth = bproc.camera.depth_via_raytracing(bvh_tree)
 
         bproc.renderer.enable_depth_output(activate_antialiasing=False)
         data = bproc.renderer.render()      
         data["depth"][0][data["depth"][0] >= 65504] = np.inf
 
         diff = np.abs(depth[~np.isinf(depth)] - data["depth"][0][~np.isinf(depth)])
-        
         self.assertTrue(np.median(diff) < 1e-4)
         self.assertTrue((diff < 1e-4).mean() > 0.99)
 
 if __name__ == '__main__':
     bproc.init()
     #test = UnitTestCheckCameraProjection()
     #test.test_depth_via_raytracing()
```

### Comparing `blenderproc-2.7.0/tests/testEntity.py` & `blenderproc-2.7.1/tests/testEntity.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/tests/testHavenLoader.py` & `blenderproc-2.7.1/tests/testHavenLoader.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/tests/testLoader.py` & `blenderproc-2.7.1/tests/testLoader.py`

 * *Files identical despite different names*

### Comparing `blenderproc-2.7.0/tests/testUtility.py` & `blenderproc-2.7.1/tests/testUtility.py`

 * *Files identical despite different names*

