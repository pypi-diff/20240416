# Comparing `tmp/glytrait-0.1.0.tar.gz` & `tmp/glytrait-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glytrait-0.1.0.tar", max compression
+gzip compressed data, was "glytrait-0.2.3.tar", max compression
```

## Comparing `glytrait-0.1.0.tar` & `glytrait-0.2.3.tar`

### file list

```diff
@@ -1,20 +1,11 @@
--rw-r--r--   0        0        0     1063 2023-06-01 11:46:23.327576 glytrait-0.1.0/LICENSE
--rw-r--r--   0        0        0    12405 2024-04-16 07:50:39.141303 glytrait-0.1.0/README.md
--rw-r--r--   0        0        0     1190 2024-04-14 11:59:39.762252 glytrait-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       74 2024-04-14 11:59:27.621443 glytrait-0.1.0/src/glytrait/__init__.py
--rw-r--r--   0        0        0    10396 2024-04-16 02:38:14.413421 glytrait-0.1.0/src/glytrait/api.py
--rw-r--r--   0        0        0     4748 2024-02-10 13:59:57.519954 glytrait-0.1.0/src/glytrait/cli.py
--rw-r--r--   0        0        0     2683 2024-04-14 11:59:08.462417 glytrait-0.1.0/src/glytrait/data_export.py
--rw-r--r--   0        0        0      923 2023-12-30 06:44:57.217908 glytrait-0.1.0/src/glytrait/data_type.py
--rw-r--r--   0        0        0      812 2024-04-14 11:59:08.463548 glytrait-0.1.0/src/glytrait/exception.py
--rw-r--r--   0        0        0    27518 2024-04-16 02:38:14.593722 glytrait-0.1.0/src/glytrait/formula.py
--rw-r--r--   0        0        0    13768 2024-02-10 13:59:57.574326 glytrait-0.1.0/src/glytrait/glycan.py
--rw-r--r--   0        0        0    14569 2024-03-08 09:00:51.155221 glytrait-0.1.0/src/glytrait/load_data.py
--rw-r--r--   0        0        0    18283 2024-04-14 11:59:08.464441 glytrait-0.1.0/src/glytrait/meta_property.py
--rw-r--r--   0        0        0     6664 2024-04-14 11:59:08.464921 glytrait-0.1.0/src/glytrait/post_filtering.py
--rw-r--r--   0        0        0     4621 2024-02-10 13:59:57.532082 glytrait-0.1.0/src/glytrait/preprocessing.py
--rw-r--r--   0        0        0     8081 2024-04-14 11:59:08.465266 glytrait-0.1.0/src/glytrait/resources/comp_formula.txt
--rw-r--r--   0        0        0    55082 2024-04-14 11:59:08.465614 glytrait-0.1.0/src/glytrait/resources/struc_formula.txt
--rw-r--r--   0        0        0     3767 2024-04-15 11:39:53.052570 glytrait-0.1.0/src/glytrait/stat.py
--rw-r--r--   0        0        0     1665 2023-12-30 06:44:57.220052 glytrait-0.1.0/src/glytrait/trait.py
--rw-r--r--   0        0        0    12818 1970-01-01 00:00:00.000000 glytrait-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      902 2023-05-29 11:06:05.560111 glytrait-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-24 08:03:06.472257 glytrait-0.2.3/glytrait/__init__.py
+-rw-r--r--   0        0        0     3845 2023-06-01 08:02:58.748682 glytrait-0.2.3/glytrait/cli.py
+-rw-r--r--   0        0        0      442 2023-05-30 03:44:18.093985 glytrait-0.2.3/glytrait/exception.py
+-rw-r--r--   0        0        0     8849 2023-06-01 01:31:32.581185 glytrait-0.2.3/glytrait/glycan.py
+-rw-r--r--   0        0        0     4847 2023-06-01 08:01:18.953222 glytrait-0.2.3/glytrait/io.py
+-rw-r--r--   0        0        0    16608 2023-06-01 08:01:18.953575 glytrait-0.2.3/glytrait/trait.py
+-rw-r--r--   0        0        0    23340 2023-05-29 10:03:43.008742 glytrait-0.2.3/glytrait/trait_forluma.txt
+-rw-r--r--   0        0        0     6889 2023-06-01 01:47:08.419603 glytrait-0.2.3/glytrait/trait_formula_template.txt
+-rw-r--r--   0        0        0      686 2023-06-01 08:01:18.953814 glytrait-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1489 1970-01-01 00:00:00.000000 glytrait-0.2.3/PKG-INFO
```

### Comparing `glytrait-0.1.0/src/glytrait/cli.py` & `glytrait-0.2.3/glytrait/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,178 +1,125 @@
-"""Command line interface for glyTrait."""
-
 from pathlib import Path
