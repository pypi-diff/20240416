# Comparing `tmp/cmem_cmemc-24.2.0rc1.tar.gz` & `tmp/cmem_cmemc-24.2.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmem_cmemc-24.2.0rc1.tar", max compression
+gzip compressed data, was "cmem_cmemc-24.2.0rc2.tar", max compression
```

## Comparing `cmem_cmemc-24.2.0rc1.tar` & `cmem_cmemc-24.2.0rc2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0    11357 2023-01-18 07:15:37.000000 cmem_cmemc-24.2.0rc1/LICENSE
--rw-r--r--   0        0        0      840 2023-08-15 09:56:56.000000 cmem_cmemc-24.2.0rc1/README-public.md
--rw-r--r--   0        0        0     5788 2024-02-19 15:45:18.770018 cmem_cmemc-24.2.0rc1/cmem_cmemc/__init__.py
--rw-r--r--   0        0        0     1326 2024-02-16 20:59:07.842060 cmem_cmemc-24.2.0rc1/cmem_cmemc/_cmemc.zsh
--rw-r--r--   0        0        0     3625 2024-02-16 20:59:07.842162 cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/__init__.py
--rw-r--r--   0        0        0    13769 2024-02-16 20:59:07.842299 cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/acl.py
--rw-r--r--   0        0        0     8657 2024-03-06 12:59:28.376102 cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/admin.py
--rw-r--r--   0        0        0     5039 2024-02-16 20:59:07.842505 cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/client.py
--rw-r--r--   0        0        0     5698 2024-02-16 20:59:07.842606 cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/config.py
--rw-r--r--   0        0        0    30225 2024-02-16 20:59:07.966011 cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/dataset.py
--rw-r--r--   0        0        0    27328 2024-02-16 20:59:07.966154 cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/graph.py
--rw-r--r--   0        0        0     7832 2024-02-16 20:59:07.842971 cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/metrics.py
--rw-r--r--   0        0        0    19267 2024-02-16 20:59:07.966266 cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/project.py
--rw-r--r--   0        0        0     9468 2024-02-16 20:59:07.966386 cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/python.py
--rw-r--r--   0        0        0    26791 2024-02-16 20:59:07.966498 cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/query.py
--rw-r--r--   0        0        0     7533 2024-02-16 20:59:07.843393 cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/resource.py
--rw-r--r--   0        0        0     8511 2024-02-16 20:59:07.843489 cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/scheduler.py
--rw-r--r--   0        0        0     6740 2024-02-16 20:59:07.843594 cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/store.py
--rw-r--r--   0        0        0    12287 2024-02-16 20:59:07.843695 cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/user.py
--rw-r--r--   0        0        0    22291 2024-03-06 16:43:53.713567 cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/validation.py
--rw-r--r--   0        0        0    11355 2024-02-16 20:59:07.843909 cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/variable.py
--rw-r--r--   0        0        0    16738 2024-02-16 20:59:07.966717 cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/vocabulary.py
--rw-r--r--   0        0        0    24649 2024-02-16 20:59:07.966835 cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/workflow.py
--rw-r--r--   0        0        0     4096 2024-02-16 20:59:07.844221 cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/workspace.py
--rw-r--r--   0        0        0    42010 2024-02-16 20:59:07.966968 cmem_cmemc-24.2.0rc1/cmem_cmemc/completion.py
--rw-r--r--   0        0        0      421 2024-02-16 20:59:07.844436 cmem_cmemc-24.2.0rc1/cmem_cmemc/constants.py
--rw-r--r--   0        0        0    17889 2024-03-06 16:43:32.717614 cmem_cmemc-24.2.0rc1/cmem_cmemc/context.py
--rw-r--r--   0        0        0      232 2024-02-16 20:59:07.844620 cmem_cmemc-24.2.0rc1/cmem_cmemc/exceptions.py
--rw-r--r--   0        0        0       43 2024-02-16 20:59:07.844720 cmem_cmemc-24.2.0rc1/cmem_cmemc/manual_helper/__init__.py
--rw-r--r--   0        0        0     3597 2024-02-16 20:59:07.844793 cmem_cmemc-24.2.0rc1/cmem_cmemc/manual_helper/graph.py
--rw-r--r--   0        0        0    12170 2024-02-16 20:59:07.967215 cmem_cmemc-24.2.0rc1/cmem_cmemc/manual_helper/multi_page.py
--rw-r--r--   0        0        0     1477 2024-02-16 20:59:07.844960 cmem_cmemc-24.2.0rc1/cmem_cmemc/manual_helper/single_page.py
--rw-r--r--   0        0        0    13255 2024-02-16 20:59:07.845090 cmem_cmemc-24.2.0rc1/cmem_cmemc/object_list.py
--rw-r--r--   0        0        0    10650 2024-02-16 20:59:07.967327 cmem_cmemc-24.2.0rc1/cmem_cmemc/utils.py
--rw-r--r--   0        0        0     3316 2024-03-06 18:35:27.601539 cmem_cmemc-24.2.0rc1/pyproject.toml
--rw-r--r--   0        0        0     2660 1970-01-01 00:00:00.000000 cmem_cmemc-24.2.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-01-18 07:15:37.000000 cmem_cmemc-24.2.0rc2/LICENSE
+-rw-r--r--   0        0        0      840 2023-08-15 09:56:56.000000 cmem_cmemc-24.2.0rc2/README-public.md
+-rw-r--r--   0        0        0     5788 2024-02-19 15:45:18.770018 cmem_cmemc-24.2.0rc2/cmem_cmemc/__init__.py
+-rw-r--r--   0        0        0     1326 2024-02-16 20:59:07.842060 cmem_cmemc-24.2.0rc2/cmem_cmemc/_cmemc.zsh
+-rw-r--r--   0        0        0     3625 2024-02-16 20:59:07.842162 cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/__init__.py
+-rw-r--r--   0        0        0    13769 2024-02-16 20:59:07.842299 cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/acl.py
+-rw-r--r--   0        0        0     8657 2024-03-06 12:59:28.376102 cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/admin.py
+-rw-r--r--   0        0        0     5039 2024-02-16 20:59:07.842505 cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/client.py
+-rw-r--r--   0        0        0     5698 2024-02-16 20:59:07.842606 cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/config.py
+-rw-r--r--   0        0        0    30225 2024-02-16 20:59:07.966011 cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/dataset.py
+-rw-r--r--   0        0        0    27328 2024-02-16 20:59:07.966154 cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/graph.py
+-rw-r--r--   0        0        0     7832 2024-02-16 20:59:07.842971 cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/metrics.py
+-rw-r--r--   0        0        0    19267 2024-02-16 20:59:07.966266 cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/project.py
+-rw-r--r--   0        0        0     9468 2024-02-16 20:59:07.966386 cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/python.py
+-rw-r--r--   0        0        0    26791 2024-02-16 20:59:07.966498 cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/query.py
+-rw-r--r--   0        0        0     7533 2024-02-16 20:59:07.843393 cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/resource.py
+-rw-r--r--   0        0        0     8511 2024-02-16 20:59:07.843489 cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/scheduler.py
+-rw-r--r--   0        0        0     6740 2024-02-16 20:59:07.843594 cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/store.py
+-rw-r--r--   0        0        0    12287 2024-02-16 20:59:07.843695 cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/user.py
+-rw-r--r--   0        0        0    26604 2024-03-08 13:46:17.357493 cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/validation.py
+-rw-r--r--   0        0        0    11355 2024-02-16 20:59:07.843909 cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/variable.py
+-rw-r--r--   0        0        0    16738 2024-02-16 20:59:07.966717 cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/vocabulary.py
+-rw-r--r--   0        0        0    24649 2024-02-16 20:59:07.966835 cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/workflow.py
+-rw-r--r--   0        0        0     4096 2024-02-16 20:59:07.844221 cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/workspace.py
+-rw-r--r--   0        0        0    42010 2024-02-16 20:59:07.966968 cmem_cmemc-24.2.0rc2/cmem_cmemc/completion.py
+-rw-r--r--   0        0        0      421 2024-02-16 20:59:07.844436 cmem_cmemc-24.2.0rc2/cmem_cmemc/constants.py
+-rw-r--r--   0        0        0    17889 2024-03-06 18:36:14.580149 cmem_cmemc-24.2.0rc2/cmem_cmemc/context.py
+-rw-r--r--   0        0        0      232 2024-02-16 20:59:07.844620 cmem_cmemc-24.2.0rc2/cmem_cmemc/exceptions.py
+-rw-r--r--   0        0        0       43 2024-02-16 20:59:07.844720 cmem_cmemc-24.2.0rc2/cmem_cmemc/manual_helper/__init__.py
+-rw-r--r--   0        0        0     3597 2024-02-16 20:59:07.844793 cmem_cmemc-24.2.0rc2/cmem_cmemc/manual_helper/graph.py
+-rw-r--r--   0        0        0    12170 2024-02-16 20:59:07.967215 cmem_cmemc-24.2.0rc2/cmem_cmemc/manual_helper/multi_page.py
+-rw-r--r--   0        0        0     1477 2024-02-16 20:59:07.844960 cmem_cmemc-24.2.0rc2/cmem_cmemc/manual_helper/single_page.py
+-rw-r--r--   0        0        0    13255 2024-02-16 20:59:07.845090 cmem_cmemc-24.2.0rc2/cmem_cmemc/object_list.py
+-rw-r--r--   0        0        0    10650 2024-02-16 20:59:07.967327 cmem_cmemc-24.2.0rc2/cmem_cmemc/utils.py
+-rw-r--r--   0        0        0     3316 2024-03-08 13:51:19.418475 cmem_cmemc-24.2.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     2660 1970-01-01 00:00:00.000000 cmem_cmemc-24.2.0rc2/PKG-INFO
```

### Comparing `cmem_cmemc-24.2.0rc1/LICENSE` & `cmem_cmemc-24.2.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-24.2.0rc1/README-public.md` & `cmem_cmemc-24.2.0rc2/README-public.md`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-24.2.0rc1/cmem_cmemc/__init__.py` & `cmem_cmemc-24.2.0rc2/cmem_cmemc/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-24.2.0rc1/cmem_cmemc/_cmemc.zsh` & `cmem_cmemc-24.2.0rc2/cmem_cmemc/_cmemc.zsh`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/__init__.py` & `cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/acl.py` & `cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/acl.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/admin.py` & `cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/admin.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/client.py` & `cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/client.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/config.py` & `cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/config.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/dataset.py` & `cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/dataset.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/graph.py` & `cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/graph.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/metrics.py` & `cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/metrics.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/project.py` & `cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/project.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/python.py` & `cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/python.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/query.py` & `cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/query.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/resource.py` & `cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/resource.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/scheduler.py` & `cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/scheduler.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/store.py` & `cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/store.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/user.py` & `cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/user.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/validation.py` & `cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/validation.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 """graph validation command group"""
+import json
+import sys
 import time
