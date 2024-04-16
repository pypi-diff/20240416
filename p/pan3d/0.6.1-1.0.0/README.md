# Comparing `tmp/pan3d-0.6.1.tar.gz` & `tmp/pan3d-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pan3d-0.6.1.tar", last modified: Tue Apr 16 18:11:18 2024, max compression
+gzip compressed data, was "pan3d-1.0.0.tar", last modified: Fri Nov 17 15:27:16 2023, max compression
```

## Comparing `pan3d-0.6.1.tar` & `pan3d-1.0.0.tar`

### file list

```diff
@@ -1,40 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:11:18.089132 pan3d-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-16 18:11:06.000000 pan3d-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-16 18:11:06.000000 pan3d-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-16 18:11:18.085132 pan3d-0.6.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:11:18.081132 pan3d-0.6.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-16 18:11:06.000000 pan3d-0.6.1/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:11:18.081132 pan3d-0.6.1/pan3d/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-16 18:11:06.000000 pan3d-0.6.1/pan3d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:11:18.085132 pan3d-0.6.1/pan3d/catalogs/
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-16 18:11:06.000000 pan3d-0.6.1/pan3d/catalogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-16 18:11:06.000000 pan3d-0.6.1/pan3d/catalogs/esgf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-04-16 18:11:06.000000 pan3d-0.6.1/pan3d/catalogs/pangeo.py
--rw-r--r--   0 runner    (1001) docker     (127)    21292 2024-04-16 18:11:06.000000 pan3d-0.6.1/pan3d/dataset_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    27559 2024-04-16 18:11:06.000000 pan3d-0.6.1/pan3d/dataset_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-16 18:11:06.000000 pan3d-0.6.1/pan3d/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-16 18:11:06.000000 pan3d-0.6.1/pan3d/serve_viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:11:18.085132 pan3d-0.6.1/pan3d/ui/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-16 18:11:06.000000 pan3d-0.6.1/pan3d/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-04-16 18:11:06.000000 pan3d-0.6.1/pan3d/ui/axis_drawer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-04-16 18:11:06.000000 pan3d-0.6.1/pan3d/ui/catalog_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     8398 2024-04-16 18:11:06.000000 pan3d-0.6.1/pan3d/ui/coordinate_configure.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-16 18:11:06.000000 pan3d-0.6.1/pan3d/ui/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-04-16 18:11:06.000000 pan3d-0.6.1/pan3d/ui/file_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-04-16 18:11:06.000000 pan3d-0.6.1/pan3d/ui/main_drawer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-16 18:11:06.000000 pan3d-0.6.1/pan3d/ui/render_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-16 18:11:06.000000 pan3d-0.6.1/pan3d/ui/toolbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-04-16 18:11:06.000000 pan3d-0.6.1/pan3d/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:11:18.085132 pan3d-0.6.1/pan3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-16 18:11:18.000000 pan3d-0.6.1/pan3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-16 18:11:18.000000 pan3d-0.6.1/pan3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 18:11:18.000000 pan3d-0.6.1/pan3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-16 18:11:18.000000 pan3d-0.6.1/pan3d.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-16 18:11:18.000000 pan3d-0.6.1/pan3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 18:11:18.000000 pan3d-0.6.1/pan3d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-16 18:11:06.000000 pan3d-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 18:11:18.089132 pan3d-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-16 18:11:08.000000 pan3d-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:11:18.085132 pan3d-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-04-16 18:11:06.000000 pan3d-0.6.1/tests/test_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-04-16 18:11:06.000000 pan3d-0.6.1/tests/test_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 15:27:16.772598 pan3d-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2023-11-17 15:27:03.000000 pan3d-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2023-11-17 15:27:16.772598 pan3d-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2023-11-17 15:27:03.000000 pan3d-1.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 15:27:16.768598 pan3d-1.0.0/pan3d/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2023-11-17 15:27:03.000000 pan3d-1.0.0/pan3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2023-11-17 15:27:03.000000 pan3d-1.0.0/pan3d/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22792 2023-11-17 15:27:03.000000 pan3d-1.0.0/pan3d/dataset_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2023-11-17 15:27:03.000000 pan3d-1.0.0/pan3d/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2023-11-17 15:27:03.000000 pan3d-1.0.0/pan3d/pangeo_forge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 15:27:16.772598 pan3d-1.0.0/pan3d/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2023-11-17 15:27:03.000000 pan3d-1.0.0/pan3d/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2023-11-17 15:27:03.000000 pan3d-1.0.0/pan3d/ui/axis_drawer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8725 2023-11-17 15:27:03.000000 pan3d-1.0.0/pan3d/ui/coordinate_configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4808 2023-11-17 15:27:03.000000 pan3d-1.0.0/pan3d/ui/file_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5204 2023-11-17 15:27:03.000000 pan3d-1.0.0/pan3d/ui/main_drawer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3363 2023-11-17 15:27:03.000000 pan3d-1.0.0/pan3d/ui/render_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2023-11-17 15:27:03.000000 pan3d-1.0.0/pan3d/ui/toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2023-11-17 15:27:03.000000 pan3d-1.0.0/pan3d/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 15:27:16.768598 pan3d-1.0.0/pan3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2023-11-17 15:27:16.000000 pan3d-1.0.0/pan3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2023-11-17 15:27:16.000000 pan3d-1.0.0/pan3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-17 15:27:16.000000 pan3d-1.0.0/pan3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2023-11-17 15:27:16.000000 pan3d-1.0.0/pan3d.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2023-11-17 15:27:16.000000 pan3d-1.0.0/pan3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-17 15:27:16.000000 pan3d-1.0.0/pan3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-11-17 15:27:03.000000 pan3d-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-17 15:27:16.772598 pan3d-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-17 15:27:03.000000 pan3d-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 15:27:16.772598 pan3d-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2023-11-17 15:27:03.000000 pan3d-1.0.0/tests/test_config.py
```

### Comparing `pan3d-0.6.1/LICENSE` & `pan3d-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pan3d-0.6.1/pan3d/serve_viewer.py` & `pan3d-1.0.0/pan3d/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 from argparse import ArgumentParser, BooleanOptionalAction
 from pan3d.dataset_builder import DatasetBuilder
 
 
