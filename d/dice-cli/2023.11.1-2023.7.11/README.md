# Comparing `tmp/dice_cli-2023.11.1.tar.gz` & `tmp/dice_cli-2023.7.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dice_cli-2023.11.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "dice_cli-2023.7.11.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `dice_cli-2023.11.1.tar` & `dice_cli-2023.7.11.tar`

### file list

```diff
@@ -1,39 +1,38 @@
--rw-r--r--   0        0        0     1522 2024-04-16 15:04:37.021726 dice_cli-2023.11.1/LICENSE
--rw-r--r--   0        0        0     3558 2024-04-16 15:04:37.021726 dice_cli-2023.11.1/README.md
--rw-r--r--   0        0        0     2487 2024-04-16 15:04:37.021726 dice_cli-2023.11.1/pyproject.toml
--rw-r--r--   0        0        0       54 2024-04-16 15:04:37.021726 dice_cli-2023.11.1/src/dice_cli/__init__.py
--rw-r--r--   0        0        0     1501 2024-04-16 15:04:37.021726 dice_cli-2023.11.1/src/dice_cli/_date.py
--rw-r--r--   0        0        0      279 2024-04-16 15:04:37.021726 dice_cli-2023.11.1/src/dice_cli/_io/__init__.py
--rw-r--r--   0        0        0     1172 2024-04-16 15:04:37.021726 dice_cli-2023.11.1/src/dice_cli/_io/_csv.py
--rw-r--r--   0        0        0      655 2024-04-16 15:04:37.021726 dice_cli-2023.11.1/src/dice_cli/_io/_remote.py
--rw-r--r--   0        0        0      953 2024-04-16 15:04:37.021726 dice_cli-2023.11.1/src/dice_cli/admin/__init__.py
--rw-r--r--   0        0        0     1256 2024-04-16 15:04:37.021726 dice_cli-2023.11.1/src/dice_cli/admin/_print_unused_id_ranges.py
--rw-r--r--   0        0        0      902 2024-04-16 15:04:37.021726 dice_cli-2023.11.1/src/dice_cli/admin/_print_used_id_ranges.py
--rw-r--r--   0        0        0     1547 2024-04-16 15:04:37.021726 dice_cli-2023.11.1/src/dice_cli/admin/_scan_groups_and_users.py
--rw-r--r--   0        0        0      777 2024-04-16 15:04:37.021726 dice_cli-2023.11.1/src/dice_cli/admin/deploy/__init__.py
--rw-r--r--   0        0        0     2659 2024-04-16 15:04:37.021726 dice_cli-2023.11.1/src/dice_cli/admin/deploy/_hdfs_mount.py
--rw-r--r--   0        0        0     2783 2024-04-16 15:04:37.021726 dice_cli-2023.11.1/src/dice_cli/admin/investigate/__init__.py
--rw-r--r--   0        0        0     8573 2024-04-16 15:04:37.025726 dice_cli-2023.11.1/src/dice_cli/admin/report/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 15:04:37.025726 dice_cli-2023.11.1/src/dice_cli/admin/report/_consistency_check_grid.py
--rw-r--r--   0        0        0      735 2024-04-16 15:04:37.025726 dice_cli-2023.11.1/src/dice_cli/admin/report/_dns.py
--rw-r--r--   0        0        0     5004 2024-04-16 15:04:37.025726 dice_cli-2023.11.1/src/dice_cli/admin/report/_inventory.py
--rw-r--r--   0        0        0     3845 2024-04-16 15:04:37.025726 dice_cli-2023.11.1/src/dice_cli/admin/report/_network.py
--rw-r--r--   0        0        0     1994 2024-04-16 15:04:37.025726 dice_cli-2023.11.1/src/dice_cli/admin/report/_resources.py
--rw-r--r--   0        0        0     1122 2024-04-16 15:04:37.025726 dice_cli-2023.11.1/src/dice_cli/admin/report/_storage.py
--rw-r--r--   0        0        0     1015 2024-04-16 15:04:37.025726 dice_cli-2023.11.1/src/dice_cli/benchmark/__init__.py
--rw-r--r--   0        0        0      173 2024-04-16 15:04:37.025726 dice_cli-2023.11.1/src/dice_cli/cache.py
--rw-r--r--   0        0        0     1670 2024-04-16 15:04:37.025726 dice_cli-2023.11.1/src/dice_cli/check/__init__.py
--rw-r--r--   0        0        0     1783 2024-04-16 15:04:37.025726 dice_cli-2023.11.1/src/dice_cli/check/_environment.py
--rw-r--r--   0        0        0     1138 2024-04-16 15:04:37.025726 dice_cli-2023.11.1/src/dice_cli/dicectl.py
--rw-r--r--   0        0        0      268 2024-04-16 15:04:37.025726 dice_cli-2023.11.1/src/dice_cli/docs/__init__.py
--rw-r--r--   0        0        0     1044 2024-04-16 15:04:37.025726 dice_cli-2023.11.1/src/dice_cli/fs/__init__.py
--rw-r--r--   0        0        0      196 2024-04-16 15:04:37.025726 dice_cli-2023.11.1/src/dice_cli/fs/_copy_from_local.py
--rw-r--r--   0        0        0     1964 2024-04-16 15:04:37.025726 dice_cli-2023.11.1/src/dice_cli/info/__init__.py
--rw-r--r--   0        0        0      359 2024-04-16 15:04:37.025726 dice_cli-2023.11.1/src/dice_cli/job/__init__.py
--rw-r--r--   0        0        0     2459 2024-04-16 15:04:37.025726 dice_cli-2023.11.1/src/dice_cli/logger.py
--rw-r--r--   0        0        0     4166 2024-04-16 15:04:37.025726 dice_cli-2023.11.1/src/dice_cli/main.py
--rw-r--r--   0        0        0        0 2024-04-16 15:04:37.025726 dice_cli-2023.11.1/src/dice_cli/migrate/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 15:04:37.025726 dice_cli-2023.11.1/src/dice_cli/py.typed
--rw-r--r--   0        0        0        0 2024-04-16 15:04:37.025726 dice_cli-2023.11.1/src/dice_cli/restore/__init__.py
--rw-r--r--   0        0        0       81 2024-04-16 15:04:37.025726 dice_cli-2023.11.1/src/dice_cli/sync/__init__.py
--rw-r--r--   0        0        0     5266 1970-01-01 00:00:00.000000 dice_cli-2023.11.1/PKG-INFO
+-rw-r--r--   0        0        0     1522 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/LICENSE
+-rw-r--r--   0        0        0     3558 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/README.md
+-rw-r--r--   0        0        0     2482 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/pyproject.toml
+-rw-r--r--   0        0        0       55 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/__init__.py
+-rw-r--r--   0        0        0     1501 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/_date.py
+-rw-r--r--   0        0        0      279 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/_io/__init__.py
+-rw-r--r--   0        0        0     1172 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/_io/_csv.py
+-rw-r--r--   0        0        0      655 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/_io/_remote.py
+-rw-r--r--   0        0        0      953 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/admin/__init__.py
+-rw-r--r--   0        0        0     1256 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/admin/_print_unused_id_ranges.py
+-rw-r--r--   0        0        0      902 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/admin/_print_used_id_ranges.py
+-rw-r--r--   0        0        0     1547 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/admin/_scan_groups_and_users.py
+-rw-r--r--   0        0        0      777 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/admin/deploy/__init__.py
+-rw-r--r--   0        0        0     2659 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/admin/deploy/_hdfs_mount.py
+-rw-r--r--   0        0        0     2783 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/admin/investigate/__init__.py
+-rw-r--r--   0        0        0     6411 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/admin/report/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/admin/report/_consistency_check_grid.py
+-rw-r--r--   0        0        0      735 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/admin/report/_dns.py
+-rw-r--r--   0        0        0     4942 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/admin/report/_inventory.py
+-rw-r--r--   0        0        0     3845 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/admin/report/_network.py
+-rw-r--r--   0        0        0     1122 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/admin/report/_storage.py
+-rw-r--r--   0        0        0     1015 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/benchmark/__init__.py
+-rw-r--r--   0        0        0      173 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/cache.py
+-rw-r--r--   0        0        0     1670 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/check/__init__.py
+-rw-r--r--   0        0        0     1783 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/check/_environment.py
+-rw-r--r--   0        0        0     1138 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/dicectl.py
+-rw-r--r--   0        0        0      268 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/docs/__init__.py
+-rw-r--r--   0        0        0     1044 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/fs/__init__.py
+-rw-r--r--   0        0        0      196 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/fs/_copy_from_local.py
+-rw-r--r--   0        0        0     1964 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/info/__init__.py
+-rw-r--r--   0        0        0      359 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/job/__init__.py
+-rw-r--r--   0        0        0     2459 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/logger.py
+-rw-r--r--   0        0        0     4166 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/main.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/migrate/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/py.typed
+-rw-r--r--   0        0        0        0 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/restore/__init__.py
+-rw-r--r--   0        0        0       81 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/sync/__init__.py
+-rw-r--r--   0        0        0     5261 1970-01-01 00:00:00.000000 dice_cli-2023.7.11/PKG-INFO
```