+from collections import Counter
 from datetime import UTC, datetime
+from pathlib import Path
 
 import click
 import requests
 import timeago
 from click import Context, UsageError
 from click.shell_completion import CompletionItem
 from cmem.cmempy.dp.shacl import validation
@@ -23,32 +27,67 @@
     ObjectList,
     compare_int_greater_than,
     transform_lower,
 )
 from cmem_cmemc.utils import struct_to_table
 
 
-def _report_to_junit(report: dict) -> str:
-    """Create a jUnit XML document from a report dictionary"""
-    test_cases: list[TestCase] = []
-
-    for result in report["results"]:
-        resource_iri = result["resourceIri"]
-        for _ in result["violations"]:
-            constraint_name = _["reportEntryConstraintMessageTemplate"]["constraintName"]
-            message = _["messages"][0]["value"]
-            new_case = TestCase(
-                name=f"{constraint_name} @ {resource_iri}",
-                url=resource_iri,
-                stdout=message,
-                category=_["severity"],
+def _reports_to_junit(reports: list[dict]) -> str:
+    """Create a jUnit XML document from a list of report dictionaries"""
+    test_suites: list[TestSuite] = []
+
+    for report in reports:
+        test_cases: list[TestCase] = []
+        context_graph = report["contextGraphIri"]
+        shape_graph = report["shapeGraphIri"]
+        time_elapsed = (report["executionFinished"] - report["executionStarted"]) / 1000
+        violations: dict[str, list[dict]] = {}
+        for resource in sorted(report["resources"]):
+            # get a list of all tested resources
+            violations[resource] = []
+        average_elapsed_sec = time_elapsed / len(violations)
+        for result in report["results"]:
+            # collection violations per resource
+            resource_iri = result["resourceIri"]
+            violations[resource_iri] = result["violations"]
+        for resource in violations:
+            # create on test case per resource
+            resource_violations = violations[resource]
+            violations_count = len(violations[resource])
+            constraints = Counter(
+                _["reportEntryConstraintMessageTemplate"]["constraintName"]
+                for _ in resource_violations
+            )
+            test_case_name = f"{resource}"
+            if violations_count == 0:
+                test_case_name += " has no violations"
+            if violations_count == 1:
+                test_case_name += f" has 1 violation ({next(iter(constraints.keys()))})"
+            if violations_count > 1:
+                constrains_str = ""
+                for constraint, constraint_count in constraints.items():
+                    constrains_str += f", {constraint_count}x{constraint}"
+                test_case_name += f" has {violations_count} violations ({constrains_str[2:]})"
+
+            test_case = TestCase(
+                name=test_case_name,
+                classname=f"{context_graph} tested with {shape_graph}",
+                elapsed_sec=average_elapsed_sec,
             )
-            test_cases.append(new_case)
-    test_suite = TestSuite("eccenca Corporate Memory Graph Validation", test_cases)
-    return str(to_xml_report_string([test_suite], encoding="utf-8"))
+            if violations_count > 0:
+                test_case.add_failure_info(output=json.dumps(resource_violations, indent=2))
+            test_cases.append(test_case)
+        test_suite = TestSuite(
+            name=f"Testing {context_graph} with shapes from {shape_graph}.",
+            test_cases=test_cases,
+            id=report["id"],
+            timestamp=report["executionFinished"],
+        )
+        test_suites.append(test_suite)
+    return str(to_xml_report_string(test_suites, encoding="utf-8"))
 
 
 def get_sorted_validations_list(ctx: Context) -> list[dict]:  # noqa: ARG001
     """Get a sorted list of validation objects (aggregations)"""
     objects = validation.get_all_aggregations()
     return sorted(objects, key=lambda o: str(o.get("executionStarted", "SCHEDULED")))
 
@@ -195,14 +234,28 @@
         _get_batch_validation_option(_)
         for _ in validation.get_all_aggregations()
         if _["state"] == validation.STATUS_RUNNING
     ]
     return _finalize_completion(candidates=options, incomplete=incomplete)
 
 
