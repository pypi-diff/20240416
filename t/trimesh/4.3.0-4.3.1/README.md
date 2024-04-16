# Comparing `tmp/trimesh-4.3.0.tar.gz` & `tmp/trimesh-4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trimesh-4.3.0.tar", last modified: Tue Apr  9 18:10:18 2024, max compression
+gzip compressed data, was "trimesh-4.3.1.tar", last modified: Tue Apr 16 18:43:46 2024, max compression
```

## Comparing `trimesh-4.3.0.tar` & `trimesh-4.3.1.tar`

### file list

```diff
@@ -1,264 +1,265 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:18.148617 trimesh-4.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-09 18:10:07.000000 trimesh-4.3.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    18182 2024-04-09 18:10:18.148617 trimesh-4.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14071 2024-04-09 18:10:07.000000 trimesh-4.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-09 18:10:07.000000 trimesh-4.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 18:10:18.148617 trimesh-4.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:18.120616 trimesh-4.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_3dxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_3mf.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_adjacency.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_align.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_arc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_binvox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_boolean.py
--rw-r--r--   0 runner    (1001) docker     (127)    12174 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)    11564 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_collision.py
--rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_convex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_crash.py
--rw-r--r--   0 runner    (1001) docker     (127)    12266 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_curvature.py
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_dae.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     7979 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_dxf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_edges.py
--rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_except.py
--rw-r--r--   0 runner    (1001) docker     (127)    12468 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_extrude.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_facets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_fill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_geom.py
--rw-r--r--   0 runner    (1001) docker     (127)    41146 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_gltf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_gmsh.py
--rw-r--r--   0 runner    (1001) docker     (127)    10564 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    11551 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_html.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_identifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)    16218 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_inertia.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_integralmeancurvature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_interval.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_light.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_loaded.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_medial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_minimal.py
--rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_mutate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_normals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_nsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    19037 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_obj.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_packing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_path_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_pathlib.py
--rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_pbr.py
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_permutate.py
--rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_ply.py
--rw-r--r--   0 runner    (1001) docker     (127)    11077 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_points.py
--rw-r--r--   0 runner    (1001) docker     (127)    10397 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_polygons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_poses.py
--rw-r--r--   0 runner    (1001) docker     (127)    13601 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)     9492 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_proximity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_raster.py
--rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_ray.py
--rw-r--r--   0 runner    (1001) docker     (127)    15254 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)    10463 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_remesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_render.py
--rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_repair.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_repr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_resolvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8302 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_runlength.py
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    17970 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_scene.py
--rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_scenegraph.py
--rw-r--r--   0 runner    (1001) docker     (127)    18035 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_section.py
--rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_segments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_smooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_splines.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_stl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_svg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_sweep.py
--rw-r--r--   0 runner    (1001) docker     (127)     8647 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_texture.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_thickness.py
--rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_trackball.py
--rw-r--r--   0 runner    (1001) docker     (127)     9163 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_transformations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_triangles.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_typed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_units.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_unwrap.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_upstream.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_urdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    18466 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_vertices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_visual.py
--rw-r--r--   0 runner    (1001) docker     (127)    14542 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_voxel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:18.128616 trimesh-4.3.0/trimesh/
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   102604 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/boolean.py
--rw-r--r--   0 runner    (1001) docker     (127)    20795 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)    20087 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)    22582 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/collision.py
--rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/convex.py
--rw-r--r--   0 runner    (1001) docker     (127)    45776 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/curvature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:18.132617 trimesh-4.3.0/trimesh/exchange/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/exchange/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17608 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/exchange/binvox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/exchange/cascade.py
--rw-r--r--   0 runner    (1001) docker     (127)    14673 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/exchange/dae.py
--rw-r--r--   0 runner    (1001) docker     (127)    10480 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/exchange/export.py
--rw-r--r--   0 runner    (1001) docker     (127)    68462 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/exchange/gltf.py
--rw-r--r--   0 runner    (1001) docker     (127)    21659 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/exchange/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/exchange/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    34419 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/exchange/obj.py
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/exchange/off.py
--rw-r--r--   0 runner    (1001) docker     (127)    33004 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/exchange/ply.py
--rw-r--r--   0 runner    (1001) docker     (127)    10151 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/exchange/stl.py
--rw-r--r--   0 runner    (1001) docker     (127)    15866 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/exchange/threedxml.py
--rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/exchange/threemf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/exchange/urdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/exchange/xaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/exchange/xyz.py
--rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)    30523 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    26162 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)     8225 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/inertia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:18.132617 trimesh-4.3.0/trimesh/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/interfaces/blender.py
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/interfaces/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     9006 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/interfaces/gmsh.py
--rw-r--r--   0 runner    (1001) docker     (127)    28268 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/intersections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/interval.py
--rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/nsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     9903 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/parent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:18.136617 trimesh-4.3.0/trimesh/path/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/arc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/curve.py
--rw-r--r--   0 runner    (1001) docker     (127)    21244 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/entities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:18.136617 trimesh-4.3.0/trimesh/path/exchange/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/exchange/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33119 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/exchange/dxf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/exchange/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/exchange/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/exchange/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    23095 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/exchange/svg_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/intersections.py
--rw-r--r--   0 runner    (1001) docker     (127)    26100 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/packing.py
--rw-r--r--   0 runner    (1001) docker     (127)    43902 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/path.py
--rw-r--r--   0 runner    (1001) docker     (127)    31112 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/polygons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/raster.py
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/repair.py
--rw-r--r--   0 runner    (1001) docker     (127)    16350 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/segments.py
--rw-r--r--   0 runner    (1001) docker     (127)    12549 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/simplify.py
--rw-r--r--   0 runner    (1001) docker     (127)    14267 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/traversal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/permutate.py
--rw-r--r--   0 runner    (1001) docker     (127)    19968 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/points.py
--rw-r--r--   0 runner    (1001) docker     (127)    10267 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/poses.py
--rw-r--r--   0 runner    (1001) docker     (127)    33332 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)    19114 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/proximity.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:18.136617 trimesh-4.3.0/trimesh/ray/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/ray/ray_pyembree.py
--rw-r--r--   0 runner    (1001) docker     (127)    12741 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/ray/ray_triangle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/ray/ray_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    40188 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14936 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/remesh.py
--rw-r--r--   0 runner    (1001) docker     (127)    12194 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/rendering.py
--rw-r--r--   0 runner    (1001) docker     (127)    15055 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/repair.py
--rw-r--r--   0 runner    (1001) docker     (127)    15386 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resolvers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:18.136617 trimesh-4.3.0/trimesh/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/creation.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:18.140617 trimesh-4.3.0/trimesh/resources/schema/
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/schema/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    24785 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/schema/gltf2.schema.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:18.140617 trimesh-4.3.0/trimesh/resources/schema/primitive/
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/schema/primitive/box.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/schema/primitive/capsule.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/schema/primitive/cylinder.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/schema/primitive/extrusion.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/schema/primitive/primitive.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/schema/primitive/scenegraph.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/schema/primitive/sphere.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/schema/primitive/transform.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/schema/primitive/trimesh.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/schema/primitive/wkt.polygon.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/schema/urdf.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:18.140617 trimesh-4.3.0/trimesh/resources/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/templates/base.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/templates/blender_boolean.py.tmpl
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/templates/blender_unwrap.py.template
--rw-r--r--   0 runner    (1001) docker     (127)    15667 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/templates/dxf.json
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/templates/path.svg
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/templates/ply.json
--rw-r--r--   0 runner    (1001) docker     (127)   167999 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/templates/viewer.zip
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/units_to_inches.json
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:18.144617 trimesh-4.3.0/trimesh/scene/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/scene/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12162 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/scene/cameras.py
--rw-r--r--   0 runner    (1001) docker     (127)     8471 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/scene/lighting.py
--rw-r--r--   0 runner    (1001) docker     (127)    48032 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/scene/scene.py
--rw-r--r--   0 runner    (1001) docker     (127)    27630 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/scene/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)    10954 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/smoothing.py
--rw-r--r--   0 runner    (1001) docker     (127)    74544 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/transformations.py
--rw-r--r--   0 runner    (1001) docker     (127)    21710 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/triangles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/typed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/units.py
--rw-r--r--   0 runner    (1001) docker     (127)    66709 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:18.144617 trimesh-4.3.0/trimesh/viewer/
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/viewer/notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/viewer/trackball.py
--rw-r--r--   0 runner    (1001) docker     (127)     9202 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/viewer/widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    30971 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/viewer/windowed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:18.144617 trimesh-4.3.0/trimesh/visual/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/visual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/visual/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    29109 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/visual/color.py
--rw-r--r--   0 runner    (1001) docker     (127)    15270 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/visual/gloss.py
--rw-r--r--   0 runner    (1001) docker     (127)    34678 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/visual/material.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/visual/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/visual/texture.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:18.144617 trimesh-4.3.0/trimesh/voxel/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/voxel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12572 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/voxel/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9364 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/voxel/creation.py
--rw-r--r--   0 runner    (1001) docker     (127)    27755 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/voxel/encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/voxel/morphology.py
--rw-r--r--   0 runner    (1001) docker     (127)    11761 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/voxel/ops.py
--rw-r--r--   0 runner    (1001) docker     (127)    20278 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/voxel/runlength.py
--rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/voxel/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:18.144617 trimesh-4.3.0/trimesh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18182 2024-04-09 18:10:18.000000 trimesh-4.3.0/trimesh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-04-09 18:10:18.000000 trimesh-4.3.0/trimesh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 18:10:18.000000 trimesh-4.3.0/trimesh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-09 18:10:18.000000 trimesh-4.3.0/trimesh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 18:10:18.000000 trimesh-4.3.0/trimesh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:46.437662 trimesh-4.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-16 18:43:30.000000 trimesh-4.3.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18182 2024-04-16 18:43:46.437662 trimesh-4.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14071 2024-04-16 18:43:30.000000 trimesh-4.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-16 18:43:30.000000 trimesh-4.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 18:43:46.437662 trimesh-4.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:46.405662 trimesh-4.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_3dxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_3mf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_adjacency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_align.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_arc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_binvox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_boolean.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12174 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11564 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_collision.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_convex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_crash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12266 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_curvature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_dae.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7979 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_dxf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_edges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_except.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12468 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_extrude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_facets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_fill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_geom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41146 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_gltf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_gmsh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10564 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11551 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16218 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_inertia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_integralmeancurvature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_medial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_minimal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_mutate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_normals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_nsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19037 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_obj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_packing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_path_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_path_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_pbr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_permutate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_ply.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11077 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10397 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_polygons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_poses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13601 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9492 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_proximity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_raster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_ray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15254 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10463 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_remesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_repair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8302 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_runlength.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17970 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_scene.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_scenegraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18035 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_section.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_segments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_splines.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_stl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_svg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8647 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_texture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_thickness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_trackball.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9163 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_triangles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_typed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_unwrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_upstream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_urdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18466 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_vertices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_visual.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14542 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_voxel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:46.417662 trimesh-4.3.1/trimesh/
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   102604 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20795 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20087 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22582 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/collision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/convex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45776 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/curvature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:46.417662 trimesh-4.3.1/trimesh/exchange/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/exchange/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17608 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/exchange/binvox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/exchange/cascade.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14673 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/exchange/dae.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10480 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/exchange/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68462 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/exchange/gltf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21659 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/exchange/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/exchange/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34419 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/exchange/obj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/exchange/off.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33004 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/exchange/ply.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10151 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/exchange/stl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15866 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/exchange/threedxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/exchange/threemf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/exchange/urdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/exchange/xaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/exchange/xyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30523 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26162 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8225 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/inertia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:46.417662 trimesh-4.3.1/trimesh/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/interfaces/blender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/interfaces/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9006 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/interfaces/gmsh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28268 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/intersections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/nsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9903 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/parent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:46.421662 trimesh-4.3.1/trimesh/path/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/arc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21244 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/entities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:46.421662 trimesh-4.3.1/trimesh/path/exchange/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/exchange/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33119 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/exchange/dxf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/exchange/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/exchange/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/exchange/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23095 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/exchange/svg_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/intersections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26100 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/packing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43902 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31112 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/polygons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/raster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/repair.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16350 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/segments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12549 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/simplify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16063 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/traversal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/permutate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19968 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/points.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10267 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/poses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33332 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19114 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/proximity.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:46.421662 trimesh-4.3.1/trimesh/ray/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/ray/ray_pyembree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12741 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/ray/ray_triangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/ray/ray_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40188 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14936 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/remesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12194 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/rendering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15055 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/repair.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15386 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resolvers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:46.425662 trimesh-4.3.1/trimesh/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/creation.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:46.425662 trimesh-4.3.1/trimesh/resources/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/schema/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    24785 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/schema/gltf2.schema.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:46.425662 trimesh-4.3.1/trimesh/resources/schema/primitive/
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/schema/primitive/box.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/schema/primitive/capsule.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/schema/primitive/cylinder.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/schema/primitive/extrusion.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/schema/primitive/primitive.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/schema/primitive/scenegraph.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/schema/primitive/sphere.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/schema/primitive/transform.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/schema/primitive/trimesh.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/schema/primitive/wkt.polygon.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/schema/urdf.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:46.425662 trimesh-4.3.1/trimesh/resources/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/templates/base.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/templates/blender_boolean.py.tmpl
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/templates/blender_unwrap.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)    15667 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/templates/dxf.json
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/templates/path.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/templates/ply.json
+-rw-r--r--   0 runner    (1001) docker     (127)   167999 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/templates/viewer.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/units_to_inches.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:46.433662 trimesh-4.3.1/trimesh/scene/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/scene/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12162 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/scene/cameras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8471 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/scene/lighting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48032 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/scene/scene.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27630 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/scene/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10954 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74544 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21710 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/triangles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/typed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66709 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:46.433662 trimesh-4.3.1/trimesh/viewer/
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/viewer/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/viewer/trackball.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9202 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/viewer/widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30971 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/viewer/windowed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:46.433662 trimesh-4.3.1/trimesh/visual/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/visual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/visual/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29109 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/visual/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15270 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/visual/gloss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34678 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/visual/material.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/visual/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/visual/texture.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:46.433662 trimesh-4.3.1/trimesh/voxel/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/voxel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12572 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/voxel/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9364 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/voxel/creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27755 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/voxel/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/voxel/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11761 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/voxel/ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20278 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/voxel/runlength.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/voxel/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:46.433662 trimesh-4.3.1/trimesh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18182 2024-04-16 18:43:46.000000 trimesh-4.3.1/trimesh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6131 2024-04-16 18:43:46.000000 trimesh-4.3.1/trimesh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 18:43:46.000000 trimesh-4.3.1/trimesh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-16 18:43:46.000000 trimesh-4.3.1/trimesh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-16 18:43:46.000000 trimesh-4.3.1/trimesh.egg-info/top_level.txt
```

### Comparing `trimesh-4.3.0/LICENSE.md` & `trimesh-4.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/PKG-INFO` & `trimesh-4.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trimesh
-Version: 4.3.0
+Version: 4.3.1
 Summary: Import, export, process, analyze and view triangular meshes.
 Author-email: Michael Dawson-Haggerty <mikedh@kerfed.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Michael Dawson-Haggerty
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `trimesh-4.3.0/README.md` & `trimesh-4.3.1/README.md`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/pyproject.toml` & `trimesh-4.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools >= 61.0", "wheel"]
 
 [project]
 name = "trimesh"
 requires-python = ">=3.7"