### Comparing `dice_cli-2023.11.1/LICENSE` & `dice_cli-2023.7.11/LICENSE`

 * *Files identical despite different names*

### Comparing `dice_cli-2023.11.1/README.md` & `dice_cli-2023.7.11/README.md`

 * *Files identical despite different names*

### Comparing `dice_cli-2023.11.1/pyproject.toml` & `dice_cli-2023.7.11/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
   "Development Status :: 1 - Planning",
 ]
 
 
 dynamic = ["version"]
 dependencies = [
   "colorama >=0.4.0",
-  "dice-lib >=2024.04.01",
+  "dice-lib >=0.5.0",
   "diskcache >=5.4.0",
   "htcondor >=9.0.0",
   "plumbum >=1.7.2",
   "prettytable >=3.2.0",
   "tabulate >=0.8.9",
   "tqdm < 5.0.0",
   "typer >=0.4.0",
```

### Comparing `dice_cli-2023.11.1/src/dice_cli/_date.py` & `dice_cli-2023.7.11/src/dice_cli/_date.py`

 * *Files identical despite different names*

### Comparing `dice_cli-2023.11.1/src/dice_cli/_io/_csv.py` & `dice_cli-2023.7.11/src/dice_cli/_io/_csv.py`

 * *Files identical despite different names*

### Comparing `dice_cli-2023.11.1/src/dice_cli/_io/_remote.py` & `dice_cli-2023.7.11/src/dice_cli/_io/_remote.py`

 * *Files identical despite different names*

### Comparing `dice_cli-2023.11.1/src/dice_cli/admin/__init__.py` & `dice_cli-2023.7.11/src/dice_cli/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `dice_cli-2023.11.1/src/dice_cli/admin/_print_unused_id_ranges.py` & `dice_cli-2023.7.11/src/dice_cli/admin/_print_unused_id_ranges.py`

 * *Files identical despite different names*

### Comparing `dice_cli-2023.11.1/src/dice_cli/admin/_print_used_id_ranges.py` & `dice_cli-2023.7.11/src/dice_cli/admin/_print_used_id_ranges.py`

 * *Files identical despite different names*

### Comparing `dice_cli-2023.11.1/src/dice_cli/admin/_scan_groups_and_users.py` & `dice_cli-2023.7.11/src/dice_cli/admin/_scan_groups_and_users.py`

 * *Files identical despite different names*

### Comparing `dice_cli-2023.11.1/src/dice_cli/admin/deploy/__init__.py` & `dice_cli-2023.7.11/src/dice_cli/admin/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `dice_cli-2023.11.1/src/dice_cli/admin/deploy/_hdfs_mount.py` & `dice_cli-2023.7.11/src/dice_cli/admin/deploy/_hdfs_mount.py`

 * *Files identical despite different names*

### Comparing `dice_cli-2023.11.1/src/dice_cli/admin/investigate/__init__.py` & `dice_cli-2023.7.11/src/dice_cli/admin/investigate/__init__.py`

 * *Files identical despite different names*

### Comparing `dice_cli-2023.11.1/src/dice_cli/admin/report/__init__.py` & `dice_cli-2023.7.11/src/dice_cli/admin/report/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from pathlib import Path
 from typing import List, Optional, cast
 
-import pandas as pd
 import typer
 from dice_lib.date import current_formatted_date
 from tabulate import tabulate
 
 from dice_cli._io import (
     read_list_data_from_csv,
     write_list_data_as_dict_to_csv,
@@ -35,47 +34,35 @@
         "--output",
         help="Output file",
     ),
     resolve_usernames: bool = typer.Option(False, "--resolve-usernames"),
     print_to_console: bool = typer.Option(
         False, "--print", help="Print to console instead of output file"
     ),
-    no_summary: bool = typer.Option(False, "--no-summary", help="Do not print summary"),
 ) -> None:
     """
     Generate a report of the storage usage of the given paths.
 
     :param paths: The paths to generate the report for.
-    :param output_file: The file to write the report to.
+    :param output_directory: The directory to write the report to.
     :param resolve_usernames: Whether to resolve usernames to their real names.
     """
     if not output_file and not print_to_console:
         today = current_formatted_date()
         output_file = Path(f"/tmp/{today}_dice_admin_storage_report.csv")
 
     headers, report = generate_storage_report(paths, resolve_usernames)
     if not print_to_console:
         write_list_data_to_csv(report, headers, cast(Path, output_file))
         admin_logger.info(f"Report saved to {output_file}")
     else:
         admin_logger.info(tabulate(report, headers=headers, tablefmt="psql"))
 
