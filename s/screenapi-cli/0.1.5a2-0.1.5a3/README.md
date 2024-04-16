# Comparing `tmp/screenapi_cli-0.1.5a2.tar.gz` & `tmp/screenapi_cli-0.1.5a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screenapi_cli-0.1.5a2.tar", max compression
+gzip compressed data, was "screenapi_cli-0.1.5a3.tar", max compression
```

## Comparing `screenapi_cli-0.1.5a2.tar` & `screenapi_cli-0.1.5a3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1092 2024-03-23 16:06:49.120124 screenapi_cli-0.1.5a2/LICENSE
--rw-r--r--   0        0        0     1381 2024-03-25 19:41:34.179648 screenapi_cli-0.1.5a2/README.md
--rw-r--r--   0        0        0        0 2024-03-26 06:15:38.237432 screenapi_cli-0.1.5a2/app/__init__.py
--rw-r--r--   0        0        0     9241 2024-04-11 16:34:55.215188 screenapi_cli-0.1.5a2/app/__main__.py
--rw-r--r--   0        0        0     1360 2024-04-01 07:33:03.304661 screenapi_cli-0.1.5a2/app/common.py
--rw-r--r--   0        0        0        0 2024-03-24 18:09:29.678307 screenapi_cli-0.1.5a2/app/export/__init__.py
--rw-r--r--   0        0        0     1435 2024-03-26 08:34:32.751466 screenapi_cli-0.1.5a2/app/export/cli.py
--rw-r--r--   0        0        0        0 2024-03-24 14:33:45.903715 screenapi_cli-0.1.5a2/app/setup/__init__.py
--rw-r--r--   0        0        0     1083 2024-03-25 19:15:41.722738 screenapi_cli-0.1.5a2/app/setup/utils.py
--rw-r--r--   0        0        0       97 2024-03-24 17:32:30.550768 screenapi_cli-0.1.5a2/app/txt/__init__.py
--rw-r--r--   0        0        0     5737 2024-03-29 09:45:40.583647 screenapi_cli-0.1.5a2/app/txt/cli.py
--rw-r--r--   0        0        0     6056 2024-03-25 18:55:58.756247 screenapi_cli-0.1.5a2/app/txt/deprecated_cli.py
--rw-r--r--   0        0        0        0 2024-03-27 04:52:19.596215 screenapi_cli-0.1.5a2/app/xlsx/__init__.py
--rw-r--r--   0        0        0    10708 2024-04-11 16:39:15.866431 screenapi_cli-0.1.5a2/app/xlsx/main.py
--rw-r--r--   0        0        0      795 2024-04-11 16:46:32.022697 screenapi_cli-0.1.5a2/pyproject.toml
--rw-r--r--   0        0        0     2092 1970-01-01 00:00:00.000000 screenapi_cli-0.1.5a2/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-03-23 16:06:49.120124 screenapi_cli-0.1.5a3/LICENSE
+-rw-r--r--   0        0        0     1381 2024-03-25 19:41:34.179648 screenapi_cli-0.1.5a3/README.md
+-rw-r--r--   0        0        0        0 2024-03-26 06:15:38.237432 screenapi_cli-0.1.5a3/app/__init__.py
+-rw-r--r--   0        0        0     9241 2024-04-11 16:34:55.215188 screenapi_cli-0.1.5a3/app/__main__.py
+-rw-r--r--   0        0        0     1360 2024-04-01 07:33:03.304661 screenapi_cli-0.1.5a3/app/common.py
+-rw-r--r--   0        0        0        0 2024-03-24 18:09:29.678307 screenapi_cli-0.1.5a3/app/export/__init__.py
+-rw-r--r--   0        0        0     1689 2024-04-15 17:50:49.954658 screenapi_cli-0.1.5a3/app/export/cli.py
+-rw-r--r--   0        0        0        0 2024-03-24 14:33:45.903715 screenapi_cli-0.1.5a3/app/setup/__init__.py
+-rw-r--r--   0        0        0     1083 2024-03-25 19:15:41.722738 screenapi_cli-0.1.5a3/app/setup/utils.py
+-rw-r--r--   0        0        0       97 2024-03-24 17:32:30.550768 screenapi_cli-0.1.5a3/app/txt/__init__.py
+-rw-r--r--   0        0        0     5737 2024-03-29 09:45:40.583647 screenapi_cli-0.1.5a3/app/txt/cli.py
+-rw-r--r--   0        0        0     6056 2024-03-25 18:55:58.756247 screenapi_cli-0.1.5a3/app/txt/deprecated_cli.py
+-rw-r--r--   0        0        0        0 2024-03-27 04:52:19.596215 screenapi_cli-0.1.5a3/app/xlsx/__init__.py
+-rw-r--r--   0        0        0    11219 2024-04-16 15:41:00.869229 screenapi_cli-0.1.5a3/app/xlsx/main.py
+-rw-r--r--   0        0        0      795 2024-04-16 16:11:49.480663 screenapi_cli-0.1.5a3/pyproject.toml
+-rw-r--r--   0        0        0     2092 1970-01-01 00:00:00.000000 screenapi_cli-0.1.5a3/PKG-INFO
```

### Comparing `screenapi_cli-0.1.5a2/LICENSE` & `screenapi_cli-0.1.5a3/LICENSE`

 * *Files identical despite different names*

### Comparing `screenapi_cli-0.1.5a2/README.md` & `screenapi_cli-0.1.5a3/README.md`

 * *Files identical despite different names*

### Comparing `screenapi_cli-0.1.5a2/app/__main__.py` & `screenapi_cli-0.1.5a3/app/__main__.py`

 * *Files identical despite different names*

### Comparing `screenapi_cli-0.1.5a2/app/common.py` & `screenapi_cli-0.1.5a3/app/common.py`

 * *Files identical despite different names*

### Comparing `screenapi_cli-0.1.5a2/app/export/cli.py` & `screenapi_cli-0.1.5a3/app/export/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,19 +23,22 @@
 
     if len(json_files) == 0:
         print("No JSON files found in the input directory.", input_dir)
         return
 
     with Progress() as progress:
         task = progress.add_task("Processing JSON file", total=len(json_files))