-def serve():
+def main():
     parser = ArgumentParser(
         prog="Pan3D",
-        description="Launch the Pan3D Dataset Viewer",
+        description="Launch the Pan3D Dataset Builder",
     )
 
-    parser.add_argument("--config_path")
-    parser.add_argument("--dataset")
-    parser.add_argument("--catalogs", nargs="+")
-    parser.add_argument("--server", action=BooleanOptionalAction)
-    parser.add_argument("--debug", action=BooleanOptionalAction)
+    parser.add_argument("-C", "--config_path")
+    parser.add_argument("-D", "--dataset_path")
+    parser.add_argument("-P", "--pangeo", action=BooleanOptionalAction)
+    parser.add_argument("-S", "--server", action=BooleanOptionalAction)
 
     args = parser.parse_args()
 
-    builder = DatasetBuilder(
-        dataset=args.dataset,
-        catalogs=args.catalogs,
-    )
+    builder = DatasetBuilder(dataset_path=args.dataset_path, pangeo=args.pangeo)
     if args.config_path:
         builder.import_config(args.config_path)
-    builder.viewer.start(debug=args.debug)
+    builder.viewer.server.start()
 
 
 if __name__ == "__main__":
-    serve()
+    main()
```

### Comparing `pan3d-0.6.1/pan3d/ui/axis_drawer.py` & `pan3d-1.0.0/pan3d/ui/axis_drawer.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         da_x="da_x",
         da_y="da_y",
         da_z="da_z",
         da_t="da_t",
         da_t_index="da_t_index",
     ):
         super().__init__(
-            v_model=(ui_axis_drawer,),
+            v_model=ui_axis_drawer,
             classes="pa-2",
             width="350",
             location="right",
             permanent=True,
             style="position: absolute",
         )
         axes = [
@@ -48,71 +48,67 @@
                 "label": "T",
                 "name_var": da_t,
                 "index_var": da_t_index,
             },
         ]
         with self:
             with vuetify.VExpansionPanels(
-                model_value=("[0, 1]",),
+                model_value=([0, 1],),
                 multiple=True,
                 accordion=True,
-                v_if=(da_coordinates,),
+                v_if=da_coordinates,
             ):
                 with vuetify.VExpansionPanel(title="Assigned Coordinates"):
                     with vuetify.VExpansionPanelText():
                         for axis in axes:
                             with vuetify.VSheet(classes="d-flex"):
                                 html.Span(axis["label"], classes="pt-2")
                                 with html.Div(
-                                    v_show=(f"{axis['name_var']}",), style="width: 100%"
+                                    v_show=f"{axis['name_var']}", style="width: 100%"
                                 ):
                                     CoordinateConfigure(
                                         axes,
                                         da_coordinates,
                                         f"{da_coordinates}.find((c) => c.name === {axis['name_var']})",
                                         ui_expanded_coordinates,
                                         ui_current_time_string,
                                         coordinate_select_axis_function,
                                         coordinate_change_slice_function,
                                         coordinate_toggle_expansion_function,
                                         axis_info=axis,
                                     )
                                 with vuetify.VCard(
-                                    v_show=(f"!{axis['name_var']}",),
+                                    v_show=f"!{axis['name_var']}",
                                     height="45",
                                     classes="ml-3 mb-1",
                                     style="flex-grow: 1",
                                 ):
                                     vuetify.VCardSubtitle(
                                         f"No coordinate assigned to {axis['label']}",
                                         classes="text-center pt-3",
                                     )
 
                 with vuetify.VExpansionPanel(title="Available Coordinates"):
                     with vuetify.VExpansionPanelText():
                         with html.Div(
-                            v_for=("coord in da_coordinates",),
-                            v_show=(
-                                f"![{da_x}, {da_y}, {da_z}, {da_t}].includes(coord.name)",
-                            ),
+                            v_for="coord in da_coordinates",
+                            v_show=f"![{da_x}, {da_y}, {da_z}, {da_t}].includes(coord.name)",
                         ):
                             CoordinateConfigure(
                                 axes,
                                 da_coordinates,
                                 "coord",
                                 ui_expanded_coordinates,
                                 ui_current_time_string,
                                 coordinate_select_axis_function,
                                 coordinate_change_slice_function,
                                 coordinate_toggle_expansion_function,
                             )
                         html.Span(
                             "No coordinates remain.",
-                            v_show=(
-                                f"""
+                            v_show=f"""
                                 da_coordinates.every(
                                     (c) => [{da_x}, {da_y}, {da_z}, {da_t}].includes(c.name)
                                 )
                             """,
-                            ),
                             classes="mx-5",
                         )
```

### Comparing `pan3d-0.6.1/pan3d/ui/catalog_search.py` & `pan3d-1.0.0/pan3d/ui/main_drawer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,129 +1,124 @@
 from trame.widgets import html
 from trame.widgets import vuetify3 as vuetify
 
 
-class CatalogSearch(vuetify.VDialog):
+class MainDrawer(vuetify.VNavigationDrawer):
     def __init__(
         self,
-        update_catalog_search_term_function,
-        catalog_search_function,
-        catalog_term_search_function,
-        catalog="catalog",
-        available_catalogs="available_catalogs",
-        ui_search_catalogs="ui_search_catalogs",
-        catalog_current_search="catalog_current_search",
-        ui_catalog_term_search_loading="ui_catalog_term_search_loading",
-        ui_catalog_search_message="ui_catalog_search_message",
+        dataset_ready="dataset_ready",
+        dataset_path="dataset_path",
+        da_attrs="da_attrs",
+        da_vars="da_vars",
+        da_vars_attrs="da_vars_attrs",
+        available_datasets="available_datasets",
+        ui_main_drawer="ui_main_drawer",
+        ui_more_info_link="ui_more_info_link",
+        da_active="da_active",
+        da_x="da_x",
+        da_y="da_y",
+        da_z="da_z",
+        da_t="da_t",
+        da_t_index="da_t_index",
     ):
-        super().__init__(v_model=(ui_search_catalogs,), max_width=800)
+        super().__init__(
+            v_model=ui_main_drawer, classes="pa-2", permanent=True, width=300
+        )
         with self:
-            with vuetify.Template(v_slot_activator=("{ props }",)):
-                vuetify.VBtn(
-                    "Search Catalogs",
-                    click=f"{ui_search_catalogs} = true",
-                    size="small",
-                    block=True,
-                    classes="my-2",
-                )
-            with vuetify.VCard():
-                with vuetify.VCardText():
-                    vuetify.VBtn(
-                        flat=True,
-                        icon="mdi-close",
-                        style="float: right",
-                        click=f"{ui_search_catalogs} = false",
-                    )
-                    vuetify.VCardTitle("Search a catalog")
-
-                    vuetify.VSelect(
-                        label="Choose a catalog",
-                        v_show=(f"{available_catalogs}.length > 1",),
-                        items=(available_catalogs, []),
-                        v_model=(catalog,),
-                        item_title="name",
-                        density="compact",
-                        return_object=True,
-                        hide_details=True,
-                    )
-
-                    vuetify.VCardSubtitle(
-                        "Select or enter search terms",
-                        classes="mt-5",
-                        style="display: inline-block",
-                    )
-                    with vuetify.VTooltip(
-                        location="bottom",
-                        text="For each search term, you may specify one or more acceptable values.",
-                    ):
-                        with vuetify.Template(v_slot_activator=("{ props }",)):
-                            vuetify.VIcon(
+            vuetify.VSelect(
+                label="Choose a dataset",
+                v_model=dataset_path,
+                items=(available_datasets,),
+                item_title="name",
+                item_value="url",
+                density="compact",
+                hide_details=True,
+            )
+
+            with vuetify.VListItem(v_show=(dataset_ready,)):
+                with html.Div(
+                    classes="d-flex pa-2", style="justify-content: space-between"
+                ):
+                    html.Span("Attributes")
+                    with vuetify.VDialog(max_width=800):
+                        with vuetify.Template(v_slot_activator="{ props }"):
+                            vuetify.VBtn(
+                                icon="mdi-dots-horizontal",
+                                size="x-small",
+                                variant="plain",
                                 v_bind="props",
-                                icon="mdi-information-outline",
-                                style="vertical-align: baseline",
                             )
-
-                    with vuetify.VBtn(
-                        size="small",
-                        classes="mt-3",
-                        style="float: right",
-                        loading=(ui_catalog_term_search_loading,),
-                        disabled=(ui_catalog_term_search_loading,),
-                        click=catalog_term_search_function,
-                    ):
-                        html.Span("Search for term options")
-                        vuetify.VTooltip(
-                            activator="parent",
-                            location="bottom",
-                            text="""
-                                Perform an unfiltered search on the catalog
-                                to find all unique values for all searchable terms.
-                                The results will appear as selectable options in
-                                the value input dropdowns.
-                                """,
-                        )
-
-                    with vuetify.VTable(v_if=(catalog,), style="max-height: 500px"):
-                        with html.Tbody():
-                            with html.Tr(
-                                v_for=(f"term in {catalog}.search_terms",),
+                        with vuetify.VCard():
+                            vuetify.VCardTitle(
+                                "Dataset Attributes",
+                                v_show=f"{da_attrs}.length",
+                                classes="font-weight-bold",
+                            )
+                            vuetify.VCardText(
+                                "No attributes.", v_show=f"{da_attrs}.length === 0"
+                            )
+                            with vuetify.VTable(
+                                v_show=f"{dataset_ready} && {da_attrs}.length",
+                                density="compact",
+                            ):
+                                with html.Tbody():
+                                    with html.Tr(
+                                        v_for=f"data_attr in {da_attrs}",
+                                    ):
+                                        html.Td("{{ data_attr.key }}")
+                                        html.Td("{{ data_attr.value }}")
+
+            html.A(
+                "More information about this dataset",
+                href=(ui_more_info_link,),
+                v_show=(ui_more_info_link,),
+                target="_blank",
+                classes="mx-3",
+            )
+
+            vuetify.VDivider(v_show=(dataset_ready,), classes="my-2")
+
+            vuetify.VCardText(
+                "Available Arrays",
+                v_show=dataset_ready,
+                classes="font-weight-bold",
+            )
+            vuetify.VCardText(
+                "No data variables found.",
+                v_show=(f"{dataset_ready} && {da_vars}.length === 0",),
+            )
+            with vuetify.VListItem(
+                v_for=f"array in {da_vars}",
+                active=(f"array.name === {da_active}",),
+                click=f"{da_active} = array.name",
+            ):
+                with html.Div(
+                    classes="d-flex pa-2", style="justify-content: space-between"
+                ):
+                    html.Span("{{ array.name }}")
+                    with vuetify.VDialog(max_width=800):
+                        with vuetify.Template(v_slot_activator="{ props }"):
+                            vuetify.VBtn(
+                                icon="mdi-dots-horizontal",
+                                size="x-small",
+                                variant="plain",
+                                v_bind="props",
+                            )
+                        with vuetify.VCard():
+                            vuetify.VCardTitle(
+                                "Array Attributes",
+                                classes="font-weight-bold",
+                            )
+                            vuetify.VCardText(
+                                "No attributes.",
+                                v_show=f"{da_vars_attrs}[array.name].length === 0",
+                            )
+                            with vuetify.VTable(
+                                v_show=f"{da_vars_attrs}[array.name].length",
+                                density="compact",
                             ):
-                                html.Td("{{ term.key }}", style="width: 100px")
-                                with html.Td():
-                                    vuetify.VCombobox(
-                                        label="Enter value",
-                                        items=("term.options", []),
-                                        multiple=True,
-                                        chips=True,
-                                        closable_chips=True,
-                                        clearable=True,
-                                        model_value=(
-                                            f"{catalog_current_search}[term.key]",
-                                            [],
-                                        ),
-                                        update_modelValue=(
-                                            update_catalog_search_term_function,
-                                            "[term.key, $event]",
-                                        ),
-                                    )
-
-                    with vuetify.VBtn(
-                        color="primary",
-                        style="float: right",
-                        loading=(ui_catalog_term_search_loading,),
-                        disabled=(ui_catalog_term_search_loading,),
-                        click=catalog_search_function,
-                    ):
-                        html.Span("Search")
-                        vuetify.VTooltip(
-                            activator="parent",
-                            location="bottom",
-                            text="""
-                                Perform a filtered search with the union of all selected terms.
-                                The results will be grouped and added to the list of available datasets.
-                                """,
-                        )
-
-                    html.Span(
-                        "{{ %s }}" % ui_catalog_search_message,
-                        v_show=ui_catalog_search_message,
-                    )
+                                with html.Tbody():
+                                    with html.Tr(
+                                        v_for=f"data_attr in {da_vars_attrs}[array.name]",
+                                    ):
+                                        html.Td("{{ data_attr.key }}")
+                                        html.Td("{{ data_attr.value }}")
```

### Comparing `pan3d-0.6.1/pan3d/ui/coordinate_configure.py` & `pan3d-1.0.0/pan3d/ui/coordinate_configure.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,129 +17,139 @@
         super().__init__(width="95%", classes="ml-3 mb-1")
 
         with self:
             with vuetify.VExpansionPanels(
                 model_value=(ui_expanded_coordinates, []),
                 accordion=True,
                 multiple=True,
-                v_show=(coordinate_info,),
+                v_show=coordinate_info,
                 update_modelValue=(
                     coordinate_toggle_expansion_function,
                     f"[{coordinate_info}.name]",
                 ),
             ):
-                with vuetify.VExpansionPanel(value=(f"{coordinate_info}?.name",)):
+                with vuetify.VExpansionPanel(value=(f"{coordinate_info}?.name", 0)):
                     vuetify.VExpansionPanelTitle("{{ %s?.name }}" % coordinate_info)
                     with vuetify.VExpansionPanelText():
                         vuetify.VCardSubtitle("Attributes")
-                        with vuetify.VTable(
-                            density="compact", v_show=(coordinate_info,)
-                        ):
+                        with vuetify.VTable(density="compact", v_show=coordinate_info):
                             with html.Tbody():
                                 with html.Tr(
-                                    v_for=(f"data_attr in {coordinate_info}?.attrs",),
+                                    v_for=f"data_attr in {coordinate_info}?.attrs",
                                 ):
                                     html.Td("{{ data_attr.key }}")
                                     html.Td("{{ data_attr.value }}")
 
                         if axis_info and axis_info["index_var"] != "undefined":
                             vuetify.VCardSubtitle(
                                 "Current: {{ %s }}" % ui_current_time_string,
                                 classes="mt-3",
                             )
                             with vuetify.VSlider(
-                                v_model=(axis_info["index_var"],),
+                                v_model=axis_info["index_var"],
                                 min=0,
-                                max=(f"{coordinate_info}?.size - 1",),
-                                step=(f"{coordinate_info}?.step",),
+                                max=(
+                                    f"{coordinate_info}?.size - 1",
+                                    0,
+                                ),
+                                step=(f"{coordinate_info}?.step", 1),
                                 classes="mx-5",
                             ):
                                 with vuetify.Template(
-                                    v_slot_append=("{ props, item, parent }",)
+                                    v_slot_append="{ props, item, parent }"
                                 ):
                                     vuetify.VTextField(
-                                        v_model=(axis_info["index_var"],),
+                                        v_model=axis_info["index_var"],
                                         min=0,
-                                        max=(f"{coordinate_info}?.size - 1",),
-                                        step=(f"{coordinate_info}?.step",),
+                                        max=(
+                                            f"{coordinate_info}?.size - 1",
+                                            0,
+                                        ),
+                                        step=(f"{coordinate_info}?.step", 1),
                                         hide_details=True,
                                         density="compact",
-                                        style="width: 100px",
+                                        style="width: 80px",
                                         type="number",
                                         __properties=["min", "max"],
                                     )
 
                         else:
-                            vuetify.VCardSubtitle(
-                                "Select values",
-                                v_if=(f"{coordinate_info}?.numeric",),
-                                classes="mt-3",
-                            )
+                            vuetify.VCardSubtitle("Select values", classes="mt-3")
                             with vuetify.VContainer(
-                                classes="d-flex pa-0",
-                                style="column-gap: 3px",
-                                v_if=(f"{coordinate_info}?.numeric",),
+                                classes="d-flex pa-0", style="column-gap: 3px"
                             ):
                                 vuetify.VTextField(
-                                    model_value=(f"{coordinate_info}?.start",),
+                                    model_value=(f"{coordinate_info}?.start", 0),
                                     label="Start",
                                     hide_details=True,
                                     density="compact",
                                     type="number",
-                                    min=(f"{coordinate_info}?.range[0]",),
-                                    max=(f"{coordinate_info}?.range[1]",),
+                                    min=(
+                                        f"{coordinate_info}?.range[0]",
+                                        0,
+                                    ),
+                                    max=(
+                                        f"{coordinate_info}?.range[1]",
+                                        0,
+                                    ),
                                     step="0.01",
                                     __properties=["min", "max", "step"],
-                                    change_prevent=(
+                                    input=(
                                         coordinate_change_slice_function,
                                         f"[{coordinate_info}.name, 'start', $event.target.value]",
                                     ),
-                                    __events=[("change_prevent", "change.prevent")],
+                                    __events=[("input", "input.prevent")],
                                     style="flex-grow: 1",
                                 )
                                 vuetify.VTextField(
-                                    model_value=(f"{coordinate_info}?.stop",),
+                                    model_value=(f"{coordinate_info}?.stop", 0),
                                     label="Stop",
                                     hide_details=True,
                                     density="compact",
                                     type="number",
-                                    min=(f"{coordinate_info}?.range[0]",),
-                                    max=(f"{coordinate_info}?.range[1]",),
+                                    min=(
+                                        f"{coordinate_info}?.range[0]",
+                                        0,
+                                    ),
+                                    max=(
+                                        f"{coordinate_info}?.range[1]",
+                                        0,
+                                    ),
                                     step="0.01",
                                     __properties=["min", "max", "step"],
-                                    change_prevent=(
+                                    input=(
                                         coordinate_change_slice_function,
                                         f"[{coordinate_info}.name, 'stop', $event.target.value]",
                                     ),
-                                    __events=[("change_prevent", "change.prevent")],
+                                    __events=[("input", "input.prevent")],
                                     style="flex-grow: 1",
                                 )
                                 vuetify.VTextField(
-                                    model_value=(f"{coordinate_info}?.step",),
+                                    model_value=(f"{coordinate_info}?.step", 1),
                                     label="Step",
                                     hide_details=True,
                                     density="compact",
                                     type="number",
                                     min="1",
-                                    max=(f"{coordinate_info}?.size",),
+                                    max=(f"{coordinate_info}?.size", 0),
                                     __properties=["min", "max"],
-                                    change_prevent=(
+                                    input=(
                                         coordinate_change_slice_function,
                                         f"[{coordinate_info}.name, 'step', $event.target.value]",
                                     ),
-                                    __events=[("change_prevent", "change.prevent")],
+                                    __events=[("input", "input.prevent")],
                                     style="flex-grow: 1",
                                 )
 
                         vuetify.VCardSubtitle("Assign axis", classes="mt-3")
                         with vuetify.VSelect(
-                            items=(str(axes),),
+                            items=(axes,),
                             item_title="label",
                             item_value="name_var",
-                            model_value=(str(axis_info) or "undefined",),
+                            model_value=(axis_info or "undefined",),
                             clearable=True,
                             click_clear=(
                                 coordinate_select_axis_function,
                                 # args: coord name, current axis, new axis
                                 f"[{axis_info['name_var']}, '{axis_info['name_var']}', 'undefined']",
                             )
                             if axis_info
@@ -151,10 +161,10 @@
                                     {coordinate_info}.name,
                                     '{axis_info["name_var"] if axis_info else "undefined"}',
                                     $event
                                 ]""",
                             ),
                         ):
                             with vuetify.Template(
-                                v_slot_selection=("{ props, item, parent }",)
+                                v_slot_selection="{ props, item, parent }"
                             ):
                                 html.Span(axis_info["label"] if axis_info else "")