+def _complete_finished_batch_validations(
+    ctx: click.Context,  # noqa: ARG001
+    param: click.Argument,  # noqa: ARG001
+    incomplete: str,
+) -> list[CompletionItem]:
+    """Provide completion for finished batch validations"""
+    options = [
+        _get_batch_validation_option(_)
+        for _ in validation.get_all_aggregations()
+        if _["state"] == validation.STATUS_FINISHED
+    ]
+    return _finalize_completion(candidates=options, incomplete=incomplete)
+
+
 def show_process_summary(app: ApplicationContext, process_id: str) -> None:
     """Show summary of the validation process"""
     app.echo_info_table(
         struct_to_table(validation.get_aggregation(batch_id=process_id)),
         headers=["Key", "Value"],
         sort_column=0,
         caption="Validation Summary",
@@ -549,48 +602,99 @@
             )
     app.echo_info(f"Graph validation process with ID {process_id} ... ", nl=False)
     validation.cancel(batch_id=process_id)
     app.echo_success("cancelled")
 
 
 @click.command(cls=CmemcCommand, name="export")
-@click.argument("process_id", type=click.STRING, shell_complete=_complete_all_batch_validations)
+@click.argument(
+    "process_ids", nargs=-1, type=click.STRING, shell_complete=_complete_finished_batch_validations
+)
+@click.option(
+    "--output-file",
+    type=click.Path(writable=True, allow_dash=False, dir_okay=False),
+    default="report.xml",
+    show_default=True,
+    help="Export the report to this file. Existing files will be overwritten.",
+)
+@click.option(
+    "--exit-1",
+    type=click.Choice(["never", "error"]),
+    default="error",
+    show_default=True,
+    help="Specify, when this command returns with exit code 1. Available options are "
+    "'never' (exit 0, even if there are violations in the reports), "
+    "'error' (exit 1 if there is at least one violation in a report).), ",
+)
 @click.option(
     "--format",
     "format_",
     type=click.Choice(["JSON", "XML"], case_sensitive=True),
-    default="JSON",
+    default="XML",
     help="Export either the plain JSON report or a distilled jUnit XML report.",
     show_default=True,
 )
 @click.pass_context