+from typing import Optional
 
 import click
 import emoji
 
-from glytrait.api import GlyTrait
 from glytrait.exception import GlyTraitError
-from glytrait.formula import save_builtin_formula
+from glytrait.io import read_input, write_output
+from glytrait.trait import (
+    save_trait_formula_template,
+    load_formulas,
+    build_meta_property_table,
+    calcu_derived_trait,
+    calcu_direct_trait
+)
 
 UNDIFINED = "__UNDEFINED__"
 
 
-def save_builtin_formulas_callback(ctx, param, value):
-    """Save a copy of the built-in formulas."""
+def save_template_callback(ctx, param, value):
+    """Save a template for the user to fill in."""
     if value == UNDIFINED:
         return
     if Path(value).exists() and not Path(value).is_dir():
-        msg = "The path to save the built-in formulas must be a directory."
-        raise click.BadParameter(msg)
+        raise click.BadParameter("The path to save the template must be a directory.")
     else:
-        save_builtin_formula(value)
+        save_trait_formula_template(value)
         msg = (
-            f"Built-in formulas saved to: "
-            f"{value}/struc_builtin_formulas.txt, {value}/comp_builtin_formulas.txt"
+            f"Template saved to {value}. :victory_hand:\n"
+            f"You can edit the template and use `glytrait INPUT_FILE OUTPUT_FILE -f "
+            f"TEMPLATE_FILE` to provide additional traits to glyTrait."
         )
         click.echo(emoji.emojize(msg))
         ctx.exit()
 
 
+def valid_input_file(ctx, param, value):
+    """Validate input file."""
+    if Path(value).suffix != ".csv":
+        raise click.BadParameter("Input file must be a csv file.")
+    return value
+
+
+def valid_output_file(ctx, param, value):
+    """Validate output file."""
+    if value is not None and Path(value).suffix != ".xlsx":
+        raise click.BadParameter("Output file must be a xlsx file.")
+    return value
+
+
+def valid_formula_file(ctx, param, value):
+    """Validate formula file."""
+    if value is not None and Path(value).suffix != ".txt":
+        raise click.BadParameter("Formula file must be a txt file.")
+    return value
+
+
 @click.command()
 @click.argument(
-    "abundance-file",
-    type=click.Path(exists=True, file_okay=True, dir_okay=False),
-    required=False,
-)
-@click.argument(
-    "glycan-file",
-    type=click.Path(exists=True, file_okay=True, dir_okay=True),
+    "input_file",
+    type=click.Path(exists=True),
     required=False,
+    callback=valid_input_file,
 )
+@click.option("-o", "--output_file", type=click.Path(), callback=valid_output_file)
 @click.option(
-    "-g",
-    "--group-file",
-    type=click.Path(exists=True, file_okay=True, dir_okay=False),
-    help="Group file path.",
-)
-@click.option(
-    "-o",
-    "--output-dir",
-    type=click.Path(dir_okay=True, file_okay=False),
-    help="Output file path. Default is the input file name with '_glytrait.xlsx' "
-    "suffix.",
-)
-@click.option(
-    "-m",
-    "--mode",
-    type=click.Choice(["structure", "composition", "S", "C"]),
-    default="structure",
-    help="Mode to run glyTrait, either 'structure' or 'composition'. "
-    "You can also use 'S' or 'C' for short. "
-    "Default is 'structure'.",
-)
-@click.option(
-    "-r",
-    "--filter-glycan-ratio",
-    type=click.FLOAT,
-    default=1,
-    help="Glycans with missing value ratio greater than this value will be filtered out.",
-)
-@click.option(
-    "-i",
-    "--impute-method",
-    type=click.Choice(["zero", "min", "lod", "mean", "median"]),
-    default="zero",
-    help="Method to impute missing values.",
-)
-@click.option(
-    "-l",
-    "--sia-linkage",
-    is_flag=True,
-    help="Include sialic acid linkage traits.",
+    "-s", "--sia_linkage", is_flag=True, help="Include sialic acid linkage traits."
 )
 @click.option(
     "-f",
-    "--formula-file",
+    "--formula_file",
     type=click.Path(exists=True),
     help="User formula file.",
+    callback=valid_formula_file,
 )
 @click.option(
-    "--filter/--no-filter",
-    default=True,
-    help="Filter out invalid derived traits. Default is filtering."
-    "Use --no-filter to disable filtering.",
-)
-@click.option(
-    "-c",
-    "--corr-threshold",
-    type=click.FLOAT,
-    default=1,
-    help="Threshold for correlation between traits. "
-    "Default is 1, which means only traits with perfect collinearity "
-    "will be filtered. Use -1 to disable filtering.",
-)
-@click.option(
-    "-b",
-    "--builtin-formulas",
+    "-t",
+    "--save_template",
     type=click.Path(),
-    callback=save_builtin_formulas_callback,
+    callback=save_template_callback,
     is_eager=True,
     expose_value=False,
     default=UNDIFINED,
-    help="The directory path to save a copy of the built-in formulas.",
+    help="Save a template for the user to fill in.",
 )