-version = "4.3.0"
+version = "4.3.1"
 authors = [{name = "Michael Dawson-Haggerty", email = "mikedh@kerfed.com"}]
 license = {file = "LICENSE.md"}
 description = "Import, export, process, analyze and view triangular meshes."
 keywords = ["graphics", "mesh", "geometry", "3D"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
```

### Comparing `trimesh-4.3.0/tests/test_3dxml.py` & `trimesh-4.3.1/tests/test_3dxml.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_3mf.py` & `trimesh-4.3.1/tests/test_3mf.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_adjacency.py` & `trimesh-4.3.1/tests/test_adjacency.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_align.py` & `trimesh-4.3.1/tests/test_align.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_arc.py` & `trimesh-4.3.1/tests/test_arc.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_base.py` & `trimesh-4.3.1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_binvox.py` & `trimesh-4.3.1/tests/test_binvox.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_boolean.py` & `trimesh-4.3.1/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_bounds.py` & `trimesh-4.3.1/tests/test_bounds.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_cache.py` & `trimesh-4.3.1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_camera.py` & `trimesh-4.3.1/tests/test_camera.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_collision.py` & `trimesh-4.3.1/tests/test_collision.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_color.py` & `trimesh-4.3.1/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_convex.py` & `trimesh-4.3.1/tests/test_convex.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_copy.py` & `trimesh-4.3.1/tests/test_copy.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_crash.py` & `trimesh-4.3.1/tests/test_crash.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_creation.py` & `trimesh-4.3.1/tests/test_creation.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_curvature.py` & `trimesh-4.3.1/tests/test_curvature.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_dae.py` & `trimesh-4.3.1/tests/test_dae.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_decomposition.py` & `trimesh-4.3.1/tests/test_decomposition.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_dxf.py` & `trimesh-4.3.1/tests/test_dxf.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_edges.py` & `trimesh-4.3.1/tests/test_edges.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_encoding.py` & `trimesh-4.3.1/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_except.py` & `trimesh-4.3.1/tests/test_except.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_export.py` & `trimesh-4.3.1/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_extrude.py` & `trimesh-4.3.1/tests/test_extrude.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_facets.py` & `trimesh-4.3.1/tests/test_facets.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_fill.py` & `trimesh-4.3.1/tests/test_fill.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_geom.py` & `trimesh-4.3.1/tests/test_geom.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_gltf.py` & `trimesh-4.3.1/tests/test_gltf.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_gmsh.py` & `trimesh-4.3.1/tests/test_gmsh.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_graph.py` & `trimesh-4.3.1/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_grouping.py` & `trimesh-4.3.1/tests/test_grouping.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_html.py` & `trimesh-4.3.1/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_identifier.py` & `trimesh-4.3.1/tests/test_identifier.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_import.py` & `trimesh-4.3.1/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_inertia.py` & `trimesh-4.3.1/tests/test_inertia.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_integralmeancurvature.py` & `trimesh-4.3.1/tests/test_integralmeancurvature.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_interval.py` & `trimesh-4.3.1/tests/test_interval.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_light.py` & `trimesh-4.3.1/tests/test_light.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_loaded.py` & `trimesh-4.3.1/tests/test_loaded.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_medial.py` & `trimesh-4.3.1/tests/test_medial.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_merge.py` & `trimesh-4.3.1/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_mesh.py` & `trimesh-4.3.1/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_meta.py` & `trimesh-4.3.1/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_minimal.py` & `trimesh-4.3.1/tests/test_minimal.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_mutate.py` & `trimesh-4.3.1/tests/test_mutate.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_normals.py` & `trimesh-4.3.1/tests/test_normals.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_nsphere.py` & `trimesh-4.3.1/tests/test_nsphere.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_obj.py` & `trimesh-4.3.1/tests/test_obj.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_off.py` & `trimesh-4.3.1/tests/test_off.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_operators.py` & `trimesh-4.3.1/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_packing.py` & `trimesh-4.3.1/tests/test_packing.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_path_creation.py` & `trimesh-4.3.1/tests/test_path_creation.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_pathlib.py` & `trimesh-4.3.1/tests/test_pathlib.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_paths.py` & `trimesh-4.3.1/tests/test_paths.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_pbr.py` & `trimesh-4.3.1/tests/test_pbr.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_permutate.py` & `trimesh-4.3.1/tests/test_permutate.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_ply.py` & `trimesh-4.3.1/tests/test_ply.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_points.py` & `trimesh-4.3.1/tests/test_points.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_polygons.py` & `trimesh-4.3.1/tests/test_polygons.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_poses.py` & `trimesh-4.3.1/tests/test_poses.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_primitives.py` & `trimesh-4.3.1/tests/test_primitives.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_proximity.py` & `trimesh-4.3.1/tests/test_proximity.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_raster.py` & `trimesh-4.3.1/tests/test_raster.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_ray.py` & `trimesh-4.3.1/tests/test_ray.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_registration.py` & `trimesh-4.3.1/tests/test_registration.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_remesh.py` & `trimesh-4.3.1/tests/test_remesh.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_render.py` & `trimesh-4.3.1/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_repair.py` & `trimesh-4.3.1/tests/test_repair.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_repr.py` & `trimesh-4.3.1/tests/test_repr.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_resolvers.py` & `trimesh-4.3.1/tests/test_resolvers.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_runlength.py` & `trimesh-4.3.1/tests/test_runlength.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_sample.py` & `trimesh-4.3.1/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_scene.py` & `trimesh-4.3.1/tests/test_scene.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_scenegraph.py` & `trimesh-4.3.1/tests/test_scenegraph.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_section.py` & `trimesh-4.3.1/tests/test_section.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_segments.py` & `trimesh-4.3.1/tests/test_segments.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_simplify.py` & `trimesh-4.3.1/tests/test_simplify.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_smooth.py` & `trimesh-4.3.1/tests/test_smooth.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_smoothing.py` & `trimesh-4.3.1/tests/test_smoothing.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_splines.py` & `trimesh-4.3.1/tests/test_splines.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_step.py` & `trimesh-4.3.1/tests/test_step.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_stl.py` & `trimesh-4.3.1/tests/test_stl.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_svg.py` & `trimesh-4.3.1/tests/test_svg.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_sweep.py` & `trimesh-4.3.1/tests/test_sweep.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_texture.py` & `trimesh-4.3.1/tests/test_texture.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_thickness.py` & `trimesh-4.3.1/tests/test_thickness.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_trackball.py` & `trimesh-4.3.1/tests/test_trackball.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_transformations.py` & `trimesh-4.3.1/tests/test_transformations.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_triangles.py` & `trimesh-4.3.1/tests/test_triangles.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_units.py` & `trimesh-4.3.1/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_unwrap.py` & `trimesh-4.3.1/tests/test_unwrap.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_upstream.py` & `trimesh-4.3.1/tests/test_upstream.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_urdf.py` & `trimesh-4.3.1/tests/test_urdf.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_util.py` & `trimesh-4.3.1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_vector.py` & `trimesh-4.3.1/tests/test_vector.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_vertices.py` & `trimesh-4.3.1/tests/test_vertices.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_viewer.py` & `trimesh-4.3.1/tests/test_viewer.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_visual.py` & `trimesh-4.3.1/tests/test_visual.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/tests/test_voxel.py` & `trimesh-4.3.1/tests/test_voxel.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/__init__.py` & `trimesh-4.3.1/trimesh/__init__.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/base.py` & `trimesh-4.3.1/trimesh/base.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/boolean.py` & `trimesh-4.3.1/trimesh/boolean.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/bounds.py` & `trimesh-4.3.1/trimesh/bounds.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/caching.py` & `trimesh-4.3.1/trimesh/caching.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/collision.py` & `trimesh-4.3.1/trimesh/collision.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/comparison.py` & `trimesh-4.3.1/trimesh/comparison.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/constants.py` & `trimesh-4.3.1/trimesh/constants.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/convex.py` & `trimesh-4.3.1/trimesh/convex.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/creation.py` & `trimesh-4.3.1/trimesh/creation.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/curvature.py` & `trimesh-4.3.1/trimesh/curvature.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/decomposition.py` & `trimesh-4.3.1/trimesh/decomposition.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/exceptions.py` & `trimesh-4.3.1/trimesh/exceptions.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/exchange/binvox.py` & `trimesh-4.3.1/trimesh/exchange/binvox.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/exchange/cascade.py` & `trimesh-4.3.1/trimesh/exchange/cascade.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/exchange/dae.py` & `trimesh-4.3.1/trimesh/exchange/dae.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/exchange/export.py` & `trimesh-4.3.1/trimesh/exchange/export.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/exchange/gltf.py` & `trimesh-4.3.1/trimesh/exchange/gltf.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/exchange/load.py` & `trimesh-4.3.1/trimesh/exchange/load.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/exchange/misc.py` & `trimesh-4.3.1/trimesh/exchange/misc.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/exchange/obj.py` & `trimesh-4.3.1/trimesh/exchange/obj.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/exchange/off.py` & `trimesh-4.3.1/trimesh/exchange/off.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/exchange/ply.py` & `trimesh-4.3.1/trimesh/exchange/ply.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/exchange/stl.py` & `trimesh-4.3.1/trimesh/exchange/stl.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/exchange/threedxml.py` & `trimesh-4.3.1/trimesh/exchange/threedxml.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/exchange/threemf.py` & `trimesh-4.3.1/trimesh/exchange/threemf.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/exchange/urdf.py` & `trimesh-4.3.1/trimesh/exchange/urdf.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/exchange/xaml.py` & `trimesh-4.3.1/trimesh/exchange/xaml.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/exchange/xyz.py` & `trimesh-4.3.1/trimesh/exchange/xyz.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/geometry.py` & `trimesh-4.3.1/trimesh/geometry.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/graph.py` & `trimesh-4.3.1/trimesh/graph.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/grouping.py` & `trimesh-4.3.1/trimesh/grouping.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/inertia.py` & `trimesh-4.3.1/trimesh/inertia.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/interfaces/blender.py` & `trimesh-4.3.1/trimesh/interfaces/blender.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/interfaces/generic.py` & `trimesh-4.3.1/trimesh/interfaces/generic.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/interfaces/gmsh.py` & `trimesh-4.3.1/trimesh/interfaces/gmsh.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/intersections.py` & `trimesh-4.3.1/trimesh/intersections.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/interval.py` & `trimesh-4.3.1/trimesh/interval.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/nsphere.py` & `trimesh-4.3.1/trimesh/nsphere.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/parent.py` & `trimesh-4.3.1/trimesh/parent.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/path/arc.py` & `trimesh-4.3.1/trimesh/path/arc.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/path/creation.py` & `trimesh-4.3.1/trimesh/path/creation.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/path/curve.py` & `trimesh-4.3.1/trimesh/path/curve.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/path/entities.py` & `trimesh-4.3.1/trimesh/path/entities.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/path/exchange/dxf.py` & `trimesh-4.3.1/trimesh/path/exchange/dxf.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/path/exchange/export.py` & `trimesh-4.3.1/trimesh/path/exchange/export.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/path/exchange/load.py` & `trimesh-4.3.1/trimesh/path/exchange/load.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/path/exchange/misc.py` & `trimesh-4.3.1/trimesh/path/exchange/misc.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/path/exchange/svg_io.py` & `trimesh-4.3.1/trimesh/path/exchange/svg_io.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/path/intersections.py` & `trimesh-4.3.1/trimesh/path/intersections.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/path/packing.py` & `trimesh-4.3.1/trimesh/path/packing.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/path/path.py` & `trimesh-4.3.1/trimesh/path/path.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/path/polygons.py` & `trimesh-4.3.1/trimesh/path/polygons.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/path/raster.py` & `trimesh-4.3.1/trimesh/path/raster.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/path/repair.py` & `trimesh-4.3.1/trimesh/path/repair.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/path/segments.py` & `trimesh-4.3.1/trimesh/path/segments.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/path/simplify.py` & `trimesh-4.3.1/trimesh/path/simplify.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/path/traversal.py` & `trimesh-4.3.1/trimesh/path/traversal.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import copy
 
 import numpy as np
 
 from .. import constants, grouping, util
+from ..typed import ArrayLike, Integer, NDArray, Number, Optional
 from .util import is_ccw
 
 try:
     import networkx as nx
 except BaseException as E:
     # create a dummy module which will raise the ImportError
     # or other exception only when someone tries to use networkx
@@ -242,15 +243,15 @@
         # reversing will make array non c- contiguous
         discrete = np.ascontiguousarray(discrete[::-1])
 
     return discrete
 
 
 class PathSample:
-    def __init__(self, points):
+    def __init__(self, points: ArrayLike):
         # make sure input array is numpy
         self._points = np.array(points)
         # find the direction of each segment
         self._vectors = np.diff(self._points, axis=0)
         # find the length of each segment
         self._norms = util.row_norm(self._vectors)
         # unit vectors for each segment
@@ -259,35 +260,76 @@
         self._unit_vec[nonzero] /= self._norms[nonzero].reshape((-1, 1))
         # total distance in the path
         self.length = self._norms.sum()
         # cumulative sum of section length
         # note that this is sorted
         self._cum_norm = np.cumsum(self._norms)
 
-    def sample(self, distances):
+    def sample(
+        self, distances: ArrayLike, include_original: bool = False
+    ) -> NDArray[np.float64]:
+        """
+        Return points at the distances along the path requested.
+
+        Parameters
+        ----------
+        distances
+          Distances along the path to sample at.
+        include_original
+          Include the original vertices even if they are not
+          specified in `distance`. Useful as this will return
+          a result with identical area and length, however
+          indexes of `distance` will not correspond with result.
+
+        Returns
+        --------
+        samples : (n, dimension)
+          Samples requested.
+          `n==len(distances)` if not `include_original`
+        """
         # return the indices in cum_norm that each sample would
         # need to be inserted at to maintain the sorted property
         positions = np.searchsorted(self._cum_norm, distances)
         positions = np.clip(positions, 0, len(self._unit_vec) - 1)
         offsets = np.append(0, self._cum_norm)[positions]
         # the distance past the reference vertex we need to travel
         projection = distances - offsets
         # find out which direction we need to project
         direction = self._unit_vec[positions]
         # find out which vertex we're offset from
         origin = self._points[positions]
+
         # just the parametric equation for a line
         resampled = origin + (direction * projection.reshape((-1, 1)))
 
+        if include_original:
+            # find the insertion index of the original positions
+            unique, index = np.unique(positions, return_index=True)
+            # see if we already have this point
+            ok = projection[index] > 1e-12
+
+            # insert the original vertices into the resampled array
+            resampled = np.insert(resampled, index[ok], self._points[unique[ok]], axis=0)
+
         return resampled
 
-    def truncate(self, distance):
+    def truncate(self, distance: Number) -> NDArray[np.float64]:
         """
         Return a truncated version of the path.
         Only one vertex (at the endpoint) will be added.
+
+        Parameters
+        ----------
+        distance
+          Distance along the path to truncate at.
+
+        Returns
+        ----------
+        path
+          Path clipped to `distance` requested.
         """
         position = np.searchsorted(self._cum_norm, distance)
         offset = distance - self._cum_norm[position - 1]
 
         if offset < constants.tol_path.merge:
             truncated = self._points[: position + 1]
         else:
@@ -300,15 +342,21 @@
         assert (
             util.row_norm(np.diff(truncated, axis=0)).sum() - distance
         ) < constants.tol_path.merge
 
         return truncated
 
 
-def resample_path(points, count=None, step=None, step_round=True):
+def resample_path(
+    points: ArrayLike,
+    count: Optional[Integer] = None,
+    step: Optional[Number] = None,
+    step_round: bool = True,
+    include_original: bool = False,
+) -> NDArray[np.float64]:
     """
     Given a path along (n,d) points, resample them such that the
     distance traversed along the path is constant in between each
     of the resampled points. Note that this can produce clipping at
     corners, as the original vertices are NOT guaranteed to be in the
     new, resampled path.
 
@@ -316,26 +364,29 @@
     Result can be uniformly distributed (np.linspace) by specifying count
     Result can have a specific distance (np.arange) by specifying step
 
 
     Parameters
     ----------
     points:   (n, d) float
-        Points in space
+      Points in space
     count : int,
-        Number of points to sample evenly (aka np.linspace)
+      Number of points to sample evenly (aka np.linspace)
     step : float
-        Distance each step should take along the path (aka np.arange)
+      Distance each step should take along the path (aka np.arange)
+    step_round
+      Alter `step` to the nearest integer division of overall length.
+    include_original
+      Include the exact original points in the output.
 
     Returns
     ----------
     resampled : (j,d) float
         Points on the path
     """
-
     points = np.array(points, dtype=np.float64)
     # generate samples along the perimeter from kwarg count or step
     if (count is not None) and (step is not None):
         raise ValueError("Only step OR count can be specified")
     if (count is None) and (step is None):
         raise ValueError("Either step or count must be specified")
 
@@ -347,20 +398,21 @@
         count = int(np.ceil(sampler.length / step))
 
     if count is not None:
         samples = np.linspace(0, sampler.length, count)
     elif step is not None:
         samples = np.arange(0, sampler.length, step)
 
-    resampled = sampler.sample(samples)
+    resampled = sampler.sample(samples, include_original=include_original)
 
-    check = util.row_norm(points[[0, -1]] - resampled[[0, -1]])
-    assert check[0] < constants.tol_path.merge
-    if count is not None:
-        assert check[1] < constants.tol_path.merge
+    if constants.tol.strict:
+        check = util.row_norm(points[[0, -1]] - resampled[[0, -1]])
+        assert check[0] < constants.tol_path.merge
+        if count is not None:
+            assert check[1] < constants.tol_path.merge
 
     return resampled
 
 
 def split(path):
     """
     Split a Path2D into multiple Path2D objects where each
```

### Comparing `trimesh-4.3.0/trimesh/path/util.py` & `trimesh-4.3.1/trimesh/path/util.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/permutate.py` & `trimesh-4.3.1/trimesh/permutate.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/points.py` & `trimesh-4.3.1/trimesh/points.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/poses.py` & `trimesh-4.3.1/trimesh/poses.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/primitives.py` & `trimesh-4.3.1/trimesh/primitives.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/proximity.py` & `trimesh-4.3.1/trimesh/proximity.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/ray/ray_pyembree.py` & `trimesh-4.3.1/trimesh/ray/ray_pyembree.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/ray/ray_triangle.py` & `trimesh-4.3.1/trimesh/ray/ray_triangle.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/ray/ray_util.py` & `trimesh-4.3.1/trimesh/ray/ray_util.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/registration.py` & `trimesh-4.3.1/trimesh/registration.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/remesh.py` & `trimesh-4.3.1/trimesh/remesh.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/rendering.py` & `trimesh-4.3.1/trimesh/rendering.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/repair.py` & `trimesh-4.3.1/trimesh/repair.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/resolvers.py` & `trimesh-4.3.1/trimesh/resolvers.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/resources/__init__.py` & `trimesh-4.3.1/trimesh/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/resources/creation.json` & `trimesh-4.3.1/trimesh/resources/creation.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/resources/schema/gltf2.schema.zip` & `trimesh-4.3.1/trimesh/resources/schema/gltf2.schema.zip`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/resources/schema/primitive/box.schema.json` & `trimesh-4.3.1/trimesh/resources/schema/primitive/box.schema.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/resources/schema/primitive/capsule.schema.json` & `trimesh-4.3.1/trimesh/resources/schema/primitive/capsule.schema.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/resources/schema/primitive/cylinder.schema.json` & `trimesh-4.3.1/trimesh/resources/schema/primitive/cylinder.schema.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/resources/schema/primitive/extrusion.schema.json` & `trimesh-4.3.1/trimesh/resources/schema/primitive/extrusion.schema.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/resources/schema/primitive/scenegraph.schema.json` & `trimesh-4.3.1/trimesh/resources/schema/primitive/scenegraph.schema.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/resources/schema/primitive/sphere.schema.json` & `trimesh-4.3.1/trimesh/resources/schema/primitive/sphere.schema.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/resources/schema/primitive/trimesh.schema.json` & `trimesh-4.3.1/trimesh/resources/schema/primitive/trimesh.schema.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/resources/schema/urdf.xsd` & `trimesh-4.3.1/trimesh/resources/schema/urdf.xsd`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/resources/templates/blender_boolean.py.tmpl` & `trimesh-4.3.1/trimesh/resources/templates/blender_boolean.py.tmpl`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/resources/templates/blender_unwrap.py.template` & `trimesh-4.3.1/trimesh/resources/templates/blender_unwrap.py.template`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/resources/templates/dxf.json` & `trimesh-4.3.1/trimesh/resources/templates/dxf.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/resources/templates/viewer.zip` & `trimesh-4.3.1/trimesh/resources/templates/viewer.zip`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/resources/units_to_inches.json` & `trimesh-4.3.1/trimesh/resources/units_to_inches.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/sample.py` & `trimesh-4.3.1/trimesh/sample.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/scene/cameras.py` & `trimesh-4.3.1/trimesh/scene/cameras.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/scene/lighting.py` & `trimesh-4.3.1/trimesh/scene/lighting.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/scene/scene.py` & `trimesh-4.3.1/trimesh/scene/scene.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/scene/transforms.py` & `trimesh-4.3.1/trimesh/scene/transforms.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/schemas.py` & `trimesh-4.3.1/trimesh/schemas.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/smoothing.py` & `trimesh-4.3.1/trimesh/smoothing.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/transformations.py` & `trimesh-4.3.1/trimesh/transformations.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/triangles.py` & `trimesh-4.3.1/trimesh/triangles.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/typed.py` & `trimesh-4.3.1/trimesh/typed.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/units.py` & `trimesh-4.3.1/trimesh/units.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/util.py` & `trimesh-4.3.1/trimesh/util.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/version.py` & `trimesh-4.3.1/trimesh/version.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/viewer/__init__.py` & `trimesh-4.3.1/trimesh/viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/viewer/notebook.py` & `trimesh-4.3.1/trimesh/viewer/notebook.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/viewer/trackball.py` & `trimesh-4.3.1/trimesh/viewer/trackball.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/viewer/widget.py` & `trimesh-4.3.1/trimesh/viewer/widget.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/viewer/windowed.py` & `trimesh-4.3.1/trimesh/viewer/windowed.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/visual/__init__.py` & `trimesh-4.3.1/trimesh/visual/__init__.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/visual/base.py` & `trimesh-4.3.1/trimesh/visual/base.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/visual/color.py` & `trimesh-4.3.1/trimesh/visual/color.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/visual/gloss.py` & `trimesh-4.3.1/trimesh/visual/gloss.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/visual/material.py` & `trimesh-4.3.1/trimesh/visual/material.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/visual/objects.py` & `trimesh-4.3.1/trimesh/visual/objects.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/visual/texture.py` & `trimesh-4.3.1/trimesh/visual/texture.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/voxel/base.py` & `trimesh-4.3.1/trimesh/voxel/base.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/voxel/creation.py` & `trimesh-4.3.1/trimesh/voxel/creation.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/voxel/encoding.py` & `trimesh-4.3.1/trimesh/voxel/encoding.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/voxel/morphology.py` & `trimesh-4.3.1/trimesh/voxel/morphology.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/voxel/ops.py` & `trimesh-4.3.1/trimesh/voxel/ops.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/voxel/runlength.py` & `trimesh-4.3.1/trimesh/voxel/runlength.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh/voxel/transforms.py` & `trimesh-4.3.1/trimesh/voxel/transforms.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.0/trimesh.egg-info/PKG-INFO` & `trimesh-4.3.1/trimesh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trimesh
-Version: 4.3.0
+Version: 4.3.1
 Summary: Import, export, process, analyze and view triangular meshes.
 Author-email: Michael Dawson-Haggerty <mikedh@kerfed.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Michael Dawson-Haggerty
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `trimesh-4.3.0/trimesh.egg-info/SOURCES.txt` & `trimesh-4.3.1/trimesh.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 tests/test_normals.py
 tests/test_nsphere.py
 tests/test_obj.py
 tests/test_off.py
 tests/test_operators.py
 tests/test_packing.py
 tests/test_path_creation.py
+tests/test_path_sample.py
 tests/test_pathlib.py
 tests/test_paths.py
 tests/test_pbr.py
 tests/test_permutate.py
 tests/test_ply.py
 tests/test_points.py
 tests/test_polygons.py
```