-def export_command(ctx: Context, process_id: str, format_: str) -> None:
-    """Export the report of a finished validation process to a file.
+def export_command(
+    ctx: Context, process_ids: tuple[str], output_file: str, exit_1: str, format_: str
+) -> None:
+    """Export a report of finished validation processes to a file.
 
-    This command exports JSON documents or jUnit XML reports in order to process
+    This command exports a jUnit XML or JSON report in order to process
     them somewhere else (e.g. a CI pipeline).
 
+    You can export a single report of multiple validation processes.
+
+    For jUnit XML: Each validation process result will be transformed to
+    a single test suite. All violations of one resource in a result will be
+    collected and attached to a single test case in that test suite.
+
     Note: Validation processes IDs can be listed with the `graph validation list`
     command, or by utilizing the tab completion of this command.
     """
+    if len(process_ids) == 0:
+        raise UsageError("This command needs at least one validation process ID.")
     app: ApplicationContext = ctx.obj
-    process = None
+    process_ids_to_test = {_: True for _ in process_ids}
+    overall_violations = 0
+    overall_resources = 0
     for _ in validation.get_all_aggregations():
-        if _["id"] == process_id:
-            process = _
-    if process is None:
-        raise UsageError(f"Validation process with ID '{process_id}' is not known (anymore).")
-    if process["state"] != "FINISHED":
-        raise UsageError(f"Validation process with ID '{process_id}' is still running.")
-
-    report = validation.get(batch_id=process_id)
-    if format_ == "JSON":
-        app.echo_info_json(report)
-    if format_ == "XML":
-        app.echo_info_xml(_report_to_junit(report))
+        if _["id"] in process_ids_to_test:
+            if _["state"] != "FINISHED":
+                raise UsageError(f"Validation process with ID '{_['id']}' is still running.")
+            del process_ids_to_test[_["id"]]
+            overall_violations += int(_["violationsCount"])
+            overall_resources += int(_["resourceProcessedCount"])
+    if len(process_ids_to_test) > 0:
+        raise UsageError(
+            "Validation processes with the following IDs not known (anymore): "
+            + ", ".join(process_ids_to_test)
+        )
+    reports = []
+    for process_id in process_ids:
+        report = validation.get(batch_id=process_id)
+        reports.append(report)
+    app.echo_info(
+        f"Export of {len(reports)} validation report(s) with"
+        f" {overall_violations} violations in {overall_resources} resources"
+        f" to {output_file} ... ",
+        nl=False,
+    )
+    with Path(output_file, mode="w", encoding="utf-8") as file:
+        if format_ == "XML":
+            file.write_text(_reports_to_junit(reports))
+        if format_ == "JSON":
+            file.write_text(json.dumps(reports, indent=2))
+    app.echo_success("done")
+    if exit_1 == "error" and overall_violations > 0:
+        app.echo_error(
+            "Exit 1 since violations where found in the reports "
+            "(can be suppressed with '--exit-1 never')."
+        )
+        sys.exit(1)
 
 
 @click.group(cls=CmemcGroup, name="validation")
 def validation_group() -> CmemcGroup:  # type: ignore[empty-body]
     """Validate resources in a graph.
 
     This command group is dedicated to the management of resource validation processes.
