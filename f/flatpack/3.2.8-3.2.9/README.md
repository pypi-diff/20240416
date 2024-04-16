# Comparing `tmp/flatpack-3.2.8.tar.gz` & `tmp/flatpack-3.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatpack-3.2.8.tar", last modified: Sun Mar 17 22:27:29 2024, max compression
+gzip compressed data, was "flatpack-3.2.9.tar", last modified: Wed Mar 20 20:05:01 2024, max compression
```

## Comparing `flatpack-3.2.8.tar` & `flatpack-3.2.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-03-17 22:27:29.506883 flatpack-3.2.8/
--rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.2.8/LICENSE
--rw-r--r--   0 romlingroup   (501) staff       (20)     4153 2024-03-17 22:27:29.506675 flatpack-3.2.8/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)     3690 2024-03-10 07:16:34.000000 flatpack-3.2.8/README.md
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-03-17 22:27:29.505145 flatpack-3.2.8/flatpack/
--rw-r--r--   0 romlingroup   (501) staff       (20)      132 2024-01-31 06:56:56.000000 flatpack-3.2.8/flatpack/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.2.8/flatpack/config.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.2.8/flatpack/datasets.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1057 2024-01-31 06:56:56.000000 flatpack-3.2.8/flatpack/instructions.py
--rw-r--r--   0 romlingroup   (501) staff       (20)    21729 2024-03-17 22:27:23.000000 flatpack-3.2.8/flatpack/main.py
--rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.2.8/flatpack/models.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-03-17 22:27:29.506343 flatpack-3.2.8/flatpack/modules/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.2.8/flatpack/modules/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.2.8/flatpack/modules/lstm.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.2.8/flatpack/modules/rnn.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     7014 2024-03-09 20:05:44.000000 flatpack-3.2.8/flatpack/parsers.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.2.8/flatpack/utils.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-03-17 22:27:29.505902 flatpack-3.2.8/flatpack.egg-info/
--rw-r--r--   0 romlingroup   (501) staff       (20)     4153 2024-03-17 22:27:29.000000 flatpack-3.2.8/flatpack.egg-info/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)      458 2024-03-17 22:27:29.000000 flatpack-3.2.8/flatpack.egg-info/SOURCES.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-03-17 22:27:29.000000 flatpack-3.2.8/flatpack.egg-info/dependency_links.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-03-17 22:27:29.000000 flatpack-3.2.8/flatpack.egg-info/entry_points.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)      111 2024-03-17 22:27:29.000000 flatpack-3.2.8/flatpack.egg-info/requires.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-03-17 22:27:29.000000 flatpack-3.2.8/flatpack.egg-info/top_level.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-03-17 22:27:29.506924 flatpack-3.2.8/setup.cfg
--rw-r--r--   0 romlingroup   (501) staff       (20)      766 2024-03-17 22:25:45.000000 flatpack-3.2.8/setup.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-03-20 20:05:01.844903 flatpack-3.2.9/
+-rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.2.9/LICENSE
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4153 2024-03-20 20:05:01.844622 flatpack-3.2.9/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)     3690 2024-03-10 07:16:34.000000 flatpack-3.2.9/README.md
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-03-20 20:05:01.842363 flatpack-3.2.9/flatpack/
+-rw-r--r--   0 romlingroup   (501) staff       (20)      132 2024-01-31 06:56:56.000000 flatpack-3.2.9/flatpack/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.2.9/flatpack/config.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.2.9/flatpack/datasets.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1057 2024-01-31 06:56:56.000000 flatpack-3.2.9/flatpack/instructions.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)    21848 2024-03-20 20:04:45.000000 flatpack-3.2.9/flatpack/main.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.2.9/flatpack/models.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-03-20 20:05:01.844168 flatpack-3.2.9/flatpack/modules/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.2.9/flatpack/modules/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.2.9/flatpack/modules/lstm.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.2.9/flatpack/modules/rnn.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     7014 2024-03-09 20:05:44.000000 flatpack-3.2.9/flatpack/parsers.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.2.9/flatpack/utils.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-03-20 20:05:01.843435 flatpack-3.2.9/flatpack.egg-info/
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4153 2024-03-20 20:05:01.000000 flatpack-3.2.9/flatpack.egg-info/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)      458 2024-03-20 20:05:01.000000 flatpack-3.2.9/flatpack.egg-info/SOURCES.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-03-20 20:05:01.000000 flatpack-3.2.9/flatpack.egg-info/dependency_links.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-03-20 20:05:01.000000 flatpack-3.2.9/flatpack.egg-info/entry_points.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)      111 2024-03-20 20:05:01.000000 flatpack-3.2.9/flatpack.egg-info/requires.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-03-20 20:05:01.000000 flatpack-3.2.9/flatpack.egg-info/top_level.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-03-20 20:05:01.844972 flatpack-3.2.9/setup.cfg
+-rw-r--r--   0 romlingroup   (501) staff       (20)      766 2024-03-20 19:23:18.000000 flatpack-3.2.9/setup.py
```

### Comparing `flatpack-3.2.8/LICENSE` & `flatpack-3.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `flatpack-3.2.8/PKG-INFO` & `flatpack-3.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.2.8
+Version: 3.2.9
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: chromadb==0.4.24
```