-@click.version_option()
-def cli(
-    abundance_file,
-    glycan_file,
-    group_file,
-    output_dir,
-    mode,
-    filter_glycan_ratio,
-    impute_method,
-    sia_linkage,
-    formula_file,
-    filter,
-    corr_threshold,
-):
-    """Run the glytrait workflow."""
-    if abundance_file is None:
-        msg = r"""
-Welcome to GlyTrait!
-
-   _____ _    _______        _ _   
-  / ____| |  |__   __|      (_) |  
- | |  __| |_   _| |_ __ __ _ _| |_ 
- | | |_ | | | | | | '__/ _` | | __|
- | |__| | | |_| | | | | (_| | | |_ 
-  \_____|_|\__, |_|_|  \__,_|_|\__|
-            __/ |                  
-           |___/                   
-
-Use `glytrait --help` for more information.
-"""
-        click.echo(msg)
-        return
+def cli(input_file, output_file, sia_linkage, formula_file):
+    """Run the glytrait workflow.
 
-    if output_dir is None:
-        output_dir = Path(abundance_file).with_name(
-            Path(abundance_file).stem + "_glytrait"
+    You can use the `--save_template` option to save the formula template
+    to the specified directory, then edit the template and
+    use it to provide additional traits to glyTrait.
+    """
+    if output_file is None:
+        output_file = str(
+            Path(input_file).with_name(Path(input_file).stem + "_glytrait.xlsx")
         )
-    Path(output_dir).mkdir(parents=True, exist_ok=True)
-    mode = "composition" if mode.lower() in ["c", "composition"] else "structure"
+    else:
+        Path(output_file).parent.mkdir(parents=True, exist_ok=True)
     try:
-        gt = GlyTrait(
-            mode=mode,
-            filter_max_na=filter_glycan_ratio,
-            impute_method=impute_method,
-            post_filtering=filter,
-            correlation_threshold=corr_threshold,
-            sia_linkage=sia_linkage,
-            custom_formula_file=formula_file,
-        )
-        gt.run(
-            output_dir=str(output_dir),
-            abundance_file=abundance_file,
-            glycan_file=glycan_file,
-            group_file=group_file,
-        )
+        run_workflow(input_file, output_file, sia_linkage, formula_file)
     except GlyTraitError as e:
         raise click.UsageError(str(e) + emoji.emojize(" :thumbs_down:"))
-    msg = f"Done :thumbs_up:! Output written to {output_dir}."
+    msg = f"Done :thumbs_up:! Output written to {output_file}."
     click.echo(emoji.emojize(msg))
 
 
+def run_workflow(
+    input_file: str,
+    output_file: str,
+    sia_linkage: bool = False,
+    user_formula_file: Optional[str] = None,
+) -> None:
+    """Run the workflow."""
+    glycans, abund_df = read_input(input_file)
+    formulas = load_formulas(user_formula_file)
+    if not sia_linkage:
+        formulas = [f for f in formulas if f.sia_linkage is False]
+    meta_prop_df = build_meta_property_table(abund_df.columns, glycans, sia_linkage)
+    derived_traits = calcu_derived_trait(abund_df, meta_prop_df, formulas)
+    direct_traits = calcu_direct_trait(abund_df)
+    write_output(output_file, derived_traits, direct_traits, meta_prop_df, formulas)
+
+
 if __name__ == "__main__":
     cli()
```