```

### Comparing `cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/variable.py` & `cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/variable.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/vocabulary.py` & `cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/vocabulary.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/workflow.py` & `cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/workflow.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-24.2.0rc1/cmem_cmemc/commands/workspace.py` & `cmem_cmemc-24.2.0rc2/cmem_cmemc/commands/workspace.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-24.2.0rc1/cmem_cmemc/completion.py` & `cmem_cmemc-24.2.0rc2/cmem_cmemc/completion.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-24.2.0rc1/cmem_cmemc/context.py` & `cmem_cmemc-24.2.0rc2/cmem_cmemc/context.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-24.2.0rc1/cmem_cmemc/manual_helper/graph.py` & `cmem_cmemc-24.2.0rc2/cmem_cmemc/manual_helper/graph.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-24.2.0rc1/cmem_cmemc/manual_helper/multi_page.py` & `cmem_cmemc-24.2.0rc2/cmem_cmemc/manual_helper/multi_page.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-24.2.0rc1/cmem_cmemc/manual_helper/single_page.py` & `cmem_cmemc-24.2.0rc2/cmem_cmemc/manual_helper/single_page.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-24.2.0rc1/cmem_cmemc/object_list.py` & `cmem_cmemc-24.2.0rc2/cmem_cmemc/object_list.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-24.2.0rc1/cmem_cmemc/utils.py` & `cmem_cmemc-24.2.0rc2/cmem_cmemc/utils.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-24.2.0rc1/pyproject.toml` & `cmem_cmemc-24.2.0rc2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmem-cmemc"
-version = "24.2.0rc1"
+version = "24.2.0rc2"
 description = "Command line client for eccenca Corporate Memory"
 license = "Apache 2.0"
 classifiers = ["Development Status :: 5 - Production/Stable", "Intended Audience :: Developers", "Intended Audience :: Science/Research", "Intended Audience :: System Administrators", "License :: OSI Approved :: Apache Software License", "Programming Language :: Python :: 3.9", "Topic :: Software Development :: Testing", "Topic :: Database", "Topic :: Utilities"]
 homepage = "https://eccenca.com/go/cmemc"
 authors = ["eccenca <cmempy-developer@eccenca.com>", "Sebastian Tramp <sebastian.tramp@eccenca.com>"]
 readme = "README-public.md"
```

### Comparing `cmem_cmemc-24.2.0rc1/PKG-INFO` & `cmem_cmemc-24.2.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmem-cmemc
-Version: 24.2.0rc1
+Version: 24.2.0rc2
 Summary: Command line client for eccenca Corporate Memory
 Home-page: https://eccenca.com/go/cmemc
 License: Apache 2.0
 Author: eccenca
 Author-email: cmempy-developer@eccenca.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