-    if no_summary:
-        # TODO: move functionality to separate function
-        # Produce summary for the top 5 users
-        # sort by "Size [B]" descending
-        df = pd.DataFrame(report, columns=headers)
-        df["Size [B]"] = df["Size [B]"].astype(int)
-        df = df.sort_values(by=["Size [B]"], ascending=False)
-        df["Size [human-readable]"] = df["Size [human-readable]"].astype(str)
-
-        admin_logger.info("Summary for top 5 users:")
-        admin_logger.info(
-            tabulate(df.head(5), headers=headers, tablefmt="psql", showindex=False)
-        )
+    headers, report = generate_storage_report(paths, resolve_usernames)
+    write_list_data_to_csv(report, headers, cast(Path, output_file))
 
 
 @app.command()
 def consistency_check_grid(
     grid_endpoint: str = typer.Argument(...),
     storage_endpoint: str = typer.Argument(...),
     output_file: Optional[Path] = typer.Option(
@@ -196,55 +183,7 @@
         write_list_data_to_csv(dns_report, headers, cast(Path, output_file))
         admin_logger.info(f"Report saved to {output_file}")
     else:
         admin_logger.info(
             tabulate(dns_report, headers=headers, tablefmt="github"),
             extra={"markup": False},
         )
-
-
-@app.command()
-def resources(
-    host_inventory_file: Path = typer.Argument(...),
-    output_file: Optional[Path] = typer.Option(
-        None,
-        "-o",
-        "--output",
-        help="Output file",
-    ),
-    print_to_console: bool = typer.Option(
-        False, "--print", help="Print to console instead of output file"
-    ),
-    group: str = typer.Option(
-        "htcondor_workers",
-        "--group",
-        help="Group of hosts to generate report for",
-    ),
-) -> None:
-    """
-    Generate a report of the resources of the given hosts.
-    """
-    if not output_file and not print_to_console:
-        today = current_formatted_date()
-        output_file = Path(f"/tmp/{today}_dice_admin_resources_report.csv")
-
-    admin_logger.warning(":construction: Work in progress :construction:")
-    from ._resources import _resources_report
-
-    # the inventory file is a csv file with columns defined in _inventory.py
-    # we are only interested in the FQDN column for "Description/Purpose"==group
-    df = pd.read_csv(host_inventory_file)
-    if group == "all":
-        hosts = df["FQDN"].tolist()
-    else:
-        htcondor_workers = df[df["Description/Purpose"] == group]
-    hosts = htcondor_workers["FQDN"].tolist()
-
-    headers, resources_report = _resources_report(hosts)
-    if not print_to_console:
-        write_list_data_to_csv(resources_report, headers, cast(Path, output_file))
-        admin_logger.info(f"Report saved to {output_file}")
-    else:
-        admin_logger.info(
-            tabulate(resources_report, headers=headers, tablefmt="github"),
-            extra={"markup": False},
-        )
```

### Comparing `dice_cli-2023.11.1/src/dice_cli/admin/report/_dns.py` & `dice_cli-2023.7.11/src/dice_cli/admin/report/_dns.py`

 * *Files identical despite different names*

### Comparing `dice_cli-2023.11.1/src/dice_cli/admin/report/_inventory.py` & `dice_cli-2023.7.11/src/dice_cli/admin/report/_inventory.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 ]
 
 
 @admin_cache.memoize(expire=60 * 60, tag="inventory._get_host_info")
 def _get_host_info(ipv4_address: str, user: str) -> Dict[str, str]:
     admin_logger.debug(f"Getting host info for {ipv4_address}")
     # TODO: find a way to do all below as a single command
-    # NOTE: this is a good candidate for the DICE API service
     with SshMachine(ipv4_address, user=user, keyfile=None) as rem:
         puppet_agent = rem["puppet"]["agent"]
         facter = rem["facter"]
 
         hostname = rem["hostname"]("-s")
         domain = rem["hostname"]("-d")
         cnames = ",".join(set(rem["hostname"]("-A").split(" ")))
```

### Comparing `dice_cli-2023.11.1/src/dice_cli/admin/report/_network.py` & `dice_cli-2023.7.11/src/dice_cli/admin/report/_network.py`

 * *Files identical despite different names*

### Comparing `dice_cli-2023.11.1/src/dice_cli/admin/report/_storage.py` & `dice_cli-2023.7.11/src/dice_cli/admin/report/_storage.py`

 * *Files identical despite different names*

### Comparing `dice_cli-2023.11.1/src/dice_cli/benchmark/__init__.py` & `dice_cli-2023.7.11/src/dice_cli/benchmark/__init__.py`

 * *Files identical despite different names*

### Comparing `dice_cli-2023.11.1/src/dice_cli/check/__init__.py` & `dice_cli-2023.7.11/src/dice_cli/check/__init__.py`

 * *Files identical despite different names*

### Comparing `dice_cli-2023.11.1/src/dice_cli/check/_environment.py` & `dice_cli-2023.7.11/src/dice_cli/check/_environment.py`

 * *Files identical despite different names*

### Comparing `dice_cli-2023.11.1/src/dice_cli/dicectl.py` & `dice_cli-2023.7.11/src/dice_cli/dicectl.py`

 * *Files identical despite different names*

### Comparing `dice_cli-2023.11.1/src/dice_cli/fs/__init__.py` & `dice_cli-2023.7.11/src/dice_cli/fs/__init__.py`

 * *Files identical despite different names*

### Comparing `dice_cli-2023.11.1/src/dice_cli/info/__init__.py` & `dice_cli-2023.7.11/src/dice_cli/info/__init__.py`

 * *Files identical despite different names*

### Comparing `dice_cli-2023.11.1/src/dice_cli/logger.py` & `dice_cli-2023.7.11/src/dice_cli/logger.py`

 * *Files identical despite different names*

### Comparing `dice_cli-2023.11.1/src/dice_cli/main.py` & `dice_cli-2023.7.11/src/dice_cli/main.py`

 * *Files identical despite different names*

### Comparing `dice_cli-2023.11.1/PKG-INFO` & `dice_cli-2023.7.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dice_cli
-Version: 2023.11.1
+Version: 2023.7.11
 Summary: Command-line interface for DICE
 Author-email: Luke Kreczko <kreczko@cern.ch>
 Maintainer-email: The UoB DICE team <lcg-admin@bristol.ac.uk>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering
@@ -14,15 +14,15 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 1 - Planning
 Requires-Dist: colorama >=0.4.0
-Requires-Dist: dice-lib >=2024.04.01
+Requires-Dist: dice-lib >=0.5.0
 Requires-Dist: diskcache >=5.4.0
 Requires-Dist: htcondor >=9.0.0
 Requires-Dist: plumbum >=1.7.2
 Requires-Dist: prettytable >=3.2.0
 Requires-Dist: tabulate >=0.8.9
 Requires-Dist: tqdm < 5.0.0
 Requires-Dist: typer >=0.4.0
```