```

### Comparing `pan3d-0.6.1/pan3d/ui/file_select.py` & `pan3d-1.0.0/pan3d/ui/file_select.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,63 @@
+import json
 from trame.widgets import html, vuetify3 as vuetify
 from trame.app import get_server
 
 server = get_server()
 
 
 class FileSelect(vuetify.VCard):
     def __init__(
         self,
         import_function,
         export_function,
         ui_action_name="ui_action_name",
-        ui_action_config_file="ui_action_config_file",
+        ui_selected_config_file="ui_selected_config_file",
         state_export="state_export",
         ui_action_message="ui_action_message",
-        ui_import_loading="ui_import_loading",
     ):
+        def submit_import():
+            files = server.state[ui_selected_config_file]
+            if files and len(files) > 0:
+                file_content = server.state[ui_selected_config_file][0]["content"]
+                import_function(json.loads(file_content.decode()))
+
         super().__init__()
         with self:
-            with vuetify.VCardText(v_show=(ui_action_name,)):
+            with vuetify.VCardText(v_show=ui_action_name):
                 vuetify.VBtn(
                     flat=True,
                     icon="mdi-close",
                     style="float: right",
                     click=f"{ui_action_name} = undefined",
                 )
                 vuetify.VCardTitle(
                     "{{ %s }}" % ui_action_message,
-                    v_show=(ui_action_message,),
+                    v_show=ui_action_message,
                 )