### Comparing `flatpack-3.2.8/README.md` & `flatpack-3.2.9/README.md`

 * *Files identical despite different names*

### Comparing `flatpack-3.2.8/flatpack/datasets.py` & `flatpack-3.2.9/flatpack/datasets.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.2.8/flatpack/instructions.py` & `flatpack-3.2.9/flatpack/instructions.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.2.8/flatpack/main.py` & `flatpack-3.2.9/flatpack/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,18 +33,24 @@
 config = {
     "api_key": None
 }
 
 
 def safe_cleanup():
     try:
-        # Your cleanup code here
-        print("🦺 Safe cleanup completed.")
+        files_to_delete = ["flatpack.sh", "device.sh"]
+        current_directory = Path.cwd()
+
+        for filename in files_to_delete:
+            file_path = current_directory / filename
+
+            if file_path.exists():
+                file_path.unlink()
+                print(f"Deleted {filename}.")
     except Exception as e:
-        # Log the exception or silently pass
         print(f"Exception during safe_cleanup: {e}")
 
 
 atexit.register(safe_cleanup)
 
 
 class SessionManager:
@@ -111,27 +117,27 @@
             encrypted_api_key_bytes = encrypted_api_key_str.encode()
             return fpk_decrypt_data(encrypted_api_key_bytes, encryption_key)
         else:
             return None
 
 
 def fpk_cache_last_flatpack(directory_name: str):
-    """Cache the last installed flatpack's directory name to a file within the corresponding build directory."""
-    # The directory where the flatpack is installed, which includes the build directory
+    """Cache the last unboxed flatpack's directory name to a file within the corresponding build directory."""
+    # The directory where the flatpack is unboxed, which includes the build directory
     flatpack_dir = Path.cwd()
     flatpack_dir.mkdir(parents=True, exist_ok=True)  # Ensure the directory exists
 
-    # The cache file that contains the name of the last installed flatpack
+    # The cache file that contains the name of the last unboxed flatpack
     cache_file_path = flatpack_dir / 'last_flatpack.cache'
     with open(cache_file_path, 'w') as f:
         f.write(directory_name)
 
 
 def fpk_get_last_flatpack(directory_name: str) -> Optional[str]:
-    """Retrieve the last installed flatpack's directory name from the cache file within the correct build directory."""
+    """Retrieve the last unboxed flatpack's directory name from the cache file within the correct build directory."""
     flatpack_dir = Path.cwd()
     cache_file_path = flatpack_dir / 'last_flatpack.cache'
     if cache_file_path.exists():
         return cache_file_path.read_text().strip()
     return None
 
 
@@ -186,17 +192,17 @@
 permissions and limitations under the License.
 {please_note}
 To accept, type 'YES'. To decline, type 'NO'.
 -----------------------------------------------------
 """
 
     please_note_content = """
-PLEASE NOTE: The flatpack you are about to install is
+PLEASE NOTE: The flatpack you are about to unbox is
 governed by its own licenses and terms, separate from