-        for file_name in json_files:
+        for index, file_name in enumerate(json_files, start=1):
             file_path = os.path.join(input_dir, file_name)
             df = process_and_append_data(file_path, df)
+            # Calculate the percentage and update the task description
+            percentage = (index / len(json_files)) * 100
             progress.update(
                 task,
+                description=f"Processing JSON file {index}/{len(json_files)} ({percentage:.2f}%)",
                 advance=1,
             )
 
     # print(df.head())
     df["sl"] = pd.RangeIndex(start=1, stop=len(df) + 1)
     df = df.reindex(columns=[sort_by, *df.columns[:-1]])
     df.sort_values(by=sort_by, inplace=True)
```

### Comparing `screenapi_cli-0.1.5a2/app/setup/utils.py` & `screenapi_cli-0.1.5a3/app/setup/utils.py`

 * *Files identical despite different names*

### Comparing `screenapi_cli-0.1.5a2/app/txt/cli.py` & `screenapi_cli-0.1.5a3/app/txt/cli.py`

 * *Files identical despite different names*

### Comparing `screenapi_cli-0.1.5a2/app/txt/deprecated_cli.py` & `screenapi_cli-0.1.5a3/app/txt/deprecated_cli.py`

 * *Files identical despite different names*

### Comparing `screenapi_cli-0.1.5a2/app/xlsx/main.py` & `screenapi_cli-0.1.5a3/app/xlsx/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -172,15 +172,26 @@
     for root, dirs, files in os.walk(output_dir):
         if root.startswith(("images")):
             continue
         for file in files:
             if file.startswith("converted"):
                 continue
             if file.endswith(".json"):
-                ids.append(int(os.path.basename(file).split(".")[0]))
+                with open(os.path.join(root, file)) as _f:
+                    d = json.loads(_f.read())
+                    try:
+                        if d.get("title") in ["", "0"] or d.get("description") in [
+                            "",
+                            "0",
+                        ]:
+                            os.remove(os.path.join(root, file))
+                        else:
+                            ids.append(int(os.path.basename(file).split(".")[0]))
+                    except Exception as e:
+                        print(e)
 
     print("Already done: ", len(ids))
     return ids
 
 
 def request(options: dict[str, Any]):
     client: Client = options["client"]
@@ -222,37 +233,36 @@
         str(data.get("sl")) + ".json",
     )
 
     os.makedirs(Path(output_filename).parent, exist_ok=True)
 
     try:
         for key, value in jsonResponse.items():
+            if key == "username" or key == "description" or key == "title":
+                if jsonResponse[key] not in ["", "0"]:
+                    data["description"] = jsonResponse[key]
+
             if key in data:
+                if key == "description":
+                    continue
                 data[key] = value
 
-            # if key == "description":
-            #     data[key] = (
-            #         jsonResponse.get("title")
-            #         if jsonResponse.get("description") == "0"
-            #         else jsonResponse.get("description")
-            #     )
-
         with open(output_filename, "w") as file:
             json.dump(data, file, indent=2)
         # print(f"Saved to {output_filename}")
         progress.update(taskId, advance=1)
     except Exception as error:
         print(f"Error saving to {output_filename}: {error}")
 
 
 def main(
     input_path: Path,
     site: sheetType,
     output_dir: Optional[Path] = None,
-    # save: Optional[bool] = True,
+    save: Optional[bool] = True,
     max_workers: Optional[int] = config.get("default", "max_workers"),
     overwrite: Optional[bool] = False,
     skip_images: Optional[bool] = False,
 ):
     global OUTPUT_DIR
     if output_dir is None:
         # global output_dir
@@ -340,12 +350,15 @@
         ),
     )
 
     print("Done!")
 
 
 if __name__ == "__main__":
-    convert_to_json(
-        input_path=Path("/home/rony/Downloads/Elle 18 09-04-2024_Shreya Jain.xlsx"),
-        site=sheetType.ecom,
+    main(
+        input_path=Path("dumps/goibibo.xlsx"),
+        site=sheetType.social,
         save=True,
+        overwrite=True,
+        skip_images=True,
+        max_workers=5,
     )
```

### Comparing `screenapi_cli-0.1.5a2/pyproject.toml` & `screenapi_cli-0.1.5a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "screenapi-cli"
-version = "0.1.5a2"
+version = "0.1.5a3"
 description = "A cli interface to interact with screenapi"
 authors = ["RONY <iamrony777@pm.me>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "app" },
 ]
```

### Comparing `screenapi_cli-0.1.5a2/PKG-INFO` & `screenapi_cli-0.1.5a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screenapi-cli
-Version: 0.1.5a2
+Version: 0.1.5a3
 Summary: A cli interface to interact with screenapi
 License: MIT
 Author: RONY
 Author-email: iamrony777@pm.me
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