-                with html.Div(v_show=(f"!{ui_action_message}",)):
+                with html.Div(v_show=f"!{ui_action_message}"):
                     vuetify.VCardTitle("{{ %s }} File Select" % ui_action_name)
 
                     vuetify.VFileInput(
-                        v_model=(ui_action_config_file,),
-                        v_show=(f"{ui_action_name} === 'Import'",),
+                        v_model=ui_selected_config_file,
+                        v_show=f"{ui_action_name} === 'Import'",
                         accept=".json",
                         label="Config File",
                     )
                     vuetify.VBtn(
-                        v_show=(
-                            f"{ui_action_name} === 'Import' && {ui_action_config_file} && !{ui_import_loading}",
-                        ),
+                        v_show=f"{ui_action_name} === 'Import' && {ui_selected_config_file}",
                         variant="tonal",
                         text=(ui_action_name,),
-                        click=import_function,
+                        click=submit_import,
                         style="width: 100%",
                     )
-                    vuetify.VCardSubtitle(
-                        "Reading configuration file and applying changes...",
-                        v_show=(ui_import_loading,),
-                    )
-                    vuetify.VProgressLinear(
-                        v_show=(ui_import_loading,),
-                        indeterminate=True,
-                    )
 
                     vuetify.VTextField(
-                        v_model=(ui_action_config_file,),
-                        v_show=(
-                            f"{ui_action_name} === 'Export' && {ui_action_config_file} != false",
-                        ),
+                        v_model=ui_selected_config_file,
+                        v_show=f"{ui_action_name} === 'Export' && {ui_selected_config_file} != false",
                         label="Download Location",
                         prepend_icon="mdi-paperclip",
                         # FileSystem API is only available on some browsers:
                         # https://caniuse.com/native-filesystem-api
                         click="""
                             if ($event){
                                 try {
@@ -83,20 +77,18 @@
                                     });
                                 } catch {
                                     %s = false;
                                     window.alert('Your browser does not support selecting a download location. Your download will be made to the default location, saved as pan3d_state.json.')
                                 }
                             }
                         """
-                        % (state_export, ui_action_message, ui_action_config_file),
+                        % (state_export, ui_action_message, ui_selected_config_file),
                     )
                     vuetify.VBtn(
-                        v_show=(
-                            f"{ui_action_name} === 'Export' && {ui_action_config_file} === false",
-                        ),
+                        v_show=f"{ui_action_name} === 'Export' && {ui_selected_config_file} === false",
                         variant="tonal",
                         text="Download pan3d_state.json",
                         click=f"""
                             var content = JSON.stringify({state_export}, null, 4);
                             var a = window.document.createElement('a');
                             a.href = 'data:application/json;charset=utf-8,'  + encodeURIComponent(content);
                             a.download = 'pan3d_state.json';
```

### Comparing `pan3d-0.6.1/pan3d/ui/render_options.py` & `pan3d-1.0.0/pan3d/ui/render_options.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,89 +9,78 @@
         z_scale="render_z_scale",
         colormap="render_colormap",
         colormap_options="render_colormap_options",
         transparency="render_transparency",
         transparency_function="render_transparency_function",
         transparency_function_options="render_transparency_function_options",
         scalar_warp="render_scalar_warp",
-        cartographic="render_cartographic",
     ):
         super().__init__(
             location="start",
             transition="slide-y-transition",
             close_on_content_click=False,
         )
         with self:
             with vuetify.Template(
                 activator="{ props }",
                 __properties=[
                     ("activator", "v-slot:activator"),
                 ],
             ):
                 vuetify.VBtn(
-                    v_bind=("props",),
+                    v_bind="props",
                     size="small",
-                    icon="mdi-cog",
+                    icon="mdi-dots-vertical",
                     style="position: absolute; right: 20px; top: 20px; z-index:2",
                 )
             with vuetify.VCard(classes="pa-3"):
                 vuetify.VSelect(
                     label="Colormap",
-                    v_model=(colormap,),
+                    v_model=colormap,
                     items=(colormap_options,),
                     density="compact",
                 )
                 vuetify.VCheckbox(
-                    label="Transparency", v_model=(transparency,), density="compact"
+                    label="Transparency", v_model=transparency, density="compact"
                 )
                 vuetify.VSelect(
                     label="Transparency Function",
                     v_show=(transparency,),
-                    v_model=(transparency_function,),
+                    v_model=transparency_function,
                     items=(transparency_function_options,),
                     density="compact",
                 )
-                # Scalar warp mode and cartographic mode are mutually exclusive
                 vuetify.VCheckbox(
-                    label="Warp by Scalars",
-                    v_model=(scalar_warp,),
-                    disabled=(cartographic,),
-                    density="compact",
-                )
-                vuetify.VCheckbox(
-                    label="Cartographic",
-                    v_model=(cartographic,),
-                    disabled=(scalar_warp,),
-                    density="compact",
+                    label="Warp by Scalars", v_model=scalar_warp, density="compact"
                 )
                 with vuetify.VContainer(classes="d-flex pa-0", style="column-gap: 3px"):
                     vuetify.VTextField(
-                        v_model=(x_scale,),
+                        v_model=x_scale,
                         label="X Scale",
                         min=1,
                         step=1,
                         hide_details=True,
                         density="compact",
                         style="width: 80px",
                         type="number",
                         __properties=["min", "step"],
                     )
                     vuetify.VTextField(
-                        v_model=(y_scale,),
+                        v_model=y_scale,
                         label="Y Scale",
                         min=1,
                         step=1,
                         hide_details=True,
                         density="compact",
                         style="width: 80px",
                         type="number",
                         __properties=["min", "step"],
                     )
                     vuetify.VTextField(
-                        v_model=(z_scale,),
+                        v_model=z_scale,
                         label="Z Scale",
                         min=1,
                         step=1,
                         hide_details=True,
                         density="compact",
                         style="width: 80px",
                         type="number",
```

### Comparing `pan3d-0.6.1/pan3d/ui/toolbar.py` & `pan3d-1.0.0/pan3d/ui/toolbar.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,70 +12,45 @@
         ui_main_drawer="ui_main_drawer",
         ui_axis_drawer="ui_axis_drawer",
         ui_action_name="ui_action_name",
         ui_loading="ui_loading",
         ui_unapplied_changes="ui_unapplied_changes",
         da_active="da_active",
         da_size="da_size",
-        render_auto="render_auto",
     ):
         super().__init__()
         with self:
-            with vuetify.VBtn(
-                size="x-large",
-                classes="pa-0 ma-0",
-                style="min-width: 60px",
-                click=f"{ui_main_drawer} = !{ui_main_drawer}",
-            ):
-                vuetify.VIcon("mdi-database-cog-outline")
-                vuetify.VIcon(
-                    "{{ %s? 'mdi-chevron-left' : 'mdi-chevron-right' }}"
-                    % ui_main_drawer
-                )
-
+            vuetify.VAppBarNavIcon(click=f"{ui_main_drawer} = !{ui_main_drawer}")
             vuetify.VAppBarTitle("Pan3D Viewer")
-            vuetify.VProgressLinear(
-                v_show=(ui_loading,),
-                indeterminate=True,
-                absolute=True,
-            )
             with html.Div(
-                classes="d-flex flex-row-reverse fill-height",
+                classes="d-flex flex-row-reverse pa-3 fill-height",
                 style="column-gap: 10px; align-items: center",
             ):
-                with vuetify.VBtn(
-                    size="x-large",
-                    classes="pa-0 ma-0",
-                    style="min-width: 60px",
-                    click=f"{ui_axis_drawer} = !{ui_axis_drawer}",
-                ):
-                    vuetify.VIcon("mdi-axis-arrow-info")
-                    vuetify.VIcon(
-                        "{{ %s? 'mdi-chevron-right' : 'mdi-chevron-left' }}"
-                        % ui_axis_drawer
-                    )
-                vuetify.VCheckbox(
-                    label="Auto Render", v_model=(render_auto,), hide_details=True
+                vuetify.VAppBarNavIcon(click=f"{ui_axis_drawer} = !{ui_axis_drawer}")
+                vuetify.VProgressCircular(
+                    v_show=(ui_loading,),
+                    indeterminate=True,
+                    classes="mx-10",
                 )
                 with vuetify.VBtn(
                     click=reset_function,
-                    v_show=(f"{ui_unapplied_changes} && !{render_auto}",),
+                    v_show=ui_unapplied_changes,
                     variant="tonal",
                 ):
                     html.Span("Apply & Render")
-                    html.Span("({{ %s }})" % da_size, v_show=(da_size,))
+                    html.Span("({{ %s }})" % da_size, v_show=da_size)
                 vuetify.VBtn(
                     click=f"{ui_action_name} = 'Export'",
                     variant="tonal",
                     text="Export",
                 )
                 vuetify.VBtn(
                     click=f"{ui_action_name} = 'Import'",
                     variant="tonal",
                     text="Import",
                 )
-                with vuetify.VDialog(v_model=(ui_action_name,), max_width=800):
+                with vuetify.VDialog(v_model=ui_action_name, max_width=800):
                     FileSelect(
                         import_function,
                         export_function,
                         ui_action_name=ui_action_name,
                     )
```