-this installer. You may find further details at:
+this software. You may find further details at:
 
 https://fpk.ai/w/{}
 """.format(directory_name)
 
     please_note_colored = fpk_colorize(please_note_content, "yellow")
     print(disclaimer_template.format(please_note=please_note_colored))
 
@@ -253,25 +259,25 @@
     for root, _, files in os.walk(directory_path):
         for file in files:
             if any(file.endswith(fmt) for fmt in model_file_formats):
                 model_files.append(os.path.join(root, file))
     return model_files
 
 
-def fpk_install(directory_name: str, session, verbose: bool = False, local: bool = False):
-    # Define the directory where the flatpack will be installed, which includes the build directory
+def fpk_unbox(directory_name: str, session, verbose: bool = False, local: bool = False):
+    # Define the directory where the flatpack will be unboxed, which includes the build directory
     flatpack_dir = Path.cwd() / directory_name
     flatpack_dir.mkdir(parents=True, exist_ok=True)  # Ensure the directory exists
     build_dir = flatpack_dir / "build"
     build_dir.mkdir(parents=True, exist_ok=True)  # Explicitly ensure that build_dir exists
 
     # Define the path for the temporary flatpack TOML file
     temp_toml_path = build_dir / 'temp_flatpack.toml'
 
-    # Handle local directory installation
+    # Handle local directory unboxing
     if local:
         local_directory_path = flatpack_dir  # Use flatpack_dir directly since it already points to the correct location
         # Assuming flatpack.toml is required in the directory
         toml_path = local_directory_path / 'flatpack.toml'
         if not toml_path.exists():
             print(f"❌ flatpack.toml not found in the specified directory: '{directory_name}'.")
             return
@@ -296,15 +302,15 @@
     # Save the bash script in the build directory
     bash_script_path = build_dir / 'flatpack.sh'
     bash_script_path.write_text(bash_script_content)
 
     # Remove the temporary TOML file after it's no longer needed
     temp_toml_path.unlink()
 
-    print(f"Installing {directory_name}...")
+    print(f"Unboxing {directory_name}...")
 
     # Execute the bash script
     command = ["bash", str(bash_script_path)]
 
     try:
         if verbose:
             process = subprocess.Popen(command)
@@ -380,15 +386,15 @@
 
     try:
         response = session.post(LOGGING_ENDPOINT, params=params, json=data, headers=headers, timeout=10)
     except httpx.RequestError as e:
         print(f"Failed to send request: {e}")
 
 
-def fpk_process_output(output, session, last_installed_flatpack):
+def fpk_process_output(output, session, last_unboxed_flatpack):
     """Process output and log it."""
     # Get the API key for logging
     api_key = fpk_get_api_key()
 
     # Regular expression pattern to match ANSI escape codes
     ansi_escape = re.compile(r'\x1B(?:[@-Z\\-_]|\[[0-?]*[ -/]*[@-~])')
 
@@ -403,42 +409,42 @@
         # If the line isn't empty, process it
         if line:
             # Display the line with a prefix
             print(f"(*) {line}", flush=True)
 
             # If we have an API key, log the line to the API
             if api_key:
-                fpk_log_to_api(line, session, api_key=api_key, model_name=last_installed_flatpack)
+                fpk_log_to_api(line, session, api_key=api_key, model_name=last_unboxed_flatpack)
 
 
-def fpk_train(directory: str, session: httpx.Client = None):
-    """Train a model using a training script from the last installed flatpack."""
+def fpk_build(directory: str, session: httpx.Client = None):
+    """Build a model using a building script from the last unboxed flatpack."""
     cache_file_path = Path('last_flatpack.cache')
     print(f"Looking for cached flatpack in {cache_file_path}.")
 
     if directory and fpk_valid_directory_name(directory):
         print(f"Using provided directory: {directory}")
-        last_installed_flatpack = directory
+        last_unboxed_flatpack = directory
     elif cache_file_path.exists():
         print(f"Found cached flatpack in {cache_file_path}.")
-        last_installed_flatpack = cache_file_path.read_text().strip()
-        if not fpk_valid_directory_name(last_installed_flatpack):
-            print(f"❌ Invalid directory name from cache: '{last_installed_flatpack}'.")
+        last_unboxed_flatpack = cache_file_path.read_text().strip()
+        if not fpk_valid_directory_name(last_unboxed_flatpack):
+            print(f"❌ Invalid directory name from cache: '{last_unboxed_flatpack}'.")
             return
     else:
         print("❌ No cached flatpack found, and no valid directory provided.")
         return
 
-    training_script_path = Path(last_installed_flatpack) / 'build' / 'train.sh'
-    if not training_script_path.exists():
-        print(f"❌ Training script not found in {last_installed_flatpack}.")
+    building_script_path = Path(last_unboxed_flatpack) / 'build' / 'build.sh'
+    if not building_script_path.exists():
+        print(f"❌ Building script not found in {last_unboxed_flatpack}.")
         return
 
     env = dict(os.environ, PYTHONUNBUFFERED="1")
-    safe_script_path = shlex.quote(str(training_script_path))
+    safe_script_path = shlex.quote(str(building_script_path))
 
     try:
         proc = subprocess.Popen(["bash", "-u", safe_script_path], stdin=subprocess.PIPE,
                                 stdout=subprocess.PIPE, stderr=subprocess.PIPE, bufsize=1, universal_newlines=True,
                                 env=env)
 
         outputs = [proc.stdout, proc.stderr]
@@ -448,15 +454,15 @@
             if retcode is not None:  # Subprocess has exited
                 break
 
             rlist, _, _ = select.select(outputs, [], [], 0.1)
             for r in rlist:
                 line = r.readline()
                 if line:
-                    fpk_process_output(line, session, last_installed_flatpack)
+                    fpk_process_output(line, session, last_unboxed_flatpack)
 
                     if not line.endswith('\n'):
                         try:
                             user_input = input()
                             print(user_input, file=proc.stdin)
                         except EOFError:
                             # Handle end-of-file condition (e.g., if input redirection is closed)
@@ -515,69 +521,69 @@
     try:
         with SessionManager() as session:
             parser = argparse.ArgumentParser(description='flatpack command line interface')
             parser.add_argument('command', help='Command to run')
             parser.add_argument('input', nargs='?', default=None, help='Input for the callback')
             parser.add_argument('--verbose', action='store_true', help='Display detailed outputs for debugging.')
             parser.add_argument('--local', action='store_true',
-                                help='Install from a local directory instead of GitHub.')
+                                help='Unbox from a local directory instead of GitHub.')
 
             args = parser.parse_args()
             command = args.command
 
             fpk_get_api_key()
 
             if command == "find":
                 print(fpk_find_models())
             elif command == "help":
                 print("[HELP]")
             elif command == "get-api-key":
                 print(fpk_get_api_key())
-            elif command == "install":
+            elif command == "unbox":
                 if not args.input:
-                    print("❌ Please specify a flatpack for the install command.")
+                    print("❌ Please specify a flatpack for the unbox command.")
                     return
 
                 directory_name = args.input
 
                 if not args.local:
-                    # If not installing from a local directory, check if the flatpack exists in GitHub directories
+                    # If not unboxing from a local directory, check if the flatpack exists in GitHub directories
                     existing_dirs = fpk_fetch_github_dirs(session)
                     if directory_name not in existing_dirs:
                         print(f"❌ The flatpack '{directory_name}' does not exist.")
                         return
 
-                    # Display disclaimer and proceed with installation
+                    # Display disclaimer and proceed with unboxing
                     fpk_display_disclaimer(directory_name)
 
                     while True:
                         user_response = input().strip().upper()
                         if user_response == "YES":
                             break
                         elif user_response == "NO":
-                            print("❌ Installation aborted by user.")
+                            print("❌ Unboxing aborted by user.")
                             return
                         else:
                             print("❌ Invalid input. Please type 'YES' to accept or 'NO' to decline.")
 
                 if args.local:
-                    # For local installation, directly proceed without GitHub check
+                    # For local unboxing, directly proceed without GitHub check
                     local_directory_path = Path(directory_name)
                     if not local_directory_path.exists() or not local_directory_path.is_dir():
                         print(f"❌ Local directory does not exist: '{directory_name}'.")
                         return
                     toml_path = local_directory_path / 'flatpack.toml'
                     if not toml_path.exists():
                         print(f"❌ flatpack.toml not found in the specified directory: '{directory_name}'.")
                         return
 
                 print("Verbose mode:", args.verbose)
 
                 print(f"✅ Directory name resolved to: '{directory_name}'")
-                fpk_install(directory_name, session, verbose=args.verbose, local=args.local)
+                fpk_unbox(directory_name, session, verbose=args.verbose, local=args.local)
             elif command == "list":
                 print(fpk_list_directories(session))
             elif command == "run":
 
                 try:
                     port = 8000
                     listener = ngrok.forward(port, authtoken_from_env=True)
@@ -595,17 +601,17 @@
 
             elif command == "set-api-key":
                 if not args.input:
                     print("❌ Please provide an API key to set.")
                     return
                 fpk_set_api_key(args.input)
                 print("API key set successfully!")
-            elif command == "train":
+            elif command == "build":
                 directory_name = args.input
-                fpk_train(directory_name, session)
+                fpk_build(directory_name, session)
             elif command == "version":
                 print("[VERSION]")
             else:
                 print(f"Unknown command: {command}")
 
     except Exception as e:
         print(f"An unexpected error occurred: {e}")
```

### Comparing `flatpack-3.2.8/flatpack/modules/lstm.py` & `flatpack-3.2.9/flatpack/modules/lstm.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.2.8/flatpack/modules/rnn.py` & `flatpack-3.2.9/flatpack/modules/rnn.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.2.8/flatpack/parsers.py` & `flatpack-3.2.9/flatpack/parsers.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.2.8/flatpack.egg-info/PKG-INFO` & `flatpack-3.2.9/flatpack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.2.8
+Version: 3.2.9
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: chromadb==0.4.24
```

### Comparing `flatpack-3.2.8/setup.py` & `flatpack-3.2.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="flatpack",
-    version="3.2.8",
+    version="3.2.9",
     license="Apache Software License (Apache-2.0)",
     packages=find_packages(),
     install_requires=[
         "chromadb==0.4.24",
         "cryptography==42.0.5",
         "fastapi==0.110.0",
         "httpx==0.27.0",
```

